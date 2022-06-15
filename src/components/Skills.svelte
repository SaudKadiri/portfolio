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
                ["Swift", 95, "#F05138"],
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

<br>
<b>Programming Languages</b>
<div id="barchart_values"></div>


<ul style="display: flex; justify-content: space-between;">
    <li><b>Frameworks and Tools</b>
        <ul>
            <li>Django</li>
            <li>VS Code</li>
            <li>Docker</li>
            <li>Tensorflow</li>
            <li>PyTorch</li>
            <li>Flask</li>
            <li>etc.</li>
        </ul>
    </li><li><b>App Development</b>
        <ul>
            <li>SwiftUI</li>
            <li>XCode</li>
            <li>Svelte</li>
            <li>Android Studio</li>
        </ul>
    </li><li><b>Courses</b>
        <ul>
            <li>CS50, CS50AI and CS50P (edX)</li>
            <li>Deeplearning.ai (Coursera)</li>
            <li>C Programming Coursera Specialization</li>
            <li>Google Cloud Coursera</li>
        </ul>
    </li>
</ul>
<br>