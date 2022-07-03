<body>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.5.0/Chart.min.js"></script>

    <script>
        new Chart(document.getElementById("bar-chart-horizontal"), {
            type: 'horizontalBar',
            data: {
            labels: ["ARM ASM", "C/C++", "Python3", "JavaScript", "Swift"],
            datasets: [
                {
                    label: "Relative knowledge",
                    backgroundColor: ["darkgray", "#225398","#46709E","yellow","#f05138"],
                    data: [80,90,97,84,95]
                }
            ]
            },
            options: {
                color: '#fff',
            categorySpacing: 500,
            }
        });
        // Chart.defaults.global.defaultFontColor = "white";
        Chart.defaults.gloabal.ho
    </script>
</body>
<br>
<b>Programming Languages</b>
<br>
<canvas id="bar-chart-horizontal" width="800" height="450"></canvas>
<style>
    p {
        color: grey;
    }
</style>

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


