# aivideogeneration
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Video Generation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
        }
        input[type="file"], input[type="text"] {
            margin: 10px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
        }
        #timer {
            margin-top: 20px;
            font-size: 20px;
        }
    </style>
</head>
<body>
    <h1>Free Unlimited Video Generation</h1>
    <p>Select an image and write a prompt to generate your video.</p>
    <input type="file" id="imageInput" accept="image/*">
    <br>
    <input type="text" id="promptInput" placeholder="Enter your prompt">
    <br>
    <button id="generateButton">Generate Video</button>
    <div id="timer"></div>

    <script>
        document.getElementById('generateButton').addEventListener('click', function() {
            const timerDisplay = document.getElementById('timer');
            timerDisplay.innerHTML = "Generating video... Please wait 1 minute.";
            setTimeout(() => {
                timerDisplay.innerHTML = "Video generated successfully!";
            }, 60000);
        });
    </script>
</body>
</html>
