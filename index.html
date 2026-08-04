<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>🏛️ Липецкая область — интерактивный гид</title>

    <!-- ===== LEAFLET ===== -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js">
    </script>

    <!-- ===== ШРИФТ ===== -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800;900&display=swap" rel="stylesheet" />

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Montserrat', 'Segoe UI', Arial, sans-serif;
            background: #0a150a;
            min-height: 100vh;
            color: #d4e8d4;
        }
        .navbar {
            background: linear-gradient(145deg, #0f1a0f, #162216);
            padding: 14px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 2px solid #2d4a2d;
            position: sticky;
            top: 0;
            z-index: 999;
            backdrop-filter: blur(12px);
            flex-wrap: wrap;
            gap: 12px;
        }
        .navbar .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 22px;
            font-weight: 800;
            background: linear-gradient(135deg, #8bc34a, #ffd700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-decoration: none;
            cursor: pointer;
        }
        .navbar .logo span {
            font-size: 30px;
            -webkit-text-fill-color: initial;
        }
        .navbar .nav-links {
            display: flex;
            gap: 8px;
            flex-wrap: wrap;
        }
        .navbar .nav-links button {
            background: transparent;
            border: 2px solid #2d4a2d;
            color: #b8d8b8;
            padding: 8px 22px;
            border-radius: 30px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 600;
            font-size: 14px;
            cursor: pointer;
            transition: all 0.25s ease;
        }
        .navbar .nav-links button:hover {
            border-color: #ffd700;
            color: #ffd700;
            background: rgba(255, 215, 0, 0.06);
        }
        .navbar .nav-links button.active {
            border-color: #ffd700;
            background: rgba(255, 215, 0, 0.12);
            color: #ffd700;
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.05);
        }
        .page {
            display: none;
            max-width: 1300px;
            margin: 0 auto;
            padding: 30px 25px 40px;
            animation: fadeIn 0.5s ease;
        }
        .page.active {
            display: block;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .main-header {
            text-align: center;
            margin-bottom: 35px;
        }
        .main-header h1 {
            font-size: 40px;
            font-weight: 900;
            background: linear-gradient(135deg, #8bc34a, #cddc39, #ffd700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            letter-spacing: 1px;
        }
        .main-header p {
            color: #8aaa8a;
            font-size: 17px;
            margin-top: 6px;
            font-weight: 400;
        }
        .section-title {
            font-size: 24px;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 20px;
        }
        .section-title span {
            font-size: 30px;
        }
        .quiz-section {
            background: linear-gradient(145deg, #162216, #1a2a1a);
            border-radius: 30px;
            padding: 30px 35px 35px;
            border: 1px solid #2d4a2d;
            margin-bottom: 35px;
        }
        .quiz-question {
            font-size: 19px;
            font-weight: 600;
            color: #e8f4e8;
            margin-bottom: 16px;
            min-height: 50px;
        }
        .quiz-options {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-bottom: 16px;
        }
        .quiz-options button {
            background: rgba(255, 255, 255, 0.04);
            border: 2px solid #2d4a2d;
            color: #c8e0c8;
            padding: 12px 28px;
            border-radius: 40px;
            font-family: 'Montserrat', sans-serif;
            font-size: 15px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.15s ease;
        }
        .quiz-options button:hover:not(:disabled) {
            border-color: #8bc34a;
            background: rgba(139, 195, 74, 0.08);
            transform: translateY(-2px);
        }
        .quiz-options button:active:not(:disabled) {
            transform: translateY(1px);
        }
        .quiz-options button.correct {
            border-color: #7bed9f;
            background: rgba(123, 237, 159, 0.18);
            color: #7bed9f;
        }
        .quiz-options button.wrong {
            border-color: #ff6b6b;
            background: rgba(255, 107, 107, 0.15);
            color: #ff6b6b;
        }
        .quiz-options button:disabled {
            cursor: default;
            opacity: 0.6;
        }
        .quiz-feedback {
            padding: 14px 20px;
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.03);
            min-height: 52px;
            display: flex;
            align-items: center;
            gap: 14px;
            flex-wrap: wrap;
            border: 1px solid #1e3a1e;
            font-size: 15px;
        }
        .quiz-feedback .btn-next {
            margin-left: auto;
            background: #ffd700;
            color: #1a2a1a;
            border: none;
            padding: 8px 26px;
            border-radius: 30px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 14px;
            cursor: pointer;
            transition: 0.15s;
            box-shadow: 0 4px 0 #b89a2a;
        }
        .quiz-feedback .btn-next:active {
            transform: translateY(4px);
            box-shadow: 0 0px 0 #b89a2a;
        }
        .quiz-score {
            margin-top: 14px;
            color: #8aaa8a;
            font-size: 14px;
            font-weight: 600;
            text-align: right;
        }
        .quiz-score strong {
            color: #d4e8d4;
        }
        .city-section {
            background: linear-gradient(145deg, #162216, #1a2a1a);
            border-radius: 30px;
            padding: 25px 30px 30px;
            border: 1px solid #2d4a2d;
            margin-bottom: 30px;
        }
        .city-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 16px;
        }
        .city-card {
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid #2d4a2d;
            border-radius: 18px;
            overflow: hidden;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        .city-card:hover {
            border-color: #ffd700;
            transform: translateY(-5px);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.4);
        }
        .city-card .city-image {
            width: 100%;
            height: 140px;
            background: #1a2a1a;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }
        .city-card .city-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: 0.3s;
        }
        .city-card:hover .city-image img {
            transform: scale(1.05);
        }
        .city-card .city-image .no-image {
            color: #ff6b6b;
            font-size: 16px;
            font-weight: 700;
            text-align: center;
            padding: 10px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100%;
        }
        .city-card .city-image .no-image span {
            font-size: 40px;
        }
        .city-card .city-info {
            padding: 14px 16px 16px;
        }
        .city-card .city-name {
            font-weight: 700;
            font-size: 16px;
            color: #d4e8d4;
        }
        .city-card .city-desc {
            font-size: 12px;
            color: #7a9a7a;
            margin-top: 2px;
        }
        .city-card .city-emoji {
            font-size: 14px;
            margin-right: 6px;
        }
        .city-card.capital {
            border-color: #ffd700;
            background: rgba(255, 215, 0, 0.05);
        }
        .city-card.capital .city-name {
            color: #ffd700;
        }
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.85);
            backdrop-filter: blur(12px);
            z-index: 9999;
            justify-content: center;
            align-items: center;
            animation: fadeIn 0.3s ease;
        }
        .modal-overlay.active {
            display: flex;
        }
        .modal-content {
            background: #1a2a1a;
            border-radius: 30px;
            max-width: 700px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
            border: 2px solid #2d4a2d;
            padding: 0;
            animation: slideUp 0.3s ease;
        }
        @keyframes slideUp {
            from {
                transform: translateY(40px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
        .modal-content .modal-image {
            width: 100%;
            height: 350px;
            overflow: hidden;
            border-radius: 30px 30px 0 0;
            background: #0a150a;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .modal-content .modal-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .modal-content .modal-image .no-image {
            color: #ff6b6b;
            font-size: 20px;
            font-weight: 700;
            text-align: center;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100%;
        }
        .modal-content .modal-image .no-image span {
            font-size: 80px;
        }
        .modal-content .modal-body {
            padding: 24px 28px 28px;
        }
        .modal-content .modal-body h2 {
            font-size: 28px;
            font-weight: 800;
            color: #ffd700;
            margin-bottom: 6px;
        }
        .modal-content .modal-body .modal-sub {
            color: #8aaa8a;
            font-size: 14px;
            margin-bottom: 14px;
        }
        .modal-content .modal-body p {
            color: #c8e0c8;
            line-height: 1.7;
            font-size: 15px;
        }
        .modal-content .modal-body .modal-badge {
            display: inline-block;
            background: rgba(255, 215, 0, 0.15);
            color: #ffd700;
            padding: 2px 16px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 700;
            margin-bottom: 12px;
        }
        .modal-content .modal-body .modal-close {
            margin-top: 18px;
            background: #ffd700;
            color: #1a2a1a;
            border: none;
            padding: 10px 30px;
            border-radius: 30px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 14px;
            cursor: pointer;
            transition: 0.15s;
            box-shadow: 0 4px 0 #b89a2a;
        }
        .modal-content .modal-body .modal-close:active {
            transform: translateY(4px);
            box-shadow: 0 0px 0 #b89a2a;
        }
        .facts-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 16px;
            margin-top: 30px;
        }
        .fact-card {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid #1e3a1e;
            border-radius: 20px;
            padding: 20px 18px;
            text-align: center;
            transition: 0.2s;
        }
        .fact-card:hover {
            border-color: #2d4a2d;
            transform: translateY(-2px);
        }
        .fact-card .fact-emoji {
            font-size: 30px;
            display: block;
            margin-bottom: 6px;
        }
        .fact-card .fact-number {
            font-size: 24px;
            font-weight: 800;
            color: #ffd700;
        }
        .fact-card .fact-label {
            font-size: 13px;
            color: #8aaa8a;
            margin-top: 4px;
        }
        #map-page .map-wrapper {
            background: #162216;
            border-radius: 30px;
            padding: 18px;
            border: 1px solid #2d4a2d;
        }
        #map {
            height: 700px;
            border-radius: 20px;
            background: #1a2a1a;
            border: 2px solid #2d4a2d;
        }
        .map-legend {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px 35px;
            margin-top: 16px;
            padding: 12px 20px;
            background: rgba(10, 25, 10, 0.5);
            border-radius: 16px;
            border: 1px solid #2d4a2d;
        }
        .map-legend .item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 13px;
            color: #b8d8b8;
        }
        .map-legend .item .box {
            width: 20px;
            height: 20px;
            border-radius: 4px;
            border: 1px solid #4a7a4a;
            flex-shrink: 0;
        }
        .map-legend .item .box.circle {
            border-radius: 50%;
            width: 16px;
            height: 16px;
        }
        .map-legend .item .box.border-red {
            border: 3px solid #ff1744;
            background: transparent;
            border-radius: 4px;
            width: 30px;
            height: 4px;
        }
        .map-legend .item .box.dashed {
            border: 2px dashed #4a6a4a;
            background: transparent;
            width: 30px;
            height: 2px;
            border-radius: 0;
        }
        .footer-site {
            text-align: center;
            padding: 25px 20px 15px;
            border-top: 1px solid #1a2a1a;
            color: #4a6a4a;
            font-size: 13px;
            max-width: 1300px;
            margin: 0 auto;
        }
        .footer-site span {
            color: #6a8a6a;
        }
        .leaflet-popup-content {
            font-family: 'Montserrat', 'Segoe UI', Arial, sans-serif !important;
            font-size: 14px !important;
            min-width: 180px;
        }
        .leaflet-popup-content strong {
            color: #1e5a1e;
            font-size: 18px;
            display: block;
            margin-bottom: 4px;
        }
        .leaflet-popup-content .popup-desc {
            color: #333;
            font-size: 13px;
            line-height: 1.5;
        }
        .leaflet-popup-content .popup-badge {
            display: inline-block;
            background: #2d6a2d;
            color: white;
            padding: 2px 14px;
            border-radius: 20px;
            font-size: 10px;
            font-weight: 700;
            text-transform: uppercase;
            margin-top: 6px;
        }
        .leaflet-popup-content .popup-badge.capital {
            background: #ffd700;
            color: #1a2a1a;
        }
        .leaflet-popup-content-wrapper {
            border-radius: 16px !important;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.4) !important;
        }
        .leaflet-popup-tip {
            background: white !important;
        }
        .custom-marker {
            background: none;
            border: none;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.8);
        }
        .compass-container {
            background: rgba(10, 25, 10, 0.88);
            backdrop-filter: blur(8px);
            border: 2px solid #3a6a3a;
            border-radius: 50%;
            width: 60px;
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.6);
            position: relative;
            transition: 0.3s;
        }
        .compass-container:hover {
            border-color: #ffd700;
            transform: scale(1.05);
        }
        .compass-container .n {
            position: absolute;
            top: 4px;
            font-size: 13px;
            font-weight: 900;
            color: #ff6b6b;
        }
        .compass-container .s {
            position: absolute;
            bottom: 4px;
            font-size: 10px;
            font-weight: 600;
            color: #6a8a6a;
        }
        .compass-container .w {
            position: absolute;
            left: 5px;
            font-size: 10px;
            font-weight: 600;
            color: #6a8a6a;
        }
        .compass-container .e {
            position: absolute;
            right: 5px;
            font-size: 10px;
            font-weight: 600;
            color: #6a8a6a;
        }
        .compass-container .line-v {
            width: 2px;
            height: 32px;
            background: rgba(255, 107, 107, 0.2);
            position: absolute;
        }
        .compass-container .line-h {
            width: 32px;
            height: 2px;
            background: rgba(200, 200, 200, 0.12);
            position: absolute;
        }
        .compass-container .center-dot {
            width: 5px;
            height: 5px;
            background: #ffd700;
            border-radius: 50%;
            position: absolute;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.3);
        }

        /* ============================================================
                   ВАЖНО: СТИЛИ ДЛЯ КАСТОМНЫХ МАРКЕРОВ
                   ============================================================ */
        .my-marker {
            background: none !important;
            border: none !important;
            font-size: 32px !important;
            line-height: 32px !important;
            text-align: center !important;
            text-shadow: 0 0 20px rgba(0, 0, 0, 0.9), 0 0 40px rgba(0, 0, 0, 0.5) !important;
        }

        .my-marker-star {
            color: #ffd700 !important;
            font-size: 42px !important;
            text-shadow: 0 0 30px rgba(255, 215, 0, 0.6) !important;
        }

        .my-marker-dot {
            color: #ff6b6b !important;
            font-size: 28px !important;
        }

        @media (max-width: 768px) {
            .navbar {
                padding: 10px 16px;
            }
            .navbar .logo {
                font-size: 18px;
            }
            .navbar .logo span {
                font-size: 24px;
            }
            .navbar .nav-links button {
                padding: 6px 14px;
                font-size: 12px;
            }
            .page {
                padding: 16px 12px 30px;
            }
            .main-header h1 {
                font-size: 28px;
            }
            .main-header p {
                font-size: 14px;
            }
            .section-title {
                font-size: 20px;
            }
            .quiz-section {
                padding: 20px 18px 24px;
            }
            .quiz-question {
                font-size: 16px;
            }
            .quiz-options button {
                padding: 10px 18px;
                font-size: 13px;
            }
            .city-grid {
                grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            }
            .city-card .city-image {
                height: 110px;
            }
            #map {
                height: 460px;
            }
            .facts-section {
                grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
                gap: 12px;
            }
            .fact-card .fact-number {
                font-size: 20px;
            }
            .map-legend {
                gap: 10px 18px;
                font-size: 11px;
                padding: 10px 14px;
            }
            .map-legend .item {
                font-size: 11px;
            }
            .modal-content .modal-image {
                height: 220px;
            }
            .modal-content .modal-body {
                padding: 18px 20px 22px;
            }
            .modal-content .modal-body h2 {
                font-size: 22px;
            }
        }
        @media (max-width: 480px) {
            .navbar .logo {
                font-size: 15px;
            }
            .navbar .nav-links button {
                padding: 5px 12px;
                font-size: 11px;
            }
            .main-header h1 {
                font-size: 22px;
            }
            .quiz-options button {
                padding: 8px 14px;
                font-size: 12px;
                width: 100%;
            }
            .city-grid {
                grid-template-columns: repeat(auto-fill, minmax(130px, 1fr));
                gap: 10px;
            }
            .city-card .city-image {
                height: 90px;
            }
            .city-card .city-info {
                padding: 10px 12px 12px;
            }
            .city-card .city-name {
                font-size: 14px;
            }
            #map {
                height: 340px;
            }
            .quiz-feedback {
                font-size: 13px;
                padding: 12px 14px;
            }
            .quiz-feedback .btn-next {
                font-size: 12px;
                padding: 6px 18px;
            }
            .modal-content .modal-image {
                height: 170px;
            }
            .modal-content .modal-body h2 {
                font-size: 19px;
            }
            .modal-content .modal-body p {
                font-size: 14px;
            }
        }
    </style>
