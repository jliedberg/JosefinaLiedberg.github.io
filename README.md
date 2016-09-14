# JosefinaLiedberg.github.io
<!DOCTYPE html>
<html>
<head>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.2.2/Chart.js">
</script>
<link rel="stylesheet" href="css/main.css" type="text/css">
</head>

<body>

<center>

<h1>Music Sales Report, Sweden 2015</h1>

<img src="https://solangefrancois.files.wordpress.com/2014/08/bach.jpg">
<p> </p>
<p> </p>
<p> </p>
<p> </p>
<p> </p>
<p> </p>
<p> </p>
<p> </p>

<canvas id="myChart" width:400px; height:400px ></canvas>
<script>
Chart.defaults.global.defaultFontColor = '#fff';
Chart.defaults.global.defaultFontFamily = "Comic Sans MS";

var ctx = document.getElementById("myChart");
var myChart = new Chart(ctx, {
    type: 'pie',
    data: {
        labels: ["Singles", "CD's", "Vinyls", "Musicvideos", "Streaming Services", "Downloads", "Others"],
        datasets: [{
            label: '# Music sales',
            data: [0.1, 11, 3, 0.6, 82.7, 2.3, 0.1],
            backgroundColor: [
                'rgba(70, 130, 180, 0.8)',
                'rgba(99, 184, 255, 0.8)',
                'rgba(79, 148, 205, 0.8)',
                'rgba(54, 100, 139, 0.8)',
                'rgba(141, 182, 205, 0.8)',
                'rgba(173, 216, 230, 0.8)',
                'rgba(126, 192, 238, 0.8)' ,
            ],
            borderColor: [
                'rgba(70, 130, 180, 1)',
                'rgba(99, 184, 255, 1)',
                'rgba(79, 148, 205, 1)',
                'rgba(54, 100, 139, 1)',
                'rgba(141, 182, 205, 1)',
                'rgba(173, 216, 230, 1)' ,
                'rgba(126, 192, 238, 1)' ,
            ],
            borderWidth: 2
        }]
    },
    options: {
    	fontFamily : "'Comic Sans'",
    	legend: {
    		label: {
	    		fontSize: 50
	    	}
    	},
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero:true
                }
            }]
        }
    }
});
</script>
	
</body>
</html>
