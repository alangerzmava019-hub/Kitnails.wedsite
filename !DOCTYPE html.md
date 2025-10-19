<!DOCTYPE html>  
<html lang="ru">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Knails - Студия маникюра</title>  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,500;0,600;1,400&family=Marck+Script&display=swap" rel="stylesheet">  
    <style>  
        * {  
            margin: 0;  
            padding: 0;  
            box-sizing: border-box;  
        }  
          
        body {  
            background: linear-gradient(135deg, #fff5f7, #ffe4ec);  
            color: #8b4a65;  
            line-height: 1.6;  
            position: relative;  
            overflow-x: hidden;  
            font-family: 'Playfair Display', serif;  
        }  
          
        /* Логотип */  
        .logo-container {  
            display: flex;  
            align-items: center;  
            justify-content: center;  
            gap: 15px;  
            margin: 20px 0;  
        }  
          
        .logo-icon {  
            font-size: 3rem;  
            background: linear-gradient(135deg, #ff69b4, #ff1493);  
            -webkit-background-clip: text;  
            -webkit-text-fill-color: transparent;  
            filter: drop-shadow(2px 2px 4px rgba(255, 105, 180, 0.3));  
            animation: sparkle 2s ease-in-out infinite;  
        }  
          
        @keyframes sparkle {  
            0%, 100% { transform: scale(1) rotate(0deg); }  
            50% { transform: scale(1.1) rotate(5deg); }  
        }  
          
        .logo-text {  
            font-family: 'Dancing Script', cursive;  
            font-size: 3.5rem;  
            font-weight: 700;  
            color: #8b4a65;  
            text-shadow: 2px 2px 4px rgba(255, 182, 193, 0.4);  
        }  
          
        /* Стикеры */  
        .sticker {  
            position: absolute;  
            font-size: 2.2rem;  
            opacity: 0.7;  
            animation: float 6s ease-in-out infinite;  
            z-index: 1;  
            pointer-events: none;  
        }  
          
        .sticker-1 { top: 8%; left: 4%; animation-delay: 0s; }  
        .sticker-2 { top: 12%; right: 6%; animation-delay: 1s; }  
        .sticker-3 { top: 35%; left: 2%; animation-delay: 2s; }  
        .sticker-4 { top: 55%; right: 3%; animation-delay: 3s; }  
        .sticker-5 { top: 75%; left: 8%; animation-delay: 4s; }  
        .sticker-6 { top: 25%; right: 12%; animation-delay: 0.5s; }  
        .sticker-7 { top: 15%; left: 15%; animation-delay: 1.5s; }  
        .sticker-8 { top: 65%; right: 15%; animation-delay: 2.5s; }  
        .sticker-9 { top: 45%; left: 10%; animation-delay: 3.5s; }  
        .sticker-10 { top: 85%; right: 8%; animation-delay: 4.5s; }  
        .sticker-11 { top: 5%; right: 20%; animation-delay: 1.2s; }  
        .sticker-12 { top: 95%; left: 20%; animation-delay: 2.8s; }  
        .sticker-13 { top: 70%; left: 25%; animation-delay: 0.8s; }  
        .sticker-14 { top: 30%; right: 25%; animation-delay: 3.2s; }  
        .sticker-15 { top: 50%; left: 30%; animation-delay: 1.8s; }  
        .sticker-16 { top: 40%; right: 30%; animation-delay: 4.2s; }  
        .sticker-17 { top: 20%; left: 35%; animation-delay: 2.2s; }  
        .sticker-18 { top: 80%; right: 35%; animation-delay: 0.3s; }  
        .sticker-19 { top: 60%; left: 40%; animation-delay: 3.8s; }  
        .sticker-20 { top: 10%; right: 40%; animation-delay: 1.7s; }  
          
        @keyframes float {  
            0%, 100% { transform: translateY(0px) rotate(0deg) scale(1); }  
            33% { transform: translateY(-15px) rotate(3deg) scale(1.05); }  
            66% { transform: translateY(10px) rotate(-2deg) scale(0.95); }  
        }  
          
        .container {  
            max-width: 1200px;  
            margin: 0 auto;  
            padding: 0 20px;  
            position: relative;  
            z-index: 2;  
        }  
          
        /* Нежно-розовые таблички */  
        .pink-card {  
            background: linear-gradient(135deg, #ffd6e0, #ffc2d1);  
            border-radius: 25px;  
            margin: 25px 0;  
            padding: 35px;  
            box-shadow: 0 10px 30px rgba(255, 182, 193, 0.3);  
            position: relative;  
            overflow: hidden;  
            border: 2px solid rgba(255, 255, 255, 0.5);  
            backdrop-filter: blur(10px);  
        }  
          
        .pink-card::before {  
            content: '';  
            position: absolute;  
            top: 0;  
            left: 0;  
            right: 0;  
            height: 6px;  
            background: linear-gradient(90deg, #ffb6c1, #ff91a4, #ff69b4);  
        }  
          
        .pink-card h1, .pink-card h2, .pink-card h3 {  
            color: #8b4a65;  
            text-shadow: 1px 1px 2px rgba(255, 255, 255, 0.8);  
        }  
          
        .pink-card p, .pink-card li {  
            color: #7a3d5a;  
            font-size: 1.15rem;  
        }  
          
        /* Шапка */  
        header {  
            text-align: center;  
            padding: 15px 0;  
        }  
          
        .tagline {  
            font-family: 'Marck Script', cursive;  
            font-size: 1.4rem;  
            color: #9c5c7b;  
            margin-bottom: 15px;  
            font-style: italic;  
        }  
          
        .search-bar {  
            display: flex;  
            justify-content: center;  
            margin: 25px 0;  
        }  
          
        .search-bar input {  
            padding: 16px 35px;  
            width: 70%;  
            max-width: 450px;  
            border: 2px solid #ffb6c1;  
            border-radius: 35px;  
            font-size: 1.1rem;  
            outline: none;  
            text-align: center;  
            background: rgba(255, 255, 255, 0.9);  
            color: #8b4a65;  
            font-family: 'Playfair Display', serif;  
            font-style: italic;  
        }  
          
        .search-bar input::placeholder {  
            color: #ff91a4;  
            font-style: italic;  
        }  
          
        /* Навигация */  
        nav {  
            background: linear-gradient(135deg, #ffc2d1, #ffb6c1);  
            padding: 18px 0;  
            border-radius: 20px;  
            box-shadow: 0 6px 20px rgba(255, 182, 193, 0.4);  
        }  
          
        nav ul {  
            display: flex;  
            justify-content: center;  
            list-style: none;  
            flex-wrap: wrap;  
        }  
          
        nav ul li {  
            margin: 8px 25px;  
        }  
          
        nav ul li a {  
            color: #8b4a65;  
            text-decoration: none;  
            font-weight: 500;  
            font-size: 1.2rem;  
            padding: 12px 25px;  
            border-radius: 30px;  
            transition: all 0.3s ease;  
            background: rgba(255, 255, 255, 0.3);  
            font-family: 'Dancing Script', cursive;  
            font-size: 1.4rem;  
        }  
          
        nav ul li a:hover {  
            background: rgba(255, 255, 255, 0.5);  
            transform: translateY(-3px);  
            box-shadow: 0 5px 15px rgba(255, 182, 193, 0.3);  
        }  
          
        /* Основной контент */  
        .main-content {  
            display: grid;  
            grid-template-columns: 2fr 1fr;  
            gap: 30px;  
            margin: 30px 0;  
        }  
          
        @media (max-width: 768px) {  
            .main-content {  
                grid-template-columns: 1fr;  
            }  
        }  
          
        /* Приветствие */  
        .welcome {  
            margin-bottom: 30px;  
        }  
          
        .welcome h1 {  
            color: #8b4a65;  
            margin-bottom: 25px;  
            font-size: 2.8rem;  
            text-align: center;  
            font-family: 'Dancing Script', cursive;  
        }  
          
        .welcome p {  
            margin-bottom: 20px;  
            font-size: 1.25rem;  
            line-height: 1.8;  
            font-family: 'Playfair Display', serif;  
            font-style: italic;  
        }  
          
        /* Слайдер */  
        .slider {  
            position: relative;  
            border-radius: 25px;  
            overflow: hidden;  
            box-shadow: 0 12px 35px rgba(0,0,0,0.15);  
            margin: 35px 0;  
        }  
          
        .slides {  
            display: flex;  
            transition: transform 0.6s ease-in-out;  
            height: 550px;  
        }  
          
        .slide {  
            min-width: 100%;  
            height: 100%;  
        }  
          
        .slide img {  
            width: 100%;  
            height: 100%;  
            object-fit: cover;  
        }  
          
        .slider-nav {  
            position: absolute;  
            bottom: 25px;  
            left: 50%;  
            transform: translateX(-50%);  
            display: flex;  
            gap: 12px;  
        }  
          
        .slider-dot {  
            width: 14px;  
            height: 14px;  
            border-radius: 50%;  
            background: rgba(255,255,255,0.6);  
            cursor: pointer;  
            transition: all 0.3s;  
            border: 2px solid rgba(255, 255, 255, 0.8);  
        }  
          
        .slider-dot.active {  
            background: white;  
            transform: scale(1.2);  
        }  
          
        /* Сертификаты */  
        .certificates {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));  
            gap: 25px;  
            margin: 35px 0;  
        }  
          
        .certificate {  
            background: linear-gradient(135deg, #ffb6c1, #ff91a4);  
            border-radius: 20px;  
            padding: 30px;  
            text-align: center;  
            color: #7a3d5a;  
            box-shadow: 0 8px 25px rgba(255, 105, 180, 0.2);  
            transition: all 0.4s ease;  
            position: relative;  
            overflow: hidden;  
            border: 2px solid rgba(255, 255, 255, 0.3);  
        }  
          
        .certificate:hover {  
            transform: translateY(-8px) scale(1.02);  
            box-shadow: 0 15px 35px rgba(255, 105, 180, 0.3);  
        }  
          
        .certificate::before {  
            content: '💖';  
            position: absolute;  
            top: 15px;  
            right: 15px;  
            font-size: 1.8rem;  
        }  
          
        .certificate h3 {  
            font-size: 1.6rem;  
            margin-bottom: 20px;  
            font-family: 'Dancing Script', cursive;  
        }  
          
        .certificate .price {  
            font-size: 2.3rem;  
            font-weight: bold;  
            margin: 20px 0;  
            color: #8b4a65;  
            font-family: 'Playfair Display', serif;  
        }  
          
        .certificate .savings {  
            background: rgba(255,255,255,0.3);  
            padding: 8px 15px;  
            border-radius: 15px;  
            font-size: 1rem;  
            margin: 15px 0;  
            font-family: 'Marck Script', cursive;  
        }  
          
        .buy-btn {  
            background: linear-gradient(135deg, #8b4a65, #9c5c7b);  
            color: white;  
            border: none;  
            padding: 15px 30px;  
            border-radius: 30px;  
            font-weight: 500;  
            cursor: pointer;  
            transition: all 0.3s ease;  
            margin-top: 20px;  
            width: 100%;  
            font-family: 'Playfair Display', serif;  
            font-size: 1.1rem;  
            letter-spacing: 0.5px;  
        }  
          
        .buy-btn:hover {  
            background: linear-gradient(135deg, #9c5c7b, #ad6e8b);  
            transform: translateY(-2px);  
            box-shadow: 0 8px 20px rgba(139, 74, 101, 0.3);  
        }  
          
        /* Прогресс скидки */  
        .discount-progress {  
            background: rgba(255,255,255,0.4);  
            padding: 20px;  
            border-radius: 15px;  
            margin: 25px 0;  
            text-align: center;  
            border: 1px solid rgba(255, 255, 255, 0.5);  
        }  
          
        .progress-bar {  
            background: rgba(255,255,255,0.3);  
            height: 12px;  
            border-radius: 8px;  
            margin: 15px 0;  
            overflow: hidden;  
        }  
          
        .progress-fill {  
            background: linear-gradient(90deg, #ff91a4, #ff69b4);  
            height: 100%;  
            border-radius: 8px;  
            transition: width 0.7s ease;  
        }  
          
        /* Боковая панель */  
        .sidebar {  
            background: linear-gradient(135deg, #ffd6e0, #ffc2d1);  
            padding: 30px;  
            border-radius: 25px;  
            box-shadow: 0 10px 30px rgba(255, 182, 193, 0.3);  
            border: 2px solid rgba(255, 255, 255, 0.4);  
        }  
          
        .sidebar h3 {  
            color: #8b4a65;  
            margin-bottom: 25px;  
            font-size: 1.8rem;  
            text-align: center;  
            font-family: 'Dancing Script', cursive;  
        }  
          
        .master-icon {  
            width: 140px;  
            height: 140px;  
            border-radius: 50%;  
            margin: 0 auto 25px;  
            background: linear-gradient(135deg, #ffb6c1, #ff91a4);  
            display: flex;  
            align-items: center;  
            justify-content: center;  
            font-size: 3.5rem;  
            color: white;  
            border: 4px solid white;  
            box-shadow: 0 8px 25px rgba(255, 182, 193, 0.4);  
        }  
          
        /* Кнопка записи */  
        .book-btn {  
            display: block;  
            width: 100%;  
            padding: 20px;  
            background: linear-gradient(135deg, #ff91a4, #ff69b4);  
            color: white;  
            border: none;  
            border-radius: 35px;  
            font-size: 1.5rem;  
            font-weight: 600;  
            cursor: pointer;  
            transition: all 0.4s ease;  
            margin: 30px 0;  
            box-shadow: 0 8px 25px rgba(255, 105, 180, 0.4);  
            font-family: 'Dancing Script', cursive;  
            letter-spacing: 1px;  
        }  
          
        .book-btn:hover {  
            transform: translateY(-4px) scale(1.02);  
            box-shadow: 0 12px 35px rgba(255, 105, 180, 0.5);  
            background: linear-gradient(135deg, #ff69b4, #ff1493);  
        }  
          
        /* Модальное окно */  
        .modal {  
            display: none;  
            position: fixed;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            background: rgba(139, 74, 101, 0.9);  
            z-index: 1000;  
            justify-content: center;  
            align-items: center;  
            backdrop-filter: blur(8px);  
        }  
          
        .modal-content {  
            background: linear-gradient(135deg, #ffd6e0, #ffc2d1);  
            padding: 45px;  
            border-radius: 30px;  
            width: 90%;  
            max-width: 500px;  
            text-align: center;  
            box-shadow: 0 25px 50px rgba(0,0,0,0.2);  
            position: relative;  
            border: 3px solid rgba(255, 255, 255, 0.5);  
        }  
          
        .modal h2 {  
            color: #8b4a65;  
            margin-bottom: 30px;  
            font-size: 2.3rem;  
            font-family: 'Dancing Script', cursive;  
        }  
          
        .contact-links {  
            display: flex;  
            flex-direction: column;  
            gap: 20px;  
            margin: 30px 0;  
        }  
          
        .contact-link {  
            display: flex;  
            align-items: center;  
            justify-content: center;  
            text-decoration: none;  
            color: #7a3d5a;  
            transition: all 0.3s ease;  
            padding: 20px;  
            border-radius: 20px;  
            background: rgba(255,255,255,0.3);  
            border: 2px solid rgba(255, 255, 255, 0.4);  
        }  
          
        .contact-link:hover {  
            transform: scale(1.05);  
            background: rgba(255,255,255,0.5);  
            border-color: #ffb6c1;  
        }  
          
        .contact-icon {  
            font-size: 2.8rem;  
            margin-right: 20px;  
        }  
          
        .contact-text {  
            text-align: left;  
        }  
          
        .contact-text strong {  
            display: block;  
            font-size: 1.3rem;  
            margin-bottom: 8px;  
            font-family: 'Dancing Script', cursive;  
        }  
          
        .telegram { color: #0088cc; }  
        .whatsapp { color: #25D366; }  
          
        .close-btn {  
            background: linear-gradient(135deg, #8b4a65, #9c5c7b);  
            color: white;  
            border: none;  
            padding: 15px 40px;  
            border-radius: 30px;  
            cursor: pointer;  
            margin-top: 25px;  
            font-size: 1.2rem;  
            font-weight: 500;  
            transition: all 0.3s ease;  
            font-family: 'Playfair Display', serif;  
        }  
          
        .close-btn:hover {  
            transform: translateY(-2px);  
            box-shadow: 0 8px 20px rgba(139, 74, 101, 0.4);  
        }  
          
        /* Футер */  
        footer {  
            background: linear-gradient(135deg, #ffc2d1, #ffb6c1);  
            color: #8b4a65;  
            padding: 40px 0;  
            text-align: center;  
            border-radius: 25px;  
            margin-top: 50px;  
            border: 2px solid rgba(255, 255, 255, 0.4);  
        }  
          
        .social-links {  
            display: flex;  
            justify-content: center;  
            gap: 30px;  
            margin: 25px 0;  
        }  
          
        .social-link {  
            color: #8b4a65;  
            font-size: 2.2rem;  
            transition: all 0.3s ease;  
            text-decoration: none;  
        }  
          
        .social-link:hover {  
            transform: scale(1.4) rotate(5deg);  
            color: #ff69b4;  
        }  
          
        .services-list {  
            list-style: none;  
            padding: 0;  
        }  
          
        .services-list li {  
            padding: 15px 0;  
            border-bottom: 1px solid rgba(255,255,255,0.4);  
            font-size: 1.2rem;  
            font-family: 'Playfair Display', serif;  
            font-style: italic;  
        }  
          
        .services-list li:before {  
            content: "✨ ";  
            color: #ff69b4;  
        }  
          
        .highlight {  
            background: rgba(255,255,255,0.3);  
            padding: 5px 12px;  
            border-radius: 12px;  
            font-weight: 500;  
            font-family: 'Marck Script', cursive;  
        }  
          
        .experience-badge {  
            background: linear-gradient(135deg, #ff91a4, #ff69b4);  
            color: white;  
            padding: 12px 25px;  
            border-radius: 25px;  
            display: inline-block;  
            margin: 15px 0;  
            font-weight: 500;  
            box-shadow: 0 6px 20px rgba(255, 105, 180, 0.3);  
            font-family: 'Dancing Script', cursive;  
            font-size: 1.3rem;  
        }  
          
        /* Галерея работ */  
        .works-gallery {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));  
            gap: 20px;  
            margin: 30px 0;  
        }  
          
        .work-item {  
            border-radius: 18px;  
            overflow: hidden;  
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);  
            transition: all 0.4s ease;  
            height: 220px;  
            position: relative;  
        }  
          
        .work-item:hover {  
            transform: translateY(-8px) rotate(1deg);  
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);  
        }  
          
        .work-item img {  
            width: 100%;  
            height: 100%;  
            object-fit: cover;  
        }  
          
        .section-title {  
            text-align: center;  
            font-size: 2.5rem;  
            margin-bottom: 35px;  
            color: #8b4a65;  
            font-family: 'Dancing Script', cursive;  
            position: relative;  
        }  
          
        .section-title::after {  
            content: '';  
            display: block;  
            width: 100px;  
            height: 3px;  
            background: linear-gradient(90deg, #ffb6c1, #ff69b4);  
            margin: 15px auto;  
            border-radius: 2px;  
        }  
          
        /* Красивые шрифты */  
        .feminine-font {  
            font-family: 'Dancing Script', cursive;  
            font-weight: 600;  
        }  
          
        .elegant-font {  
            font-family: 'Playfair Display', serif;  
            font-style: italic;  
        }  
          
        .handwritten-font {  
            font-family: 'Marck Script', cursive;  
        }  
    </style>  
</head>  
<body>  
    <!-- Стикеры (20 штук) -->  
    <div class="sticker sticker-1">💕</div>  
    <div class="sticker sticker-2">🐻</div>  
    <div class="sticker sticker-3">😻</div>  
    <div class="sticker sticker-4">💅</div>  
    <div class="sticker sticker-5">💕</div>  
    <div class="sticker sticker-6">🐻</div>  
    <div class="sticker sticker-7">😻</div>  
    <div class="sticker sticker-8">💅</div>  
    <div class="sticker sticker-9">💕</div>  
    <div class="sticker sticker-10">🐻</div>  
    <div class="sticker sticker-11">😻</div>  
    <div class="sticker sticker-12">💅</div>  
    <div class="sticker sticker-13">💕</div>  
    <div class="sticker sticker-14">🐻</div>  
    <div class="sticker sticker-15">😻</div>  
    <div class="sticker sticker-16">💅</div>  
    <div class="sticker sticker-17">💕</div>  
    <div class="sticker sticker-18">🐻</div>  
    <div class="sticker sticker-19">😻</div>  
    <div class="sticker sticker-20">💅</div>  
  
    <div class="container">  
        <header class="pink-card">  
            <div class="logo-container">  
                <div class="logo-icon">⚡️</div>  
                <div class="logo-text">Knails</div>  
            </div>  
            <div class="tagline handwritten-font">Мгновенная красота, которая заряжает энергией!</div>  
            <div class="search-bar">  
                <input type="text" placeholder="Найдите свой идеальный маникюр...">  
            </div>  
        </header>  
          
        <nav class="pink-card">  
            <ul>  
                <li><a href="#home" class="feminine-font">Главная</a></li>  
                <li><a href="#certificates" class="feminine-font">Сертификаты</a></li>  
                <li><a href="#portfolio" class="feminine-font">Портфолио</a></li>  
                <li><a href="#about" class="feminine-font">О мастере</a></li>  
                <li><a href="#contacts" class="feminine-font">Контакты</a></li>  
            </ul>  
        </nav>  
  
        <!-- Слайдер с вашими работами -->  
        <div class="slider pink-card">  
            <div class="slides" id="slides">  
                <div class="slide">  
                    <img src="https://ltdfoto.ru/image/v2sjZ8" alt="Элегантный маникюр с дизайном">  
                </div>  
                <div class="slide">  
                    <img src="https://ltdfoto.ru/image/v2s1RA" alt="Нежный нюдовый маникюр">  
                </div>  
                <div class="slide">  
                    <img src="https://ltdfoto.ru/image/v2sgdw" alt="Классический френч">  
                </div>  
                <div class="slide">  
                    <img src="https://ltdfoto.ru/image/v2srKG" alt="Современный дизайн">  
                </div>  
                <div class="slide">  
                    <img src="https://ltdfoto.ru/image/v2s38U" alt="Трендовый маникюр">  
                </div>  
            </div>  
            <div class="slider-nav" id="sliderNav">  
                <div class="slider-dot active"></div>  
                <div class="slider-dot"></div>  
                <div class="slider-dot"></div>  
                <div class="slider-dot"></div>  
                <div class="slider-dot"></div>  
            </div>  
        </div>  
          
        <!-- Сертификаты -->  
        <section id="certificates" class="pink-card">  
            <h2 class="section-title feminine-font">Волшебные сертификаты</h2>  
              
            <div class="certificates">  
                <div class="certificate">  
                    <h3 class="feminine-font">Наращивание ногтей</h3>  
                    <p class="elegant-font">3 волшебных посещения</p>  
                    <div class="price elegant-font">4.560 ₽</div>  
                    <div class="savings handwritten-font">Ваша выгода 15%</div>  
                    <button class="buy-btn" onclick="buyCertificate('extension', 3)">Подарить красоту</button>  
                </div>  
                  
                <div class="certificate">  
                    <h3 class="feminine-font">Наращивание ногтей</h3>  
                    <p class="elegant-font">5 прекрасных посещений</p>  
                    <div class="price elegant-font">7.599 ₽</div>  
                    <div class="savings handwritten-font">Ваша выгода 25%</div>  
                    <button class="buy-btn" onclick="buyCertificate('extension', 5)">Подарить красоту</button>  
                </div>  
                  
                <div class="certificate">  
                    <h3 class="feminine-font">Гель-лак</h3>  
                    <p class="elegant-font">3 нежных посещения</p>  
                    <div class="price elegant-font">3.599 ₽</div>  
                    <div class="savings handwritten-font">Ваша выгода 15%</div>  
                    <button class="buy-btn" onclick="buyCertificate('gel', 3)">Подарить красоту</button>  
                </div>  
                  
                <div class="certificate">  
                    <h3 class="feminine-font">Гель-лак</h3>  
                    <p class="elegant-font">5 восхитительных посещений</p>  
                    <div class="price elegant-font">5.999 ₽</div>  
                    <div class="savings handwritten-font">Ваша выгода 25%</div>  
                    <button class="buy-btn" onclick="buyCertificate('gel', 5)">Подарить красоту</button>  
                </div>  
            </div>  
              
            <!-- Прогресс скидки -->  
            <div class="discount-progress" id="discountProgress" style="display: none;">  
                <h4 class="feminine-font" style="font-size: 1.8rem;">✨ Ваш путь к особой скидке ✨</h4>  
                <p id="progressText" class="elegant-font">До волшебной скидки осталось: <span id="visitsLeft">0</span> посещений</p>  
                <div class="progress-bar">  
                    <div class="progress-fill" id="progressFill" style="width: 0%"></div>  
                </div>  
                <p id="nextDiscountInfo" class="handwritten-font" style="font-size: 1.1rem; margin-top: 15px;"></p>  
            </div>  
        </section>  
          
        <!-- Дополнительная галерея работ -->  
        <section id="portfolio" class="pink-card">  
            <h2 class="section-title feminine-font">Галерея вдохновения</h2>  
            <div class="works-gallery">  
                <div class="work-item">  
                    <img src="https://ltdfoto.ru/image/v2sUEs" alt="Креативный дизайн ногтей">  
                </div>  
                <div class="work-item">  
                    <img src="https://ltdfoto.ru/image/v2sbvC" alt="Элегантный маникюр">  
                </div>  
                <div class="work-item">  
                    <img src="https://ltdfoto.ru/image/v2sjZ8" alt="Стильный дизайн">  
                </div>  
                <div class="work-item">  
                    <img src="https://ltdfoto.ru/image/v2s1RA" alt="Нежная классика">  
                </div>  
                <div class="work-item">  
                    <img src="https://ltdfoto.ru/image/v2sgdw" alt="Современный тренд">  
                </div>  
                <div class="work-item">  
                    <img src="https://ltdfoto.ru/image/v2srKG" alt="Искусство на ногтях">  
                </div>  
            </div>  
        </section>  
          
        <div class="main-content">  
            <div class="content">  
                <section id="home" class="welcome pink-card">  
                    <h1 class="feminine-font">Добро пожаловать в сказку красоты! 💫</h1>  
                    <p class="elegant-font">Дорогие мои, позвольте пригласить вас в уютный мир Knails — место, где рождается настоящая женская магия!</p>  
                    <p class="elegant-font">Здесь каждый ноготочек становится холстом для искусства, а ваши ручки — воплощением изящества и нежности.</p>  
                    <p class="elegant-font">Я верю, что красота начинается с мелочей, и готова подарить вашим пальчикам ту самую сказку, которую они заслуживают!</p>  
                </section>  
                  
                <section id="about" class="pink-card">  
                    <h2 class="section-title feminine-font">Немного о вашем мастере 💕</h2>  
                    <div class="experience-badge">✨ Три года творчества и вдохновения ✨</div>  
                    <p class="elegant-font">Милые дамы, я — Катя, и вот уже три года я посвящаю себя искусству создания прекрасного.</p>  
                    <p class="elegant-font">Моя миссия — дарить вашим ноготочкам ту самую идеальную форму и цвет, от которого невозможно отвести восхищенный взгляд! 💅</p>  
                    <p class="elegant-font">За эти волшебные годы я прошла путь от классической элегантности до самых смелых и трендовых дизайнов.</p>  
                    <p class="elegant-font">Особую нежность я питаю к сложным случаям — обожаю видеть, как даже самые «безнадежные» ноготки расцветают и начинают сиять! ✨</p>  
                    <p class="elegant-font">💨 Я — мастер скорости и качества! Ваша коррекция займет всего час, но каждая деталь будет безупречна.</p>  
                    <p class="elegant-font">Если вы ищете того, кто не просто делает маникюр, а вкладывает душу в каждый штрих — вы нашли свою волшебницу! ❤️</p>  
                    <p class="elegant-font">📍 Приходите, и ваши ручки получат ту самую заботу и эстетику, о которой они всегда мечтали!</p>  
                </section>  
            </div>  
              
            <div class="sidebar">  
                <div class="master-icon">  
                    ⚡️  
                </div>  
                <h3 class="feminine-font">Ваша фея красоты</h3>  
                <p class="elegant-font">Катя — мастер, который превращает обычный маникюр в настоящее искусство</p>  
                  
                <button class="book-btn feminine-font" id="bookBtn">  
                    ✨ Записаться на сеанс красоты  
                </button>  
                  
                <h3 class="feminine-font">Мои волшебные услуги</h3>  
                <ul class="services-list">  
                    <li class="elegant-font">Маникюр с покрытием гель-лаком</li>  
                    <li class="elegant-font">Укрепление и восстановление</li>  
                    <li class="elegant-font">Художественный дизайн</li>  
                    <li class="elegant-font">Френч любой сложности</li>  
                    <li class="elegant-font">Стемпинг и узоры</li>  
                    <li class="elegant-font">Таинственный кошачий глаз</li>  
                    <li class="elegant-font">Восстановление ноготков</li>  
                    <li class="elegant-font">Быстрая и качественная коррекция</li>  
                </ul>  
                  
                <div style="margin-top: 30px; text-align: center;">  
                    <h3 class="feminine-font">Мой мир вдохновения</h3>  
                    <a href="https://www.instagram.com/kateina_nails?igsh=aDkzejEzbTRrdXJk&utm_source=qr" class="social-link" target="_blank" style="color: #8b4a65; font-size: 1.4rem; font-family: 'Marck Script', cursive;">  
                        <i class="fab fa-instagram"></i> @kateina_nails  
                    </a>  
                </div>  
            </div>  
        </div>  
          
        <footer class="pink-card">  
            <div class="logo-container">  
                <div class="logo-icon">⚡️</div>  
                <div class="logo-text">Knails</div>  
            </div>  
            <p class="elegant-font">Ваша красота - наша страсть!</p>  
            <div class="social-links">  
                <a href="https://www.instagram.com/kateina_nails?igsh=aDkzejEzbTRrdXJk&utm_source=qr" class="social-link" target="_blank">  
                    <i class="fab fa-instagram"></i>  
                </a>  
            </div>  
            <p class="handwritten-font">© 2024 Knails. Все права защищены.</p>  
            <p style="margin-top: 15px; font-size: 1rem; font-family: 'Marck Script', cursive;">С любовью для ваших ноготочков! 💖</p>  
        </footer>  
    </div>  
      
    <!-- Модальное окно для записи -->  
    <div class="modal" id="bookingModal">  
        <div class="modal-content">  
            <h2 class="feminine-font">Запись в Knails 📅</h2>  
            <p class="elegant-font">Свяжитесь со мной для записи:</p>  
              
            <div class="contact-links">  
                <a href="https://t.me/Lazaryan0" class="contact-link" target="_blank">  
                    <i class="fab fa-telegram contact-icon telegram"></i>  
                    <div class="contact-text">  
                        <strong class="feminine-font">Telegram</strong>  
                        <span class="elegant-font">@Lazaryan0</span>  
                    </div>  
                </a>  
                <a href="https://wa.me/79881605058" class="contact-link" target="_blank">  
                    <i class="fab fa-whatsapp contact-icon whatsapp"></i>  
                    <div class="contact-text">  
                        <strong class="feminine-font">WhatsApp</strong>  
                        <span class="elegant-font">+7 988 160-50-58</span>  
                    </div>  
                </a>  
            </div>  
              
            <button class="close-btn">Закрыть</button>  
        </div>  
    </div>  
  
    <script>  
        // Система покупок и скидок  
        let purchasedVisits = 0;  
        const discountThreshold = 10;  
          
        function buyCertificate(type, visits) {  
            purchasedVisits += visits;  
              
            const progressElement = document.getElementById('discountProgress');  
            const progressText = document.getElementById('progressText');  
            const visitsLeftElement = document.getElementById('visitsLeft');  
            const progressFill = document.getElementById('progressFill');  
            const nextDiscountInfo = document.getElementById('nextDiscountInfo');  
              
            progressElement.style.display = 'block';  
              
            const visitsLeft = Math.max(0, discountThreshold - purchasedVisits);  
            const progressPercentage = Math.min(100, (purchasedVisits / discountThreshold) * 100);  
              
            visitsLeftElement.textContent = visitsLeft;  
            progressFill.style.width = progressPercentage + '%';  
              
            if (purchasedVisits >= discountThreshold) {  
                progressText.innerHTML = '🎉 Поздравляем! Вы получили скидку 30% на следующую покупку!';  
                nextDiscountInfo.textContent = 'Промокод для скидки: KN30';  
            } else {  
                progressText.innerHTML = `До следующей скидки осталось: <strong>${visitsLeft}</strong> посещений`;  
                nextDiscountInfo.textContent = `После ${discountThreshold} посещений вы получите скидку 30%!`;  
            }  
              
            let serviceName = type === 'extension' ? 'наращивание ногтей' : 'гель-лак';  
            alert(`🎊 Спасибо за покупку!\n\nВы приобрели сертификат на ${serviceName} - ${visits} посещений\n\nОбщее количество посещений: ${purchasedVisits}\n\n${visitsLeft > 0 ? `До скидки осталось: ${visitsLeft} посещений` : '🎉 Вы получили скидку 30%!'}`);  
        }  
          
        // Слайдер  
        let currentSlide = 0;  
        const slides = document.getElementById('slides');  
        const dots = document.querySelectorAll('.slider-dot');  
        const totalSlides = 5;  
  
        function showSlide(n) {  
            currentSlide = (n + totalSlides) % totalSlides;  
            slides.style.transform = `translateX(-${currentSlide * 100}%)`;  
              
            dots.forEach((dot, index) => {  
                dot.classList.toggle('active', index === currentSlide);  
            });  
        }  
  
        function nextSlide() {  
            showSlide(currentSlide + 1);  
        }  
  
        setInterval(nextSlide, 4000);  
  
        dots.forEach((dot, index) => {  
            dot.addEventListener('click', () => showSlide(index));  
        });  
  
        // Модальное окно  
        document.getElementById('bookBtn').addEventListener('click', function() {  
            document.getElementById('bookingModal').style.display = 'flex';  
        });  
          
        document.querySelector('.close-btn').addEventListener('click', function() {  
            document.getElementById('bookingModal').style.display = 'none';  
        });  
          
        window.addEventListener('click', function(event) {  
            if (event.target === document.getElementById('bookingModal')) {  
                document.getElementById('bookingModal').style.display = 'none';  
            }  
        });  
  
        // Поисковая строка  
        document.querySelector('.search-bar input').addEventListener('focus', function() {  
            if (!this.value) {  
                this.value = 'Knails ';  
            }  
        });  
    </script>  
</body>  
</html>  
