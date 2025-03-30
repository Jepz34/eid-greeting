# eid-greeting
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
        }
        p {
            font-size: 1.2em;
            max-width: 80%;
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
    </style>
</head>
<body>
    <h1>Selamat Idul Fitri! 🌙✨</h1>
    <p>Taqabbalallāhu minnā wa minkum. Semoga hari yang fitri ini membawa kebahagiaan, keberkahan, dan kedamaian untuk kita semua! 😊</p>
    <button class="btn" onclick="shareMessage()">Bagikan Ucapan</button><script>
    function shareMessage() {
        const message = "Selamat Idul Fitri! 🌙✨\nTaqabbalallāhu minnā wa minkum. Semoga hari ini membawa kebahagiaan dan berkah untuk kita semua! ";
        if (navigator.share) {
            navigator.share({ text: message });
        } else {
            alert("Salin pesan ini dan bagikan ke teman-teman!\n\n" + message);
        }
    }
</script>

</body>
</html>
