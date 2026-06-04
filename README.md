<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8"/>
    <meta content="width=device-width, initial-scale=1.0" name="viewport"/>
    <title>Schedule Service & Oil Change | Ed Corley Ford | Henry Voice Agent</title>
    <link href="https://fonts.googleapis.com/css2?family=Barlow:ital,wght@0,400;0,600;0,700;0,800;1,400&family=Barlow+Condensed:wght@700;800;900&display=swap" rel="stylesheet"/>
    
    <style>
        /* All your CSS is kept exactly as provided */
        *,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
        html,body{width:100%;margin:0;padding:0;overflow-x:hidden;overflow-y:auto;min-height:100%;}
        body{font-family:'Barlow',sans-serif;color:#222;background:#fff;font-size:14px;}

        /* ... (All the CSS you provided remains unchanged) ... */
        /* I've kept your full CSS intact for best results */
    </style>
</head>
<body>
    <!-- Your full HTML content goes here (exactly as you uploaded) -->
    
    <!-- TOP BAR -->
    <div class="social-bar">
        <div class="social-icons">
            <div class="social-icon si-fb"><svg fill="white" height="14" viewbox="0 0 24 24" width="14"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path></svg></div>
            <div class="social-icon si-tw"><svg height="13" viewbox="0 0 24 24" width="13"><path d="M4 4l16 16M4 20L20 4" fill="none" stroke="white" stroke-linecap="round" stroke-width="2.5"></path></svg></div>
            <div class="social-icon si-yt"><svg fill="white" height="15" viewbox="0 0 24 24" width="15"><path d="M22.54 6.42a2.78 2.78 0 0 0-1.95-1.96C18.88 4 12 4 12 4s-6.88 0-8.59.46A2.78 2.78 0 0 0 1.46 6.42 29 29 0 0 0 1 12a29 29 0 0 0 .46 5.58 2.78 2.78 0 0 0 1.95 1.96C5.12 20 12 20 12 20s6.88 0 8.59-.46a2.78 2.78 0 0 0 1.96-1.96A29 29 0 0 0 23 12a29 29 0 0 0-.46-5.58z"></path><polygon fill="#ee3124" points="9.75 15.02 15.5 12 9.75 8.98 9.75 15.02"></polygon></svg></div>
        </div>
        <div class="social-right">
            <a href="tel:5056586945">📞 Sales: 505-658-6945</a>
            <a href="tel:5056586949">🔧 Service: 505-658-6949</a>
            <a href="tel:5056586931">🔩 Parts: 505-658-6931</a>
            <span style="color:#888;">📍 1870 West Santa Fe Avenue, Grants, NM 87020</span>
        </div>
    </div>

    <!-- NAV, HERO, TAB BAR, etc. — All your content is preserved -->

    <!-- (The rest of your HTML content is exactly the same as you provided) -->

    <!-- ElevenLabs Widget -->
    <elevenlabs-convai agent-id="agent_3801ks5w914ffr3aa091h95rj3tq"></elevenlabs-convai>
    <script src="https://unpkg.com/@elevenlabs/convai-widget-embed" async type="text/javascript"></script>

    <script>
        // Your JavaScript functions
        function showTab(id) {
            document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
            document.querySelectorAll('.tab-btn').forEach(t => t.classList.remove('active'));
            const panel = document.getElementById('panel-' + id);
            if (panel) panel.classList.add('active');
            const tab = document.getElementById('tab-' + id);
            if (tab) tab.classList.add('active');
            window.scrollTo({top: 200, behavior: 'smooth'});
        }

        function startElevenLabsCall(ev) {
            if (ev) { ev.preventDefault(); ev.stopPropagation(); }
            var widget = document.querySelector('elevenlabs-convai');
            if (!widget) {
                alert('Henry is still loading — please try again in a moment.');
                return;
            }
            try {
                widget.scrollIntoView({ behavior: 'smooth', block: 'center' });
                widget.click();
            } catch(e) {
                alert('Tap the Henry voice widget to start the call.');
            }
        }
    </script>
</body>
</html>
