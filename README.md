<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pondok Pesantren Tahfidz Quran Qurrota Ayun - Sorong</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }

        /* Navigation */
        nav {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav .logo {
            color: white;
            font-size: 1.3rem;
            font-weight: bold;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        nav a:hover {
            opacity: 0.8;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(26, 95, 63, 0.85), rgba(26, 95, 63, 0.85)), 
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23f0f0f0" width="1200" height="600"/><path fill="%23e0e0e0" d="M0 300L50 320L100 310L150 330L200 315L250 335L300 320L350 340L400 325L450 345L500 330L550 350L600 335L650 355L700 340L750 360L800 345L850 365L900 350L950 370L1000 355L1050 375L1100 360L1150 380L1200 365V600H0Z"/></svg>');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 8rem 2rem;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
        }

        .btn {
            display: inline-block;
            padding: 1rem 2.5rem;
            background: #ffc107;
            color: #1a5f3f;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
        }

        /* Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        /* Sections */
        section {
            padding: 5rem 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            color: #1a5f3f;
            margin-bottom: 3rem;
            position: relative;
            padding-bottom: 1rem;
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

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text {
            font-size: 1.1rem;
            line-height: 1.8;
        }

        .about-image {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            height: 400px;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        /* Programs Section */
        #program {
            background: #f8f9fa;
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .program-card {
            background: white;
            padding: 2.5rem;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .program-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }

        .program-icon {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            color: #1a5f3f;
        }

        .program-card h3 {
            color: #1a5f3f;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }

        /* Features Section */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .feature-item {
            text-align: center;
            padding: 2rem;
        }

        .feature-icon {
            font-size: 3rem;
            color: #2d8659;
            margin-bottom: 1rem;
        }

        .feature-item h3 {
            color: #1a5f3f;
            margin-bottom: 0.5rem;
        }

        /* Contact Section */
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
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.1);
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            backdrop-filter: blur(10px);
        }

        .contact-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .contact-item h3 {
            margin-bottom: 0.5rem;
            font-size: 1.3rem;
        }

        /* Footer */
        footer {
            background: #1a3d2e;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        /* Mobile Menu */
        .menu-toggle {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }

        @media (max-width: 768px) {
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: #1a5f3f;
                flex-direction: column;
                padding: 1rem;
                gap: 1rem;
            }

            nav ul.active {
                display: flex;
            }

            .menu-toggle {
                display: block;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .section-title {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="container">
            <div class="logo">🕌 PP Qurrota Ayun</div>
            <button class="menu-toggle" onclick="toggleMenu()">☰</button>
            <ul id="menu">
                <li><a href="#beranda">Beranda</a></li>
                <li><a href="#tentang">Tentang</a></li>
                <li><a href="#program">Program</a></li>
                <li><a href="#keunggulan">Keunggulan</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="beranda">
        <h1>Pondok Pesantren Tahfidz Qur'an<br>Qurrota A'yun</h1>
        <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
        <p>📍 Kota Sorong, Papua Barat Daya</p>
        <a href="#kontak" class="btn">Daftar Sekarang</a>
    </section>

    <!-- About Section -->
    <section id="tentang">
        <div class="container">
            <h2 class="section-title">Tentang Kami</h2>
            <div class="about-content">
                <div class="about-text">
                    <h3 style="color: #1a5f3f; margin-bottom: 1rem;">Selamat Datang di Pondok Pesantren Tahfidz Quran Qurrota Ayun</h3>
                    <p style="margin-bottom: 1rem;">
                        Pondok Pesantren Tahfidz Quran Qurrota Ayun adalah lembaga pendidikan Islam yang berkomitmen untuk mencetak generasi Qurani yang hafal Al-Quran, berakhlak mulia, dan berprestasi akademik.
                    </p>
                    <p style="margin-bottom: 1rem;">
                        Berlokasi di Kota Sorong, Papua Barat Daya, kami menyediakan lingkungan belajar yang kondusif dengan metode pembelajaran modern yang tetap menjunjung tinggi nilai-nilai Islam.
                    </p>
                    <p>
                        Dengan tenaga pengajar yang berpengalaman dan berkualitas, kami siap membimbing putra-putri Anda menjadi generasi yang hafal Al-Quran dan siap menghadapi tantangan masa depan.
                    </p>
                </div>
                <div class="about-image">
                    📖
                </div>
            </div>
        </div>
    </section>

    <!-- Programs Section -->
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

    <!-- Features Section -->
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

    <!-- Contact Section -->
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
                    <h3>Pendaftaran</h3>
                    <p>Hubungi kami untuk informasi<br>pendaftaran santri baru</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Pondok Pesantren Tahfidz Quran Qurrota Ayun. All rights reserved.</p>
        <p>Membentuk Generasi Qurani Berakhlak Mulia</p>
    </footer>

    <script>
        function toggleMenu() {
            const menu = document.getElementById('menu');
            menu.classList.toggle('active');
        }

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                    // Close mobile menu after click
                    document.getElementById('menu').classList.remove('active');
                }
            });
        });
    </script>
</body>
</html>
