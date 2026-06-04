<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Schedule Service & Oil Change | Ed Corley Ford</title>
    <link href="https://fonts.googleapis.com/css2?family=Barlow:wght@400;600;700;800&family=Barlow+Condensed:wght@700;800;900&display=swap" rel="stylesheet">
    
    <style>
        *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
        body { font-family: 'Barlow', sans-serif; color: #222; background: #fff; font-size: 14px; line-height: 1.5; }
        
        .social-bar { background: #111; padding: 8px 20px; display: flex; align-items: center; justify-content: space-between; position: relative; }
        .social-icons { position: absolute; left: 50%; transform: translateX(-50%); display: flex; gap: 8px; }
        .social-icon { width: 28px; height: 28px; border-radius: 4px; display: flex; align-items: center; justify-content: center; color: white; font-size: 14px; }
        
        nav { background: #fff; border-bottom: 3px solid #c8102e; position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 6px rgba(0,0,0,0.1); }
        .nav-inner { max-width: 1400px; margin: 0 auto; padding: 0 20px; display: flex; align-items: center; height: 78px; }
        .nav-logo { display: flex; align-items: center; gap: 10px; text-decoration: none; }
        .nav-links { display: flex; list-style: none; gap: 10px; margin-left: auto; }
        .nav-links a { padding: 10px 14px; font-weight: 600; color: #222; text-decoration: none; border-radius: 6px; }
        .nav-links a:hover { background: #f0f4ff; color: #003478; }
        
        .service-hero { background: linear-gradient(135deg, #003478, #001f4d); color: white; text-align: center; padding: 50px 20px; }
        .service-hero h1 { font-family: 'Barlow Condensed', sans-serif; font-size: 36px; margin-bottom: 10px; }
        
        .tab-bar { background: #fff; border-bottom: 2px solid #ddd; display: flex; justify-content: center; gap: 10px; padding: 12px; }
        .tab-btn { padding: 12px 24px; font-weight: 700; border: 2px solid #ddd; border-radius: 50px; cursor: pointer; }
        .tab-btn.active { border-color: #c8102e; background: #fff8f8; color: #c8102e; }
        
        .tab-panel { display: none; max-width: 1200px; margin: 0 auto; padding: 40px 20px; }
        .tab-panel.active { display: block; }
        
        .henry-voice-button {
            background: #c8102e; color: white; border: none; padding: 16px 32px; 
            border-radius: 50px; font-size: 17px; font-weight: 900; cursor: pointer;
            text-transform: uppercase; margin: 20px 0;
        }
        .henry-voice-button:hover { background: #a00d25; transform: scale(1.05); }
        
        footer { background: #111; color: #aaa; text-align: center; padding: 30px; font-size: 12px; }
    </style>
</head>
<body>

    <!-- TOP BAR -->
    <div class="social-bar">
        <div class="social-icons">
            <div class="social-icon" style="background:#1877f2;">f</div>
            <div class="social-icon" style="background:#000;">𝕏</div>
            <div class="social-icon" style="background:#ee3124;">▶</div>
        </div>
        <div style="color:#bbb; font-size:12px; margin-left:auto; display:flex; gap:15px;">
            <a href="tel:5056586945" style="color:#bbb;">📞 Sales: 505-658-6945</a>
            <a href="tel:5056586949" style="color:#bbb;">🔧 Service: 505-658-6949</a>
        </div>
    </div>

    <!-- NAV -->
    <nav>
        <div class="nav-inner">
            <a class="nav-logo" href="#">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3e/Ford_Logo_2023.svg/512px-Ford_Logo_2023.svg.png" height="52" alt="Ford">
                <img src="https://via.placeholder.com/280x70/003478/ffffff?text=ED+CORLEY+FORD" height="64" alt="Ed Corley Ford">
            </a>
            
            <ul class="nav-links">
                <li><a href="javascript:void(0)" onclick="showTab('schedule')">📅 Schedule Service</a></li>
                <li><a href="javascript:void(0)" onclick="showTab('oilchange')">🛢️ Oil Change</a></li>
            </ul>
        </div>
    </nav>

    <!-- HERO -->
    <div class="service-hero">
        <h1>Ed Corley Ford Service Center</h1>
        <p>Factory-trained technicians • Genuine Ford Parts • Grants, NM</p>
        <button onclick="startElevenLabsCall(event)" class="henry-voice-button">
            🎙️ Click Here to Speak to Henry Live 24/7
        </button>
    </div>

    <!-- TAB BAR -->
    <div class="tab-bar">
        <button class="tab-btn active" id="tab-schedule" onclick="showTab('schedule')">📅 Schedule Service</button>
        <button class="tab-btn" id="tab-oilchange" onclick="showTab('oilchange')">🛢️ Oil Change</button>
    </div>

    <!-- SCHEDULE PANEL -->
    <div class="tab-panel active" id="panel-schedule">
        <h2 style="text-align:center; margin:30px 0;">Schedule Your Service</h2>
        <button onclick="startElevenLabsCall(event)" class="henry-voice-button" style="display:block; margin:0 auto;">
            🎙️ Talk to Henry - Fastest Booking
        </button>
    </div>

    <!-- OIL CHANGE PANEL -->
    <div class="tab-panel" id="panel-oilchange">
        <h2 style="text-align:center; margin:30px 0;">Oil Change Services</h2>
        <p style="text-align:center;">Coming soon with pricing and options...</p>
    </div>

    <!-- FOOTER -->
    <footer>
        <p>© 2026 Ed Corley Ford Sales Inc.</p>
        <p>1870 West Santa Fe Avenue, Grants, NM 87020</p>
        <p>Service: (505) 658-6949</p>
    </footer>

    <!-- Henry Voice Widget -->
    <elevenlabs-convai agent-id="agent_3801ks5w914ffr3aa091h95rj3tq"></elevenlabs-convai>
    <script src="https://unpkg.com/@elevenlabs/convai-widget-embed" async></script>

    <script>
        function showTab(id) {
            document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
            document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
            document.getElementById('panel-' + id).classList.add('active');
            document.getElementById('tab-' + id).classList.add('active');
        }

        function startElevenLabsCall(e) {
            if (e) e.preventDefault();
            const widget = document.querySelector('elevenlabs-convai');
            if (widget) {
                widget.scrollIntoView({ behavior: "smooth" });
                setTimeout(() => widget.click(), 500);
            } else {
                alert("Henry is loading. Please wait a moment.");
            }
        }
    </script>
</body>
</html>
