<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes" />
    <title>🛡️ Shamshir Ali – Report Violating Channel</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Inter:wght@300;400;600;700;800&display=swap');

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Inter', 'Segoe UI', sans-serif;
            background: #0a0a0f;
            color: #e0e0e0;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 16px;
            background-image: radial-gradient(ellipse at 10% 20%, rgba(0, 255, 65, 0.02) 0%, transparent 50%),
                              radial-gradient(ellipse at 90% 80%, rgba(0, 150, 255, 0.02) 0%, transparent 50%);
        }

        .container {
            max-width: 820px;
            width: 100%;
            background: rgba(16, 16, 24, 0.88);
            backdrop-filter: blur(14px);
            border-radius: 36px;
            padding: 44px 38px;
            border: 1px solid rgba(0, 255, 100, 0.12);
            box-shadow: 0 30px 70px rgba(0, 0, 0, 0.85), 0 0 0 1px rgba(0, 255, 100, 0.05) inset;
        }

        .header { text-align: center; margin-bottom: 28px; }
        .badge {
            display: inline-block;
            background: rgba(0, 255, 100, 0.08);
            border: 1px solid rgba(0, 255, 100, 0.2);
            border-radius: 100px;
            padding: 6px 22px;
            font-size: 11px;
            letter-spacing: 2.5px;
            color: #00ff64;
            text-transform: uppercase;
            font-weight: 700;
            margin-bottom: 12px;
        }
        .title {
            font-family: 'Orbitron', monospace;
            font-size: 38px;
            font-weight: 700;
            background: linear-gradient(135deg, #00ff64, #00b4d8, #00ff64);
            background-size: 200% 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shimmer 4s ease-in-out infinite;
            letter-spacing: 1px;
        }
        @keyframes shimmer {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .sub { color: #8892b0; font-size: 15px; margin-top: 8px; font-weight: 300; letter-spacing: 0.3px; }
        .glow-line { width: 70px; height: 2px; background: linear-gradient(90deg, transparent, #00ff64, transparent); margin: 18px auto; border-radius: 2px; opacity: 0.35; }

        .info-box {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 16px;
            padding: 16px 20px;
            margin-bottom: 14px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 14px;
            text-align: left;
        }
        .info-box strong { color: #00ff64; }
        .info-box .label { color: #8892b0; }

        .to-box {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 16px;
            padding: 14px 20px;
            margin-bottom: 14px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 13.5px;
            color: #8892b0;
            text-align: center;
        }
        .to-box .addr {
            color: #58a6ff;
            font-weight: 600;
            direction: ltr;
            display: inline-block;
            margin: 0 4px;
        }

        .id-box {
            background: rgba(0, 255, 100, 0.04);
            border-radius: 12px;
            padding: 10px 18px;
            border: 1px solid rgba(0, 255, 100, 0.15);
            font-size: 14px;
            text-align: center;
            margin-bottom: 14px;
            color: #00ff64;
        }
        .id-box strong { color: #fff; }

        .email-selector {
            margin: 15px 0;
            padding: 12px;
            background: rgba(255,255,255,0.03);
            border-radius: 12px;
            border: 1px solid rgba(255,255,255,0.06);
            max-height: 200px;
            overflow-y: auto;
        }
        .email-selector::-webkit-scrollbar { width: 4px; }
        .email-selector::-webkit-scrollbar-track { background: rgba(255,255,255,0.02); border-radius: 10px; }
        .email-selector::-webkit-scrollbar-thumb { background: #00ff64; border-radius: 10px; }

        .email-selector label {
            display: block;
            padding: 6px 10px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 12px;
            color: #8892b0;
            transition: 0.2s;
            border-left: 2px solid transparent;
        }
        .email-selector label:hover { background: rgba(0,255,100,0.05); color: #e0e0e0; }
        .email-selector label.selected {
            background: rgba(0,255,100,0.08);
            color: #00ff64;
            border-left-color: #00ff64;
        }
        .email-selector input[type="radio"] {
            margin-left: 10px;
            accent-color: #00ff64;
            transform: scale(1.1);
        }

        .email-card {
            background: rgba(255, 255, 255, 0.02);
            border-radius: 18px;
            padding: 24px 26px;
            border: 1px solid rgba(255, 255, 255, 0.04);
            transition: all 0.3s ease;
            margin-top: 10px;
        }
        .email-card:hover {
            border-color: rgba(0, 255, 100, 0.15);
            background: rgba(255, 255, 255, 0.04);
            box-shadow: 0 8px 35px rgba(0, 0, 0, 0.4);
        }
        .email-card .subject {
            color: #e6f1ff;
            font-weight: 700;
            font-size: 16px;
            margin-bottom: 10px;
            text-align: center;
        }

        .email-card .body-preview {
            color: #c9d1d9;
            font-size: 13px;
            direction: ltr;
            text-align: left;
            font-family: 'Courier New', monospace;
            white-space: pre-wrap;
            word-break: break-word;
            line-height: 1.9;
            max-height: 320px;
            overflow-y: auto;
            padding: 16px 18px;
            background: rgba(0, 0, 0, 0.35);
            border-radius: 12px;
            margin-bottom: 12px;
            border: 1px solid rgba(255, 255, 255, 0.04);
        }
        .email-card .body-preview::-webkit-scrollbar { width: 4px; }
        .email-card .body-preview::-webkit-scrollbar-track { background: rgba(255,255,255,0.02); border-radius: 10px; }
        .email-card .body-preview::-webkit-scrollbar-thumb { background: #00ff64; border-radius: 10px; }

        .email-card .links {
            font-size: 12px;
            color: #58a6ff;
            margin: 12px 0 8px;
            direction: ltr;
            text-align: left;
        }
        .email-card .links a { color: #58a6ff; text-decoration: none; transition: color 0.2s; }
        .email-card .links a:hover { color: #79c0ff; text-decoration: underline; }

        .btn-group {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 18px;
        }
        .btn-gmail {
            background: #da3b2a;
            color: #fff;
            padding: 14px 36px;
            border-radius: 12px;
            font-size: 16px;
            font-weight: 700;
            border: none;
            cursor: pointer;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            transition: all 0.25s ease;
            font-family: 'Inter', sans-serif;
            width: 100%;
            justify-content: center;
        }
        .btn-gmail:hover { background: #c6281a; transform: scale(0.97); box-shadow: 0 0 30px rgba(218, 59, 42, 0.2); }

        .btn-copy {
            background: #1f6feb;
            color: #fff;
            padding: 14px 36px;
            border-radius: 12px;
            font-size: 16px;
            font-weight: 700;
            border: none;
            cursor: pointer;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            transition: all 0.25s ease;
            font-family: 'Inter', sans-serif;
            width: 100%;
            justify-content: center;
        }
        .btn-copy:hover { background: #388bfd; transform: scale(0.97); }

        .status-msg { text-align: center; font-size: 13px; color: #8892b0; margin-top: 10px; min-height: 22px; }

        .footer {
            text-align: center;
            font-size: 12px;
            color: #495670;
            margin-top: 28px;
            border-top: 1px solid rgba(255, 255, 255, 0.04);
            padding-top: 22px;
        }
        .footer a { color: #8892b0; text-decoration: none; transition: color 0.3s; }
        .footer a:hover { color: #00ff64; }
        .footer-links { display: flex; justify-content: center; gap: 24px; flex-wrap: wrap; margin-top: 10px; }
        .badge-count { text-align: center; font-size: 12px; color: #495670; margin: 4px 0 8px 0; }

        .btn-group { flex-direction: column; gap: 12px; }
        .email-card .body-preview { font-size: 15px; max-height: 400px; padding: 18px 20px; line-height: 2; }
        .email-card .subject { font-size: 18px; }
        .to-box .addr { font-size: 16px; }
        .info-box { font-size: 16px; padding: 18px 22px; }
        .id-box { font-size: 16px; padding: 14px 20px; }
        .email-selector label { font-size: 14px; padding: 10px 14px; }
        .badge-count { font-size: 14px; }

        @media (max-width: 640px) {
            .container { padding: 20px 16px; }
            .title { font-size: 28px; }
            .email-card { padding: 16px; }
            .email-card .body-preview { font-size: 14px; padding: 14px; max-height: 350px; }
            .btn-gmail, .btn-copy { font-size: 17px; padding: 14px; }
            .to-box { font-size: 14px; }
            .info-box { font-size: 14px; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">
        <div class="badge">⚡ Security Reporting System</div>
        <h1 class="title">🛡️ Shamshir Ali</h1>
        <p class="sub">Report a Violating Telegram Channel – Direct Gmail</p>
        <div class="glow-line"></div>
    </div>

    <div class="info-box">
        <strong>📌 Violating Channel Info:</strong><br />
        <span class="label">Channel ID:</span> <strong>-1001601955559</strong><br />
        <span class="label">Username:</span> <strong>@hadafmohakeme2</strong>
    </div>

    <div class="id-box">
        🆔 <strong>Channel ID:</strong> -1001601955559 &nbsp;|&nbsp; <strong>Username:</strong> @hadafmohakeme2
    </div>

    <div class="to-box">
        <strong>📨 Send to:</strong><br />
        <span class="addr">grievance-in@telegram.org</span>
    </div>

    <div class="badge-count">📝 Select one of <strong>50 unique</strong> email templates</div>
    <div class="email-selector" id="emailSelector"></div>

    <div class="email-card">
        <div class="subject" id="emailSubject">Loading...</div>
        <div class="body-preview" id="emailBody">Loading...</div>

        <div class="links">
            🔗 <strong>Violating Links (18 total):</strong><br />
            <a href="https://t.me/hadafmohakeme2/7389" target="_blank">7389</a> ·
            <a href="https://t.me/hadafmohakeme2/7376" target="_blank">7376</a> ·
            <a href="https://t.me/hadafmohakeme2/7363" target="_blank">7363</a> ·
            <a href="https://t.me/hadafmohakeme2/7352" target="_blank">7352</a> ·
            <a href="https://t.me/hadafmohakeme2/7341" target="_blank">7341</a> ·
            <a href="https://t.me/hadafmohakeme2/7333" target="_blank">7333</a> ·
            <a href="https://t.me/hadafmohakeme2/7322" target="_blank">7322</a> ·
            <a href="https://t.me/hadafmohakeme2/7314" target="_blank">7314</a> ·
            <a href="https://t.me/hadafmohakeme2/7303" target="_blank">7303</a> ·
            <a href="https://t.me/hadafmohakeme2/7292" target="_blank">7292</a> ·
            <a href="https://t.me/hadafmohakeme2/7283" target="_blank">7283</a> ·
            <a href="https://t.me/hadafmohakeme2/7274" target="_blank">7274</a> ·
            <a href="https://t.me/hadafmohakeme2/7264" target="_blank">7264</a> ·
            <a href="https://t.me/hadafmohakeme2/7250" target="_blank">7250</a> ·
            <a href="https://t.me/hadafmohakeme2/7233" target="_blank">7233</a> ·
            <a href="https://t.me/hadafmohakeme2/7216" target="_blank">7216</a> ·
            <a href="https://t.me/hadafmohakeme2/7202" target="_blank">7202</a> ·
            <a href="https://t.me/hadafmohakeme2/7183" target="_blank">7183</a>
        </div>

        <div class="btn-group">
            <a href="#" class="btn-gmail" onclick="sendGmail()">📧 Send via Gmail</a>
            <button class="btn-copy" onclick="copyEmail()">📋 Copy Text</button>
        </div>
        <div class="status-msg" id="statusMsg"></div>
    </div>

    <div class="footer">
        📨 Send to: grievance-in@telegram.org
        <div class="footer-links">
            <span>© 2026 Shamshir Ali</span>
            <a href="https://github.com/cyberzxr" target="_blank">🐙 GitHub</a>
            <a href="https://t.me/ShamshirAliBot" target="_blank">🤖 Telegram Bot</a>
        </div>
    </div>
</div>

<script>
// ============================================================
// CONFIGURATION
// ============================================================
const TO_EMAILS = ["grievance-in@telegram.org"];
const CHANNEL_USERNAME = "@hadafmohakeme2";
const CHANNEL_ID = "-1001601955559";

const ALL_LINKS = [
    "https://t.me/hadafmohakeme2/7389",
    "https://t.me/hadafmohakeme2/7376",
    "https://t.me/hadafmohakeme2/7363",
    "https://t.me/hadafmohakeme2/7352",
    "https://t.me/hadafmohakeme2/7341",
    "https://t.me/hadafmohakeme2/7333",
    "https://t.me/hadafmohakeme2/7322",
    "https://t.me/hadafmohakeme2/7314",
    "https://t.me/hadafmohakeme2/7303",
    "https://t.me/hadafmohakeme2/7292",
    "https://t.me/hadafmohakeme2/7283",
    "https://t.me/hadafmohakeme2/7274",
    "https://t.me/hadafmohakeme2/7264",
    "https://t.me/hadafmohakeme2/7250",
    "https://t.me/hadafmohakeme2/7233",
    "https://t.me/hadafmohakeme2/7216",
    "https://t.me/hadafmohakeme2/7202",
    "https://t.me/hadafmohakeme2/7183"
];

// ============================================================
// 50 UNIQUE EMAIL TEMPLATES
// ============================================================
const templates = [];

const identities = [
    "a human rights activist", "a journalist", "a lawyer", "a concerned citizen",
    "a teacher", "a doctor", "a student", "a researcher", "a writer",
    "a community leader", "a refugee", "a peace activist", "a humanitarian",
    "a psychologist", "a social worker", "a volunteer", "a nurse", "a counselor",
    "a mentor", "a guide", "a helper", "a friend", "a neighbor", "a colleague",
    "a partner", "a teammate", "a classmate", "a roommate", "a citizen of the world",
    "a believer in justice", "a seeker of truth", "a defender of freedom",
    "a protector of the vulnerable", "a voice for the voiceless", "a fighter for rights",
    "a lover of peace", "a hater of oppression", "a dreamer of a better world",
    "an artist", "a musician", "a scientist", "a philosopher", "a historian"
];

const intros = [
    "I am writing to urgently report a channel that is actively endangering lives.",
    "I am deeply concerned about the harmful activities of a channel that must be shut down.",
    "This is an urgent report regarding a channel that is violating Telegram's policies.",
    "I am reporting a channel that is being used as a tool for persecution and doxing.",
    "The following channel is systematically sharing private information of innocent people.",
    "I have documented serious violations by a channel that targets political opponents.",
    "This channel is causing real-world harm and must be investigated immediately.",
    "I am a concerned user and I want to report dangerous behavior on Telegram.",
    "The channel I am reporting is actively putting people's lives at risk.",
    "I have evidence of a channel that is violating Telegram's Terms of Service."
];

const bodies = [
    "They are posting names, addresses, phone numbers, and photos of individuals who have expressed political opinions. This information is being used by authorities to arrest and harm these individuals.",
    "The channel encourages violence and hatred against specific groups. They share content that incites real-world violence and persecution.",
    "They are sharing private information of activists, journalists, and human rights defenders. This has led to arrests and disappearances.",
    "The channel is being used to coordinate harassment campaigns against individuals who speak out. This is a clear violation of Telegram's rules.",
    "They are posting personal data of people who have participated in protests. This information is being used to identify and arrest them.",
    "The channel is a hub for spreading misinformation and inciting violence against political opponents. This is a serious threat to safety.",
    "They are sharing details of individuals' locations, workplaces, and family members. This puts entire families at risk.",
    "The channel has been active for months and has caused numerous arrests. It is a direct threat to human rights.",
    "They are using Telegram to organize campaigns of intimidation and harassment against innocent citizens.",
    "The content on this channel is designed to incite fear and silence political opposition. It is a clear violation of Telegram's policies."
];

const closings = [
    "I urge you to investigate and block this channel immediately.",
    "Please take immediate action to remove this channel and protect users.",
    "This channel must be shut down to prevent further harm.",
    "I request that you take this report seriously and block the channel.",
    "Please investigate and take appropriate action against this channel.",
    "This is a serious violation that requires immediate attention.",
    "I hope you will act swiftly to remove this dangerous channel.",
    "Please protect Telegram users by blocking this channel.",
    "This channel is a threat to safety and must be removed.",
    "I trust you will take the necessary action to stop this harmful activity."
];

for (let i = 0; i < 50; i++) {
    const identity = identities[i % identities.length];
    const intro = intros[i % intros.length];
    const body = bodies[i % bodies.length];
    const closing = closings[i % closings.length];
    const num = i + 1;

    const subject = `🚨 URGENT: Report Violating Channel ${CHANNEL_USERNAME} (Report #${num})`;

    const emailBody = `Dear Telegram Trust & Safety Team,

${intro}

The channel is called ${CHANNEL_USERNAME} (ID: ${CHANNEL_ID}) and has been active for a long time.

${body}

I have documented multiple examples of this harmful activity. Here are the links to the posts:

${ALL_LINKS.join('\n')}

${closing}

Thank you for your attention to this serious matter.

Sincerely,
${identity.charAt(0).toUpperCase() + identity.slice(1)}

Channel ID: ${CHANNEL_ID}
Username: ${CHANNEL_USERNAME}
Links: ${ALL_LINKS.join(', ')}`;

    templates.push({ subject, body: emailBody });
}

// ============================================================
// RENDER
// ============================================================
let selectedIndex = 0;

function renderSelector() {
    const container = document.getElementById('emailSelector');
    let html = '';
    templates.forEach((t, i) => {
        const isSelected = i === selectedIndex;
        html += `
            <label class="${isSelected ? 'selected' : ''}" onclick="selectTemplate(${i})">
                <input type="radio" name="template" value="${i}" ${isSelected ? 'checked' : ''}>
                #${i+1}: ${t.subject.substring(0, 55)}${t.subject.length > 55 ? '...' : ''}
            </label>
        `;
    });
    container.innerHTML = html;
}

function selectTemplate(index) {
    selectedIndex = index;
    renderSelector();
    updateDisplay();
}

function updateDisplay() {
    const t = templates[selectedIndex];
    document.getElementById('emailSubject').textContent = t.subject;
    document.getElementById('emailBody').textContent = t.body;
}

// ============================================================
// ACTIONS
// ============================================================
function getCurrentTemplate() {
    return templates[selectedIndex];
}

function sendGmail() {
    event.preventDefault();
    const t = getCurrentTemplate();
    const to = TO_EMAILS.join(',');
    const subject = encodeURIComponent(t.subject);
    const body = encodeURIComponent(t.body);
    
    // استفاده از intent گوگل برای باز کردن مستقیم اپ جیمیل
    const gmailIntent = `intent://mailto/${to}?subject=${subject}&body=${body}#Intent;package=com.google.android.gm;end;`;
    const gmailApp = `googlegmail://co?to=${to}&subject=${subject}&body=${body}`;
    const gmailWeb = `https://mail.google.com/mail/?view=cm&fs=1&to=${to}&su=${subject}&body=${body}`;
    
    const isMobile = /Android|iPhone|iPad|iPod/i.test(navigator.userAgent);
    
    if (isMobile) {
        // برای اندروید: استفاده از intent
        if (/Android/i.test(navigator.userAgent)) {
            window.location.href = gmailIntent;
        } else {
            // برای iOS: استفاده از googlegmail://
            window.location.href = gmailApp;
        }
        
        // fallback به مرورگر
        setTimeout(function() {
            window.open(gmailWeb, '_blank');
        }, 1500);
    } else {
        window.open(gmailWeb, '_blank');
    }
    
    showStatus('📨 Opening Gmail app...');
}

function copyEmail() {
    const t = getCurrentTemplate();
    const text = `Subject: ${t.subject}\n\n${t.body}`;
    navigator.clipboard.writeText(text)
        .then(() => showStatus('✅ Copied to clipboard!', '#00ff64'))
        .catch(() => showStatus('❌ Failed to copy', '#f85149'));
}

function showStatus(msg, color = '#8892b0') {
    const el = document.getElementById('statusMsg');
    el.textContent = msg;
    el.style.color = color;
    setTimeout(() => { el.textContent = ''; }, 3500);
}

// ============================================================
// INIT
// ============================================================
renderSelector();
updateDisplay();
</script>

</body>
</html>
