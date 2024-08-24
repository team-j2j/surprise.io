
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surprise for You</title>
    <style>
    body {
        font-family: 'Arial', sans-serif;
        background-color: #222;
        color: #f5f5f5;
        text-align: center;
        padding-top: 50px;
    }
    h1 {
        font-size: 2.5em;
        margin-bottom: 20px;
    }
    .quote {
        font-size: 1.5em;
        margin-bottom: 20px;
    }
    .heart {
        width: 150px;
        height: 150px;
        position: relative;
        margin: 0 auto;
        transform: rotate(45deg);
        animation: rotateHeart 4s infinite linear;
        background: transparent;
    }
    .heart:before, .heart:after {
        content: "";
        width: 150px;
        height: 150px;
        border-radius: 50%;
        background: transparent;
        border: 5px solid #ff0047; /* Neon red */
        position: absolute;
        top: 0;
        left: 0;
    }
    .heart:before {
        transform: scale(0.5) translate(-50%, 0);
    }
    .heart:after {
        transform: scale(0.5) translate(50%, 0);
    }
    .heart-inner {
        width: 150px;
        height: 150px;
        background-image: url('her-picture.jpg'); /* Add your image here */
        background-size: cover;
        background-position: center;
        position: absolute;
        top: 0;
        left: 0;
        border-radius: 50%;
    }
    @keyframes rotateHeart {
        0% { transform: rotate(0deg) rotate(45deg); }
        100% { transform: rotate(360deg) rotate(45deg); }
    }
    </style>
</head>
<body>
    <h1>For You, Ms Jyoti Ji</h1>
    <div class="quote">Jyoti, you are really special to me, and I can’t thank you enough. Just being you is more than enough for me. Remember, the journey ahead may be challenging, but every step you take is a step closer to your goals. Stay consistent and keep pushing forward—success is just around the corner. Believe in yourself, and you will conquer every obstacle. Prepare really well for your placements, make your parents proud, and i know you will do it, just stop thinking too much, i want to always stay by yourside. Good luck with your placements! Stay focused and keep going strong." ~ Legend Jatin Kalal</div>
    <div class="heart">
        <div class="heart-inner"></div>
    </div>
    <audio autoplay>
        <source src="background-music.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
</body>
</html>
