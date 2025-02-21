<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Telefoningiz kuzatuv ostida! 😱</title>
    <style>
        body {
            background-color: black;
            color: red;
            font-family: 'Courier New', Courier, monospace;
            font-size: 20px;
            padding: 20px;
            animation: flicker 1.5s infinite alternate;
        }
        
        @keyframes flicker {
            0% { opacity: 1; }
            50% { opacity: 0.5; }
            100% { opacity: 1; }
        }

        #output {
            white-space: pre-line;
            font-size: 22px;
        }
    </style>
</head>
<body>
    <div id="output"></div>

    <script>
        const messages = [
            "📡 Telefoningizga ulanish...",
            "🔍 Kamera faollashmoqda...",
            "📂 Galereya skanerlash...",
            "📨 Telegram yozishmalarini ochish...",
            "🧾 Click va Payme hisoblarini tekshirish...",
            "⚠️ OG'OH BO'LING! Telefoningiz nazorat ostida! 😱",
            "💻 Sizning barcha ma'lumotlaringiz bizda!",
            "🔒 Xavfsizlik kodlaringizni qidirmoqda...",
            "🚨 Xavf! Telefoningizda sizni kuzatib borayotgan noma'lum shaxs bor!",
            "📡 Telefoningizning GPS joylashuvi aniqlanmoqda...",
            "📞 Hozirgi vaqtda kimdir sizni tinglamoqda...",
            "⚠️ OG'OH BO'LING! Telefoningizdan uzilishga juda kech!",
            "😱 BU YERDA XAVFLI! Xato! Telefoningizni tezda o'chirib qo'ying!",
            "💀 Telefoningizda hech qanday xavfsizlik yo'q. Sizning barcha ma'lumotlaringiz bizning qo'limizda!"
        ];

        let index = 0;
        function showMessage() {
            if (index < messages.length) {
                document.getElementById("output").innerHTML += messages[index] + "<br>";
                index++;
                setTimeout(showMessage, 1500);  // Уменьшаем задержку, чтобы ускорить появление сообщений
            }
        }

        showMessage();
    </script>
</body>
</html>
