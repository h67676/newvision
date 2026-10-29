<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0, viewport-fit=cover">
  <meta name="theme-color" content="#0a0a0f">
  <title>NEW VISION INTERNATIONAL — استمارة التسجيل</title>

  <!-- Font Tajawal & Inter -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg-dark: #08080d;
      --card-bg: rgba(20, 20, 32, 0.55);
      --card-border: rgba(255, 140, 0, 0.22);
      --accent-orange: #ff8c00;
      --accent-orange-glow: rgba(255, 140, 0, 0.45);
      --accent-purple: #a855f7;
      --accent-purple-glow: rgba(168, 85, 247, 0.35);
      --text-main: #f8fafc;
      --text-muted: #a0aec0;
      --glass-input: rgba(10, 10, 18, 0.6);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Tajawal', 'Inter', sans-serif;
      -webkit-tap-highlight-color: transparent;
    }

    body {
      background-color: var(--bg-dark);
      color: var(--text-main);
      min-height: 100vh;
      min-height: -webkit-fill-available;
      display: flex;
      flex-direction: column;
      align-items: center;
      position: relative;
      overflow-x: hidden;
    }

    /* Ambient Background Animated Orbs for Ultra-Glass Effect */
    .bg-orbs {
      position: fixed;
      top: 0; left: 0; width: 100vw; height: 100vh;
      pointer-events: none;
      z-index: 0;
      overflow: hidden;
    }
    .orb {
      position: absolute;
      border-radius: 50%;
      filter: blur(120px);
      opacity: 0.4;
      animation: floatOrb 12s infinite alternate ease-in-out;
    }
    .orb-1 {
      width: clamp(300px, 45vw, 550px);
      height: clamp(300px, 45vw, 550px);
      background: #ff8c00;
      top: -100px;
      right: -80px;
    }
    .orb-2 {
      width: clamp(320px, 50vw, 600px);
      height: clamp(320px, 50vw, 600px);
      background: #7e22ce;
      bottom: -120px;
      left: -80px;
      animation-delay: -6s;
    }

    @keyframes floatOrb {
      0% { transform: translate(0, 0) scale(1); }
      100% { transform: translate(30px, 40px) scale(1.1); }
    }

    /* Glass Header */
    header {
      width: 100%;
      padding: clamp(0.9rem, 2.5vw, 1.3rem) clamp(1rem, 6vw, 8%);
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: rgba(10, 10, 15, 0.65);
      border-bottom: 1px solid var(--card-border);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      position: relative;
      z-index: 10;
      gap: 1rem;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
    }

    .company-logo {
      display: flex;
      align-items: center;
      gap: 0.9rem;
      flex-shrink: 0;
    }

    .logo-diamond {
      width: clamp(40px, 5vw, 50px);
      height: clamp(40px, 5vw, 50px);
      background: rgba(10, 10, 15, 0.8);
      border: 2.5px solid var(--accent-orange);
      border-radius: 14px;
      transform: rotate(45deg);
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 0 20px var(--accent-orange-glow);
    }

    .logo-symbol {
      transform: rotate(-45deg);
      font-size: clamp(1.3rem, 2.2vw, 1.6rem);
      font-weight: 800;
      color: var(--accent-purple);
      text-shadow: 0 0 12px var(--accent-purple-glow);
    }

    .logo-text-wrap {
      display: flex;
      flex-direction: column;
    }

    .logo-title {
      font-weight: 800;
      font-size: clamp(1rem, 1.6vw, 1.2rem);
      color: #fff;
      letter-spacing: 0.5px;
    }

    .logo-sub {
      font-size: clamp(0.65rem, 1vw, 0.75rem);
      color: var(--accent-orange);
      letter-spacing: 1.5px;
      font-weight: 700;
    }

    .company-title {
      font-size: clamp(1.05rem, 1.8vw, 1.35rem);
      font-weight: 800;
      color: #fff;
      text-align: center;
    }
    .company-title span {
      color: var(--accent-purple);
      font-size: clamp(0.78rem, 1.2vw, 0.88rem);
      display: block;
      font-weight: 500;
      margin-top: 2px;
    }

    /* Glass Language Button */
    .lang-btn {
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid rgba(255, 140, 0, 0.35);
      padding: 0.55rem 1.1rem;
      border-radius: 14px;
      color: #fff;
      font-size: 0.85rem;
      font-weight: 700;
      cursor: pointer;
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
      display: flex;
      align-items: center;
      gap: 0.5rem;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
      flex-shrink: 0;
    }

    .lang-btn:hover {
      background: rgba(255, 140, 0, 0.18);
      border-color: var(--accent-orange);
      box-shadow: 0 0 20px var(--accent-orange-glow);
      transform: translateY(-2px);
    }

    /* Main Container & Modern Glass Form */
    main {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: 540px;
      padding: clamp(1.8rem, 5vw, 3rem) 1.2rem;
      margin: auto 0;
    }

    .form-card {
      background: var(--card-bg);
      border: 1px solid var(--card-border);
      border-radius: clamp(20px, 4vw, 28px);
      padding: clamp(2rem, 5vw, 2.8rem) clamp(1.4rem, 4vw, 2.2rem);
      backdrop-filter: blur(25px);
      -webkit-backdrop-filter: blur(25px);
      box-shadow: 0 30px 60px rgba(0, 0, 0, 0.7), inset 0 1px 0 rgba(255, 255, 255, 0.1);
      position: relative;
    }

    .form-card h2 {
      font-size: clamp(1.4rem, 2.5vw, 1.7rem);
      color: #fff;
      margin-bottom: 0.4rem;
      text-align: center;
      font-weight: 800;
    }

    .form-card p {
      color: var(--text-muted);
      font-size: clamp(0.88rem, 1.5vw, 0.98rem);
      text-align: center;
      margin-bottom: 2rem;
    }

    .form-group {
      margin-bottom: 1.3rem;
    }

    .form-group label {
      display: block;
      margin-bottom: 0.45rem;
      font-size: 0.95rem;
      color: var(--text-main);
      font-weight: 600;
    }

    .form-control {
      width: 100%;
      padding: 0.9rem 1.2rem;
      background: var(--glass-input);
      border: 1px solid rgba(255, 255, 255, 0.12);
      border-radius: 14px;
      color: #fff;
      font-size: 1rem;
      outline: none;
      transition: all 0.3s ease;
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
    }

    .form-control:focus {
      border-color: var(--accent-orange);
      background: rgba(15, 15, 25, 0.85);
      box-shadow: 0 0 20px var(--accent-orange-glow);
    }

    /* Elevated Glass Button */
    .btn-submit {
      width: 100%;
      padding: 1rem;
      margin-top: 1.2rem;
      background: linear-gradient(135deg, var(--accent-orange), #ea580c);
      border: none;
      border-radius: 14px;
      color: #fff;
      font-size: 1.1rem;
      font-weight: 800;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 6px 25px var(--accent-orange-glow);
    }

    .btn-submit:disabled {
      background: #27272a;
      color: #71717a;
      cursor: not-allowed;
      box-shadow: none;
      opacity: 0.55;
    }

    .btn-submit:not(:disabled):hover {
      transform: translateY(-2px);
      box-shadow: 0 10px 30px rgba(255, 140, 0, 0.65);
    }

    .status-msg {
      margin-top: 1.2rem;
      padding: 0.9rem;
      border-radius: 12px;
      text-align: center;
      font-weight: 700;
      display: none;
      backdrop-filter: blur(10px);
    }

    .status-msg.success {
      background: rgba(34, 197, 94, 0.15);
      border: 1px solid #22c55e;
      color: #4ade80;
    }

    footer {
      position: relative;
      z-index: 10;
      padding: 1.5rem;
      color: var(--text-muted);
      font-size: 0.82rem;
      text-align: center;
    }

    @media (max-width: 640px) {
      header {
        flex-wrap: wrap;
        justify-content: space-between;
      }
      .company-title {
        order: 3;
        width: 100%;
        margin-top: 0.5rem;
        padding-top: 0.5rem;
        border-top: 1px solid rgba(255, 255, 255, 0.08);
      }
    }
  </style>
</head>
<body>

  <!-- Ambient Animated Glass Orbs -->
  <div class="bg-orbs">
    <div class="orb orb-1"></div>
    <div class="orb orb-2"></div>
  </div>

  <!-- Glass Header -->
  <header>
    <div class="company-logo">
      <div class="logo-diamond">
        <span class="logo-symbol">N</span>
      </div>
      <div class="logo-text-wrap">
        <span class="logo-title">NEW VISION</span>
        <span class="logo-sub">INTERNATIONAL</span>
      </div>
    </div>

    <div class="company-title">
      <span id="txt-header-title">نيوفيزيون انترناسيونال</span>
      <span id="txt-header-sub">استمارة التسجيل الرسمية</span>
    </div>

    <button class="lang-btn" id="langToggle" aria-label="تغيير اللغة">
      🌐 <span id="langLabel">Français</span>
    </button>
  </header>

  <!-- Main Glass Card Form -->
  <main>
    <div class="form-card">
      <h2 id="txt-form-title">ابدأ خطوتك الأولى الآن</h2>
      <p id="txt-form-subtitle">يرجى إكمال جميع البيانات لتفعيل زر الإرسال</p>

      <form id="registrationForm">
        <div class="form-group">
          <label for="firstName" id="lbl-firstName">الاسم</label>
          <input type="text" id="firstName" name="الاسم" class="form-control" placeholder="أدخل اسمك" required>
        </div>

        <div class="form-group">
          <label for="lastName" id="lbl-lastName">اللقب</label>
          <input type="text" id="lastName" name="اللقب" class="form-control" placeholder="أدخل لقبك" required>
        </div>

        <div class="form-group">
          <label for="phone" id="lbl-phone">رقم الهاتف</label>
          <input type="tel" id="phone" name="رقم الهاتف" class="form-control" placeholder="06XX XX XX XX" required>
        </div>

        <div class="form-group">
          <label for="job" id="lbl-job">ماذا تعمل / المهنة</label>
          <input type="text" id="job" name="المهنة" class="form-control" placeholder="مثال: مهندس، طالب، تاجر..." required>
        </div>

        <button type="submit" id="submitBtn" class="btn-submit" disabled>إرسال البيانات</button>
        
        <div id="statusMsg" class="status-msg"></div>
      </form>
    </div>
  </main>

  <footer>
    <span id="txt-footer">© 2026 NEW VISION INTERNATIONAL — جميع الحقوق محفوظة.</span>
  </footer>

  <script>
    const form = document.getElementById('registrationForm');
    const submitBtn = document.getElementById('submitBtn');
    const inputs = form.querySelectorAll('.form-control');
    const statusMsg = document.getElementById('statusMsg');
    const langToggle = document.getElementById('langToggle');
    const langLabel = document.getElementById('langLabel');

    const translations = {
      ar: {
        dir: 'rtl',
        lang: 'ar',
        headerTitle: 'نيوفيزيون انترناسيونال',
        headerSub: 'استمارة التسجيل الرسمية',
        formTitle: 'ابدأ خطوتك الأولى الآن',
        formSubtitle: 'يرجى إكمال جميع البيانات لتفعيل زر الإرسال',
        firstName: 'الاسم',
        phFirstName: 'أدخل اسمك',
        lastName: 'اللقب',
        phLastName: 'أدخل لقبك',
        phone: 'رقم الهاتف',
        phPhone: '06XX XX XX XX',
        job: 'ماذا تعمل / المهنة',
        phJob: 'مثال: مهندس، طالب، تاجر...',
        submit: 'إرسال البيانات',
        sending: 'جاري الإرسال...',
        success: '✓ تم إرسال معلوماتك بنجاح إلى N-Vision International!',
        error: 'حدث خطأ أثناء الإرسال، يرجى المحاولة لاحقاً.',
        footer: '© 2026 NEW VISION INTERNATIONAL — جميع الحقوق محفوظة.',
        btnLang: 'Français'
      },
      fr: {
        dir: 'ltr',
        lang: 'fr',
        headerTitle: 'N-VISION INTERNATIONAL',
        headerSub: 'Formulaire d\'inscription officiel',
        formTitle: 'Faites votre premier pas maintenant',
        formSubtitle: 'Veuillez remplir tous les champs pour activer le bouton',
        firstName: 'Prénom',
        phFirstName: 'Entrez votre prénom',
        lastName: 'Nom',
        phLastName: 'Entrez votre nom',
        phone: 'Numéro de téléphone',
        phPhone: '06XX XX XX XX',
        job: 'Profession / Occupation',
        phJob: 'Ex: Ingénieur, Étudiant, Commerçant...',
        submit: 'Envoyer les données',
        sending: 'Envoi en cours...',
        success: '✓ Vos informations ont été envoyées avec succès à N-Vision International !',
        error: 'Une erreur est survenue, veuillez réessayer plus tard.',
        footer: '© 2026 NEW VISION INTERNATIONAL — Tous droits réservés.',
        btnLang: 'العربية'
      }
    };

    let currentLang = 'ar';

    function setLanguage(lang) {
      currentLang = lang;
      const t = translations[lang];
      
      document.documentElement.setAttribute('dir', t.dir);
      document.documentElement.setAttribute('lang', t.lang);
      
      document.getElementById('txt-header-title').innerText = t.headerTitle;
      document.getElementById('txt-header-sub').innerText = t.headerSub;
      document.getElementById('txt-form-title').innerText = t.formTitle;
      document.getElementById('txt-form-subtitle').innerText = t.formSubtitle;
      
      document.getElementById('lbl-firstName').innerText = t.firstName;
      document.getElementById('firstName').placeholder = t.phFirstName;
      
      document.getElementById('lbl-lastName').innerText = t.lastName;
      document.getElementById('lastName').placeholder = t.phLastName;
      
      document.getElementById('lbl-phone').innerText = t.phone;
      document.getElementById('phone').placeholder = t.phPhone;
      
      document.getElementById('lbl-job').innerText = t.job;
      document.getElementById('job').placeholder = t.phJob;
      
      submitBtn.innerText = t.submit;
      document.getElementById('txt-footer').innerText = t.footer;
      langLabel.innerText = t.btnLang;
    }

    langToggle.addEventListener('click', () => {
      setLanguage(currentLang === 'ar' ? 'fr' : 'ar');
    });

    function checkInputs() {
      let allFilled = true;
      inputs.forEach(input => {
        if (input.value.trim() === '') {
          allFilled = false;
        }
      });
      submitBtn.disabled = !allFilled;
    }

    inputs.forEach(input => {
      input.addEventListener('input', checkInputs);
    });

    form.addEventListener('submit', async function(e) {
      e.preventDefault();
      const t = translations[currentLang];
      
      submitBtn.disabled = true;
      submitBtn.innerText = t.sending;

      const formData = new FormData(form);

      try {
        const response = await fetch('https://formspree.io/f/xnppzzrb', {
          method: 'POST',
          body: formData,
          headers: {
            'Accept': 'application/json'
          }
        });

        if (response.ok) {
          statusMsg.className = 'status-msg success';
          statusMsg.innerText = t.success;
          statusMsg.style.display = 'block';
          form.reset();
          checkInputs();
          submitBtn.innerText = t.submit;
        } else {
          alert(t.error);
          submitBtn.innerText = t.submit;
          checkInputs();
        }
      } catch (error) {
        alert(t.error);
        submitBtn.innerText = t.submit;
        checkInputs();
      }
    });
  </script>
</body>
</html>
