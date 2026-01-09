<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MortonovskyDEV | GitHub</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
            color: #e6edf3;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .card {
            background: rgba(22, 27, 34, 0.9);
            backdrop-filter: blur(10px);
            border: 1px solid #30363d;
            border-radius: 24px;
            max-width: 800px;
            width: 100%;
            overflow: hidden;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
        }

        .card-header {
            padding: 40px 40px 30px;
            border-bottom: 1px solid #30363d;
            position: relative;
        }

        .card-header::after {
            content: '';
            position: absolute;
            bottom: -1px;
            left: 0;
            width: 100%;
            height: 1px;
            background: linear-gradient(90deg, #ff7b72, #58a6ff, #f0883e, #7ee787);
        }

        .profile {
            display: flex;
            align-items: center;
            gap: 25px;
            flex-wrap: wrap;
        }

        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid #30363d;
            background: linear-gradient(45deg, #238636, #2ea043);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 48px;
            font-weight: 700;
            color: #fff;
            flex-shrink: 0;
        }

        .info h1 {
            font-size: 42px;
            font-weight: 700;
            margin-bottom: 8px;
            background: linear-gradient(90deg, #ff7b72, #58a6ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .info .tagline {
            font-size: 20px;
            color: #8b949e;
            margin-bottom: 15px;
            font-weight: 300;
        }

        .badge {
            display: inline-block;
            background: rgba(88, 166, 255, 0.15);
            color: #58a6ff;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            font-family: 'JetBrains Mono', monospace;
            border: 1px solid rgba(88, 166, 255, 0.3);
        }

        .card-body {
            padding: 40px;
        }

        .section-title {
            font-size: 20px;
            font-weight: 600;
            margin-bottom: 25px;
            color: #f0f6fc;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title::before {
            content: '⟩';
            color: #f0883e;
            font-family: 'JetBrains Mono', monospace;
            font-weight: 700;
        }

        .languages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            gap: 16px;
            margin-bottom: 40px;
        }

        .language {
            background: rgba(48, 54, 61, 0.5);
            border: 1px solid #30363d;
            border-radius: 12px;
            padding: 20px;
            transition: all 0.3s ease;
        }

        .language:hover {
            transform: translateY(-5px);
            border-color: #58a6ff;
            background: rgba(88, 166, 255, 0.05);
        }

        .language-icon {
            font-size: 32px;
            margin-bottom: 12px;
            display: block;
        }

        .language-name {
            font-weight: 600;
            margin-bottom: 5px;
            color: #f0f6fc;
        }

        .language-level {
            font-size: 13px;
            color: #8b949e;
            font-family: 'JetBrains Mono', monospace;
        }

        .stats {
            display: flex;
            gap: 30px;
            flex-wrap: wrap;
            margin-bottom: 40px;
        }

        .stat-item {
            text-align: center;
        }

        .stat-value {
            font-size: 36px;
            font-weight: 700;
            background: linear-gradient(90deg, #7ee787, #f0883e);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            line-height: 1;
        }

        .stat-label {
            font-size: 14px;
            color: #8b949e;
            margin-top: 5px;
        }

        .links {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .link-button {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            padding: 12px 24px;
            border-radius: 12px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            font-size: 16px;
            border: 1px solid #30363d;
            color: #f0f6fc;
            background: rgba(48, 54, 61, 0.5);
        }

        .link-button.primary {
            background: linear-gradient(90deg, #238636, #2ea043);
            border-color: #2ea043;
            color: #fff;
        }

        .link-button:hover {
            transform: translateY(-3px);
            border-color: #58a6ff;
        }

        .link-button.primary:hover {
            background: linear-gradient(90deg, #2ea043, #3fb950);
        }

        footer {
            padding: 25px 40px;
            border-top: 1px solid #30363d;
            text-align: center;
            color: #8b949e;
            font-size: 14px;
        }

        .glow {
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(88, 166, 255, 0.1) 0%, transparent 70%);
            pointer-events: none;
            z-index: -1;
        }

        @media (max-width: 768px) {
            .profile {
                flex-direction: column;
                text-align: center;
                gap: 20px;
            }
            .info h1 {
                font-size: 36px;
            }
            .card-header, .card-body {
                padding: 30px 25px;
            }
            .languages-grid {
                grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
            }
        }
    </style>
</head>
<body>
    <div class="glow" style="top: 10%; left: 10%;"></div>
    <div class="glow" style="bottom: 10%; right: 10%; background: radial-gradient(circle, rgba(126, 231, 135, 0.1) 0%, transparent 70%);"></div>

    <div class="card">
        <div class="card-header">
            <div class="profile">
                <div class="avatar">M</div>
                <div class="info">
                    <h1>MortonovskyDEV</h1>
                    <div class="tagline">Разработчик • Создаю цифровые решения</div>
                    <span class="badge">2 года опыта в разработке</span>
                </div>
            </div>
        </div>

        <div class="card-body">
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-value">2+</div>
                    <div class="stat-label">Года опыта</div>
                </div>
                <div class="stat-item">
                    <div class="stat-value">5</div>
                    <div class="stat-label">Языков</div>
                </div>
                <div class="stat-item">
                    <div class="stat-value">∞</div>
                    <div class="stat-label">Проектов</div>
                </div>
            </div>

            <div class="section-title">Технологический стек</div>
            <div class="languages-grid">
                <div class="language">
                    <span class="language-icon">🟨</span>
                    <div class="language-name">JavaScript</div>
                    <div class="language-level">Frontend & Backend</div>
                </div>
                <div class="language">
                    <span class="language-icon">🟧</span>
                    <div class="language-name">HTML & CSS</div>
                    <div class="language-level">Верстка & Стили</div>
                </div>
                <div class="language">
                    <span class="language-icon">🟦</span>
                    <div class="language-name">C++</div>
                    <div class="language-level">Системное ПО</div>
                </div>
                <div class="language">
                    <span class="language-icon">🟩</span>
                    <div class="language-name">Python</div>
                    <div class="language-level">Скрипты & AI/ML</div>
                </div>
            </div>

            <div class="links">
                <a href="https://github.com/MortonovskyDEV" class="link-button primary" target="_blank">
                    <svg width="20" height="20" fill="currentColor" viewBox="0 0 24 24">
                        <path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"/>
                    </svg>
                    GitHub Профиль
                </a>
                <a href="https://github.com/MortonovskyDEV?tab=repositories" class="link-button" target="_blank">
                    📁 Репозитории
                </a>
            </div>
        </div>

        <footer>
            © 2023 MortonovskyDEV. Код — это поэзия. Каждая строка имеет значение.
        </footer>
    </div>
</body>
</html>
