<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Gift For You</title>
    <style>
        body { margin: 0; height: 100vh; display: flex; align-items: center; justify-content: center; background: #0a0a0a; font-family: 'Georgia', serif; overflow: hidden; color: white; }
        #gift-container { text-align: center; cursor: pointer; transition: transform 0.3s; }
        #gift-box { font-size: 100px; transition: 0.5s; }
        .hidden { display: none; }
        #message-card { padding: 20px; max-width: 80%; background: rgba(255, 255, 255, 0.1); backdrop-filter: blur(10px); border-radius: 20px; border: 1px solid rgba(255, 215, 0, 0.3); animation: fadeIn 2s; }
        h1 { color: #ffd700; margin-bottom: 10px; font-size: 1.5rem; }
        p { line-height: 1.6; font-size: 1.1rem; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
        .hearts { position: absolute; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; }
    </style>
</head>
<body>
    <div id="gift-container" onclick="openGift()">
        <div id="gift-box">🎁</div>
        <p id="tap-text">Tap to open your 2026 surprise...</p>
        
        <div id="message-card" class="hidden">
            <h1>Happy New Year, My Love ✨</h1>
            <p>As the clock strikes midnight, I wanted you to know that you are my greatest gift. Every second with you is a treasure. Let's make 2026 our most beautiful chapter yet. I love you forever.</p>
            <p style="color: #ffd700;">❤️ Always Yours</p>
        </div>
    </div>

    <script>
        function openGift() {
            document.getElementById('gift-box').style.transform = 'scale(2) rotate(20deg)';
            document.getElementById('gift-box').style.opacity = '0';
            setTimeout(() => {
                document.getElementById('gift-box').classList.add('hidden');
                document.getElementById('tap-text').classList.add('hidden');
                document.getElementById('message-card').classList.remove('hidden');
            }, 500);
        }
    </script>
</body>
</html>
# GraphicGlimmers.github.io
