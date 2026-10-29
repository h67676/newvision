<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0, viewport-fit=cover">
  <meta name="theme-color" content="#07070a">
  <title>NEW VISION INTERNATIONAL — Inscription</title>

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg: #07070a;
      --card-bg: rgba(18, 18, 26, 0.45);
      --card-border: rgba(255, 255, 255, 0.08);
      --accent-orange: #ff8c00;
      --accent-purple: #a855f7;
      --text-primary: #ffffff;
      --text-secondary: #94a3b8;
      --input-bg: rgba(255, 255, 255, 0.03);
      --input-border: rgba(255, 255, 255, 0.08);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Tajawal', 'Plus Jakarta Sans', sans-serif;
      -webkit-tap-highlight-color: transparent;
    }

    body {
      background-color: var(--bg);
      color: var(--text-primary);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;
      position: relative;
      overflow-x: hidden;
    }

    /* Minimal Glowing Background Effect */
    .glow-container {
      position: fixed;
      top: 0; left: 0; width: 100vw; height: 100vh;
      pointer-events: none;
      z-index: 0;
    }
    .glow-spot {
      position: absolute;
      border-radius: 50%;
      filter: blur(140px);
      opacity: 0.25;
    }
    .spot-1 {
      width: 450px; height: 450px;
      background: var(--accent-orange);
      top: -150px; right: -100px;
    }
    .spot-2 {
      width: 500px; height: 500px;
      background: var(--accent-purple);
      bottom: -180px; left: -120px;
    }

    /* Minimal Modern Header */
    header {
      width: 100%;
      max-width: 1000px;
      padding: 1.5rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: relative;
      z-index: 10;
    }

    .brand-logo {
      display: flex;
      align-items: center;
      gap: 0.8rem;
    }

    .logo-icon {
      width: 42px;
      height: 42px;
      border-radius: 12px;
      background: linear-gradient(135deg, rgba(255,140,0,0.2), rgba(168,85,247,0.2));
      border: 1px solid rgba(255, 140, 0, 0.4);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      font-size: 1.2rem;
      color: var(--accent-orange);
      backdrop-filter: blur(10px);
    }

    .brand-names {
      display: flex;
      flex-direction: column;
    }

    .brand-title {
      font-weight: 800;
      font-size: 1.05rem;
      letter-spacing: 0.5px;
    }

    .brand-sub {
      font-size: 0.72rem;
      color: var(--accent-purple);
      font-weight: 600;
    }

    /* Language Switcher Badge */
    .lang-switcher {
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid rgba(255, 255, 255, 0.1);
      padding: 0.45rem 1rem;
      border-radius: 100px;
      color: #fff;
      font-size: 0.82rem;
      font-weight: 600;
      cursor: pointer;
      backdrop-filter: blur(16px);
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      gap: 0.4rem;
    }

    .lang-switcher:hover {
      border-color: var(--accent-orange);
      background: rgba(255, 140, 0, 0.1);
    }

    /* Modern Minimal Glass Card */
    main {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: 460px;
      padding: 1rem 1.2rem;
      margin: auto 0;
    }

    .card {
      background: var(--card-bg);
      border: 1px solid var(--card-border);
      border-radius: 24px;
      padding: 2.2rem 1.8rem;
      backdrop-filter: blur(30px);
      -webkit-backdrop-filter: blur(30px);
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
    }

    .card-header {
      text-align: center;
      margin-bottom: 2rem;
    }

    .card-title {
      font-size: 1.45rem;
      font-weight: 800;
      color: var(--text-primary);
      margin-bottom: 0.3rem;
    }

    .card-subtitle {
      font-size: 0.88rem;
      color: var(--text-secondary);
    }

    /* Form Fields */
    .field {
      margin-bottom: 1.2rem;
    }

    .field label {
      display: block;
      font-size: 0.88rem;
      font-weight: 600;
      color: #e2e8f0;
      margin-bottom: 0.4rem;
    }

    .field input {
      width: 100%;
      padding: 0.85rem 1rem;
      background: var(--input-bg);
      border: 1px solid var(--input-border);
      border-radius: 14px;
      color: #fff;
      font-size: 0.95rem;
      outline: none;
      transition: all 0.3s ease;
    }

    .field input:focus {
      border-color: var(--accent-orange);
      background: rgba(255, 255, 255, 0.06);
      box-shadow: 0 0 15px rgba(255, 140, 0, 0.2);
    }

    /* Fluid Modern Button */
    .submit-btn {
      width: 100%;
      padding: 0.95rem;
      margin-top: 1rem;
      background: linear-gradient(135deg, var(--accent-orange), #e67e00);
      border: none;
      border-radius: 14px;
      color: #fff;
      font-size: 1rem;
      font-weight: 700;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 8px 25px rgba(255, 140, 0, 0.3);
    }

    .submit-btn:disabled {
      background: rgba(255, 255, 255, 0.08);
      color: #64748b;
      cursor: not-allowed;
      box-shadow: none;
    }

    .submit-btn:not(:disabled):hover {
      transform: translateY(-2px);
      box-shadow: 0 12px 30px rgba(255, 140, 0, 0.5);
    }

    .alert {
      margin-top: 1rem;
      padding: 0.8rem;
      border-radius: 12px;
      text-align: center;
      font-size: 0.9rem;
      font-weight: 600;
      display: none;
    }

    .alert-success {
      background: rgba(34, 197, 94, 0.15);
      border: 1px solid rgba(34, 197, 94, 0.3);
      color: #4ade80;
    }

    footer {
      position: relative;
      z-index: 10;
      padding: 1.5rem;
      color: var(--text-secondary);
      font-size: 0.8rem;
      text-align: center;
    }
  </style>
</head>
<body>

  <!-- Background Orbs -->
  <div class="glow-container">
    <div class="glow-spot spot-1"></div>
    <div class="glow-spot spot-2"></div>
  </div>

  <!-- Header -->
  <header>
    <div class="brand-logo">
      <div class="logo-icon">N</div>
      <div class="brand-names">
        <span class="brand-title">NEW VISION</span>
        <span class="brand-sub">INTERNATIONAL</span>
      </div>
    </div>

    <button class="lang-switcher" id="langBtn">
      🌐 <span id="langText">Français</span>
    </button>
  </header>

  <!-- Card Form -->
  <main>
    <div class="card">
      <div class="card-header">
        <h1 class="card-title" id="t-title">ابدأ خطوتك الأولى الآن</h1>
        <p class="card-subtitle" id="t-sub">يرجى ملء جميع البيانات لتفعيل زر الإرسال</p>
      </div>

      <form id="appForm">
        <div class="field">
          <label for="firstName" id="l-firstName">الاسم</label>
          <input type="text" id="firstName" name="الاسم" placeholder="أدخل اسمك" required>
        </div>

        <div class="field">
          <label for="lastName" id="l-lastName">اللقب</label>
          <input type="text" id="lastName" name="اللقب" placeholder="أدخل لقبك" required>
        </div>

        <div class="field">
          <label for="phone" id="l-phone">رقم الهاتف</label>
          <input type="tel" id="phone" name="رقم الهاتف" placeholder="06XX XX XX XX" required>
        </div>

        <div class="field">
          <label for="job" id="l-job">ماذا تعمل / المهنة</label>
          <input type="text" id="job" name="المهنة" placeholder="مثال: مهندس، طالب..." required>
        </div>

        <button type="submit" id="btnSubmit" class="submit-btn" disabled>إرسال البيانات</button>

        <div id="alertMsg" class="alert alert-success"></div>
      </form>
    </div>
  </main>

  <footer>
    <span id="t-footer">© 2026 NEW VISION INTERNATIONAL — جميع الحقوق محفوظة.</span>
  </footer>

  <script>
    const form = document.getElementById('appForm');
    const submitBtn = document.getElementById('btnSubmit');
    const inputs = form.querySelectorAll('input');
    const alertMsg = document.getElementById('alertMsg');
    const langBtn = document.getElementById('langBtn');
    const langText = document.getElementById('langText');

    const i18n = {
      ar: {
        dir: 'rtl',
        lang: 'ar',
        title: 'ابدأ خطوتك الأولى الآن',
        sub: 'يرجى ملء جميع البيانات لتفعيل زر الإرسال',
        firstName: 'الاسم',
        pFirstName: 'أدخل اسمك',
        lastName: 'اللقب',
        pLastName: 'أدخل لقبك',
        phone: 'رقم الهاتف',
        pPhone: '06XX XX XX XX',
        job: 'ماذا تعمل / المهنة',
        pJob: 'مثال: مهندس، طالب...',
        submit: 'إرسال البيانات',
        sending: 'جاري الإرسال...',
        success: '✓ تم الإرسال بنجاح إلى N-Vision International !',
        footer: '© 2026 NEW VISION INTERNATIONAL — جميع الحقوق محفوظة.',
        btn: 'Français'
      },
      fr: {
        dir: 'ltr',
        lang: 'fr',
        title: 'Faites votre premier pas',
        sub: 'Veuillez remplir tous les champs pour activer le bouton',
        firstName: 'Prénom',
        pFirstName: 'Votre prénom',
        lastName: 'Nom',
        pLastName: 'Votre nom',
        phone: 'Téléphone',
        pPhone: '06XX XX XX XX',
        job: 'Profession',
        pJob: 'Ex: Étudiant, Ingénieur...',
        submit: 'Envoyer les données',
        sending: 'Envoi en cours...',
        success: '✓ Envoyé avec succès à N-Vision International !',
        footer: '© 2026 NEW VISION INTERNATIONAL — Tous droits réservés.',
        btn: 'العربية'
      }
    };

    let curLang = 'ar';

    function switchLanguage(l) {
      curLang = l;
      const data = i18n[l];
      document.documentElement.dir = data.dir;
      document.documentElement.lang = data.lang;

      document.getElementById('t-title').innerText = data.title;
      document.getElementById('t-sub').innerText = data.sub;

      document.getElementById('l-firstName').innerText = data.firstName;
      document.getElementById('firstName').placeholder = data.pFirstName;

      document.getElementById('l-lastName').innerText = data.lastName;
      document.getElementById('lastName').placeholder = data.pLastName;

      document.getElementById('l-phone').innerText = data.phone;
      document.getElementById('phone').placeholder = data.pPhone;

      document.getElementById('l-job').innerText = data.job;
      document.getElementById('job').placeholder = data.pJob;

      submitBtn.innerText = data.submit;
      document.getElementById('t-footer').innerText = data.footer;
      langText.innerText = data.btn;
    }

    langBtn.addEventListener('click', () => {
      switchLanguage(curLang === 'ar' ? 'fr' : 'ar');
    });

    function validate() {
      let valid = true;
      inputs.forEach(i => { if (i.value.trim() === '') valid = false; });
      submitBtn.disabled = !valid;
    }

    inputs.forEach(i => i.addEventListener('input', validate));

    form.addEventListener('submit', async (e) => {
      e.preventDefault();
      const data = i18n[curLang];
      submitBtn.disabled = true;
      submitBtn.innerText = data.sending;

      try {
        const res = await fetch('https://formspree.io/f/xnppzzrb', {
          method: 'POST',
          body: new FormData(form),
          headers: { 'Accept': 'application/json' }
        });

        if (res.ok) {
          alertMsg.innerText = data.success;
          alertMsg.style.display = 'block';
          form.reset();
          validate();
          submitBtn.innerText = data.submit;
        } else {
          alert('Erreur lors de l\'envoi.');
          submitBtn.innerText = data.submit;
          validate();
        }
      } catch (err) {
        alert('Erreur de connexion.');
        submitBtn.innerText = data.submit;
        validate();
      }
    });
  </script>
</body>
</html>