</head>
<body>

    <!-- ============================================================
    НАВИГАЦИЯ
    ============================================================ -->
    <nav class="navbar">
        <a href="#" class="logo" onclick="switchPage('main')">
            <span>🏛️</span> Липецкая область
        </a>
        <div class="nav-links">
            <button class="active" id="navMain" onclick="switchPage('main')">🏠 Главная</button>
            <button id="navMap" onclick="switchPage('map')">🗺️ Карта</button>
        </div>
    </nav>

    <!-- ============================================================
    ГЛАВНАЯ СТРАНИЦА
    ============================================================ -->
    <div class="page active" id="main-page">
        <div class="main-header">
            <h1>🏛️ Добро пожаловать в Липецкую область!</h1>
            <p>интерактивный гид по сердцу Черноземья 🌾</p>
        </div>

        <!-- ВИКТОРИНА -->
        <div class="quiz-section">
            <div class="section-title"><span>🧠</span> Викторина «Знаешь ли ты область?»</div>
            <div class="quiz-question" id="quizQuestion">Загрузка вопроса...</div>
            <div class="quiz-options" id="quizOptions"></div>
            <div class="quiz-feedback" id="quizFeedback">
                <span>💡 Нажми на вариант ответа</span>
            </div>
            <div class="quiz-score" id="quizScore">✅ правильно: <strong>0</strong> &nbsp;|&nbsp; ❌ неправильно: <strong>0</strong></div>
        </div>

        <!-- ГОРОДА -->
        <div class="city-section">
            <div class="section-title"><span>🏙️</span> Города Липецкой области</div>
            <div class="city-grid" id="cityGrid"></div>
        </div>

        <!-- ФАКТЫ -->
        <div class="facts-section">
            <div class="fact-card">
                <span class="fact-emoji">🏛️</span>
                <div class="fact-number">18</div>
                <div class="fact-label">городов и райцентров</div>
            </div>
            <div class="fact-card">
                <span class="fact-emoji">📅</span>
                <div class="fact-number">1703</div>
                <div class="fact-label">год основания Липецка</div>
            </div>
            <div class="fact-card">
                <span class="fact-emoji">🌊</span>
                <div class="fact-number">2</div>
                <div class="fact-label">крупные реки: Дон и Воронеж</div>
            </div>
            <div class="fact-card">
                <span class="fact-emoji">🌾</span>
                <div class="fact-number">~200</div>
                <div class="fact-label">км с севера на юг</div>
            </div>
            <div class="fact-card">
                <span class="fact-emoji">⛪</span>
                <div class="fact-number">1146</div>
                <div class="fact-label">год первого упоминания Ельца</div>
            </div>
            <div class="fact-card">
                <span class="fact-emoji">🏭</span>
                <div class="fact-number">17</div>
                <div class="fact-label">муниципальных районов</div>
            </div>
        </div>
    </div>

    <!-- ============================================================
    СТРАНИЦА КАРТЫ
    ============================================================ -->
    <div class="page" id="map-page">
        <div class="main-header">
            <h1>🗺️ Интерактивная карта</h1>
            <p>реальные границы · наведи на район — узнай подробности</p>
        </div>

        <div class="map-wrapper">
            <div id="map"></div>
            <div class="map-legend">
                <span class="item"><span class="box" style="background:#2d6a2d;"></span> районы</span>
                <span class="item"><span class="box circle" style="background:#ffd700; border-color:#ffd700;"></span> столица ⭐</span>
                <span class="item"><span class="box circle" style="background:#ff6b6b; border-color:#ff6b6b;"></span> города 📍</span>
                <span class="item"><span class="box border-red"></span> граница области</span>
                <span class="item"><span class="box dashed"></span> соседние регионы</span>
                <span class="item"><span class="box" style="background:#4a8aaa;"></span> реки</span>
            </div>
        </div>

        <div style="text-align:center; margin-top:18px; color:#6a8a6a; font-size:13px;">
            🔄 наведи на район — подсветится · кликни для подробностей
        </div>
    </div>

    <!-- ============================================================
    ФУТЕР
    ============================================================ -->
    <div class="footer-site">
        <span>🌾 интерактивный гид по Липецкой области · 2026</span>
        <br>
        <span style="font-size:11px; color:#4a6a4a;">данные с OpenStreetMap · сделано с ❤️</span>
    </div>

    <!-- ============================================================
    МОДАЛКА
    ============================================================ -->
    <div class="modal-overlay" id="cityModal">
        <div class="modal-content">
            <div class="modal-image" id="modalImage"></div>
            <div class="modal-body">
                <div class="modal-badge" id="modalBadge">🏙️ ГОРОД</div>
                <h2 id="modalTitle">Название</h2>
                <div class="modal-sub" id="modalSub">описание</div>
                <p id="modalDesc">Подробная информация о городе</p>
                <button class="modal-close" onclick="closeModal()">✕ Закрыть</button>
            </div>
        </div>
    </div>

    <!-- ============================================================
    СКРИПТ
    ============================================================ -->
    <script>
        // ============================================================
        //  1. ПЕРЕКЛЮЧЕНИЕ СТРАНИЦ
        // ============================================================
        function switchPage(page) {
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            document.getElementById(page + '-page').classList.add('active');

            document.querySelectorAll('.nav-links button').forEach(b => b.classList.remove('active'));
            document.getElementById(page === 'main' ? 'navMain' : 'navMap').classList.add('active');

            if (page === 'map' && !window.mapInitialized) {
                initMap();
            }
        }

        // ============================================================
        //  2. ВИКТОРИНА
        // ============================================================
        const QUIZ = [
            { question: 'Какой город Липецкой области считается самым древним?', options: ['Липецк', 'Елец', 'Данков', 'Задонск'], correct: 1 },
            { question: 'Что является символом Лебедяни?', options: ['Яблоня', 'Подсолнух', 'Пшеница', 'Клён'], correct: 0 },
            { question: 'В каком городе находится знаменитый Задонский монастырь?', options: ['Елец', 'Липецк', 'Задонск', 'Чаплыгин'], correct: 2 },
            { question: 'Какая река протекает через Липецк?', options: ['Дон', 'Воронеж', 'Ока', 'Волга'], correct: 1 },
            { question: 'В каком районе находится "Галичья гора"?', options: ['Данковский', 'Усманский', 'Грязинский', 'Лебедянский'], correct: 0 },
            { question: 'Кто дал имя городу Чаплыгин?', options: ['Лобачевский', 'Чаплыгин', 'Колмогоров', 'Перельман'], correct: 1 },
            { question: 'Сколько муниципальных районов в Липецкой области?', options: ['12', '15', '17', '20'], correct: 2 },
            { question: 'В каком году основан Липецк?', options: ['1603', '1703', '1803', '1903'], correct: 1 }
        ];

        let quizState = { index: 0, correct: 0, wrong: 0, answered: false };

        function loadQuiz(index) {
            if (index >= QUIZ.length) {
                document.getElementById('quizQuestion').textContent = '🎉 Викторина завершена!';
                document.getElementById('quizOptions').innerHTML = '';
                document.getElementById('quizFeedback').innerHTML = `<span>🏆 Результат: ${quizState.correct} из ${QUIZ.length}</span>`;
                document.getElementById('quizScore').innerHTML = `✅ правильно: <strong>${quizState.correct}</strong>  |  ❌ неправильно: <strong>${quizState.wrong}</strong>`;
                return;
            }

            const q = QUIZ[index];
            document.getElementById('quizQuestion').textContent = `${index+1}. ${q.question}`;
            const container = document.getElementById('quizOptions');
            container.innerHTML = '';

            q.options.forEach((text, i) => {
                const btn = document.createElement('button');
                btn.textContent = text;
                btn.addEventListener('click', () => handleAnswer(i));
                container.appendChild(btn);
            });

            document.getElementById('quizFeedback').innerHTML = '<span>💡 выбери вариант</span>';
            quizState.answered = false;
            document.querySelectorAll('#quizOptions button').forEach(b => b.disabled = false);
            updateScore();
        }

        function handleAnswer(selected) {
            if (quizState.answered) return;
            quizState.answered = true;

            const q = QUIZ[quizState.index];
            const buttons = document.querySelectorAll('#quizOptions button');

            buttons.forEach((b, i) => {
                b.disabled = true;
                if (i === q.correct) b.classList.add('correct');
                else if (i === selected && selected !== q.correct) b.classList.add('wrong');
            });

            const isCorrect = selected === q.correct;
            isCorrect ? quizState.correct++ : quizState.wrong++;

            const feedback = document.getElementById('quizFeedback');
            feedback.innerHTML = isCorrect ?
                `✅ <strong>Верно!</strong> ${q.options[q.correct]}` :
                `❌ <strong>Неверно.</strong> Правильный ответ: ${q.options[q.correct]}`;

            const nextBtn = document.createElement('button');
            nextBtn.className = 'btn-next';
            nextBtn.textContent = quizState.index < QUIZ.length - 1 ? '➡️ дальше' : '🏁 финиш';
            nextBtn.addEventListener('click', () => {
                quizState.index++;
                loadQuiz(quizState.index);
            });
            feedback.appendChild(nextBtn);
            updateScore();
        }

        function updateScore() {
            document.getElementById('quizScore').innerHTML =
                `✅ правильно: <strong>${quizState.correct}</strong>  |  ❌ неправильно: <strong>${quizState.wrong}</strong>`;
        }

        // ============================================================
        //  3. ГОРОДА (ДЛЯ ГЛАВНОЙ СТРАНИЦЫ)
        // ============================================================
        const CITIES = [
            { name: 'Липецк', emoji: '⭐', desc: 'столица', capital: true, img: 'images/lipetsk.jpg', fullDesc: 'Административный центр Липецкой области. Крупный промышленный город. Основан в 1703 году.' },
            { name: 'Елец', emoji: '⛪', desc: 'древний город', capital: false, img: 'images/elets.jpg', fullDesc: 'Известен с 1146 года. Богатая купеческая история, знаменит елецким кружевом.' },
            { name: 'Грязи', emoji: '🚂', desc: 'транспортный узел', capital: false, img: 'images/gryazi.jpg', fullDesc: 'Крупный железнодорожный узел. Название от грязевых вулканов.' },
            { name: 'Данков', emoji: '🏞️', desc: 'природа', capital: false, img: 'images/dankov.jpg', fullDesc: 'Город на Дону. Рядом — "Галичья гора" с реликтовыми растениями.' },
            { name: 'Лебедянь', emoji: '🍎', desc: 'сады', capital: false, img: 'images/lebedyan.jpg', fullDesc: 'Город-сад, знаменитый яблоневыми садами и праздником "Яблочный спас".' },
            { name: 'Чаплыгин', emoji: '🐎', desc: 'конный', capital: false, img: 'images/chaplygin.jpg', fullDesc: 'Родина математика Чаплыгина. В городе крупный конный завод.' },
            { name: 'Задонск', emoji: '🕊️', desc: 'духовный центр', capital: false, img: 'images/zadonsk.jpg', fullDesc: 'Знаменитый Задонский монастырь, мощи святителя Тихона Задонского.' },
            { name: 'Усмань', emoji: '🌲', desc: 'лес', capital: false, img: 'images/usman.jpg', fullDesc: 'Усманский бор — реликтовый лес с соснами возрастом более 200 лет.' },
            { name: 'Доброе', emoji: '🌻', desc: 'северо-восток', capital: false, img: 'images/dobroe.jpg', fullDesc: 'Центр Добровского района на реке Воронеж. Богатая история.' },
            { name: 'Красное', emoji: '🏘️', desc: 'север', capital: false, img: 'images/krasnoe.jpg', fullDesc: 'Центр Краснинского района на севере области, граничит с Тульской областью.' },
            { name: 'Тербуны', emoji: '🌾', desc: 'юго-запад', capital: false, img: 'images/terbuny.jpg', fullDesc: 'Центр Тербунского района. Здесь находится крупный сахарный завод.' },
            { name: 'Измалково', emoji: '🏡', desc: 'запад', capital: false, img: 'images/izmalkovo.jpg', fullDesc: 'Центр Измалковского района на западе области.' },
            { name: 'Долгоруково', emoji: '🏡', desc: 'юго-запад', capital: false, img: 'images/dolgorukovo.jpg', fullDesc: 'Центр Долгоруковского района на юго-западе области.' },
            { name: 'Хлевное', emoji: '🏡', desc: 'юг', capital: false, img: 'images/khlevnoe.jpg', fullDesc: 'Центр Хлевенского района на юге области.' },
            { name: 'Добринка', emoji: '🏡', desc: 'юго-восток', capital: false, img: 'images/dobrinka.jpg', fullDesc: 'Центр Добринского района на юго-востоке области.' },
            { name: 'Волово', emoji: '🏡', desc: 'запад', capital: false, img: 'images/volovo.jpg', fullDesc: 'Центр Воловского района на западе, граничит с Орловской областью.' },
            { name: 'Становое', emoji: '🏡', desc: 'северо-запад', capital: false, img: 'images/stanovoye.jpg', fullDesc: 'Центр Становлянского района на северо-западе области.' },
            { name: 'Лев-Толстой', emoji: '📚', desc: 'имение Толстого', capital: false, img: 'images/lev-tolstoy.jpg', fullDesc: 'Музей-усадьба Л.Н. Толстого, где он работал над "Анной Карениной".' }
        ];

        function renderCities() {
            const grid = document.getElementById('cityGrid');
            grid.innerHTML = '';

            CITIES.forEach(city => {
                const card = document.createElement('div');
                card.className = 'city-card' + (city.capital ? ' capital' : '');
                card.innerHTML = `
                    <div class="city-image">
                        <img src="${city.img}" alt="${city.name}" 
                             onerror="this.style.display='none'; this.parentElement.innerHTML='<div class=\\'no-image\\'><span>🤷‍♂️</span>автор распиздяй,<br>поэтому фоток нет :)</div>';">
                    </div>
                    <div class="city-info">
                        <div class="city-name"><span class="city-emoji">${city.emoji}</span>${city.name}</div>
                        <div class="city-desc">${city.desc}</div>
                    </div>
                `;
                card.addEventListener('click', () => openModal(city));
                grid.appendChild(card);
            });
        }

        // ============================================================
        //  4. МОДАЛКА
        // ============================================================
        function openModal(city) {
            document.getElementById('modalBadge').textContent = city.capital ? '⭐ СТОЛИЦА' : '🏙️ ГОРОД';
            document.getElementById('modalTitle').textContent = city.name;
            document.getElementById('modalSub').textContent = city.desc;
            document.getElementById('modalDesc').textContent = city.fullDesc;

            const imgContainer = document.getElementById('modalImage');
            imgContainer.innerHTML = `
                <img src="${city.img}" alt="${city.name}" 
                     onerror="this.style.display='none'; this.parentElement.innerHTML='<div class=\\'no-image\\'><span>🤷‍♂️</span>автор распиздяй,<br>поэтому фоток нет :)</div>';">
            `;

            document.getElementById('cityModal').classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            document.getElementById('cityModal').classList.remove('active');
            document.body.style.overflow = '';
        }

        document.getElementById('cityModal').addEventListener('click', e => { if (e.target === e.currentTarget) closeModal(); });
        document.addEventListener('keydown', e => { if (e.key === 'Escape') closeModal(); });

        // ============================================================
        //  5. КАРТА — С МАРКЕРАМИ (НАСТОЯЩИМИ!)
        // ============================================================
        let mapInitialized = false;

        function initMap() {
            if (mapInitialized) return;
            mapInitialized = true;

            // 1. СОЗДАЁМ КАРТУ
            const map = L.map('map', { center: [52.6, 39.6], zoom: 8 });

            // 2. ДОБАВЛЯЕМ СЛОЙ
            L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                attribution: '© OpenStreetMap',
                maxZoom: 18,
            }).addTo(map);

            // 3. МАСШТАБ
            L.control.scale({ position: 'bottomright', metric: true, imperial: false }).addTo(map);

            // 4. КОМПАС
            L.Control.extend({
                options: { position: 'topright' },
                onAdd: () => {
                    const div = L.DomUtil.create('div');
                    div.innerHTML = `
                        <div class="compass-container">
                            <span class="n">N</span>
                            <span class="s">S</span>
                            <span class="w">W</span>
                            <span class="e">E</span>
                            <div class="line-v"></div>
                            <div class="line-h"></div>
                            <div class="center-dot"></div>
                        </div>`;
                    return div;
                }
            }).addTo(map);

            // ============================================================
            //  ВСЕ 18 ГОРОДОВ НА КАРТЕ — ЭМОДЗИ МАРКЕРЫ (ВИДНЫ!)
            // ============================================================
            const cityCoords = [
                { name: 'Липецк', lat: 52.61, lng: 39.60, capital: true },
                { name: 'Елец', lat: 52.62, lng: 38.50, capital: false },
                { name: 'Грязи', lat: 52.50, lng: 40.00, capital: false },
                { name: 'Данков', lat: 53.25, lng: 39.15, capital: false },
                { name: 'Лебедянь', lat: 53.02, lng: 39.50, capital: false },
                { name: 'Чаплыгин', lat: 53.10, lng: 40.10, capital: false },
                { name: 'Задонск', lat: 52.40, lng: 38.90, capital: false },
                { name: 'Усмань', lat: 52.05, lng: 39.75, capital: false },
                { name: 'Доброе', lat: 52.85, lng: 39.80, capital: false },
                { name: 'Красное', lat: 53.00, lng: 38.90, capital: false },
                { name: 'Тербуны', lat: 52.15, lng: 38.30, capital: false },
                { name: 'Измалково', lat: 52.70, lng: 38.00, capital: false },
                { name: 'Долгоруково', lat: 52.35, lng: 38.40, capital: false },
                { name: 'Хлевное', lat: 52.20, lng: 39.10, capital: false },
                { name: 'Добринка', lat: 52.20, lng: 40.50, capital: false },
                { name: 'Волово', lat: 52.00, lng: 38.00, capital: false },
                { name: 'Становое', lat: 52.80, lng: 38.40, capital: false },
                { name: 'Лев-Толстой', lat: 53.20, lng: 39.45, capital: false }
            ];

            console.log('🗺️ ДОБАВЛЯЕМ МАРКЕРЫ НА КАРТУ:');

            cityCoords.forEach((c, index) => {
                // === КАСТОМНЫЙ МАРКЕР С ЭМОДЗИ ===
                const markerHtml = c.capital ?
                    `<div class="my-marker my-marker-star">⭐</div>` :
                    `<div class="my-marker my-marker-dot">📍</div>`;

                const icon = L.divIcon({
                    html: markerHtml,
                    className: 'my-marker',
                    iconSize: c.capital ? [42, 42] : [32, 32],
                    iconAnchor: c.capital ? [21, 42] : [16, 32],
                });

                const marker = L.marker([c.lat, c.lng], { icon })
                    .addTo(map)
                    .bindPopup(`
                        <strong>${c.capital ? '⭐ ' : ''}${c.name}</strong>
                        <div class="popup-desc">${c.capital ? '🏛️ Административный центр области' : 'Город Липецкой области'}</div>
                        <span class="popup-badge ${c.capital ? 'capital' : ''}">${c.capital ? '🏛️ СТОЛИЦА' : '🏙️ ГОРОД'}</span>
                    `);

                marker.on('mouseover', function() {
                    this.openPopup();
                });

                // === ПОДПИСЬ ПОД МАРКЕРОМ ===
                const label = L.divIcon({
                    html: `<div style="
                        color: #fff;
                        font-size: ${c.capital ? '15px' : '12px'};
                        font-weight: ${c.capital ? '800' : '600'};
                        text-shadow: 0 0 15px rgba(0,0,0,0.95), 0 0 30px rgba(0,0,0,0.7);
                        font-family: 'Montserrat', sans-serif;
                        background: rgba(0,0,0,0.5);
                        padding: 2px 12px;
                        border-radius: 12px;
                        border: 1px solid ${c.capital ? '#ffd700' : 'rgba(255,255,255,0.15)'};
                        backdrop-filter: blur(4px);
                        white-space: nowrap;
                        margin-top: 5px;
                    ">${c.name}</div>`,
                    className: 'city-label',
                    iconSize: [0, 0],
                    iconAnchor: [0, 0],
                });

                L.marker([c.lat - 0.03, c.lng], { icon: label, interactive: false })
                    .addTo(map);

                console.log(`   ${index+1}. ${c.capital ? '⭐' : '📍'} ${c.name} → lat:${c.lat}, lng:${c.lng}`);
            });

            // ============================================================
            //  РАЙОНЫ
            // ============================================================
            const districtIds = [
                { id: 150116, name: 'Липецкий район' },
                { id: 150117, name: 'Елецкий район' },
                { id: 150118, name: 'Грязинский район' },
                { id: 150119, name: 'Данковский район' },
                { id: 150120, name: 'Лебедянский район' },
                { id: 150121, name: 'Чаплыгинский район' },
                { id: 150122, name: 'Задонский район' },
                { id: 150123, name: 'Усманский район' },
                { id: 150124, name: 'Тербунский район' },
                { id: 150125, name: 'Добровский район' },
                { id: 150126, name: 'Краснинский район' },
                { id: 150127, name: 'Измалковский район' },
                { id: 150128, name: 'Долгоруковский район' },
                { id: 150129, name: 'Хлевенский район' },
                { id: 150130, name: 'Добринский район' },
                { id: 150131, name: 'Воловский район' },
                { id: 150132, name: 'Становлянский район' }
            ];

            const colors = ['#2d6a2d', '#256025', '#3a7a3a', '#1e5a1e'];

            districtIds.forEach((d, i) => {
                const url = `https://overpass-api.de/api/interpreter?data=[out:json];(relation(${d.id}););out%20body;>;out%20skel%20qt;`;
                fetch(url)
                    .then(r => r.json())
                    .then(data => {
                        const coords = [];
                        const nodes = {};
                        data.elements.forEach(el => { if (el.type === 'node') nodes[el.id] = [el.lat, el.lon]; });
                        data.elements.forEach(el => {
                            if (el.type === 'relation' && el.id === d.id) {
                                el.members.forEach(m => {
                                    if (m.type === 'way') {
                                        const way = data.elements.find(e => e.type === 'way' && e.id === m.ref);
                                        if (way && way.nodes) {
                                            way.nodes.forEach(n => { if (nodes[n]) coords.push(nodes[n]); });
                                        }
                                    }
                                });
                            }
                        });
                        if (coords.length > 3) {
                            const c = colors[i % colors.length];
                            const poly = L.polygon(coords, {
                                color: c,
                                weight: 2.5,
                                opacity: 0.85,
                                fillColor: c,
                                fillOpacity: 0.3,
                            }).addTo(map)
                                .bindPopup(`
                                    <strong>${d.name}</strong>
                                    <div class="popup-desc">Муниципальный район</div>
                                    <span class="popup-badge">📍 РАЙОН</span>
                                `);
                            poly.on('mouseover', function() {
                                this.setStyle({ fillOpacity: 0.55, weight: 4, color: '#ffd700' });
                                this.bringToFront();
                            });
                            poly.on('mouseout', function() {
                                this.setStyle({ fillOpacity: 0.3, weight: 2.5, color: c });
                            });
                        }
                    }).catch(() => {});
            });

            // ============================================================
            //  ГРАНИЦА ОБЛАСТИ — КРАСНАЯ!
            // ============================================================
            fetch('https://overpass-api.de/api/interpreter?data=[out:json];(relation(79975););out%20body;>;out%20skel%20qt;')
                .then(r => r.json())
                .then(data => {
                    const coords = [];
                    const nodes = {};
                    data.elements.forEach(el => { if (el.type === 'node') nodes[el.id] = [el.lat, el.lon]; });
                    data.elements.forEach(el => {
                        if (el.type === 'relation' && el.id === 79975) {
                            el.members.forEach(m => {
                                if (m.type === 'way') {
                                    const way = data.elements.find(e => e.type === 'way' && e.id === m.ref);
                                    if (way && way.nodes) {
                                        way.nodes.forEach(n => { if (nodes[n]) coords.push(nodes[n]); });
                                    }
                                }
                            });
                        }
                    });
                    if (coords.length > 3) {
                        L.polygon(coords, { color: '#ff1744', weight: 5, opacity: 0.85, fillColor: 'transparent', fillOpacity: 0 })
                            .addTo(map);
                        L.polygon(coords, { color: '#ff1744', weight: 14, opacity: 0.12, fillColor: 'transparent', fillOpacity: 0 })
                            .addTo(map);
                        console.log('✅ КРАСНАЯ ГРАНИЦА загружена!');
                    }
                }).catch(() => {});

            // ============================================================
            //  РЕКИ
            // ============================================================
            [
                [
                    [53.35, 39.05],
                    [52.00, 39.75],
                    [51.90, 39.80]
                ],
                [
                    [53.00, 39.10],
                    [51.90, 39.65]
                ]
            ].forEach(r => {
                L.polyline(r, { color: '#4a8aaa', weight: 4, opacity: 0.5 }).addTo(map);
            });

            // ============================================================
            //  СОСЕДНИЕ РЕГИОНЫ
            // ============================================================
            [
                { name: 'Рязанская обл.', lat: 53.60, lng: 40.00 },
                { name: 'Тамбовская обл.', lat: 52.30, lng: 41.50 },
                { name: 'Воронежская обл.', lat: 51.50, lng: 39.80 },
                { name: 'Орловская обл.', lat: 52.30, lng: 36.80 },
                { name: 'Тульская обл.', lat: 53.80, lng: 38.00 }
            ].forEach(n => {
                L.marker([n.lat, n.lng], {
                    icon: L.divIcon({
                        html: `<div style="background:rgba(10,25,10,0.6);backdrop-filter:blur(4px);color:#5a7a5a;font-size:10px;font-weight:600;padding:2px 10px;border-radius:12px;border:1px dashed #4a6a4a;white-space:nowrap;font-family:'Montserrat',sans-serif;">${n.name}</div>`,
                        iconSize: [0, 0],
                        iconAnchor: [0, 0]
                    }),
                    interactive: false
                }).addTo(map);
            });

            // Фокусируем карту на область
            setTimeout(() => map.fitBounds([
                [53.6, 36.0],
                [51.5, 41.5]
            ]), 500);

            console.log('🗺️ Карта загружена с 18 городами!');
            console.log('📍 ТЕПЕРЬ МАРКЕРЫ ДОЛЖНЫ БЫТЬ ВИДНЫ! ⭐ и 📍');
        }

        // ============================================================
        //  6. ЗАПУСК
        // ============================================================
        renderCities();
        loadQuiz(0);

        setTimeout(() => {
            if (!mapInitialized) {
                const tempDiv = document.createElement('div');
                tempDiv.style.display = 'none';
                document.body.appendChild(tempDiv);
                const tempMap = L.map(tempDiv, { center: [52.6, 39.6], zoom: 8 });
                tempMap.remove();
                document.body.removeChild(tempDiv);
            }
        }, 1000);

        console.log('🏛️ Сайт Липецкой области загружен!');
        console.log('📍 На карте есть все 18 городов с маркерами!');
        console.log('📸 Если нет фото — покажется "автор распиздяй"');
    </script>

</body>
</html>
