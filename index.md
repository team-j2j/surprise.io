<!DOCTYPE html>
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
        .heart, .heart-stable-container {
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
        .heart-stable-container {
            display: flex;
            justify-content: center;
            gap: 20px; /* Space between hearts */
            margin-bottom: 20px;
        }
        .heart-stable {
            border: 10px solid #ff0047; /* Neon red */
            border-radius: 50%;
            background: transparent;
            width: 150px; /* Adjusted size */
            height: 150px; /* Adjusted size */
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
        }
        .heart-stable-inner {
            width: 140px; /* Slightly smaller than the border to fit well */
            height: 140px; /* Same size as width */
            background-size: cover;
            background-position: center;
            border-radius: 50%;
            position: absolute;
            top: 5px; /* Adjust to fit nicely */
            left: 5px; /* Adjust to fit nicely */
        }
        .heart-stable:nth-child(1) .heart-stable-inner {
            background-image: url('songs/pic.jpg'); /* First image */
        }
        .heart-stable:nth-child(2) .heart-stable-inner {
            background-image: url('songs/pic2.jpeg'); /* Second image */
        }
        .heart-stable:nth-child(3) .heart-stable-inner {
            background-image: url('songs/pic3.jpeg'); /* Third image */
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
    <div class="heart-stable-container">
        <div class="heart-stable">
            <div class="heart-stable-inner"></div>
        </div>
        <div class="heart-stable">
            <div class="heart-stable-inner"></div>
        </div>
        <div class="heart-stable">
            <div class="heart-stable-inner"></div>
        </div>
    </div>
    <div class="quote-second">"Another heartfelt message goes here. You always look good, so keep up that smile, looking forward to having more trips with you. You still have no idea what all I can do for you, for now, let's keep it a surprise. My mind is constantly in how to surprise you and also don't forget about making reels, but anyway missing you a lot...."</div>
    <audio autoplay>
        <source src="songs/song.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
</body>
</html>
