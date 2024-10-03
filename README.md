<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chaîne TV Aléatoire</title>
</head>
<body>
    <h1>Chaîne TV Aléatoire</h1>
    <div id="player"></div>

    <script>
        // Liste des vidéos YouTube de la chaîne DiMADRAMAMCN
        var videoUrls = [
            'L6TwtJFCeXs', // ID de la vidéo 1
            'fCSjNbtqYgA', // ID de la vidéo 2
            'DA0HWWcWvOk', // ID de la vidéo 3
            'Wzj6TjD-8yo', // ID de la vidéo 4
            'H4ed7hJHY3k'  // ID de la vidéo 5
        ];

        // Choisir une vidéo aléatoire
        var randomVideoId = videoUrls[Math.floor(Math.random() * videoUrls.length)];

        // Charger la vidéo dans le lecteur YouTube
        var player;
        function onYouTubeIframeAPIReady() {
            player = new YT.Player('player', {
                height: '390',
                width: '640',
                videoId: randomVideoId,
            });
        }

        // Charger l'API YouTube Iframe
        var tag = document.createElement('script');
        tag.src = "https://www.youtube.com/iframe_api";
        var firstScriptTag = document.getElementsByTagName('script')[0];
        firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
    </script>
</body>
</html>
