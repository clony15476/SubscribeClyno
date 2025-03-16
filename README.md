<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unlock Script</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #111, #222);
            color: #fff;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
        }
        .container {
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            width: 90%;
            max-width: 400px;
            box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.2);
        }
        h3 {
            font-size: 18px;
            color: #ddd;
            margin-bottom: 5px;
        }
        h2 {
            color: #ffcc00;
            margin-top: 0;
        }
        .actions {
            margin-top: 20px;
        }
        .actions button {
            display: block;
            width: 100%;
            margin: 10px 0;
            padding: 12px;
            font-size: 16px;
            background: #ffcc00;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        .actions button:hover {
            background: #ffaa00;
        }
        .lock-btn {
            background: green;
            color: white;
            padding: 12px;
            width: 100%;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            display: none;
            font-size: 16px;
            transition: 0.3s;
        }
        .lock-btn:hover {
            background: darkgreen;
        }
    </style>
</head>
<body>
    <div class="container">
        <h3>كلينو | Cleano</h3>
        <h2>🎸 سكربت بلوكس فروت 🔓</h2>
        <p>قم بتنفيذ المهام لفتح الرابط</p>
        <div class="actions">
            <button id="subscribeBtn">✅ اشترك في القناة</button>
            <button id="likeBtn">👍 أعجب بالفيديو</button>
        </div>
        <button class="lock-btn" id="unlockBtn" onclick="window.location.href='https://www.mediafire.com/file/q031ugb3mvw4w80/krnl+Blox+Fruit+663.apk/file'">🔓 فتح الرابط</button>
    </div>

    <script>
        let subscribed = false;
        let liked = false;

        function checkUnlock() {
            if (subscribed && liked) {
                document.getElementById("unlockBtn").style.display = "block";
            }
        }

        document.getElementById("subscribeBtn").addEventListener("click", function() {
            subscribed = true;
            this.innerText = "✅ تم الاشتراك";
            this.style.background = "gray";
            this.disabled = true;
            window.open("https://www.youtube.com/@ClynoMun/channel/YOUR_CHANNEL_ID", "_blank");
            checkUnlock();
        });

        document.getElementById("likeBtn").addEventListener("click", function() {
            liked = true;
            this.innerText = "✅ تم الإعجاب";
            this.style.background = "gray";
            this.disabled = true;
            window.open("https://youtu.be/jloxxqlKDTo?si=ta4bJABARqT631Ei/watch?v=YOUR_VIDEO_ID", "_blank");
            checkUnlock();
        });
    </script>
</body>
</html>
