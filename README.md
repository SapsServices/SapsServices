<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Main Website</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>Click around the website to trigger the popunder ad.</p>

    <script>
        function openPopunder() {
            const popunderUrl = 'popunder.html'; // Your popunder ad URL
            const popunderWindow = window.open(popunderUrl, '_blank');
            if (popunderWindow) {
                // Move the focus back to the main window to simulate "popunder" behavior
                window.focus();
            }
        }

        // Trigger popunder ad after a certain user interaction (e.g., click)
        document.body.addEventListener('click', function() {
            openPopunder();
        });
    </script>
</body>
</html>
