# Besti-Birthday-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Bestie! 🎉</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(45deg, #ff6b6b, #feca57, #48dbfb, #ff9ff3);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
            height: 100vh;
            overflow-x: hidden;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            position: relative;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .birthday-container {
            max-width: 90%;
            animation: bounceIn 1s ease-out;
        }

        @keyframes bounceIn {
            0% { transform: scale(0.3); opacity: 0; }
            50% { transform: scale(1.05); }
            70% { transform: scale(0.9); }
            100% { transform: scale(1); opacity: 1; }
        }

        h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
            text-shadow: 3px 3px 6px rgba(0,0,0,0.3);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 3px 3px 6px rgba(0,0,0,0.3), 0 0 20px #fff; }
            to { text-shadow: 3px 3px 6px rgba(0,0,0,0.3), 0 0 30px #ffeb3b; }
        }

        .date {
            font-size: 1.5em;
            margin-bottom: 30px;
            font-weight: bold;
        }

        .message {
            font-size: 1.3em;
            line-height: 1.6;
            margin-bottom: 40px;
            max-width: 600px;
            animation: fadeInUp 1.5s ease-out 0.5s both;
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .cake {
            font-size: 4em;
            margin: 30px 0;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-20px); }
            60% { transform: translateY(-10px); }
        }

        .balloons {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
            overflow: hidden;
        }

        .balloon {
            position: absolute;
            font-size: 2em;
            animation: float 6s ease-in-out infinite;
        }

        .balloon:nth-child(1) { left: 10%; animation-delay: 0s; color: #ff6b6b; }
        .balloon:nth-child(2) { left: 20%; animation-delay: 1s; color: #feca57; }
        .balloon:nth-child(3) { left: 80%; animation-delay: 2s; color: #48dbfb; }
        .balloon:nth-child(4) { left: 90%; animation-delay: 3s; color: #ff9ff3; }
        .balloon:nth-child(5) { left: 30%; animation-delay: 4s; color: #54a0ff; }

        @keyframes float {
            0%, 100% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
            50% { transform: translateY(-20px) rotate(180deg); opacity: 1; }
        }

        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background: #ffeb3b;
            animation: confettiFall 3s linear infinite;
        }

        .confetti:nth-child(1) { left: 10%; animation-delay: 0s; background: #ff6b6b; }
        .confetti:nth-child(2) { left: 20%; animation-delay: 0.5s; background: #feca57; }
        .confetti:nth-child(3) { left: 30%; animation-delay: 1s; background: #48dbfb; }
        .confetti:nth-child(4) { left: 40%; animation-delay: 1.5s; background: #ff9ff3; }
        .confetti:nth-child(5) { left: 50%; animation-delay: 2s; background: #54a0ff; }
        .confetti:nth-child(6) { left: 60%; animation-delay: 2.5s; background: #ff6b6b; }

        @keyframes confettiFall {
            0% { transform: translateY(-100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(720deg); opacity: 0; }
        }

        .music-btn {
            position: fixed;
            top: 20px;
            right: 20px;
            background: rgba(255,255,255,0.2);
            border: none;
            border-radius: 50%;
            width: 60px;
            height: 60px;
            font-size: 1.5em;
            cursor: pointer;
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
        }

        .music-btn:hover {
            background: rgba(255,255,255,0.4);
            transform: scale(1.1);
        }

        @media (max-width: 768px) {
            h1 { font-size: 2.5em; }
            .message { font-size: 1.1em; }
            .cake { font-size: 3em; }
        }
    </style>
</head>
<body>
    <button class="music-btn" onclick="toggleMusic()" id="musicBtn">🎵</button>
    
    <div class="balloons">
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
    </div>

    <div class="confetti" style="animation-duration: 4s;"></div>
    <div class="confetti" style="animation-duration: 5s;"></div>
    <div class="confetti" style="animation-duration: 3s;"></div>
    <div class="confetti" style="animation-duration: 4.5s;"></div>
    <div class="confetti" style="animation-duration: 3.5s;"></div>
    <div class="confetti" style="animation-duration: 5.5s;"></div>

    <div class="birthday-container">
        <h1>🎉 HAPPY BIRTHDAY! 🎉</h1>
        <div class="date">29th April</div>
        <div class="cake">🎂✨</div>
        <div class="message">
            Hey Bestie! 🥳<br>
            Wishing you the happiest birthday ever!<br>
            May this year bring you endless joy, love, and all your dreams coming true! 🌟<br>
            You're the best friend anyone could ask for! 💖
        </div>
        <div style="font-size: 1.2em; margin-top: 20px;">
            Love always,<br>
            <span style="font-size: 1.5em; color: #ffeb3b;">Your Best Friend! 💕</span>
        </div>
    </div>

    <audio id="birthdayMusic" loop>
        <source src="data:audio/wav;base64,UklGRnoGAABXQVZFZm10IBAAAAABAAEAQB8AAEAfAAABAAgAZGF0YQoGAACBhYqFbF1fdJivrJBhNjVgodDbq2EcBj+a2/LDciUFLIHO8tiJNwgZaLvt559NEAxQp+PwtmMcBjiR1/LMeSwFJHfH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/LDeSFHOH8N2QQAoUXrTp66hVFApGn+DyvmwhBSq+2/L
