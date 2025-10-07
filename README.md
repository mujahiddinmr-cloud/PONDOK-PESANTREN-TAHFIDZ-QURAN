
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Pondok Pesantren Tahfidz Quran Qurrota Ayun - Sorong, Papua Barat Daya. Membentuk Generasi Qurani Berakhlak Mulia.">
    <meta name="keywords" content="pondok pesantren, tahfidz quran, sorong, papua barat daya, pesantren modern">
    <meta name="author" content="PP Qurrota Ayun">
    <title>Pondok Pesantren Tahfidz Quran Qurrota Ayun - Sorong</title>
    
    <style>
        /* ===== RESET & BASE ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            font-size: 16px;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        /* ===== CONTAINER ===== */
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* ===== NAVIGATION ===== */
        nav {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            color: white;
            font-size: clamp(1.1rem, 2.5vw, 1.4rem);
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: clamp(1rem, 3vw, 2.5rem);
        }

        .nav-menu a {
            color: white;
            text-decoration: none;
            font-size: clamp(0.9rem, 1.5vw, 1rem);
            transition: opacity 0.3s;
            padding: 0.5rem 0;
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
            padding: 0.5rem;
        }

        /* ===== HERO SECTION ===== */
        .hero {
            background: linear-gradient(rgba(26, 95, 63, 0.85), rgba(26, 95, 63, 0.85)), 
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23e8f5e9" width="1200" height="600"/><path fill="%23c8e6c9" d="M0 300L50 320L100 310L150 330L200 315L250 335L300 320L350 340L400 325L450 345L500 330L550 350L600 335L650 355L700 340L750 360L800 345L850 365L900 350L950 370L1000 355L1050 375L1100 360L1150 380L1200 365V600H0Z"/></svg>');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: white;
            padding: clamp(4rem, 12vh, 8rem) 20px;
            text-align: center;
            min-height: 70vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: clamp(1.8rem, 5vw, 3.5rem);
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            line-height: 1.2;
        }

        .hero p {
            font-size: clamp(1rem, 2.5vw, 1.3rem);
            margin-bottom: 1.5rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
        }

        .btn {
            display: inline-block;
            padding: clamp(0.9rem, 2vw, 1.2rem) clamp(1.8rem, 4vw, 3rem);
            background: #ffc107;
            color: #1a5f3f;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: clamp(0.95rem, 2vw, 1.1rem);
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            min-height: 48px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
            background: #ffb300;
        }

        /* ===== SECTIONS ===== */
        section {
            padding: clamp(3rem, 8vh, 6rem) 20px;
        }

        .section-title {
            text-align: center;
            font-size: clamp(1.8rem, 4vw, 2.8rem);
            color: #1a5f3f;
            margin-bottom: clamp(2rem, 5vh, 3.5rem);
            position: relative;
            padding-bottom: 1rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: clamp(80px, 15vw, 120px);
            height: 4px;
            background: #ffc107;
            border-radius: 2px;
        }

        /* ===== ABOUT SECTION ===== */
        .about-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(min(100%, 300px), 1fr));
            gap: clamp(2rem, 4vw, 3.5rem);
            align-items: center;
        }

        .about-text {
            font-size: clamp(0.95rem, 1.8vw, 1.1rem);
            line-height: 1.8;
        }

        .about-text h3 {
            color: #1a5f3f;
            margin-bottom: 1rem;
            font-size: clamp(1.3rem, 2.5vw, 1.6rem);
        }

        .about-text p {
            margin-bottom: 1rem;
            text-align: justify;
        }

        .about-image {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            min-height: 300px;
            height: 100%;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: clamp(3rem, 8vw, 5rem);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .about-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 15px;
        }

        /* ===== PROGRAM SECTION ===== */
        #program {
            background: #f8f9fa;
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(min(100%, 280px), 1fr));
            gap: clamp(1.5rem, 3vw, 2.5rem);
        }

        .program-card {
            background: white;
            padding: clamp(1.8rem, 4vw, 2.8rem);
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
            font-size: clamp(2.5rem, 6vw, 4rem);
            margin-bottom: 1rem;
            color: #1a5f3f;
        }

        .program-card h3 {
            color: #1a5f3f;
            margin-bottom: 1rem;
            font-size: clamp(1.2rem, 2.5vw, 1.6rem);
        }

        .program-card p {
            font-size: clamp(0.9rem, 1.8vw, 1rem);
            line-height: 1.6;
            color: #666;
        }

        /* ===== GALERI SECTION ===== */
        .galeri-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(min(100%, 280px), 1fr));
            gap: clamp(1.5rem, 3vw, 2rem);
            margin-top: 2rem;
        }

        .galeri-item {
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            cursor: pointer;
            transition: transform 0.3s;
        }

        .galeri-item:hover {
            transform: translateY(-5px);
        }

        .galeri-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.3s;
        }

        .galeri-item:hover img {
            transform: scale(1.05);
        }

        /* ===== FEATURES SECTION ===== */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(min(100%, 220px), 1fr));
            gap: clamp(1.5rem, 3vw, 2.5rem);
            margin-top: 2rem;
        }

        .feature-item {
            text-align: center;
            padding: clamp(1.5rem, 3vw, 2.5rem);
            transition: transform 0.3s;
        }

        .feature-item:hover {
            transform: translateY(-5px);
        }

        .feature-icon {
            font-size: clamp(2.5rem, 5vw, 3.5rem);
            color: #2d8659;
            margin-bottom: 1rem;
        }

        .feature-item h3 {
            color: #1a5f3f;
            margin-bottom: 0.5rem;
            font-size: clamp(1.1rem, 2vw, 1.3rem);
        }

        .feature-item p {
            font-size: clamp(0.9rem, 1.6vw, 1rem);
            color: #666;
        }

        /* ===== CONTACT SECTION ===== */
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
            grid-template-columns: repeat(auto-fit, minmax(min(100%, 250px), 1fr));
            gap: clamp(1.5rem, 3vw, 2.5rem);
            margin-top: 2rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.1);
            padding: clamp(1.5rem, 3vw, 2.5rem);
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
            font-size: clamp(2rem, 4vw, 3rem);
            margin-bottom: 1rem;
        }

        .contact-item h3 {
            margin-bottom: 0.5rem;
            font-size: clamp(1.1rem, 2vw, 1.4rem);
        }

        .contact-item p {
            font-size: clamp(0.9rem, 1.6vw, 1rem);
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

        /* ===== WHATSAPP FLOATING BUTTON ===== */
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
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
        }

        .wa-float:hover {
            background: #128C7E;
            transform: scale(1.1);
        }

        /* ===== FOOTER ===== */
        footer {
            background: #1a3d2e;
            color: white;
            text-align: center;
            padding: clamp(1.5rem, 3vw, 2.5rem);
        }

        footer p {
            font-size: clamp(0.85rem, 1.5vw, 0.95rem);
            margin-bottom: 0.5rem;
        }

        /* ===== RESPONSIVE - MOBILE ===== */
        @media (max-width: 768px) {
            .nav-menu {
                display: none;
                position: fixed;
                top: 60px;
                left: 0;
                right: 0;
                background: #1a5f3f;
                flex-direction: column;
                padding: 1.5rem;
                gap: 0;
                box-shadow: 0 5px 15px rgba(0,0,0,0.3);
                animation: slideDown 0.3s ease;
            }

            .nav-menu.active {
                display: flex;
            }

            .nav-menu li {
                border-bottom: 1px solid rgba(255,255,255,0.1);
            }

            .nav-menu li:last-child {
                border-bottom: none;
            }

            .nav-menu a {
                display: block;
                padding: 1rem 0;
                font-size: 1.05rem;
            }

            .menu-toggle {
                display: block;
            }

            .hero {
                min-height: 60vh;
                padding: 3rem 20px;
                background-attachment: scroll;
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .about-image {
                order: -1;
                min-height: 250px;
            }

            .programs-grid,
            .features-grid,
            .contact-grid,
            .galeri-grid {
                grid-template-columns: 1fr;
            }

            section {
                padding: 2.5rem 15px;
            }

            .wa-float {
                width: 55px;
                height: 55px;
                bottom: 20px;
                right: 20px;
                font-size: 1.8rem;
            }
        }

        /* ===== RESPONSIVE - TABLET ===== */
        @media (min-width: 769px) and (max-width: 1024px) {
            .programs-grid,
            .features-grid,
            .contact-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .galeri-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        /* ===== RESPONSIVE - LARGE DESKTOP ===== */
        @media (min-width: 1920px) {
            .container {
                max-width: 1600px;
            }

            html {
                font-size: 18px;
            }
        }

        /* ===== ANIMATIONS ===== */
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

    <!-- ===== NAVIGATION ===== -->
    <nav>
        <div class="container">
           <div class="logo">
    <img src=file:///C:/Users/ASUS/OneDrive/Documents/PONPES%20QURROTA%20A'AYUN/logo%20yayasan%20dan%20pondok/Gambar_WhatsApp_2023-12-11_pukul_08.20.23_95df0df1-removebg-preview.png alt="Logo" style="height: 35px;">
    <span>PP Qurrota Ayun</span>
</div>
    <span>PP Qurrota Ayun</span>
</div> PP Qurrota Ayun
            </div>
            <button class="menu-toggle" onclick="toggleMenu()" aria-label="Toggle Menu">☰</button>
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

    <!-- ===== HERO SECTION ===== -->
    <section class="hero" id="beranda">
        <div class="hero-content">
            <h1>Pondok Pesantren Tahfidz Quran<br>Qurrota Ayun</h1>
            <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
            <p>📍 Kota Sorong, Papua Barat Daya</p>
            <a href="#kontak" class="btn">Daftar Sekarang</a>
        </div>
    </section>

    <!-- ===== ABOUT SECTION ===== -->
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
                <div class="about-image">
                    📖
                    <!-- Ganti dengan gambar: <img src="gambar/foto-pesantren.jpg" alt="Foto Pesantren"> -->
                </div>
            </div>
        </div>
    </section>

    <!-- ===== PROGRAM SECTION ===== -->
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

    <!-- ===== GALERI SECTION ===== -->
    <section id="galeri">
        <div class="container">
            <h2 class="section-title">Galeri Foto</h2>
            <div class="galeri-grid">
                <div class="galeri-item">
                    <div style="width: 100%; height: 250px; background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 3rem;">📸</div>
                    <!-- Ganti dengan: <img src="gambar/galeri1.jpg" alt="Kegiatan 1"> -->
                </div>
                <div class="galeri-item">
                    <div style="width: 100%; height: 250px; background: linear-gradient(135deg, #2d8659 0%, #1a5f3f 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 3rem;">📸</div>
                    <!-- Ganti dengan: <img src="gambar/galeri2.jpg" alt="Kegiatan 2"> -->
                </div>
                <div class="galeri-item">
                    <div style="width: 100%; height: 250px; background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 3rem;">📸</div>
                    <!-- Ganti dengan: <img src="gambar/galeri3.jpg" alt="Kegiatan 3"> -->
                </div>
                <div class="galeri-item">
                    <div style="width: 100%; height: 250px; background: linear-gradient(135deg, #2d8659 0%, #1a5f3f 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 3rem;">📸</div>
                    <!-- Ganti dengan: <img src="gambar/galeri4.jpg" alt="Kegiatan 4"> -->
                </div>
                <div class="galeri-item">
                    <div style="width: 100%; height: 250px; background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 3rem;">📸</div>
                    <!-- Ganti dengan: <img src="gambar/galeri5.jpg" alt="Kegiatan 5"> -->
                </div>
                <div class="galeri-item">
                    <div style="width: 100%; height: 250px; background: linear-gradient(135deg, #2d8659 0%, #1a5f3f 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 3rem;">📸</div>
                    <!-- Ganti dengan: <img src="gambar/galeri6.jpg" alt="Kegiatan 6"> -->
                </div>
            </div>
        </div>
    </section>

    <!-- ===== FEATURES SECTION ===== -->
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

    <!-- ===== CONTACT SECTION ===== -->
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

    <!-- ===== FOOTER ===== -->
    <footer>
        <p>&copy; 2025 Pondok Pesantren Tahfidz Quran Qurrota Ayun. All rights reserved.</p>
        <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
    </footer>

    <!-- ===== WHATSAPP FLOATING BUTTON ===== -->
    <a href="https://wa.me/6281234567890?text=Assalamualaikum,%20saya%20ingin%20bertanya%20tentang%20pendaftaran" class="wa-float" target="_blank" aria-label="Chat WhatsApp">
        💬
    </a>

    <!-- ===== JAVASCRIPT ===== -->
    <script>
        // Toggle Mobile Menu
        function toggleMenu() {
            const menu = document.getElementById('navMenu');
            menu.classList.toggle('active');
        }

        // Close Menu After Click
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

        // Smooth Scroll
        document.queryS
