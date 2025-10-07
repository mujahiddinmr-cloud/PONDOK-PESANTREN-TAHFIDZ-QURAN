<!DOCTYPE html>
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

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        /* ===== CONTAINER FULL WIDTH ===== */
        .container {
            width: 100%;
            max-width: 100%;
            margin: 0 auto;
            padding: 0 5vw;
        }

        /* ===== NAVIGATION ===== */
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
            height: 100%;
        }

        .logo svg {
            height: 45px;
            width: 45px;
            flex-shrink: 0;
        }

        .logo span {
            display: inline-block;
            line-height: 1.2;
            vertical-align: middle;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
            align-items: center;
            height: 100%;
        }

        .nav-menu li {
            display: flex;
            align-items: center;
        }

        .nav-menu a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
            transition: opacity 0.3s;
            padding: 0.5rem 0;
            display: inline-block;
            vertical-align: middle;
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

        /* ===== HERO SECTION FULL ===== */
        .hero {
            background: linear-gradient(rgba(26, 95, 63, 0.85), rgba(26, 95, 63, 0.85)), 
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23e8f5e9" width="1200" height="600"/><path fill="%23c8e6c9" d="M0 300L50 320L100 310L150 330L200 315L250 335L300 320L350 340L400 325L450 345L500 330L550 350L600 335L650 355L700 340L750 360L800 345L850 365L900 350L950 370L1000 355L1050 375L1100 360L1150 380L1200 365V600H0Z"/></svg>');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: white;
            padding: 0;
            text-align: center;
            min-height: 100vh;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .hero-content {
            max-width: 900px;
            margin: 0 auto;
            padding: 2rem;
        }

        .hero h1 {
            font-size: clamp(2rem, 5vw, 3.5rem);
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            line-height: 1.3;
            font-weight: 700;
        }

        .hero p {
            font-size: clamp(1.1rem, 2.5vw, 1.4rem);
            margin-bottom: 1.5rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
            line-height: 1.6;
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
            min-height: 48px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            margin-top: 1rem;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
            background: #ffb300;
        }

        /* ===== SECTIONS FULL WIDTH ===== */
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
            line-height: 1.2;
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

        /* ===== ABOUT SECTION ===== */
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
            line-height: 1.3;
            font-weight: 700;
        }

        .about-text p {
            margin-bottom: 1.2rem;
            text-align: left;
            line-height: 1.8;
        }

        .about-image {
            background: linear-gradient(135deg, #1a5f3f 0%, #2d8659 100%);
            min-height: 400px;
            height: 100%;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 5rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        /* ===== PROGRAM SECTION ===== */
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
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
        }

        .program-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }

        .program-icon {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            color: #1a5f3f;
            line-height: 1;
        }

        .program-card h3 {
            color: #1a5f3f;
            margin-bottom: 1rem;
            font-size: 1.5rem;
            line-height: 1.3;
            font-weight: 700;
        }

        .program-card p {
            font-size: 1rem;
            line-height: 1.7;
            color: #666;
            text-align: center;
        }

        /* ===== GALERI SECTION ===== */
        .galeri-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
            margin-top: 2rem;
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

        /* ===== FEATURES SECTION ===== */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
            margin-top: 2rem;
        }

        .feature-item {
            text-align: center;
            padding: 2rem;
            transition: transform 0.3s;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
        }

        .feature-item:hover {
            transform: translateY(-5px);
        }

        .feature-icon {
            font-size: 3.5rem;
            color: #2d8659;
            margin-bottom: 1rem;
            line-height: 1;
        }

        .feature-item h3 {
            color: #1a5f3f;
            margin-bottom: 0.8rem;
            font-size: 1.3rem;
            line-height: 1.3;
            font-weight: 700;
        }

        .feature-item p {
            font-size: 1rem;
            color: #666;
            line-height: 1.6;
            text-align: center;
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
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.1);
            padding: 2.5rem;
            border-radius: 15px;
            text-align: center;
            backdrop-filter: blur(10px);
            transition: all 0.3s;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
        }

        .contact-item:hover {
            background: rgba(255,255,255,0.15);
            transform: translateY(-5px);
        }

        .contact-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
            line-height: 1;
        }

        .contact-item h3 {
            margin-bottom: 0.8rem;
            font-size: 1.4rem;
            line-height: 1.3;
            font-weight: 700;
        }

        .contact-item p {
            font-size: 1rem;
            line-height: 1.6;
            text-align: center;
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
