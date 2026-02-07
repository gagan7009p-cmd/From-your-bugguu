<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Kakkuu ❤️</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Orbitron:wght@500&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        /* --- PREMIUM CSS --- */
        :root {
            --primary: #ff0040; /* Deep Neon Red */
            --dark: #0a0a0a;
            --glass: rgba(255, 255, 255, 0.1);
            --border: rgba(255, 255, 255, 0.2);
            --glow: 0 0 20px rgba(255, 0, 64, 0.5);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            background-color: var(--dark);
            color: white;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
            background-image: radial-gradient(circle at 50% 50%, #2a000d 0%, #000 100%);
        }

        /* FLOATING HEARTS BACKGROUND */
        .bg-hearts {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            pointer-events: none;
            z-index: 0;
            overflow: hidden;
        }
        .heart-bg {
            position: absolute;
            color: var(--primary);
            opacity: 0.3;
            animation: floatUp linear infinite;
        }

        @keyframes floatUp {
            0% { transform: translateY(100vh) scale(0.5); opacity: 0; }
            50% { opacity: 0.5; }
            100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
        }

        /* --- SECTIONS --- */
        section {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
            z-index: 2;
            padding: 20px;
            text-align: center;
        }

        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 4rem;
            color: var(--primary);
            text-shadow: var(--glow);
            line-height: 1.2;
        }
        
        p {
            font-size: 1.1rem;
            color: #ddd;
            max-width: 600px;
            margin: 10px auto;
            line-height: 1.6;
        }

        /* GLASS CARDS */
        .glass-card {
            background: var(--glass);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid var(--border);
            border-radius: 20px;
            padding: 30px;
            margin: 20px;
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
            max-width: 90%;
            width: 500px;
        }

        /* ENTRANCE */
        #entrance {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: #000;
            z-index: 1000;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
        .enter-btn {
            background: linear-gradient(45deg, #ff0040, #ff4d79);
            border: none;
            padding: 15px 40px;
            color: white;
            font-size: 1.2rem;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: var(--glow);
            transition: transform 0.3s;
            font-family: 'Orbitron', sans-serif;
        }
        .enter-btn:hover { transform: scale(1.1); }

        /* GALLERY CAROUSEL (Simple Scroll) */
        .gallery-scroll {
            display: flex;
            overflow-x: auto;
            gap: 20px;
            padding: 20px;
            width: 100%;
            max-width: 800px;
            scrollbar-width: none; /* Firefox */
        }
        .gallery-scroll::-webkit-scrollbar { display: none; }
        .photo-card {
            min-width: 200px;
            height: 300px;
            background: #222;
            border-radius: 15px;
            border: 2px solid var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            color: #555;
            flex-shrink: 0;
            background-size: cover;
            background-position: center;
        }

        /* INTERACTIVE BUTTONS */
        .btn-container { display: flex; gap: 20px; margin-top: 30px; justify-content: center; position: relative; }
        .yes-btn {
            background: #2ecc71; color: white; padding: 15px 40px; border: none; border-radius: 10px; font-weight: bold; font-size: 1.2rem; cursor: pointer;
        }
        .no-btn {
            background: #e74c3c; color: white; padding: 15px 40px; border: none; border-radius: 10px; font-weight: bold; font-size: 1.2rem; cursor: pointer; position: relative;
        }

        /* FINAL MESSAGE */
        .highlight-text {
            background: -webkit-linear-gradient(#fff, #ffafbd);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: bold;
            font-size: 1.3rem;
        }
    </style>
</head>
<body>

    <video id="bg-music" loop playsinline style="display:none;">
        <source src="https://files.catbox.moe/YOUR_LINK_HERE.mp4" type="video/mp4">
    </video>

    <div id="entrance">
        <h2 style="font-family:'Great Vibes'; font-size:3rem; color:var(--primary);">For Gagan's Love</h2>
        <p>Tap to enter our world...</p>
        <br>
        <button class="enter-btn" onclick="startJourney()">START ❤️</button>
    </div>

    <div class="bg-hearts" id="heart-container"></div>

    <section>
        <div data-aos="zoom-in" data-aos-duration="1500">
            <h1 id="typewriter"></h1>
            <p style="margin-top:20px; letter-spacing: 2px;">SCROLL DOWN SLOWLY</p>
            <div style="font-size:2rem; margin-top:20px; animation: bounce 2s infinite;">🌹</div>
        </div>
    </section>

    <section>
        <div class="glass-card" data-aos="fade-up">
            <h2 style="color: var(--primary);">My Gulabo 🌹</h2>
            <br>
            <p>You are not just my girlfriend...</p>
            <p>You are my <b>Happy Place.</b></p>
            <p>Happy Rose Day Myy Loveee!</p>
        </div>
    </section>

    <section>
        <div class="glass-card" data-aos="flip-left">
            <h2>I got you something...</h2>
            <p>(Tap the box)</p>
            <div style="font-size:5rem; cursor:pointer; margin:20px;" onclick="this.innerHTML='🥀'; document.getElementById('joke').style.display='block';">🎁</div>
            <h3 id="joke" style="display:none; color:var(--primary); margin-top:10px;">Phool for myy fool ! 😜<br><span style="font-size:1rem; color:white;">(Just kidding, love you!)</span></h3>
        </div>
    </section>

    <section>
        <h2 data-aos="fade-down">Us Moments ✨</h2>
        <div class="gallery-scroll" data-aos="fade-right">
            <div class="photo-card" style="background-image: url('https://via.placeholder.com/200x300/ff0040/fff?text=Photo+1');">1</div>
            <div class="photo-card" style="background-image: url('https://via.placeholder.com/200x300/ff0040/fff?text=Photo+2');">2</div>
            <div class="photo-card" style="background-image: url('https://via.placeholder.com/200x300/ff0040/fff?text=Photo+3');">3</div>
            <div class="photo-card" style="background-image: url('https://via.placeholder.com/200x300/ff0040/fff?text=Photo+4');">4</div>
        </div>
        <p>Swipe to see more &rarr;</p>
    </section>

    <section>
        <h2 data-aos="zoom-in">Will you be mine forever?</h2>
        <div class="btn-container">
            <button class="yes-btn" onclick="celebrate()">YES! 😍</button>
            <button class="no-btn" id="noBtn" onmouseover="moveNo()" onclick="moveNo()">NO 😤</button>
        </div>
    </section>

    <section>
        <div class="glass-card" data-aos="fade-up" style="border: 2px solid var(--primary);">
            <h2 style="font-family:'Great Vibes';">My Promise</h2>
            <br>
            <p class="highlight-text">
                "Myy kakkuu now keep aside all the negative things and tensions, just smile for a while myy loveee... everything will be fine smjhe mere kakkee?"
            </p>
            <br>
            <p>🫂🫂😁🧿💖😚❤️</p>
            <br>
            <p style="font-size:0.8rem; color:#888;">Forever yours, Gagan</p>
        </div>
    </section>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    
    <script>
        // 1. Initialize Animations
        AOS.init({ duration: 1200 });

        // 2. Start Journey (Music & Typewriter)
        function startJourney() {
            document.getElementById('entrance').style.opacity = '0';
            setTimeout(() => { document.getElementById('entrance').style.display = 'none'; }, 1000);
            
            // Play Music
            var video = document.getElementById("bg-music");
            video.muted = false;
            video.play().catch(e => console.log(e));

            // Start Typewriter Effect
            typeWriter();
        }

        // Typewriter Logic
        const text = "Happy Rose Day Myy Loveee...";
        let i = 0;
        function typeWriter() {
            if (i < text.length) {
                document.getElementById("typewriter").innerHTML += text.charAt(i);
                i++;
                setTimeout(typeWriter, 100);
            }
        }

        // 3. Floating Hearts Background
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart-bg');
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.animationDuration = Math.random() * 3 + 5 + "s";
            heart.style.fontSize = Math.random() * 20 + 10 + "px";
            document.getElementById('heart-container').appendChild(heart);
            setTimeout(() => { heart.remove(); }, 8000);
        }
        setInterval(createHeart, 500);

        // 4. Runaway No Button
        function moveNo() {
            const btn = document.getElementById("noBtn");
            const x = Math.random() * 200 - 100;
            const y = Math.random() * 200 - 100;
            btn.style.transform = `translate(${x}px, ${y}px)`;
        }

        // 5. Celebration Confetti
        function celebrate() {
            confetti({
                particleCount: 150,
                spread: 70,
                origin: { y: 0.6 },
                colors: ['#ff0040', '#ffffff']
            });
            alert("I knew it! Love you loads! ❤️");
        }
    </script>
</body>
</html>
