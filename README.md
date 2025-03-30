<!DOCTYPE html><html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Idul Fitri!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: linear-gradient(to right, #ffcc00, #ff6699);
            color: white;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            transition: transform 0.3s ease-in-out;
        }
        p {
            font-size: 1.2em;
            max-width: 80%;
            display: none;
            transition: opacity 0.5s ease-in-out;
        }
        .btn {
            margin-top: 20px;
            padding: 10px 20px;
            background: white;
            color: #ff6699;
            border: none;
            border-radius: 5px;
            font-size: 1em;
            cursor: pointer;
            transition: 0.3s;
        }
        .btn:hover {
            background: #ffcc00;
            color: white;
        }
        .big-text {
            transform: scale(1.5);
        }
        .visible {
            display: block;
            opacity: 1;
        }
    </style>
</head>
<body>
    <h1 id="greeting">Selamat Idul Fitri! 🌙✨</h1>
    <p id="message">Taqabbalallāhu minnā wa minkum. Semoga hari yang fitri ini membawa kebahagiaan, keberkahan, dan kedamaian untuk kita semua! 😊💖</p>
    <button class="btn" onclick="showGreeting()">Klik untuk Ucapan Spesial</button><script>
    function showGreeting() {
        const greeting = document.getElementById("greeting");
        const message = document.getElementById("message");
        greeting.classList.toggle("big-text");
        message.classList.toggle("visible");
    }
</script>

</body>
</html>
