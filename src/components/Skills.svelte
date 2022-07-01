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
<br>
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
            <li>Flutter</li>
        </ul>
    </li><li><b>Interests</b>
        <!-- <ul>
            <li>Mathematics (Calculus)</li>
            <li>Discrete Mathematics</li>
            <li>Graph Theory</li>
            <li>Digital Logic</li>
            <li>Object Oriented Programming</li>
            <li>Data Structures and Algorithms</li>
            <li>Databases</li>
            <li>ARM Systems</li>
            <li>Theory of Computation</li>
            <li>Software Engineering</li>
            <li>Web Development</li>
            <li>System Programming and Compilers</li>
            <li>Distributed Systems</li>
            <li>Operating System Design</li>
            <li>Applied Machine Learning</li>
            <li>Cloud Computing</li>
            <li>Computer Architecture</li>
        </ul> -->
        <ul>
            <li>Compilers</li>
            <li>Systerm Programs</li>
            <li>Operating Systems (Kernel)</li>
            <li>Artificial Intelligence(AI)</li>
            <li>Machine Learning(ML)</li>
            <li>Extended Reality (XR)</li>
            <li>ARM Processors</li>
            <li>Computer Programming</li>
            <li>Unix Systems</li>
        </ul>
    </li>
</ul>
<br>


