<script>
    import Card from "./Card.svelte";
    export let field
    let src = "src/routes/saud-dnyandeep.jpg"
</script>

<Card>
    <h3>{field.title}</h3>
    {#if field.title === 'About Me'}
        <img {src} class="img" alt="Saud's selfie at his favorite place." height="250dp"/>
    {:else if field.title === 'Skills'}
        <div id="barchart_values"></div>
    {/if}
    <br>
    <p><em>{field.description}</em></p>
</Card>

<style>
    .img {
        border: 3px solid black;
        border-radius: 3px;
        margin-left: 25px;
        margin-right: auto;
    }
</style>


<head>
<!--Load the AJAX API-->
<script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
<script type="text/javascript">
    google.charts.load("current", {packages:["corechart"]});
    google.charts.setOnLoadCallback(drawChart);
    function drawChart() {
      var data = google.visualization.arrayToDataTable([
        ["Language", "Knowledge", { role: "style" } ],
        ["C/C++", 90, "#044F88"],
        ["Swift", 95, "orange"],
        ["Python", 97, "saffron"],
        ["ARM ASM", 80, "grey"]
      ]);

      var view = new google.visualization.DataView(data);
      view.setColumns([0, 1,
                       { calc: "stringify",
                         sourceColumn: 1,
                         type: "string",
                         role: "annotation" },
                       2]);

      var options = {
        width: 600,
        height: 400,
        bar: {groupWidth: "95%"},
        legend: { position: "none" },
      };
      var chart = new google.visualization.BarChart(document.getElementById("barchart_values"));
      chart.draw(view, options);
  }
  </script>
</head>
