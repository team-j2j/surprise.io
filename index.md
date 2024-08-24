
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surprise for You</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #ff4b2b, #ff416c); /* Gradient background */
            color: #f5f5f5;
            text-align: center;
            padding: 50px;
            margin: 0;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-out;
        }
        .quote, .quote-second {
            font-size: 1.5em;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-out;
            opacity: 1; /* Ensure text stays visible */
        }
        .quote-second {
            animation: fadeIn 2s ease-out 1s; /* Delayed fade-in for the second quote */
        }
        .heart, .heart-stable {
            width: 200px;
            height: 200px;
            position: relative;
            margin: 0 auto;
            background: transparent;
            margin-bottom: 20px;
        }
        .heart {
            transform: rotate(45deg);
            animation: rotateHeart 4s infinite linear;
        }
        .heart:before, .heart:after {
            content: "";
            width: 200px;
            height: 200px;
            border-radius: 50%;
            background: transparent;
            border: 10px solid #ff0047; /* Neon red */
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
            width: 200px;
            height: 200px;
            background-image: url('her.jpg'); /* Add your image here */
            background-size: cover;
            background-position: center;
            position: absolute;
            top: 0;
            left: 0;
            border-radius: 50%;
        }
        .heart-stable {
            border: 10px solid #ff0047; /* Neon red */
            border-radius: 50%;
            background: transparent;
        }
        .heart-stable-inner {
            width: 100%;
            height: 100%;
            background-image: url('songs/pic.jpg'); /* Same image or different */
            background-size: cover;
            background-position: center;
            border-radius: 50%;
        }
        @keyframes rotateHeart {
            0% { transform: rotate(0deg) rotate(45deg); }
            100% { transform: rotate(360deg) rotate(45deg); }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        audio {
            display: none; /* Hide the audio player */
        }
    </style>
</head>
<body>
    <h1>For You, Ms Jyoti Ji</h1>
    <div class="quote">Jyoti, you are really special to me, and I can’t thank you enough. Just being you is more than enough for me. Remember, the journey ahead may be challenging, but every step you take is a step closer to your goals. Stay consistent and keep pushing forward—success is just around the corner. Believe in yourself, and you will conquer every obstacle. Good luck with your placements! Stay focused and keep going strong." ~ Legend Jatin Kalal</div>
    <div class="heart">
        <div class="heart-inner"></div>
    </div>
    <div class="heart-stable">
        <div class="heart-stable-inner"></div>
    </div>
    <div class="quote-second">"Another heartfelt message goes here. You always look good, so keep up that smile, looking forward to have more trips with you, you still have no idea what all can i do still for you, for now lets keep it as surpise, my mind is constantly in how to surpise you and also dont forget about making reels, but anyway missing you a lot...."</div>
    <audio autoplay>
        <source src="songs/song.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
</body>
</html>
