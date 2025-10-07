<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Pondok Pesantren Tahfidz Quran Qurrota Ayun - Sorong, Papua Barat Daya. Membentuk Generasi Qurani Berakhlak Mulia.">
    <title>Pondok Pesantren Tahfidz Quran Qurrota Ayun - Sorong</title>
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            font-size: 16px;
            scroll-behavior: smooth;
            width: 100%;
            height: 100%;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
            width: 100%;
            min-height: 100vh;
        }

        .container {
            width: 100%;
            max-width: 100%;
            margin: 0 auto;
            padding: 0 5vw;
        }

        /* NAVIGATION */
        nav {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            width: 100%;
        }

        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 60px;
        }

        .logo {
            color: white;
            font-size: 1.2rem;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo svg {
            height: 45px;
            width: 45px;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
            align-items: center;
        }

        .nav-menu a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
            transition: opacity 0.3s;
        }

        .nav-menu a:hover {
            opacity: 0.8;
        }

        .menu-toggle {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.8rem;
            cursor: pointer;
        }

        /* HERO */
        .hero {
            background: linear-gradient(rgba(26, 95, 63, 0.85), rgba(26, 95, 63, 0.85)), 
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23e8f5e9" width="1200" height="600"/><path fill="%23c8e6c9" d="M0 300L50 320L100 310L150 330L200 315L250 335L300 320L350 340L400 325L450 345L500 330L550 350L600 335L650 355L700 340L750 360L800 345L850 365L900 350L950 370L1000 355L1050 375L1100 360L1150 380L1200 365V600H0Z"/></svg>');
            background-size: cover;
            background-position: center;
            color: white;
            min-height: 100vh;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }

        .hero-content {
            max-width: 900px;
            padding: 2rem;
        }

        .hero h1 {
            font-size: clamp(2rem, 5vw, 3.5rem);
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            line-height: 1.3;
        }

        .hero p {
            font-size: clamp(1.1rem, 2.5vw, 1.4rem);
            margin-bottom: 1.5rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
        }

        .btn {
            display: inline-block;
            padding: 1.2rem 3rem;
            background: #ffc107;
            color: #1a5f3f;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: 1.1rem;
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            margin-top: 1rem;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
            background: #ffb300;
        }

        /* SECTIONS */
        section {
            padding: 5rem 0;
            width: 100%;
        }

        .section-title {
            text-align: center;
            font-size: clamp(2rem, 4vw, 3rem);
            color: #1a5f3f;
            margin-bottom: 3rem;
            position: relative;
            padding-bottom: 1rem;
            font-weight: 700;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: #ffc107;
            border-radius: 2px;
        }

        /* ABOUT */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text {
            font-size: 1.1rem;
            line-height: 1.8;
        }

        .about-text h3 {
            color: #1a5f3f;
            margin-bottom: 1.5rem;
            font-size: 1.6rem;
            font-weight: 700;
        }

        .about-text p {
            margin-bottom: 1.2rem;
            text-align: left;
        }

        .about-image {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            min-height: 400px;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 5rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        /* PROGRAM */
        #program {
            background: #f8f9fa;
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
        }

        .program-card {
            background: white;
            padding: 2.5rem;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .program-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }

        .program-icon {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            color: #1a5f3f;
        }

        .program-card h3 {
            color: #1a5f3f;
            margin-bottom: 1rem;
            font-size: 1.5rem;
            font-weight: 700;
        }

        .program-card p {
            font-size: 1rem;
            line-height: 1.7;
            color: #666;
        }

        /* GALERI */
        .galeri-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
        }

        .galeri-item {
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            cursor: pointer;
            transition: transform 0.3s;
            aspect-ratio: 4/3;
        }

        .galeri-item:hover {
            transform: translateY(-5px);
        }

        .galeri-item > div {
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
        }

        /* FEATURES */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
        }

        .feature-item {
            text-align: center;
            padding: 2rem;
            transition: transform 0.3s;
        }

        .feature-item:hover {
            transform: translateY(-5px);
        }

        .feature-icon {
            font-size: 3.5rem;
            color: #2d8659;
            margin-bottom: 1rem;
        }

        .feature-item h3 {
            color: #1a5f3f;
            margin-bottom: 0.8rem;
            font-size: 1.3rem;
            font-weight: 700;
        }

        .feature-item p {
            font-size: 1rem;
            color: #666;
            line-height: 1.6;
        }

        /* CONTACT */
        #kontak {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            color: white;
        }

        #kontak .section-title {
            color: white;
        }

        #kontak .section-title::after {
            background: white;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.1);
            padding: 2.5rem;
            border-radius: 15px;
            text-align: center;
            backdrop-filter: blur(10px);
            transition: all 0.3s;
        }

        .contact-item:hover {
            background: rgba(255,255,255,0.15);
            transform: translateY(-5px);
        }

        .contact-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .contact-item h3 {
            margin-bottom: 0.8rem;
            font-size: 1.4rem;
            font-weight: 700;
        }

        .contact-item p {
            font-size: 1rem;
            line-height: 1.6;
        }

        .wa-button {
            display: inline-block;
            margin-top: 1rem;
            padding: 0.8rem 2rem;
            background: #25D366;
            color: white;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: all 0.3s;
        }

        .wa-button:hover {
            background: #128C7E;
            transform: scale(1.05);
        }

        /* FLOATING WA */
        .wa-float {
            position: fixed;
            bottom: 25px;
            right: 25px;
            background: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            box-shadow: 0 5px 20px rgba(0,0,0,0.3);
            z-index: 999;
            text-decoration: none;
            transition: all 0.3s;
        }

        .wa-float:hover {
            background: #128C7E;
            transform: scale(1.1);
        }

        /* FOOTER */
        footer {
            background: #1a3d2e;
            color: white;
            text-align: center;
            padding: 2rem;
            width: 100%;
        }

        footer p {
            font-size: 0.95rem;
            margin-bottom: 0.5rem;
        }

        /* RESPONSIVE */
        @media (max-width: 1024px) {
            .programs-grid,
            .features-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .contact-grid,
            .galeri-grid {
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
                background: #1a5f3f;
                flex-direction: column;
                padding: 1.5rem;
                gap: 0;
                box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            }

            .nav-menu.active {
                display: flex;
            }

            .nav-menu li {
                border-bottom: 1px solid rgba(255,255,255,0.1);
                width: 100%;
            }

            .nav-menu li:last-child {
                border-bottom: none;
            }

            .nav-menu a {
                display: block;
                padding: 1rem 0;
                font-size: 1.05rem;
            }

            .about-grid,
            .programs-grid,
            .features-grid,
            .contact-grid,
            .galeri-grid {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }

            .about-image {
                order: -1;
                min-height: 300px;
            }

            section {
                padding: 3rem 0;
            }

            .wa-float {
                width: 55px;
                height: 55px;
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>

    <nav>
        <div class="container">
            <div class="logo">
                <svg width="45" height="45" viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="150" cy="150" r="148" fill="#001a3d"/>
                    <path d="M 150,20 L 170,80 L 220,50 L 200,100 L 250,120 L 200,140 L 220,190 L 170,170 L 150,220 L 130,170 L 80,190 L 100,140 L 50,120 L 100,100 L 80,50 L 130,80 Z" fill="none" stroke="#2ecc71" stroke-width="6"/>
                    <path d="M 90,70 L 95,85 L 110,85 L 98,93 L 103,108 L 90,98 L 77,108 L 82,93 L 70,85 L 85,85 Z" fill="#FFD700"/>
                    <path d="M 210,70 L 215,85 L 230,85 L 218,93 L 223,108 L 210,98 L 197,108 L 202,93 L 190,85 L 205,85 Z" fill="#FFD700"/>
                    <path d="M 150,40 L 155,55 L 170,55 L 158,63 L 163,78 L 150,68 L 137,78 L 142,63 L 130,55 L 145,55 Z" fill="#FFD700"/>
                    <circle cx="155" cy="85" r="12" fill="#FFD700"/>
                    <circle cx="160" cy="85" r="10" fill="#001a3d"/>
                    <path d="M 90,140 L 90,190 L 145,180 L 145,130 Z" fill="#FFD700" stroke="#FFA500" stroke-width="2"/>
                    <path d="M 155,130 L 155,180 L 210,190 L 210,140 Z" fill="#FFD700" stroke="#FFA500" stroke-width="2"/>
                    <line x1="95" y1="145" x2="140" y2="142" stroke="#001a3d" stroke-width="2"/>
                    <line x1="95" y1="155" x2="140" y2="152" stroke="#001a3d" stroke-width="2"/>
                    <line x1="95" y1="165" x2="140" y2="162" stroke="#001a3d" stroke-width="2"/>
                    <line x1="160" y1="142" x2="205" y2="145" stroke="#001a3d" stroke-width="2"/>
                    <line x1="160" y1="152" x2="205" y2="155" stroke="#001a3d" stroke-width="2"/>
                    <line x1="160" y1="162" x2="205" y2="165" stroke="#001a3d" stroke-width="2"/>
                </svg>
                <span>PP Qurrota Ayun</span>
            </div>
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
            <h1>Pondok Pesantren Tahfidz Quran Qurrota Ayun</h1>
            <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
            <p>📍 Kota Sorong, Papua Barat Daya</p>
            <a href="#kontak" class="btn">Daftar Sekarang</a>
        </div>
    </section>

    <section id="tentang">
        <div class="container">
            <h2 class="section-title">Tentang Kami</h2>
            <div class="about-grid">
                <div class="about-text">
                    <h3>Selamat Datang di Pondok Pesantren Tahfidz Quran Qurrota Ayun</h3>
                    <p>Pondok Pesantren Tahfidz Quran Qurrota Ayun adalah lembaga pendidikan Islam yang berkomitmen untuk mencetak generasi Qurani yang hafal Al-Quran, berakhlak mulia, dan berprestasi akademik.</p>
                    <p>Berlokasi di Kota Sorong, Papua Barat Daya, kami menyediakan lingkungan belajar yang kondusif dengan metode pembelajaran modern yang tetap menjunjung tinggi nilai-nilai Islam.</p>
                    <p>Dengan tenaga pengajar yang berpengalaman dan berkualitas, kami siap membimbing putra-putri Anda menjadi generasi yang hafal Al-Quran dan siap menghadapi tantangan masa depan.</p>
                </div>
                <div class="about-image">📖</div>
            </div>
        </div>
    </section>

    <section id="program">
        <div class="container">
            <h2 class="section-title">Program Pendidikan</h2>
            <div class="programs-grid">
                <div class="program-card">
                    <div class="program-icon">📚</div>
                    <h3>Madrasah Ibtidaiyah (MI)</h3>
                    <p>Program pendidikan setara SD dengan fokus pada dasar-dasar tahfidz Al-Quran dan pendidikan agama Islam yang kuat.</p>
                </div>
                <div class="program-card">
                    <div class="program-icon">📝</div>
                    <h3>Madrasah Tsanawiyah (MTs)</h3>
                    <p>Program pendidikan setara SMP dengan penguatan hafalan Al-Quran dan pengembangan ilmu pengetahuan umum.</p>
                </div>
                <div class="program-card">
                    <div class="program-icon">🎓</div>
                    <h3>Madrasah Aliyah (MA)</h3>
                    <p>Program pendidikan setara SMA dengan target hafalan 30 juz dan persiapan melanjutkan ke perguruan tinggi.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="galeri">
        <div class="container">
            <h2 class="section-title">Galeri Foto</h2>
            <div class="galeri-grid">
                <div class="galeri-item"><div style="background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);">📸</div></div>
                <div class="galeri-item"><div style="background: linear-gradient(135deg, #2d8659 0%, #1a5f3f 100%);">📸</div></div>
                <div class="galeri-item"><div style="background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);">📸</div></div>
                <div class="galeri-item"><div style="background: linear-gradient(135deg, #2d8659 0%, #1a5f3f 100%);">📸</div></div>
                <div class="galeri-item"><div style="background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);">📸</div></div>
                <div class="galeri-item"><div style="background: linear-gradient(135deg, #2d8659 0%, #1a5f3f 100%);">📸</div></div>
            </div>
        </div>
    </section>

    <section id="keunggulan">
        <div class="container">
            <h2 class="section-title">Keunggulan Kami</h2>
            <div class="features-grid">
                <div class="feature-item">
                    <div class="feature-icon">🕌</div>
                    <h3>Metode Tahfidz Terpadu</h3>
                    <p>Metode pembelajaran tahfidz yang sistematis dan efektif</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">👨‍🏫</div>
                    <h3>Pengajar Berkualitas</h3>
                    <p>Ustadz dan ustadzah yang berpengalaman dan sabar</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">🏡</div>
                    <h3>Asrama Nyaman</h3>
                    <p>Fasilitas asrama yang bersih dan kondusif untuk belajar</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">📖</div>
                    <h3>Kurikulum Terintegrasi</h3>
                    <p>Perpaduan kurikulum pesantren dan nasional</p>
                </div>
            </div>
        </div>
    </section>

    <section id="kontak">
        <div class="container">
            <h2 class="section-title">Hubungi Kami</h2>
            <div class="contact-grid">
                <div class="contact-item">
                    <div class="contact-icon">📍</div>
                    <h3>Alamat</h3>
                    <p>Kota Sorong<br>Provinsi Papua Barat Daya</p>
                </div>
                <div class="contact-item">
                    <div class="contact-icon">✉️</div>
                    <h3>Email</h3>
                    <p>mujahiddin.mr@gmail.com</p>
                </div>
                <div class="contact-item">
                    <div class="contact-icon">📱</div>
                    <h3>WhatsApp</h3>
                    <p>0812-3456-7890</p>
                    <a href="https://wa.me/6281234567890?text=Assalamualaikum,%20saya%20ingin%20bertanya%20tentang%20pendaftaran" class="wa-button" target="_blank">Chat Sekarang</a>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Pondok Pesantren Tahfidz Quran Qurrota Ayun. All rights reserved.</p>
        <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
    </footer>

    <a href="https://wa.me/6281234567890?text=Assalamualaikum,%20saya%20ingin%20bertanya%20tentang%20pendaftaran" class="wa-float" target="_blank">💬</a>

    <script>
        function toggleMenu() {
            document.getElementById('navMenu').classList.toggle('active');
        }

        function closeMenu() {
            document.getElementById('navMenu').classList.remove('active');
        }

        document.addEventListener('click', function(event) {
            const menu = document.getElementById('navMenu');
            const nav = document.querySelector('nav');
            if (!nav.contains(event.target)) {
                menu.classList.remove('active');
            }
        });

        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    </script>
</body>
</html>
