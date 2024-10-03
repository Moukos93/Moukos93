<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chaîne TV DiMADRAMAMCN</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #000;
            color: #fff;
            margin: 0;
        }
        iframe {
            width: 80%;
            height: 80%;
        }
    </style>
</head>
<body>
    <iframe id="video" src="" frameborder="0" allowfullscreen></iframe>
    <script>
        const videos = [
            "https://www.youtube.com/embed/AIeEqQfMNwI",
            "https://www.youtube.com/embed/wQ7OP6gEl_s",
            "https://www.youtube.com/embed/n9SH9KZ5C6U",
            "https://www.youtube.com/embed/ugB_vPlZK3E",
            "https://www.youtube.com/embed/o_EoE_8L2Dg",
            "https://www.youtube.com/embed/X3ZtKfNP1Dg",
            "https://www.youtube.com/embed/e0ySB6hnp2U",
            "https://www.youtube.com/embed/8g6Iw3aNIHg",
            "https://www.youtube.com/embed/J_2T0kZQQjI",
            "https://www.youtube.com/embed/AuH1KHMba1w"
        ];

        function getRandomVideo() {
            const randomIndex = Math.floor(Math.random() * videos.length);
            document.getElementById('video').src = videos[randomIndex];
        }

        window.onload = getRandomVideo;
    </script>
</body>
</html>
