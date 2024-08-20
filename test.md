<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Joke Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Random Joke Generator</h1>
    <button onclick="getJoke()">Tell me a joke!</button>
    <p id="joke"></p>

    <script>
        function getJoke() {
            const jokes = [
                "Why don’t scientists trust atoms? Because they make up everything!",
                "Why did the scarecrow win an award? Because he was outstanding in his field!",
                "Why don’t skeletons fight each other? They don’t have the guts.",
                "What do you call cheese that isn't yours? Nacho cheese!",
                "Why couldn’t the bicycle stand up by itself? It was two-tired!"
            ];

            // Get a random index from the jokes array
            const randomIndex = Math.floor(Math.random() * jokes.length);

            // Display the joke
            document.getElementById('joke').textContent = jokes[randomIndex];
        }
    </script>
</body>
</html>
