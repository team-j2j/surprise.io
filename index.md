<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surprise for You</title>
    <style>
        body { font-family: 'Arial', sans-serif; background-color: #222; color: #f5f5f5; text-align: center; padding-top: 50px; }
        h1 { font-size: 2.5em; margin-bottom: 20px; }
        .quote { font-size: 1.5em; margin-bottom: 20px; }
        .heart { width: 150px; height: 150px; position: relative; margin: 0 auto; transform: rotate(45deg); animation: rotateHeart 3s infinite linear; background-image: url('her-picture.jpg'); background-size: cover; background-position: center; }
        .heart:before, .heart:after { content: ""; width: 150px; height: 150px; border-radius: 50%; background: transparent; border: 5px solid #ff0047; position: absolute; }
        .heart:before { top: -75px; left: 0; }
        .heart:after { left: 75px; top: 0; }
        @keyframes rotateHeart { 0% { transform: rotate(0deg) rotate(45deg); } 100% { transform: rotate(360deg) rotate(45deg); } }
    </style>
</head>
<body>
    <h1>For You, My Love</h1>
    <div class="quote">"Your favorite quote will go here."</div>
    <div class="heart"></div>
    <audio autoplay>
        <source src="background-music.mp4" type="audio/mp4">
        Your browser does not support the audio element.
    </audio>
</body>
</html>

