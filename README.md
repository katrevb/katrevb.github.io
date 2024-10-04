# katrevb.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HOME</title>

    <link href="https://fonts.googleapis.com/css2?family=Abril+Fatface&display=swap" rel="stylesheet">
    <style>
        @font-face {
            font-family: 'Marvel';
            src: url('E:\Websites\homepage\Marvel-Regular.ttf') format('truetype');
            font-weight: normal;
            font-style: normal;
        }

        body {
            font-family: 'Helvetica', sans-serif;
            color: #aa1616;
            margin: 0;
            padding: 0;
            text-align: center;
            position: relative;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            background-image: url("marvelerflare.com_wallpaper.jpg");
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            background-repeat: no-repeat;
        }

        .background-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(27, 27, 27, 0.6);
            z-index: -1;
        }

        header {
            background-color: #e23636;
            color: white;
            padding: 20px;
            font-size: 2.5rem;
            font-weight: bold;
            text-align: center;
            width: 100%;
            position: relative;
            font-family: 'Marvel', sans-serif;
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.3);
        }

        .menu-toggle {
            cursor: pointer;
            font-size: 2rem;
            background-color: transparent;
            color: white;
            border: none;
            position: absolute;
            left: 20px;
            top: 13px;
            z-index: 1;
        }

        nav {
            background-color: #504a4a;
            color: #f78f3f;
            width: 250px;
            height: 100vh;
            position: fixed;
            left: -250px;
            transition: left 0.3s ease;
            padding-top: 60px;
            box-shadow: 2px 0 5px rgba(0, 0, 0, 0.2);
            z-index: 2;
        }

        nav a {
            color: white;
            padding: 15px 20px;
            display: block;
            text-decoration: none;
            transition: background 0.3s ease;
        }

        nav a:hover {
            background-color: #518cca;
            color: #f78f3f;
        }

        .close-btn {
            cursor: pointer;
            font-size: 1.5rem;
            color: white;
            background: none;
            border: none;
            position: absolute;
            top: 20px;
            right: 20px;
        }

        section {
            font-family: 'Marvel', sans-serif;
            margin-top: 50px;
            padding: 40px;
            font-size: 3rem;
            line-height: 1.6;
            color: #FFDF00;
            text-align: center;
            align-items: center;
            display: flex;
            flex-direction: column;
            flex: 1;
            text-shadow: 0 3px 8px rgba(0, 0, 0, 0.3);
        }

        .hero-banner {
            position: relative;
            margin: 20px 0;
            height: 600px;
            overflow: hidden;
        }

        .banner-text {
            font-family: 'Abril Fatface', sans-serif;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: #FFDF00;
            font-size: 7rem;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
            z-index: 1;
        }

        .hero-banner img {
            max-width: 100%;
            max-height: 100%;
            object-fit: cover;
        }

        .trailer-button {
            position: absolute;
            bottom: 75px;
            left: 50%;
            transform: translateX(-50%);
            padding: 15px 30px;
            background-color: #131212;
            color: white;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            z-index: 1;
            border-radius: 5px;
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.3);
        }

        .featured-movies, .news, .characters {
            margin-top: 40px;
        }

        .movie-grid {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        .movie-card {
            margin: 15px;
            width: 250px;
            text-align: center;
            position: relative;
        }

        .movie-card img {
            width: 100%;
            height: auto;
            cursor: pointer;
        }

        .movie-card h3 {
            opacity: 0;
            transition: opacity 0.3s, font-size 0.3s;
            font-size: 1.5rem;
        }

        .movie-card:hover h3 {
            opacity: 1;
            font-size: 1.4rem;
        }

        footer {
            background-color: #504a4a;
            color: white;
            padding: 20px;
            font-size: 0.9rem;
            text-align: center;
            position: relative;
            margin-top: 50px;
            box-shadow: 0 -4px 12px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>
    <div class="background-overlay"></div>

    <header>
        <button class="menu-toggle" onclick="toggleMenu()">&#9776;</button>
        MARVEL
    </header>

    <nav id="sidebar">
        <button class="close-btn" onclick="toggleMenu()">&times;</button>
        <a href="homepage.html">Home</a>
        <a href="aboutme.html">About</a>
        <a href="contactme.html">Contact</a>
    </nav>

    <section class="hero-banner">
        <div class="banner-text">Marvel Cinematic Universe</div>
        <img src="wp7718470-marvel-for-pc-wallpapers.jpg" alt="Marvel Banner">
        <button class="trailer-button">Watch Trailer</button>
    </section>

    <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-grid">
            <div class="movie-card">
                <a href="https://en.wikipedia.org/wiki/Captain_America:_The_Winter_Soldier" target="_blank">
                    <img src="captain_america_the_winter_soldier_ver7.jpg" alt="Captain America: The Winter Soldier Poster">
                </a>
                <h3>Captain America: The Winter Soldier</h3>
            </div>
            <div class="movie-card">
                <a href="https://en.wikipedia.org/wiki/Black_Widow_(film)" target="_blank">
                    <img src="black_widow_ver9.jpg" alt="Black Widow Poster">
                </a>
                <h3>Black Widow</h3>
            </div>
            <div class="movie-card">
                <a href="https://en.wikipedia.org/wiki/Spider-Man:_Homecoming" target="_blank">
                    <img src="spiderman_homecoming.jpg" alt="Spider-Man: Homecoming Poster">
                </a>
                <h3>Spider-Man: Homecoming</h3>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Marvel Movies. All Rights Reserved.</p>
        <nav>
            <a href="#">About Us</a>
            <a href="#">Contact Us</a>
        </nav>
    </footer>

    <script>
        function toggleMenu() {
            const sidebar = document.getElementById('sidebar');
            if (sidebar.style.left === '0px') {
                sidebar.style.left = '-250px';
            } else {
                sidebar.style.left = '0px';
            }
        }
    </script>
</body>
</html>

