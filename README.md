<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Официальный портал | Аналитический модуль Минин Максим Викторович</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        /* ОФИЦИАЛЬНАЯ ПАЛИТРА РОСФИНМОНИТОРИНГА */
        :root {
            --rfm-blue: #00549c; /* Тот самый синий из шапки */
            --rfm-light-blue: #f0f7ff;
            --rfm-gray: #f5f5f5;
            --text-dark: #333333;
        }

        body {
            background-color: #ffffff;
            color: var(--text-dark);
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
        }

        /* Верхняя тонкая полоска с гербом */
        .top-line {
            background: #003a6d;
            height: 5px;
            width: 100%;
        }

        header {
            background: linear-gradient(to right, #00549c, #0078d7);
            color: white;
            padding: 40px 20px;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        header h1 {
            margin: 0;
            font-size: 2rem;
            letter-spacing: 1px;
            text-transform: uppercase;
            font-weight: 700;
        }

        .header-desc {
            font-size: 1rem;
            margin-top: 10px;
            opacity: 0.9;
            font-weight: 300;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
            display: grid;
            grid-template-columns: 350px 1fr;
            gap: 40px;
        }

        /* ЛЕВАЯ КОЛОНКА (Профиль) */
        .sidebar {
            background: white;
        }

        .photo-box {
            width: 100%;
            border: 1px solid #ddd;
            padding: 5px;
            background: white;
            box-shadow: 0 2px 15px rgba(0,0,0,0.05);
        }

        .photo-box img {
            width: 100%;
            display: block;
        }

        .status-badge {
            background: var(--rfm-light-blue);
            border-left: 4px solid var(--rfm-blue);
            padding: 15px;
            margin-top: 20px;
            font-size: 0.9rem;
            color: var(--rfm-blue);
            font-weight: 500;
        }

        /* ПРАВАЯ КОЛОНКА (Информационные блоки) */
        .main-content h2 {
            color: var(--rfm-blue);
            border-bottom: 2px solid var(--rfm-blue);
            padding-bottom: 10px;
            margin-bottom: 25px;
            font-size: 1.5rem;
            text-transform: uppercase;
        }

        .news-card {
            background: #ffffff;
            border: 1px solid #e0e0e0;
            padding: 25px;
            margin-bottom: 25px;
            transition: 0.3s;
        }

        .news-card:hover {
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
            border-color: var(--rfm-blue);
        }

        .news-card h3 {
            color: var(--rfm-blue);
            margin-top: 0;
            font-size: 1.2rem;
        }

        .tag {
            display: inline-block;
            background: var(--rfm-blue);
            color: white;
            padding: 3px 10px;
            font-size: 0.7rem;
            border-radius: 3px;
            margin-bottom: 10px;
            text-transform: uppercase;
        }

        .info-list {
            padding-left: 20px;
        }

        .info-list li {
            margin-bottom: 12px;
        }

        .info-list li b {
            color: var(--rfm-blue);
        }

        /* Футер как на сайте */
        footer {
            background: #f9f9f9;
            border-top: 1px solid #ddd;
            padding: 50px 20px;
            text-align: center;
            font-size: 0.9rem;
            color: #666;
        }

        .official-stamp {
            margin-top: 20px;
            font-weight: 700;
            color: #ccc;
            letter-spacing: 5px;
        }

        /* Кнопка "Интернет-приемная" */
        .btn-official {
            display: inline-block;
            background: var(--rfm-blue);
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            font-weight: 500;
            margin-top: 20px;
            border-radius: 2px;
        }

        @media (max-width: 850px) {
            .container { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <div class="top-line"></div>

    <header>
        <h1>Росфинмониторинг</h1>
        <div class="header-desc">Специализированный аналитический модуль экспертного совета</div>
    </header>

    <div class="container">
        
        <div class="sidebar">
            <div class="photo-box">
                <img src="me.jpg" alt="Эксперт аналитического модуля">
            </div>
            <div class="status-badge">
                ID: 2026-CH-07<br>
                СТАТУС: ДЕЙСТВУЮЩИЙ ЭКСПЕРТ<br>
                ДОСТУП: ВЫСШИЙ (УРОВЕНЬ 1)
            </div>
            
            <a href="#" class="btn-official">ИНТЕРНЕТ-ПРИЕМНАЯ</a>
        </div>

        <div class="main-content">
            <h2>Последние новости и аналитика</h2>

            <div class="news-card">
                <span class="tag">ПРОТИВОДЕЙСТВИЕ</span>
                <h3>Новые векторы финансовой безопасности</h3>
                <p>В интервью федеральным СМИ обсуждены механизмы борьбы с трансграничным мошенничеством. Основной упор сделан на внедрение <b>предиктивной аналитики</b> и межведомственную консолидацию данных банковского сектора.</p>
            </div>

            <div class="news-card">
                <span class="tag">ВЭД И КИТАЙ</span>
                <h3>Комплаенс-устойчивость импорта из КНР</h3>
                <p>Разработка и внедрение стандартов прозрачности для бизнеса, работающего с партнерами из КНР. Включает в себя:</p>
                <ul class="info-list">
                    <li><b>Аудит контрагентов:</b> Глубокая проверка поставщиков (Due Diligence).</li>
                    <li><b>Валютный контроль:</b> Сопровождение сделок на предмет соответствия 115-ФЗ.</li>
                    <li><b>Логистические риски:</b> Оптимизация маршрутов под требования регуляторов.</li>
                </ul>
            </div>

            <div class="news-card">
                <span class="tag">ЦИФРОВИЗАЦИЯ</span>
                <h3>Мониторинг 2.0: Интерфейсы будущего</h3>
                <p>Создание единой цифровой консоли для специалистов SRE и мониторинга. Визуализация данных позволяет выявлять аномалии в финансовых потоках в режиме реального времени.</p>
            </div>
        </div>

    <div class="news-block">
                <span class="tag">Социально-правовая защита</span>
                <h2>Защита интересов и прав граждан РФ</h2>
                <p>Одним из приоритетных направлений работы аналитического модуля является обеспечение <b>финансовой безопасности населения</b> и противодействие вовлечению граждан в противоправные схемы.</p>
                
                <ul style="padding-left: 20px; font-size: 14px; line-height: 1.8;">
                    <li><b>Профилактика кибермошенничества:</b> Консультационная поддержка по вопросам защиты персональных данных и предотвращения несанкционированного доступа к банковским счетам.</li>
                    <li><b>Реабилитация добросовестных участников:</b> Помощь в механизмах исключения из «черных списков» (согласно 115-ФЗ) при условии подтверждения законности операций.</li>
                    <li><b>Антифрод-мониторинг:</b> Разработка алгоритмов блокировки подозрительных переводов в пользу сомнительных платформ и финансовых пирамид.</li>
                </ul>
                
                <div style="background: #fff8e1; border: 1px solid #ffe082; padding: 15px; border-radius: 4px; margin-top: 15px; font-size: 13px;">
                    <b>Вниманию граждан:</b> Служба мониторинга напоминает, что передача своих банковских карт третьим лицам («дропперство») является нарушением законодательства и ведет к блокировке всех финансовых инструментов.
                </div>
            </div></div>

    <footer>
        <p>© 2026 Федеральная служба по финансовому мониторингу (неофициальный аналитический прототип)</p>
        <p>Москва, ул. Кирова, д. 80. Все права защищены законом.</p>
        <div class="official-stamp">РОСФИНМОНИТОРИНГ</div>
    </footer>

</body>
</html>
