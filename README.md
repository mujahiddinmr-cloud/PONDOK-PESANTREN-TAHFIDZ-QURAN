<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pondok Pesantren Tahfidz Qur'an Qurrota A'yun - Sorong</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #1a5f3f;
            --secondary: #2d8659;
            --accent: #D4AF37;
            --dark: #0f1f17;
            --light: #f8faf9;
        }

        body {
            font-family: 'Georgia', 'Times New Roman', serif;
            line-height: 1.7;
            color: #2c3e50;
            background: var(--light);
            overflow-x: hidden;
        }

        /* NAVIGATION - Elegant Sticky */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(20px);
            z-index: 1000;
            border-bottom: 1px solid rgba(212, 175, 55, 0.2);
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.05);
            transition: all 0.3s;
        }

        nav.scrolled {
            padding: 0.5rem 0;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        }

        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 1.2rem 3rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.4rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }

        .logo-svg {
            width: 55px;
            height: 55px;
        }

        .logo-text {
            display: flex;
            flex-direction: column;
            line-height: 1.2;
        }

        .logo-main {
            font-size: 1.3rem;
            color: var(--primary);
        }

        .logo-sub {
            font-size: 0.75rem;
            color: var(--accent);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2.5rem;
            align-items: center;
        }

        .nav-menu a {
            color: var(--dark);
            text-decoration: none;
            font-weight: 500;
            font-size: 0.95rem;
            position: relative;
            padding: 0.5rem 0;
            transition: color 0.3s;
        }

        .nav-menu a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent);
            transition: width 0.3s;
        }

        .nav-menu a:hover {
            color: var(--accent);
        }

        .nav-menu a:hover::after {
            width: 100%;
        }

        .menu-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.8rem;
            color: var(--primary);
            cursor: pointer;
        }

        /* HERO - Elegant Full Screen */
        .hero {
            min-height: 100vh;
            background: linear-gradient(135deg, rgba(26, 95, 63, 0.95) 0%, rgba(45, 134, 89, 0.95) 100%),
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="rgba(212,175,55,0.1)" d="M0,96L48,112C96,128,192,160,288,160C384,160,480,128,576,122.7C672,117,768,139,864,138.7C960,139,1056,117,1152,106.7C1248,96,1344,96,1392,96L1440,96L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><path d="M50 10 L55 25 L70 25 L58 35 L63 50 L50 40 L37 50 L42 35 L30 25 L45 25 Z" fill="rgba(212,175,55,0.08)"/></svg>');
            background-size: 120px;
            opacity: 0.3;
            animation: twinkle 4s ease-in-out infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.2; }
            50% { opacity: 0.4; }
        }

        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 1000px;
            padding: 3rem 2rem;
        }

        .hero-ornament {
            font-size: 2.5rem;
            color: var(--accent);
            margin-bottom: 1.5rem;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .hero-arabic {
            font-size: 2rem;
            color: var(--accent);
            margin-bottom: 1.5rem;
            font-style: italic;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }

        .hero h1 {
            font-size: clamp(2.5rem, 5vw, 4.5rem);
            font-weight: 700;
            margin-bottom: 1rem;
            line-height: 1.2;
            text-shadow: 2px 2px 8px rgba(0,0,0,0.3);
        }

        .hero-divider {
            width: 120px;
            height: 3px;
            background: var(--accent);
            margin: 1.5rem auto;
            position: relative;
        }

        .hero-divider::before,
        .hero-divider::after {
            content: '✦';
            position: absolute;
            color: var(--accent);
            font-size: 1rem;
            top: -8px;
        }

        .hero-divider::before {
            left: -25px;
        }

        .hero-divider::after {
            right: -25px;
        }

        .hero-subtitle {
            font-size: clamp(1.2rem, 2vw, 1.6rem);
            margin-bottom: 1rem;
            opacity: 0.95;
            font-weight: 400;
        }

        .hero-location {
            font-size: 1.1rem;
            color: var(--accent);
            margin-bottom: 2.5rem;
            font-weight: 500;
        }

        .hero-buttons {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 1.2rem 2.8rem;
            text-decoration: none;
            border-radius: 8px;
            font-weight: 600;
            font-size: 1rem;
            transition: all 0.3s;
            border: 2px solid transparent;
        }

        .btn-primary {
            background: var(--accent);
            color: var(--dark);
            box-shadow: 0 8px 25px rgba(212, 175, 55, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 35px rgba(212, 175, 55, 0.4);
        }

        .btn-outline {
            background: transparent;
            color: white;
            border-color: white;
        }

        .btn-outline:hover {
            background: white;
            color: var(--primary);
        }

        /* SECTIONS */
        section {
            padding: 6rem 2rem;
            position: relative;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-tag {
            display: inline-block;
            color: var(--accent);
            font-size: 0.85rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-bottom: 1rem;
        }

        .section-title {
            font-size: clamp(2.2rem, 4vw, 3.5rem);
            color: var(--primary);
            margin-bottom: 1rem;
            font-weight: 700;
            position: relative;
            display: inline-block;
        }

        .section-subtitle {
            font-size: 1.15rem;
            color: #64748b;
            max-width: 700px;
            margin: 0 auto;
            line-height: 1.8;
        }

        .title-ornament {
            text-align: center;
            margin: 1.5rem 0;
        }

        .title-ornament span {
            color: var(--accent);
            font-size: 1.2rem;
            margin: 0 1rem;
        }

        /* ABOUT - Split Layout */
        .about-section {
            background: white;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 5rem;
            align-items: center;
        }

        .about-image-wrapper {
            position: relative;
        }

        .about-image {
            width: 100%;
            height: 550px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 8rem;
            color: var(--accent);
            box-shadow: 0 20px 60px rgba(26, 95, 63, 0.25);
            position: relative;
            overflow: hidden;
        }

        .about-image::before {
            content: '';
            position: absolute;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(212, 175, 55, 0.15) 0%, transparent 70%);
            animation: rotate 25s linear infinite;
        }

        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .about-ornament {
            position: absolute;
            font-size: 5rem;
            color: var(--accent);
            opacity: 0.15;
        }

        .about-ornament-1 {
            top: -30px;
            left: -30px;
        }

        .about-ornament-2 {
            bottom: -30px;
            right: -30px;
        }

        .about-content h3 {
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            font-weight: 700;
        }

        .about-content p {
            font-size: 1.08rem;
            line-height: 1.9;
            color: #475569;
            margin-bottom: 1.5rem;
            text-align: justify;
        }

        .about-features {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
            margin-top: 2rem;
        }

        .about-feature {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 1rem;
            background: var(--light);
            border-radius: 8px;
            border-left: 3px solid var(--accent);
        }

        .about-feature-icon {
            font-size: 1.5rem;
            color: var(--accent);
        }

        .about-feature-text {
            font-size: 0.95rem;
            color: var(--primary);
            font-weight: 600;
        }

        /* PROGRAMS - Elegant Cards */
        .programs-section {
            background: linear-gradient(to bottom, var(--light) 0%, white 100%);
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2.5rem;
        }

        .program-card {
            background: white;
            border-radius: 15px;
            padding: 3rem 2.5rem;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.08);
            transition: all 0.4s;
            text-align: center;
            border: 1px solid transparent;
            position: relative;
            overflow: hidden;
        }

        .program-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--accent));
        }

        .program-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 20px 60px rgba(26, 95, 63, 0.2);
            border-color: var(--accent);
        }

        .program-icon {
            font-size: 5rem;
            margin-bottom: 1.5rem;
            display: block;
            filter: drop-shadow(0 4px 10px rgba(0, 0, 0, 0.1));
        }

        .program-card h3 {
            font-size: 1.7rem;
            color: var(--primary);
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .program-card p {
            color: #64748b;
            line-height: 1.8;
            font-size: 1.05rem;
        }

        /* GALLERY - Elegant Grid */
        .gallery-section {
            background: white;
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
        }

        .gallery-item {
            aspect-ratio: 4/3;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: all 0.3s;
            cursor: pointer;
            position: relative;
        }

        .gallery-item::before {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            opacity: 1;
            transition: opacity 0.3s;
            z-index: 1;
        }

        .gallery-placeholder {
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
            color: var(--accent);
            position: relative;
            z-index: 2;
        }

        .gallery-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 45px rgba(26, 95, 63, 0.25);
        }

        .gallery-item:hover::before {
            opacity: 0.8;
        }

        /* FEATURES - Icon Grid */
        .features-section {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            position: relative;
        }

        .features-section::before {
            content: '';
            position: absolute;
            inset: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><path d="M50 10 L55 25 L70 25 L58 35 L63 50 L50 40 L37 50 L42 35 L30 25 L45 25 Z" fill="rgba(212,175,55,0.05)"/></svg>');
            background-size: 100px;
            opacity: 0.3;
        }

        .features-section .section-tag,
        .features-section .section-title,
        .features-section .section-subtitle {
            color: white;
        }

        .features-section .section-tag {
            color: var(--accent);
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
            position: relative;
            z-index: 1;
        }

        .feature-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 2.5rem 1.5rem;
            border-radius: 12px;
            text-align: center;
            border: 1px solid rgba(212, 175, 55, 0.3);
            transition: all 0.3s;
        }

        .feature-card:hover {
            background: rgba(255, 255, 255, 0.15);
            transform: translateY(-8px);
            border-color: var(--accent);
        }

        .feature-icon {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            display: block;
            color: var(--accent);
        }

        .feature-card h4 {
            font-size: 1.3rem;
            margin-bottom: 0.8rem;
            font-weight: 600;
        }

        .feature-card p {
            font-size: 0.95rem;
            opacity: 0.9;
        }

        /* CONTACT - Premium */
        .contact-section {
            background: var(--light);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2.5rem;
        }

        .contact-card {
            background: white;
            padding: 3rem 2.5rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.08);
            border: 1px solid rgba(212, 175, 55, 0.2);
            transition: all 0.3s;
        }

        .contact-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 50px rgba(26, 95, 63, 0.15);
            border-color: var(--accent);
        }

        .contact-icon {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            display: block;
            color: var(--accent);
        }

        .contact-card h4 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--primary);
            font-weight: 700;
        }

        .contact-card p {
            font-size: 1.05rem;
            line-height: 1.7;
            color: #64748b;
        }

        .wa-button {
            display: inline-block;
            margin-top: 1.5rem;
            padding: 1rem 2.5rem;
            background: linear-gradient(135deg, #25D366, #20ba5a);
            color: white;
            text-decoration: none;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s;
            box-shadow: 0 8px 25px rgba(37, 211, 102, 0.3);
        }

        .wa-button:hover {
            transform: scale(1.05);
            box-shadow: 0 12px 35px rgba(37, 211, 102, 0.4);
        }

        /* FOOTER */
        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 3rem 2rem;
            border-top: 3px solid var(--accent);
        }

        .footer-ornament {
            color: var(--accent);
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        footer p {
            margin-bottom: 0.5rem;
            font-size: 1rem;
            opacity: 0.9;
        }

        .footer-highlight {
            color: var(--accent);
        }

        /* FLOATING WA */
        .wa-float {
            position: fixed;
            bottom: 2rem;
            right: 2rem;
            width: 65px;
            height: 65px;
            background: linear-gradient(135deg, #25D366, #20ba5a);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.2rem;
            color: white;
            text-decoration: none;
            box-shadow: 0 8px 30px rgba(37, 211, 102, 0.5);
            z-index: 999;
            transition: all 0.3s;
            border: 3px solid white;
        }

        .wa-float:hover {
            transform: scale(1.15) rotate(5deg);
            box-shadow: 0 12px 40px rgba(37, 211, 102, 0.6);
        }

        /* RESPONSIVE */
        @media (max-width: 1024px) {
            .programs-grid,
            .features-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .gallery-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 768px) {
            .menu-toggle {
                display: block;
            }

            .nav-menu {
                display: none;
                position: fixed;
                top: 80px;
                left: 0;
                right: 0;
                background: white;
                flex-direction: column;
                padding: 2rem;
                gap: 0;
                box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
                animation: slideDown 0.3s ease;
            }

            .nav-menu.active {
                display: flex;
            }

            .nav-menu li {
                width: 100%;
                border-bottom: 1px solid rgba(0, 0, 0, 0.1);
            }

            .nav-menu li:last-child {
                border-bottom: none;
            }

            .nav-menu a {
                display: block;
                padding: 1rem 0;
            }

            .about-grid,
            .programs-grid,
            .features-grid,
            .contact-grid,
            .gallery-grid {
                grid-template-columns: 1fr;
                gap: 2rem;
            }

            .about-features {
                grid-template-columns: 1fr;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }

            section {
                padding: 4rem 1.5rem;
            }
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>

    <nav id="navbar">
        <div class="nav-container">
            <a href="#" class="logo">
                <svg class="logo-svg" viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="150" cy="150" r="148" fill="#001a3d"/>
                    <path d="M 150,20 L 170,80 L 220,50 L 200,100 L 250,120 L 200,140 L 220,190 L 170,170 L 150,220 L 130,170 L 80,190 L 100,140 L 50,120 L 100,100 L 80,50 L 130,80 Z" fill="none" stroke="#D4AF37" stroke-width="6"/>
                    <path d="M 90,70 L 95,85 L 110,85 L 98,93 L 103,108 L 90,98 L 77,108 L 82,93 L 70,85 L 85,85 Z" fill="#D4AF37"/>
                    <path d="M 210,70 L 215,85 L 230,85 L 218,93 L 223,108 L 210,98 L 197,108 L 202,93 L 190,85 L 205,85 Z" fill="#D4AF37"/>
                    <path d="M 150,40 L 155,55 L 170,55 L 158,63 L 163,78 L 150,68 L 137,78 L 142,63 L 130,55 L 145,55 Z" fill="#D4AF37"/>
                    <circle cx="155" cy="85" r="12" fill="#D4AF37"/>
                    <circle cx="160" cy="85" r="10" fill="#001a3d"/>
                    <path d="M 90,140 L 90,190 L 145,180 L 145,130 Z" fill="#D4AF37" stroke="#FFA500" stroke-width="2"/>
                    <path d="M 155,130 L 155,180 L 210,190 L 210,140 Z" fill="#D4AF37" stroke="#FFA500" stroke-width="2"/>
                    <line x1="95" y1="145" x2="140" y2="142" stroke="#001a3d" stroke-width="2"/>
                    <line x1="95" y1="155" x2="140" y2="152" stroke="#001a3d" stroke-width="2"/>
                    <line x1="95" y1="165" x2="140" y2="162" stroke="#001a3d" stroke-width="2"/>
                    <line x1="160" y1="142" x2="205" y2="145" stroke="#001a3d" stroke-width="2"/>
                    <line x1="160" y1="152" x2="205" y2="155" stroke="#001a3d" stroke-width="2"/>
                    <line x1="160" y1="162" x2="205" y2="165" stroke="#001a3d" stroke-width="2"/>
                </svg>
                <div class="logo-text">
                    <span class="logo-main">Qurrota A'yun</span>
                    <span class="logo-sub">Penyejuk Hati</span>
                </div>
            </a>
            <button class="menu-toggle" onclick="toggleMenu()">☰</button>
            <ul class="nav-menu" id="navMenu">
                <li><a href="#beranda" onclick="closeMenu()">Beranda</a></li>
                <li><a href="#tentang" onclick="closeMenu()">Tentang</a></li>
                <li><a href="#program" onclick="closeMenu()">Program</a></li>
                <li><a href="#galeri" onclick="closeMenu()">Galeri</a></li>
                <li><a href="#keunggulan" onclick="closeMenu()">Keunggulan</a></li>
                <li><a href="#kontak" onclick="closeMenu()">Kontak</a></li>
            </ul>
        </div>
    </nav>

    <section class="hero" id="beranda">
        <div class="hero-content">
            <div class="hero-ornament">☪</div>
            <div class="hero-arabic">بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيم</div>
            <h1>Pondok Pesantren Tahfidz Qur'an<br>Qurrota A'yun</h1>
            <div class="hero-divider"></div>
            <p class="hero-subtitle">Membentuk Generasi Qurani Berakhlak Mulia</p>
            <p class="hero-location">📍 Kota Sorong, Papua Barat Daya</p>
            <div class="hero-buttons">
                <a href="#kontak" class="btn btn-primary">
                    <span>Daftar Sekarang</span>
                    <span>→</span>
                </a>
                <a href="#tentang" class="btn btn-outline">
                    <span>Pelajari Lebih Lanjut</span>
                </a>
            </div>
        </div>
    </section>

    <section id="tentang" class="about-section">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Tentang Kami</span>
                <h2 class="section-title">Lembaga Pendidikan Islam Terpercaya</h2>
                <div class="title-ornament">
                    <span>✦</span>
                    <span>✦</span>
                    <span>✦</span>
                </div>
                <p class="section-subtitle">Pondok Pesantren Tahfidz Qur'an Qurrota A'yun berkomitmen mencetak generasi Qurani yang hafal Al-Quran, berakhlak mulia, dan berprestasi akademik</p>
            </div>
            <div class="about-grid">
                <div class="about-image-wrapper">
                    <div class="about-ornament about-ornament-1">☪</div>
                    <div class="about-image">📖</div>
                    <div class="about-ornament about-ornament-2">☪</div>
                </div>
                <div class="about-content">
                    <h3>Selamat Datang di PP Tahfidz Qur'an Qurrota A'yun</h3>
                    <p>Pondok Pesantren Tahfidz Qur'an Qurrota A'yun adalah lembaga pendidikan Islam yang berkomitmen untuk mencetak generasi Qurani yang hafal Al-Quran, berakhlak mulia, dan berprestasi akademik.</p>
                    <p>Berlokasi di Kota Sorong, Papua Barat Daya, kami menyediakan lingkungan belajar yang kondusif dengan metode pembelajaran modern yang tetap menjunjung tinggi nilai-nilai Islam.</p>
                    <p>Dengan tenaga pengajar yang berpengalaman dan berkualitas, kami siap membimbing putra-putri Anda menjadi generasi yang hafal Al-Quran dan siap menghadapi tantangan masa depan.</p>
                    <div class="about-features">
                        <div class="about-feature">
                            <span class="about-feature-icon">✓</span>
                            <span class="about-feature-text">Metode Pembelajaran Modern</span>
                        </div>
                        <div class="about-feature">
                            <span class="about-feature-icon">✓</span>
                            <span class="about-feature-text">Pengajar Berpengalaman</span>
                        </div>
                        <div class="about-feature">
                            <span class="about-feature-icon">✓</span>
                            <span class="about-feature-text">Fasilitas Lengkap</span>
                        </div>
                        <div class="about-feature">
                            <span class="about-feature-icon">✓</span>
                            <span class="about-feature-text">Lingkungan Islami</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="program" class="programs-section">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Program Pendidikan</span>
                <h2 class="section-title">Jenjang Pendidikan</h2>
                <div class="title-ornament">
                    <span>✦</span>
                    <span>✦</span>
                    <span>✦</span>
                </div>
                <p class="section-subtitle">Pilihan program pendidikan yang sesuai dengan jenjang usia dan kebutuhan santri</p>
            </div>
            <div class="programs-grid">
                <div class="program-card">
                    <span class="program-icon">📚</span>
                    <h3>Madrasah Ibtidaiyah</h3>
                    <p>Program pendidikan setara SD dengan fokus pada dasar-dasar tahfidz Al-Quran dan pendidikan agama Islam yang kuat.</p>
                </div>
                <div class="program-card">
                    <span class="program-icon">📝</span>
                    <h3>Madrasah Tsanawiyah</h3>
                    <p>Program pendidikan setara SMP dengan penguatan hafalan Al-Quran dan pengembangan ilmu pengetahuan umum.</p>
                </div>
                <div class="program-card">
                    <span class="program-icon">🎓</span>
                    <h3>Madrasah Aliyah</h3>
                    <p>Program pendidikan setara SMA dengan target hafalan 30 juz dan persiapan melanjutkan ke perguruan tinggi.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="galeri" class="gallery-section">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Galeri Foto</span>
                <h2 class="section-title">Dokumentasi Kegiatan</h2>
                <div class="title-ornament">
                    <span>✦</span>
                    <span>✦</span>
                    <span>✦</span>
                </div>
                <p class="section-subtitle">Momen berharga dalam kegiatan pembelajaran dan aktivitas santri</p>
            </div>
            <div class="gallery-grid">
                <div class="gallery-item">
                    <div class="gallery-placeholder">📸</div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-placeholder">📸</div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-placeholder">📸</div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-placeholder">📸</div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-placeholder">📸</div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-placeholder">📸</div>
                </div>
            </div>
        </div>
    </section>

    <section id="keunggulan" class="features-section">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Keunggulan Kami</span>
                <h2 class="section-title">Mengapa Memilih Qurrota A'yun?</h2>
                <div class="title-ornament">
                    <span>✦</span>
                    <span>✦</span>
                    <span>✦</span>
                </div>
                <p class="section-subtitle">Fasilitas dan metode pembelajaran terbaik untuk membentuk generasi Qurani</p>
            </div>
            <div class="features-grid">
                <div class="feature-card">
                    <span class="feature-icon">🕌</span>
                    <h4>Metode Tahfidz Terpadu</h4>
                    <p>Sistematis dan efektif</p>
                </div>
                <div class="feature-card">
                    <span class="feature-icon">👨‍🏫</span>
                    <h4>Pengajar Berkualitas</h4>
                    <p>Berpengalaman dan sabar</p>
                </div>
                <div class="feature-card">
                    <span class="feature-icon">🏡</span>
                    <h4>Asrama Nyaman</h4>
                    <p>Bersih dan kondusif</p>
                </div>
                <div class="feature-card">
                    <span class="feature-icon">📖</span>
                    <h4>Kurikulum Terintegrasi</h4>
                    <p>Pesantren dan nasional</p>
                </div>
            </div>
        </div>
    </section>

    <section id="kontak" class="contact-section">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Hubungi Kami</span>
                <h2 class="section-title">Mari Bergabung Bersama Kami</h2>
                <div class="title-ornament">
                    <span>✦</span>
                    <span>✦</span>
                    <span>✦</span>
                </div>
                <p class="section-subtitle">Kami siap melayani dan memberikan informasi lebih lanjut tentang pendaftaran</p>
            </div>
            <div class="contact-grid">
                <div class="contact-card">
                    <span class="contact-icon">📍</span>
                    <h4>Alamat</h4>
                    <p>Kota Sorong<br>Provinsi Papua Barat Daya</p>
                </div>
                <div class="contact-card">
                    <span class="contact-icon">✉️</span>
                    <h4>Email</h4>
                    <p>mujahiddin.mr@gmail.com</p>
                </div>
                <div class="contact-card">
                    <span class="contact-icon">📱</span>
                    <h4>WhatsApp</h4>
                    <p>0812-3456-7890</p>
                    <a href="https://wa.me/6281234567890?text=Assalamualaikum,%20saya%20ingin%20bertanya%20tentang%20pendaftaran" class="wa-button" target="_blank">Chat Sekarang</a>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-ornament">✦ ☪ ✦</div>
        <p>&copy; 2025 <span class="footer-highlight">Pondok Pesantren Tahfidz Qur'an Qurrota A'yun</span></p>
        <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
        <p>Kota Sorong, Papua Barat Daya</p>
    </footer>

    <a href="https://wa.me/6281234567890?text=Assalamualaikum,%20saya%20ingin%20bertanya%20tentang%20pendaftaran" class="wa-float" target="_blank" aria-label="Chat WhatsApp">💬</a>

    <script>
        // Toggle Mobile Menu
        function toggleMenu() {
            const menu = document.getElementById('navMenu');
            menu.classList.toggle('active');
        }

        // Close Menu
        function closeMenu() {
            const menu = document.getElementById('navMenu');
            menu.classList.remove('active');
        }

        // Close Menu When Click Outside
        document.addEventListener('click', function(event) {
            const menu = document.getElementById('navMenu');
            const toggle = document.querySelector('.menu-toggle');
            const nav = document.querySelector('nav');
            
            if (!nav.contains(event.target)) {
                menu.classList.remove('active');
            }
        });

        // Navbar Scroll Effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });

        // Smooth Scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>
