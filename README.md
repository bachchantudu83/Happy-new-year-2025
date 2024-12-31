#Falnaaa_164
!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy New Year 2025!</title>
    <style>
        body {
            background-color: #000;
            color: #fff;
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .container {
            position: relative;
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        .fireworks {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            pointer-events: none;
        }
        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }
        p {
            font-size: 1.2rem;
            margin-top: 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="fireworks"></div>
        <h1>🎉 Happy New Year 2025! 🎉</h1>
        <p>Wishing you all the joy and success this year has to offer!</p>
    </div>
    <script>
        // Simulate simple fireworks
        for (let i = 0; i < 100; i++) {
            const firework = document.createElement('div');
            firework.style.cssText = \`
                position: absolute;
                width: 5px;
                height: 5px;
                border-radius: 50%;
                background: hsl(\${Math.random() * 360}, 100%, 50%);
                animation: fireworks 1s linear infinite;
                top: \${Math.random() * 100}%;
                left: \${Math.random() * 100}%;
            \`;
            document.querySelector('.fireworks').appendChild(firework);
        }

        // Add animation
        document.styleSheets[0].insertRule(\`
            @keyframes fireworks {
                0% { transform: translate(0, 0) scale(0); opacity: 1; }
                100% { transform: translate(calc(50vw - 50%), calc(50vh - 50%)) scale(4); opacity: 0; }
            }
        \`, 0);
    </script>
</body>
</html>
