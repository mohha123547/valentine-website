<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day</title>
    <style>
        body {
            background-color: pink;
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .heart {
            color: red;
            font-size: 100px;
            margin-top: 10%; /* Adjusted to push content up */
        }
        .message {
            font-size: 24px;
            color: black;
            margin: 20px 0; /* Space around the message */
        }
        .image-container {
            display: flex;
            justify-content: center; /* Center horizontally */
            margin-top: 20px; /* Space above the image */
        }
        .button-container {
            display: flex;
            justify-content: center; /* Center buttons */
            margin-top: 20px; /* Space above buttons */
        }
        #yes-button, #no-button {
            background-color: green; /* Change to your desired color */
            color: black;            /* Text color */
            border: white;           /* Remove border */
            padding: 10px 20px;     /* Add padding */
            cursor: pointer;        /* Change cursor to pointer */
            margin: 0 10px;        /* Space between buttons */
        }
        .hidden-message {
            display: none; /* Initially hide the messages */
            font-size: 18px;
            color: purple;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="heart">❤️</div>
    <div class="image-container">
        <img src="https://assets.onecompiler.app/437vq7ujm/437vq43vn/heart%20.gif" alt="Heart GIF">
    </div>
    <div class="message">WILL YOU BE MY VALENTINE?</div>
    
    <div class="button-container">
        <button id="yes-button">YES</button>
        <button id="no-button">NO</button>
        
    </div>

    <div id="yes-message" class="hidden-message">You have made me happy! 💖</div>
    <div id="no-message" class="hidden-message"> I have a crush  on you! 😔</div>

    <script>
        document.getElementById("yes-button").addEventListener("click", function() {
            document.getElementById("yes-message").style.display = "block"; // Show the YES message
            document.getElementById("no-message").style.display = "none";  // Hide the NO message
        });

        document.getElementById("no-button").addEventListener("click", function() {
            document.getElementById("no-message").style.display = "block";  // Show the NO message
            document.getElementById("yes-message").style.display = "none"; // Hide the YES message
        });
    </script>
</body>
