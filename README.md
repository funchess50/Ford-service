<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Schedule Service & Oil Change | Ed Corley Ford | Henry Voice Agent</title>
    <link href="https://fonts.googleapis.com/css2?family=Barlow:ital,wght@0,400;0,600;0,700;0,800;1,400&family=Barlow+Condensed:wght@700;800;900&display=swap" rel="stylesheet">
    
    <style>
        *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
        html, body { width: 100%; margin: 0; padding: 0; overflow-x: hidden; min-height: 100%; }
        body { font-family: 'Barlow', sans-serif; color: #222; background: #fff; font-size: 14px; line-height: 1.5; }

        /* TOP BAR */
        .social-bar {
            background: #111; padding: 7px 20px; display: flex; align-items: center; 
            justify-content: space-between; gap: 12px; position: relative;
        }
        .social-icons { display: flex; gap: 6px; position: absolute; left: 50%; transform: translateX(-50%); }
        .social-icon {
            width: 28px; height: 28px; border-radius: 4px; display: flex; 
            align-items: center; justify-content: center; cursor: pointer;
        }
        .si-fb { background: #1877f2; }
        .si-tw { background: #000; }
        .si-yt { background: #ee3124; }
        .social-right {
            display: flex; gap: 18px; align-items: center; font-size: 11px; 
            color: #bbb; margin-left: auto;
        }
        .social-right a { color: #bbb; text-decoration: none; white-space: nowrap; }

        /* NAV */
        nav {
            background: #fff; border-bottom: 3px solid #c8102e; 
            box-shadow: 0 2px 6px rgba(0,0,0,0.1); position: sticky; top: 0; z-index: 200;
        }
        .nav-inner {
            max-width: 1400px; margin: 0 auto; padding: 0 20px; 
            display: flex; align-items: center; height: 78px;
        }
        .nav-logo { display: flex; align-items: center; gap: 8px; text-decoration: none; margin-right: 28px; }
        .nav-links {
            display: flex; list-style: none; align-items: center; flex: 1; gap: 8px;
        }
        .nav-links li a {
            padding: 8px 13px; font-size: 13px; font-weight: 600; color: #222; 
            text-decoration: none; white-space: nowrap; transition: color .15s;
        }
        .nav-links li a:hover { color: #003478; }
        .nav-right { display: flex; gap: 16px; align-items: center; margin-left: auto; }

        /* HERO */
        .service-hero {
            background: linear-gradient(135deg, #003478 0%, #001f4d 100%);
            padding: 40px 24px; text-align: center; color: #fff;
        }
        .service-hero h1 {
            font-size: 34px; font-weight: 900; font-family: 'Barlow Condensed', sans-serif;
            letter-spacing: 1px; margin-bottom: 8px;
        }

        /* TAB BAR */
        .tab-bar {
            background: #fff; border-bottom: 2px solid #e0e0e0; padding: 10px 16px;
            display: flex; overflow-x: auto; gap: 12px; justify-content: center;
        }
        .tab-btn {
            padding: 12px 24px; font-size: 13px; font-weight: 700; background: #fff;
            border: 2px solid #e6e6e6; border-radius: 999px; cursor: pointer;
            white-space: nowrap; transition: all .15s;
        }
        .tab-btn.active {
            background: #fff8f8; border-color: #c8102e; color: #c8102e;
        }

        /* CONTENT */
        .tab-panel { display: none; max-width: 1200px; margin: 0 auto; padding: 36px 24px 60px; }
        .tab-panel.active { display: block; }

        .section-header {
            display: flex; align-items: center; gap: 16px; margin-bottom: 28px;
            padding-bottom: 16px; border-bottom: 2px solid #003478;
        }
        .section-title { font-size: 26px; font-weight: 800; color: #003478; }

        /* CARDS */
        .cards-grid {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 20px;
        }
        .card {
            background: #fff; border: 1px solid #e0e0e0; border-radius: 8px;
            padding: 20px; box-shadow: 0 2px 8px rgba(0,0,0,0.05);
        }
        .card-price { font-size: 26px; font-weight: 800; color: #003478; }

        /* HENRY WIDGET */
        .henry-voice-button {
            background: #c8102e; color: #fff; border: none; padding: 16px 28px;
            border-radius: 999px; font-size: 16px; font-weight: 900; cursor: pointer;
            text-transform: uppercase; letter-spacing: 0.5px;
        }
        .henry-voice-button:hover { background: #a00d25; transform: scale(1.03); }

        footer {
            background: #111; color: #999; font-size: 11px; padding: 30px 20px; text-align: center;
        }

        @media (max-width: 900px) {
            .cards-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <!-- TOP BAR -->
    <div class="social-bar">
        <div class="social-icons">
            <div class="social-icon si-fb">FB</div>
            <div class="social-icon si-tw">X</div>
            <div class="social-icon si-yt">YT</div>
        </div>
        <div class="social-right">
            <a href="tel:5056586945">📞 Sales: 505-658-6945</a>
            <a href="tel:5056586949">🔧 Service: 505-658-6949</a>
            <a href="tel:5056586931">🔩 Parts: 505-658-6931</a>
            <span>📍 1870 West Santa Fe Avenue, Grants, NM 87020</span>
        </div>
    </div>

    <!-- NAV -->
    <nav>
        <div class="nav-inner">
            <a class="nav-logo" href="index.html">
                <img alt="Ford" src="data:image/png;base64,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
