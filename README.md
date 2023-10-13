


<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>OCTOBERS VERY OWN</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-image: url('IMG-20231013-WA0004.jpg');
            background-size: cover; /* Make the background image cover the entire screen */
            background-repeat: no-repeat;
            background-attachment: fixed; /* Keep the background fixed when scrolling */
            color: #FFF;
            display: flex;
    
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        h1 {
            color: #FFF;
            margin-top: 10px; /* Increase the margin to center the heading */
            font-family: 'cursive', sans-serif;
            font-size: 24px; /* Adjust font size for mobile */
            text-shadow: 2px 2px 4px #000;
        }

        .countdown {
            font-size: 40px; /* Adjust font size for mobile */
            color: #FFF;
        }

        .party-text {
            font-size: 16px; /* Adjust font size for mobile */
            color: #FFF;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <h1>OCTOBERS VERY OWN</h1>
    <p class="countdown" id="countdown"></p>
    <p class="party-text">You have been exclusively invited to a party in Sandton.</p>
    <p class="party-text">Location to be announced 20/10/2023</p>

    <script>
        var countDownDate = new Date("October 28, 2023 00:00:00").getTime();

        var x = setInterval(function() {
            var now = new Date().getTime();
            var timeLeft = countDownDate - now;
            var days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
            var hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            var minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
            var seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);
            document.getElementById("countdown").innerHTML = days + " : " + hours + " : " + minutes + " : " + seconds;
            if (timeLeft < 0) {
                clearInterval(x);
                document.getElementById("countdown").innerHTML = "The party is here!";
            }
        }, 1000);
    </script>
</body>
</html>
   

