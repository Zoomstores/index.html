<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zoom Store | زوم ستور للشحن الفوري</title>
    <style>
        :root {
            --primary: #f39c12; /* اللون البرتقالي الجذاب */
            --bg: #0b0d0f;
            --card: #161b22;
            --text: #ffffff;
            --whatsapp: #25d366;
        }

        body {
            background-color: var(--bg);
            color: var(--text);
            font-family: 'Segoe UI', Tahoma, sans-serif;
            margin: 0; padding: 0;
        }

        /* تنسيق الهيدر والشعار الجديد */
        header {
            background: linear-gradient(to bottom, #1c2128, #0b0d0f);
            padding: 25px 15px;
            text-align: center;
            border-bottom: 3px solid var(--primary);
        }

        .logo-area {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 5px;
        }

        .logo-icon {
            font-size: 40px;
            background: var(--primary);
            color: black;
            width: 60px;
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            box-shadow: 0 0 15px var(--primary);
            margin-bottom: 10px;
        }

        .store-name {
            font-size: 28px;
            font-weight: 900;
            letter-spacing: 1px;
            color: var(--text);
            text-transform: uppercase;
        }

        .store-name span { color: var(--primary); }

        /* التنقل */
        .tabs-nav {
            display: flex;
            overflow-x: auto;
            background: #1c2128;
            padding: 10px;
            position: sticky;
            top: 0; z-index: 1000;
            border-bottom: 1px solid #30363d;
        }

        .tab-link {
            flex: 0 0 auto;
            padding: 10px 18px;
            margin-left: 8px;
            background: #0d1117;
            border-radius: 12px;
            cursor: pointer;
            font-weight: bold;
            font-size: 13px;
            color: #8b949e;
            border: 1px solid transparent;
        }

        .tab-link.active {
            background: rgba(243, 156, 18, 0.1);
            color: var(--primary);
            border: 1px solid var(--primary);
        }

        .container { padding: 15px; max-width: 500px; margin: auto; }

        .game-section { display: none; }
        .game-section.active { display: block; animation: fadeIn 0.4s; }

        .game-banner {
            width: 100%;
            height: 160px;
            border-radius: 15px;
            object-fit: cover;
            margin-bottom: 20px;
            border: 1px solid #30363d;
        }

        .section-title {
            color: var(--primary);
            border-right: 4px solid var(--primary);
            padding-right: 10px;
            margin: 15px 0;
            font-size: 18px;
        }

        .price-card {
            background: var(--card);
            border-radius: 12px;
            margin-bottom: 8px;
            padding: 12px 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border: 1px solid #30363d;
        }

        .btn-buy {
            background: var(--whatsapp);
            color: white;
            text-decoration: none;
            padding: 8px 14px;
            border-radius: 8px;
            font-size: 12px;
            font-weight: bold;
        }

        footer { text-align: center; padding: 30px; color: #484f58; font-size: 12px; background: #080a0c; }

        @keyframes fadeIn { from {opacity: 0; transform: translateY(10px);} to {opacity: 1; transform: translateY(0);} }
    </style>
</head>
<body>

<header>
    <div class="logo-area">
        <div class="logo-icon">⚡</div>
        <div class="store-name">ZOOM <span>STORE</span></div>
        <p style="font-size:12px; color:#8b949e; margin: 5px 0 0 0;">سرعة البرق في الشحن ⚡</p>
    </div>
</header>

<div class="tabs-nav">
    <div class="tab-link active" onclick="openGame(event, 'pubg')">ببجي (UC)</div>
    <div class="tab-link" onclick="openGame(event, 'freefire')">فري فاير</div>
    <div class="tab-link" onclick="openGame(event, 'pes')">بيس (eFootball)</div>
    <div class="tab-link" onclick="openGame(event, 'fifa')">فيفا (FC)</div>
</div>

<div class="container">
    
    <div id="pubg" class="game-section active">
        <img src="https://images.lucasfox.com/news/files/2021/01/PUBG-banner.jpg" class="game-banner">
        <h3 class="section-title">شدات ببجي موبايل</h3>
        <div class="price-card">
            <div style="display:flex; flex-direction:column;">
                <span style="font-weight:bold;">60 شدة</span>
                <span style="color:var(--primary); font-size:13px;">4,000 ج</span>
            </div>
            <a href="https://wa.me/249117893591?text=طلب+ببجي+60+من+زوم+ستور" class="btn-buy">اطلب الآن</a>
        </div>
        </div>

    <div id="freefire" class="game-section">
        <img src="https://wallpapers.com/images/featured/free-fire-pc-7p7p4p7p7p7p7p7p.jpg" class="game-banner">
        <h3 class="section-title">جواهر فري فاير</h3>
        <div class="price-card">
            <div style="display:flex; flex-direction:column;">
                <span style="font-weight:bold;">110 جوهرة</span>
                <span style="color:var(--primary); font-size:13px;">4,000 ج</span>
            </div>
            <a href="https://wa.me/249117893591?text=طلب+فف+110+من+زوم+ستور" class="btn-buy">اطلب الآن</a>
        </div>
    </div>

    </div>

<footer>
    <p>طرق الدفع: بنكك | فوري | ماي كاشي</p>
    <p>واتساب زوم ستور: 0117893591</p>
    <p>© 2026 Zoom Store - جميع الحقوق محفوظة</p>
</footer>

<script>
    function openGame(evt, gameName) {
        var i, content, links;
        content = document.getElementsByClassName("game-section");
        for (i = 0; i < content.length; i++) { content[i].style.display = "none"; content[i].classList.remove("active"); }
        links = document.getElementsByClassName("tab-link");
        for (i = 0; i < links.length; i++) { links[i].classList.remove("active"); }
        document.getElementById(gameName).style.display = "block";
        document.getElementById(gameName).classList.add("active");
        evt.currentTarget.classList.add("active");
    }
</script>

</body>
</html>
