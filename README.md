<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swagat Kumar Mishra | Profile</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            /* Purple-Red "Inferno" Color Palette */
            --gradient-1: #ff2a6d; /* Vibrant Crimson Red */
            --gradient-2: #6c00f7; /* Deep Electric Purple */
            --gradient-3: #c002f0; /* Hot Magenta/Pink */
            --bg-color: #0a0211;   /* Deep Purple-Tinted Black */
        }

        /* Basic Reset and Body Styling */
        * {
            margin: 0; padding: 0; box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            display: flex; justify-content: center; align-items: center;
            min-height: 100vh; padding: 20px;
            overflow: hidden;
            background-color: var(--bg-color);
            color: #e0e0e0;
        }

        /* Enhanced Aurora Background Animation */
        .aurora {
            position: absolute; top: 0; left: 0; width: 100%; height: 100%;
            z-index: -1; filter: blur(150px) saturate(1.8); opacity: 0.7;
        }
        .aurora div {
            position: absolute; border-radius: 50%; animation: move 40s ease-in-out infinite;
        }
        .aurora .d1 { width: 380px; height: 380px; background: var(--gradient-2); top: -10%; left: 20%; }
        .aurora .d2 { width: 480px; height: 480px; background: var(--gradient-1); bottom: -15%; right: 10%; animation-duration: 50s; }
        .aurora .d3 { width: 250px; height: 250px; background: var(--gradient-3); bottom: 25%; left: 15%; animation-duration: 30s; animation-direction: reverse;}

        @keyframes move {
            0%, 100% { transform: rotate(0deg) scale(1) translate(0px, 0px); }
            50% { transform: rotate(180deg) scale(1.4) translate(-40px, 60px); }
        }
        
        /* The Main Profile Card */
        .profile-card {
            position: relative;
            background: rgba(25, 25, 40, 0.7);
            padding: 50px; max-width: 480px; width: 100%;
            border-radius: 28px;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(30px);
            text-align: center;
            transform-style: preserve-3d;
            transform: perspective(1000px);
            transition: transform 0.1s linear;
            overflow: hidden;
            opacity: 0;
            animation: fadeInCard 0.8s cubic-bezier(0.25, 1, 0.5, 1) 0.2s forwards;
        }
        
        .profile-card::before {
            content: ''; position: absolute;
            width: 150%; height: 150%; top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            background: radial-gradient(circle at var(--mouse-x) var(--mouse-y), rgba(255, 42, 109, 0.15), transparent 25%);
            opacity: 0; transition: opacity 0.4s ease;
            pointer-events: none;
        }
        
        .profile-card:hover::before { opacity: 1; }

        @keyframes fadeInCard {
            to { opacity: 1; transform: perspective(1000px) translateY(0) scale(1); }
        }

        /* Profile Picture Styling */
        .profile-pic {
            width: 150px; height: 150px;
            margin: 0 auto; /* Centered */
            border-radius: 50%;
            border: 4px solid rgba(255, 255, 255, 0.5);
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.3);
            transition: all 0.4s ease;
            transform: translateZ(60px);
            background-color: #333;
            background-image: url("https://www.dropbox.com/scl/fi/drtzekzr7cmzced2oizot/Screenshot_2025-03-24-14-02-05-595_com.miui.videoplayer.jpg?rlkey=to5fxnhdor62v3kew3mbklnxr&raw=1");
            background-size: cover; background-position: center;
            animation: popIn 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275) 1.0s backwards;
        }
        .profile-card:hover .profile-pic { border-color: #fff; transform: translateZ(60px) scale(1.05); }

        /* Name Styling with New Gradient */
        .name {
            font-size: 2.4em; font-weight: 700;
            margin: 25px 0 8px;
            letter-spacing: 0.5px;
            transform: translateZ(50px);
            background: linear-gradient(90deg, var(--gradient-1), #fff, var(--gradient-3));
            background-size: 200% auto;
            -webkit-background-clip: text; background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: text-shine 5s linear infinite, slideInUp 0.8s ease 1.2s backwards;
        }
        @keyframes text-shine { to { background-position: -200% center; } }

        /* Subtitle Styling */
        .subtitle {
            font-size: 1.15em; color: #c0c0d0; font-weight: 400;
            transform: translateZ(40px);
            animation: slideInUp 0.8s ease 1.4s backwards;
        }

        @keyframes slideInUp {
            from { opacity: 0; transform: perspective(500px) translateZ(40px) translateY(30px); filter: blur(5px); }
            to { opacity: 1; transform: perspective(500px) translateZ(40px) translateY(0); filter: blur(0); }
        }

        .divider {
            height: 1px; width: 60%; margin: 30px auto;
            background: linear-gradient(90deg, transparent, rgba(255, 42, 109, 0.3), transparent);
            border: none; transform: translateZ(30px);
            animation: slideInUp 0.8s ease 1.6s backwards;
        }

        /* Social Links Section */
        .social-links {
            display: flex; justify-content: center; gap: 25px;
            transform: translateZ(30px);
        }

        .social-btn {
            display: inline-flex; justify-content: center; align-items: center;
            width: 55px; height: 55px; border-radius: 50%;
            background: rgba(255, 255, 255, 0.08);
            color: #e0e0e0; text-decoration: none; font-size: 1.5em;
            transition: all 0.35s ease;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.25);
            animation: popIn 0.6s cubic-bezier(0.68, -0.55, 0.27, 1.55) backwards;
        }

        /* MODIFIED: Adjusted animation delays for the new sequence. */
        .social-btn.github { animation-delay: 1.8s; }
        .social-btn.game { animation-delay: 2.0s; } /* ADDED: Delay for the new game button */
        .social-btn.website { animation-delay: 2.2s; } /* MODIFIED: Pushed back the delay */


        @keyframes popIn {
            from { opacity: 0; transform: scale(0.5); } to { opacity: 1; transform: scale(1); }
        }

        .social-btn:hover {
            transform: translateY(-8px) scale(1.1);
            color: #fff;
            background: rgba(255, 255, 255, 0.15); 
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.4); 
        }

        /* Mobile Responsive Styles */
        @media (max-width: 520px) {
            .profile-card { padding: 40px 25px; gap: 20px;} /* Added gap for better spacing */
            .profile-pic { width: 120px; height: 120px; }
            .name { font-size: 2em; }
            .subtitle { font-size: 1.05em; }
            .divider { width: 70%; margin: 25px auto; }
            .social-btn { width: 50px; height: 50px; font-size: 1.4em; }
            .social-links { gap: 20px; } /* Reduced gap on mobile */
        }
    </style>
