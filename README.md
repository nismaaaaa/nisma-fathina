<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biografi Nisma</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #ffb6c1;
            color: #333;
            text-align: center;
        }
        header {
            background: url('background-image.jpg') no-repeat center center/cover;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
            position: relative;
        }
        nav {
            position: absolute;
            top: 50px;
            left: 50%;
            transform: translateX(-50%);
        }
        nav a {
            font-family: 'Poppins', sans-serif;
            font-size: 2em;
            font-weight: 700;
            text-transform: uppercase;
            color: white;
            text-decoration: none;
        }
        nav a:hover {
            color: #ff69b4;
        }
        .profile-pic-container {
            width: 220px;
            height: 220px;
            border: 5px solid #ff69b4;
            border-radius: 50%;
            padding: 5px;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            overflow: hidden;
        }
        .profile-pic {
            width: 100%;
            height: auto;
            border-radius: 50%;
        }
        h1 {
            font-size: 3em;
            margin: 0;
        }
        .next-button {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #ff69b4;
            color: white;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            font-size: 16px;
            text-decoration: none; /* Menghilangkan garis bawah */
        }
        .next-button:hover {
            background: #ff1493;
            color: white;
            transform: scale(1.1);
        }
    </style>
</head>
<body>
    <div class="container active" id="home">
        <header>
            <nav>
                <a href="#">BIOGRAFI NISMA</a>
            </nav>
            <div class="profile-pic-container">
                <img src="foto nisma.jpg" alt="Foto Nisma" class="profile-pic">
            </div>
            <h2>Jejak kehidupan</h2>
            <h1>Langkah Kecil Mimpi Besar</h1>
            <p>Jelajahi Kisahku</p>
            <a href="nisma2.html" class="next-button">Explore</a>
        </header>
    </div>

    <div class="container" id="about">
        <header>
            <h1>✨ Welcome to My Story! 📖 💖</h1>
        </header>
        <div class="content">
            <div class="highlight-box">
                <h2>👋 Halo, Aku Nisma!</h2>
                <p>Berumur 20 tahun, anak kedua dari dua bersaudara! Saat ini menempuh pendidikan di Universitas Tadulako, Program Studi Sistem Informasi.</p>
            </div>
            <button class="nav-button" onclick="showPage('home')">Back</button>
            <button class="nav-button" onclick="showPage('education')">Next</button>
        </div>
    </div>

    <div class="container" id="education">
        <header>
            <h1>🎓 Education 🎓</h1>
        </header>
        <div class="content">
            <div class="highlight-box">
                <p>📚 SDN 5 Sindue (2011-2017)</p>
                <p>🏫 MTs Muhammadiyah Watulimo (2017-2020)</p>
                <p>🎓 SMK Yadika Palu (2020-2023)</p>
            </div>
        </div>
        <button class="nav-button" onclick="showPage('about')">Back</button>
        <button class="nav-button" onclick="showPage('experience')">Next</button>
    </div>

    <div class="container" id="experience">
        <header>
            <h1>Experience</h1>
        </header>
        <div class="content">
            <p>Koordinator Konsumsi di Dies Natalis HMTI, Volunteer di Pekan Raya Mosinggani.</p>
        </div>
        <button class="nav-button" onclick="showPage('education')">Back</button>
        <button class="nav-button" onclick="showPage('contact')">Next</button>
    </div>

    <div class="container" id="contact">
        <header>
            <h1>Contact Me</h1>
        </header>
        <div class="content">
            <p>📧 Email: nisma2201@gmail.com<br>📱 WhatsApp: +62 813 5655 3484<br>📷 Instagram: @nisma_fathina01</p>
        </div>
        <button class="nav-button" onclick="showPage('experience')">Back</button>
    </div>

    <script>
        function showPage(pageId) {
            document.querySelectorAll('.container').forEach(page => page.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');
        }
    </script>
</body>
</html>
