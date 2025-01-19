# Happy-birthday-swati
<!DOCTYPE html>
<html>
<head>
    <title>Happy Birthday Swati!</title>
    <style>
        body {
            background-color: #ffccff;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .message {
            display: none;
        }
        .cake {
            display: none;
        }
    </style>
</head>
<body>
    <h1>Happy Birthday Swati!</h1>
    <p>From Rishav</p>
    
    <button onclick="showBalloons()">Click for Balloons!</button>
    <div id="balloons"></div>
    
    <button onclick="showMessage()">Message from Me</button>
    <p class="message">You are very special to me and I wanted to wish you on your birthday, so I created this webpage just for you!</p>
    
    <button onclick="showCake()">Next</button>
    <div class="cake">
        <p>Click the cake to cut it!</p>
        <img src="cake.jpg" alt="Birthday Cake">
    </div>
    
    <audio id="birthdayMusic" src="birthday.mp3"></audio>
    
    <script>
        function showBalloons() {
            document.getElementById('balloons').innerHTML = '<img src="balloon.gif" alt="Balloons">';
        }
        
        function showMessage() {
            document.querySelector('.message').style.display = 'block';
        }
        
        function showCake() {
            document.querySelector('.cake').style.display = 'block';
        }
        
        document.querySelector('.cake').addEventListener('click', function() {
            document.getElementById('birthdayMusic').play();
        })
    </script>
</body>
</html>