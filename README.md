# APMantics.github.io


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Typewriter Effect</title>
    <style>
        .typewriter {
            font-family: Courier, monospace;
            font-size: 24px;
            white-space: nowrap;
            overflow: hidden;
            border-right: 3px solid black;
            display: inline-block;
        }
    </style>
</head>
<body>
    <div id="typewriter" class="typewriter"></div>

    <script>
        function typewriterEffect(elementId, text, speed) {
            let i = 0;
            let element = document.getElementById(elementId);
            function type() {
                if (i < text.length) {
                    element.innerHTML += text.charAt(i);
                    i++;
                    setTimeout(type, speed);
                }
            }
            type();
        }

        // Call the function
        typewriterEffect("typewriter", "Hello Aiden", 150); // Speed is 150ms
    </script>
</body>
</html>