</head>
<body>

    <div class="aurora">
        <div class="d1"></div>
        <div class="d2"></div>
        <div class="d3"></div>
    </div>

    <div class="profile-card">
        <div class="profile-pic"></div>
        
        <h1 class="name">SWAGs MIs ✦</h1>
        
        <p class="subtitle">Full Stack Developer | JS, CSS, HTML</p>

        <hr class="divider">
        
        <div class="social-links">
            <a href="https://github.com/Swagat-Kumar-Mishra" target="_blank" class="social-btn github">
                <i class="fab fa-github"></i>
            </a>
            <!-- ADDED: New button for your game -->
            <a href="https://Devtictactoe.blogspot.com" target="_blank" class="social-btn game">
                <i class="fas fa-gamepad"></i>
            </a>
            <a href="https://Developermoon.my.canva.site" target="_blank" class="social-btn website">
                <i class="fas fa-globe"></i>
            </a>
        </div>
    </div>

    <script>
        const card = document.querySelector('.profile-card');

        // Check if the user is not on a touch device for the 3D tilt effect
        if (!window.matchMedia("(pointer: coarse)").matches) {
            card.addEventListener('mousemove', (e) => {
                const rect = card.getBoundingClientRect();
                const x = e.clientX - rect.left;
                const y = e.clientY - rect.top;
                const centerX = rect.width / 2;
                const centerY = rect.height / 2;
                const rotateX = (y - centerY) / 25;
                const rotateY = (centerX - x) / 25;

                card.style.transform = `perspective(1000px) rotateX(${rotateX}deg) rotateY(${rotateY}deg)`;
                card.style.setProperty('--mouse-x', `${x}px`);
                card.style.setProperty('--mouse-y', `${y}px`);
            });

            card.addEventListener('mouseleave', () => {
                card.style.transform = 'perspective(1000px) rotateX(0deg) rotateY(0deg)';
            });
        }
    </script>

</body>
</html>
