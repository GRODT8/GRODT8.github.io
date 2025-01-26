# GRODT8.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GRODT - Get Rich or Die Trying</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body, html {
            height: 100%;
            font-family: Arial, sans-serif;
            overflow: hidden;
        }
        .video-container {
            position: relative;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }
        .video-container video {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
        }
        .overlay h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        .overlay p {
            font-size: 1.5rem;
        }
        .enter-site {
            margin-top: 2rem;
            padding: 0.75rem 2rem;
            font-size: 1rem;
            color: black;
            background: white;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        .enter-site:hover {
            background: #ddd;
        }
    </style>
</head>
<body>
    <div class="video-container">
        <video autoplay muted loop>
            <source src="https://cdn.pixabay.com/vimeo/848921033/Grey%20City%20Streetwear%20Fashion%20Ad.mp4?width=1920&hash=123" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        <div class="overlay">
            <h1>GRODT</h1>
            <p>Get Rich or Die Trying</p>
            <button class="enter-site" onclick="enterSite()">Enter Site</button>
        </div>
    </div>

    <script>
        function enterSite() {
            window.location.href = "shop.html";
        }
    </script>
</body>
</html>
