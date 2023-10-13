


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
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed;
            color: #FFF; /* White text color */
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        h1 {
            font-size: 20px; /* Slightly reduced font size for mobile */
            text-shadow: 2px 2px 4px #000;
        }

        .countdown {
            font-size: 36px; /* Slightly reduced font size for mobile */
        }

        .party-text {
            font-size: 14px; /* Reduced font size for mobile */
            margin-top: 10px;
        }

        /* Remove the blue underlined link */
        .party-text a {
            text-decoration: none;
            color: #FFF;
        }
    </style>
</head>
<body>
    <h1>OCTOBERS VERY OWN</h1>
    <p class="countdown" id="countdown"></p>
    <p class="party-text">You have been exclusively invited to a party in Sandton.</p>
    <p class="party-text">Location to be announced: 20/10/2023</p>
    <script>
        var countDownDate = a new Date("October 28, 2023 00:00:00").getTime();
        var x = setInterval(function() {
            var now = new Date().getTime();
            var timeLeft = countDownDate - now;
            var days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
            var hours = Math floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
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

