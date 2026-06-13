<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Официальный портал | Росфинмониторинг</title>
    <style>
        :root {
            --rfm-dark: #071931;
            --rfm-blue: #004682;
            --rfm-light-blue: #f0f4f8;
            --accent-gold: #c5a059;
            --text-dark: #222222;
            --portfolio-bg: #0f172a;
            --neon-blue: #38bdf8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, sans-serif;
        }

        body {
            background-color: var(--rfm-light-blue);
            color: var(--text-dark);
            line-height: 1.5;
        }

        /* ВЕРХНЯЯ ЛИНИЯ И МЕНЮ */
        .top-navbar {
            background-color: var(--rfm-dark);
            color: white;
            padding: 15px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 2px solid var(--accent-gold);
            font-size: 14px;
        }

        .nav-left {
            display: flex;
            align-items: center;
            gap: 12px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .nav-right {
            display: flex;
            gap: 20px;
            font-weight: 600;
        }

        .nav-right a {
            color: #e2e8f0;
            text-decoration: none;
        }

        .nav-right a:hover {
            color: var(--accent-gold);
        }

        /* ЮБИЛЕЙНЫЙ БАННЕР 25 ЛЕТ */
        .hero-banner {
            background: linear-gradient(180deg, #02254b 0%, #004481 100%);
            color: white;
            padding: 60px 20px;
            text-align: center;
            position: relative;
        }

        .hero-banner h1 {
            font-size: 46px;
            font-weight: 800;
            letter-spacing: 3px;
            margin-top: 15px;
            text-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }

        .anniversary-sub {
            font-size: 13px;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            color: #93c5fd;
            margin-top: 5px;
        }

        /* ОСНОВНОЙ КОНТЕНТ */
        .main-content {
            max-width: 1240px;
            margin: 40px auto;
            padding: 0 20px;
            display: flex;
            flex-direction: column;
            gap: 35px;
        }

        /* ИНФОРМАЦИОННАЯ СЕТКА (КАК НА СКРИНШОТАХ) */
        .info-grid {
            display: grid;
            grid-template-columns: 1fr 1.8fr;
            gap: 25px;
        }

        .block-card {
            background: white;
            border-radius: 8px;
            padding: 25px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.03);
        }

        .block-card h2 {
            font-size: 18px;
            color: var(--rfm-blue);
            margin-bottom: 20px;
            border-bottom: 2px solid var(--rfm-light-blue);
            padding-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        /* РЕАЛЬНЫЕ НОВОСТИ ИЗ СКРИНШОТА */
        .news-item {
            margin-bottom: 20px;
        }

        .news-title {
            font-size: 14px;
            font-weight: 700;
            color: #1a1a1a;
            margin-bottom: 5px;
            cursor: pointer;
        }

        .news-title:hover {
            color: var(--rfm-blue);
        }

        .news-date {
            font-size: 11px;
            color: #888888;
        }

        /* ИНФОРМАЦИОННЫЕ СООБЩЕНИЯ */
        .info-msg-box {
            text-align: center;
            padding: 20px;
            background: #fafafa;
            border: 1px solid #eef2f6;
            border-radius: 6px;
        }

        .info-msg-box h3 {
            font-size: 16px;
            margin-bottom: 15px;
            color: #333;
        }

        .btn-read-more {
            background: white;
            border: 2px solid var(--rfm-blue);
            color: var(--rfm-blue);
            padding: 8px 25px;
            font-weight: bold;
            font-size: 13px;
            text-transform: uppercase;
            cursor: pointer;
            border-radius: 4px;
            transition: all 0.2s;
        }

        .btn-read-more:hover {
            background: var(--rfm-blue);
            color: white;
        }

        /* БЛОК КЛИЕНТОЦЕНТРИЧНОСТИ (84%) */
        .metric-banner {
            background: var(--rfm-blue);
            color: white;
            padding: 25px;
            border-radius: 8px;
            text-align: center;
        }

        .metric-banner .num {
            font-size: 52px;
            font-weight: 900;
            margin: 5px 0;
        }

        /* ЗОНА ПРОВЕРКИ УДОСТОВЕРЕНИЯ (В КОНЦЕ) */
        .verify-zone {
            background: white;
            border-radius: 12px;
            padding: 35px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            border: 1px solid #dcdcdc;
            border-top: 5px solid var(--rfm-dark);
        }

        .verify-title {
            text-align: center;
            margin-bottom: 25px;
        }

        .verify-title h2 {
            font-size: 20px;
            color: var(--rfm-dark);
        }

        .input-group {
            display: flex;
            gap: 15px;
            max-width: 550px;
            margin: 0 auto;
        }

        .input-group input {
            flex: 1;
            padding: 12px 20px;
            border: 2px solid #cbd5e1;
            border-radius: 6px;
            font-size: 15px;
            outline: none;
        }

        .input-group input:focus {
            border-color: var(--rfm-blue);
        }

        .btn-go {
            background: var(--rfm-dark);
            color: white;
            border: none;
            padding: 0 30px;
            border-radius: 6px;
            font-weight: bold;
            cursor: pointer;
        }

        .btn-go:hover {
            background: var(--rfm-blue);
        }

        .error-text {
            color: #ef4444;
            font-weight: bold;
            text-align: center;
            margin-top: 15px;
            display: none;
            font-size: 14px;
        }

        /* ЛИЧНОЕ ПОРТФОЛИО (ТВОЙ ПЕРВЫЙ СКРИПТ) */
        .personal-portfolio {
            margin-top: 35px;
            background-color: var(--portfolio-bg);
            border-radius: 12px;
            padding: 35px;
            color: #f8fafc;
            display: none;
            animation: fadeIn 0.4s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .portfolio-split {
            display: grid;
            grid-template-columns: 280px 1fr;
            gap: 35px;
        }

        /* 3D КАРТОЧКА */
        .card-3d {
            width: 100%;
            height: 360px;
            perspective: 1000px;
        }

        .card-3d-inner {
            position: relative;
            width: 100%;
            height: 100%;
            text-align: center;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }

        .card-3d:hover .card-3d-inner {
            transform: rotateY(180deg);
        }

        .card-front, .card-back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            border-radius: 8px;
            padding: 20px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border: 1px solid rgba(56, 189, 248, 0.2);
        }

        .card-front { background: #1e293b; }
        .card-front img {
            width: 130px;
            height: 160px;
            object-fit: cover;
            border-radius: 6px;
            border: 2px solid var(--neon-blue);
            margin-bottom: 15px;
        }
        .card-back {
            background: #0f172a;
            transform: rotateY(180deg);
        }

        /* СКИЛЛ-БАРЫ */
        .skill-wrapper { margin-top: 15px; }
        .skill-header { display: flex; justify-content: space-between; font-size: 13px; margin-bottom: 5px; }
        .track { background: #334155; height: 6px; border-radius: 3px; overflow: hidden; }
        .fill { background: var(--neon-blue); height: 100%; width: 0%; transition: width 1s; }

        footer {
            background: var(--rfm-dark);
            color: #718096;
            padding: 25px;
            text-align: center;
            font-size: 12px;
            margin-top: 50px;
            border-top: 2px solid var(--accent-gold);
        }
    </style>
</head>
<body>

    <div class="top-navbar">
        <div class="nav-left">🏛️ Росфинмониторинг</div>
        <div class="nav-right">
            <a href="#">Поиск</a>
            <a href="#">Контакты</a>
            <a href="#">Постановка на учет</a>
            <a href="#" style="color: var(--accent-gold);">Личный кабинет</a>
        </div>
    </div>

    <div class="hero-banner">
        <div style="font-size: 28px;">🌐</div>
        <h1>РОСФИНМОНИТОРИНГ</h1>
        <div class="anniversary-sub">25 лет на страже финансовой безопасности</div>
    </div>

    <div class="main-content">

        <div class="info-grid">
            
            <div class="block-card">
                <h2>📊 Последние новости</h2>
                <div class="news-item">
                    <div class="news-title">В Санкт-Петербурге пресечена деятельность группы теневых банкиров с оборотом свыше полумиллиарда рублей</div>
                    <div class="news-date">11.06.2026</div>
                </div>
                <div class="news-item">
                    <div class="news-title">Молодежный совет ведомства провел координационное совещание по антифрод-стратегиям</div>
                    <div class="news-date">08.06.2026</div>
                </div>
            </div>

            <div class="block-card">
                <h2>✉️ Информационные сообщения</h2>
                <div class="info-msg-box">
                    <h3>В Росфинмониторинге состоится очередное заседание Коллегии</h3>
                    <button class="btn-read-more">Читать полностью</button>
                </div>
            </div>

        </div>

        <div class="metric-banner">
            <div style="font-size: 13px; text-transform: uppercase; letter-spacing: 1px;">Итоги года: Индекс клиентоцентричности</div>
            <div class="num">84%</div>
            <div style="font-size: 12px; color: #bfdbfe;">Данные Аналитического центра при Правительстве РФ</div>
        </div>

        <div class="verify-zone">
            <div class="verify-title">
                <h2>Верификация служебных удостоверений сотрудников</h2>
                <p style="font-size: 13px; color: #666; margin-top: 5px;">Введите номер документа для подтверждения статуса и вывода личной карточки аналитика</p>
            </div>

            <div class="input-group">
                <input type="text" id="certId" placeholder="Введите номер (например: ФС-999888)" onkeydown="if(event.key==='Enter') doVerify()">
                <button class="btn-go" onclick="doVerify()">Проверить</button>
            </div>

            <div class="error-text" id="errBox">Ошибка: Удостоверение не найдено в базе данных реестра ИБ.</div>

            <div class="personal-portfolio" id="pfBlock">
                <div class="portfolio-split">
                    
                    <div class="card-3d">
                        <div class="card-3d-inner">
                            <div class="card-front">
                                <img src="avatar.jpg" alt="Фото">
                                <h3 id="pName">ФИО</h3>
                                <div style="color:var(--neon-blue); font-size:13px; font-weight:bold; margin-top:5px;" id="pPost">Должность</div>
                            </div>
                            <div class="card-back">
                                <h4 style="color:var(--neon-blue); margin-bottom:10px;">Реестр контура</h4>
                                <p style="font-size:13px;">🟢 Документ активен</p>
                                <p style="font-size:11px; margin-top:20px; color:#64748b;">Защищено ФСБ РФ</p>
                            </div>
                        </div>
                    </div>

                    <div>
                        <h2 style="color:white; font-size:24px; margin-bottom:15px; border-bottom:1px solid #334155; padding-bottom:5px;" id="pTitle">Минин Максим Викторович</h2>
                        <p style="font-size:14px; color:#cbd5e1; text-align:justify;" id="pBio">Описание...</p>

                        <div style="margin-top:20px;">
                            <h4 style="color:var(--neon-blue); font-size:12px; text-transform:uppercase;">Компетенции:</h4>
                            
                            <div class="skill-wrapper">
                                <div class="skill-header"><span>Оценка рисков и ПОД/ФТ</span><span>95%</span></div>
                                <div class="track"><div class="fill" id="b1"></div></div>
                            </div>
                            <div class="skill-wrapper">
                                <div class="skill-header"><span>Управление проектами (Молодёжный совет)</span><span>90%</span></div>
                                <div class="track"><div class="fill" id="b2"></div></div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>

        </div>

    </div>

    <footer>
        <p>© 2026 Федеральная служба по финансовому мониторингу. Все права защищены.</p>
    </footer>

    <script>
        const db = {
            "ФС-999888": {
                name: "Минин Максим Викторович",
                post: "Председатель Молодёжного совета",
                bio: "Окончил Международный сетевой институт в сфере ПОД/ФТ. Специализируется на экспертной оценке финансовых угроз и создании механизмов защиты граждан от социальной инженерии. Руководит Молодёжным советом ведомства, координируя аналитическую работу молодых специалистов центрального аппарата."
            }
        };

        function doVerify() {
            const val = document.getElementById("certId").value.trim();
            const pf = document.getElementById("pfBlock");
            const err = document.getElementById("errBox");

            if(db.hasOwnProperty(val)) {
                document.getElementById("pName").innerText = db[val].name;
                document.getElementById("pTitle").innerText = db[val].name;
                document.getElementById("pPost").innerText = db[val].post;
                document.getElementById("pBio").innerText = db[val].bio;

                pf.style.display = "block";
                err.style.display = "none";

                setTimeout(() => {
                    document.getElementById("b1").style.width = "95%";
                    document.getElementById("b2").style.width = "90%";
                }, 100);
            } else {
                pf.style.display = "none";
                err.style.display = "block";
            }
        }
    </script>
</body>
</html>
