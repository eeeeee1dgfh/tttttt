<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Website Redirect</title>
</head>
<body>
    <h1>Click the button to visit a random website:</h1>
    <button id="redirectButton">Go to a Random Website</button>

    <script>
        // Function to redirect to a random website
        function redirectToRandomWebsite() {
            // Array of two website URLs
            const websites = [
                "https://www.example1.com",
                "https://www.example2.com"
            ];

            // Generate a random index (0 or 1) to select a website
            const randomIndex = Math.floor(Math.random() * 2);

            // Redirect to the selected website
            window.location.href = websites[randomIndex];
        }

        // Attach the redirectToRandomWebsite function to the button click event
        const redirectButton = document.getElementById("redirectButton");
        redirectButton.addEventListener("click", redirectToRandomWebsite);
    </script>
</body>
</html>
