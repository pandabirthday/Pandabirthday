<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Anish</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #f6d365 0%, #fda085 100%);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            text-align: center;
        }
        .message {
            background-color: rgba(255, 255, 255, 0.95);
            padding: 50px;
            border-radius: 30px;
            box-shadow: 0 12px 24px rgba(0,0,0,0.3);
            animation: popUp 1.5s ease-in-out;
        }
        h1 {
            font-size: 3em;
            color: #ff4081;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in;
        }
        p {
            font-size: 1.7em;
            color: #555;
            animation: fadeIn 2.5s ease-in;
        }
        @keyframes popUp {
            0% {
                transform: scale(0.5);
                opacity: 0;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .confetti {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 0;
        }
        .confetti-piece {
            position: absolute;
            width: 10px;
            height: 20px;
            background-color: #ff69b4;
            animation: fall linear infinite;
            opacity: 0.7;
        }
        @keyframes fall {
            0% { transform: translateY(-100vh) rotate(0deg); }
            100% { transform: translateY(100vh) rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="confetti">
        <!-- Generate multiple confetti pieces -->
        <script>
            for (let i = 0; i < 100; i++) {
                const confetti = document.createElement('div');
                confetti.classList.add('confetti-piece');
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.animationDuration = (Math.random() * 3 + 2) + 's';
                confetti.style.backgroundColor = ['#ff69b4', '#ffd700', '#00e676', '#00b0ff'][Math.floor(Math.random() * 4)];
                document.body.appendChild(confetti);
            }
        </script>
    </div>
    <div class="message">
        <h1>Happy Birthday Anish 🧡🧡</h1>
        <p>Your days filled with love, happiness, health and joy 🩵🩵<br>
        Always be Happy ⭐️💜</p>
    </div>
</body>
</html>

<!--
**pandabirthday/Pandabirthday** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
