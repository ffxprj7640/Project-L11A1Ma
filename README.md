<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restricted</title>
    <style>
        body {
            background-color: black;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            flex-direction: column;
            position: relative;
        }
        .logo {
            position: absolute;
            top: 10px;
            left: 10px;
            font-size: 48px;
            font-weight: bold;
        }
        .message {
            font-size: 24px;
            font-weight: bold;
            display: none;
        }
        .footer {
            position: absolute;
            bottom: 10px;
            left: 10px;
            font-size: 12px;
        }
        .enter-button {
            font-size: 16px;
            padding: 10px 20px;
            background-color: white;
            color: black;
            border: none;
            cursor: pointer;
        }
    </style>
    <script>
        function showMessage() {
            document.querySelector(".message").style.display = "block";
            document.querySelector(".enter-button").style.display = "none";
            
            let audio = new Audio('FNAF Ultimate Custom Night - Sleep No More.mp3');
            audio.play();
            
            setTimeout(function() {
                document.querySelector(".message").textContent = "Just a moment";
            }, 5000);
            setTimeout(function() {
                document.querySelector(".message").textContent = "Just a few seconds";
            }, 10000);
            setTimeout(function() {
                document.querySelector(".message").textContent = "Just gotta verify something";
            }, 15000);
            setTimeout(function() {
                document.querySelector(".message").textContent = "75. Ever heard of the code L11A1M?";
            }, 20000);
            setTimeout(function() {
                window.close();
            }, 25000);
        }
    </script>
</head>
<body>
    <div class="logo">F</div>
    <button class="enter-button" onclick="showMessage()">Enter Main Log</button>
    <div class="message">Looking for question 75?</div>
    <div class="footer">FCID - A1 Service</div>
</body>
</html>
