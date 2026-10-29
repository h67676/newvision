<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <meta name="theme-color" content="#0a0a0f">
  <title>NEW VISION INTERNATIONAL — استمارة التسجيل</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">
  <style>
    :root{--bg:#08080d;--card:rgba(20,20,32,.62);--border:rgba(255,140,0,.22);--orange:#ff8c00;--orange-glow:rgba(255,140,0,.4);--purple:#a855f7;--purple-glow:rgba(168,85,247,.35);--text:#f8fafc;--muted:#a0aec0;--input:rgba(10,10,18,.65)}
    *{box-sizing:border-box;margin:0;padding:0;font-family:'Tajawal','Inter',sans-serif;-webkit-tap-highlight-color:transparent}
    body{background:var(--bg);color:var(--text);min-height:100vh;display:flex;flex-direction:column;align-items:center;position:relative;overflow-x:hidden}
    .bg-orbs{position:fixed;inset:0;pointer-events:none;z-index:0;overflow:hidden}
    .orb{position:absolute;border-radius:50%;filter:blur(120px);opacity:.4;animation:floatOrb 12s infinite alternate ease-in-out}
    .orb-1{width:clamp(300px,45vw,550px);height:clamp(300px,45vw,550px);background:#ff8c00;top:-100px;right:-80px}
    .orb-2{width:clamp(320px,50vw,600px);height:clamp(320px,50vw,600px);background:#7e22ce;bottom:-120px;left:-80px;animation-delay:-6s}
    @keyframes floatOrb{to{transform:translate(30px,40px) scale(1.1)}}
    header{width:100%;padding:clamp(.9rem,2.5vw,1.3rem) clamp(1rem,6vw,8%);display:flex;justify-content:space-between;align-items:center;background:rgba(10,10,15,.65);border-bottom:1px solid var(--border);backdrop-filter:blur(20px);position:relative;z-index:10;gap:1rem;box-shadow:0 10px 30px #0006}
    .company-logo{display:flex;align-items:center;gap:.9rem;flex-shrink:0}.logo-diamond{width:clamp(40px,5vw,50px);height:clamp(40px,5vw,50px);background:#0a0a0fcc;border:2.5px solid var(--orange);border-radius:14px;transform:rotate(45deg);display:flex;align-items:center;justify-content:center;box-shadow:0 0 20px var(--orange-glow)}
    .logo-symbol{transform:rotate(-45deg);font-size:clamp(1.3rem,2.2vw,1.6rem);font-weight:800;color:var(--purple);text-shadow:0 0 12px var(--purple-glow)}.logo-text-wrap{display:flex;flex-direction:column}.logo-title{font-weight:800;font-size:clamp(1rem,1.6vw,1.2rem);color:#fff;letter-spacing:.5px}.logo-sub{font-size:clamp(.65rem,1vw,.75rem);color:var(--orange);letter-spacing:1.5px;font-weight:700}
    .company-title{font-size:clamp(1.05rem,1.8vw,1.35rem);font-weight:800;color:#fff;text-align:center}.company-title span{color:var(--purple);font-size:clamp(.78rem,1.2vw,.88rem);display:block;font-weight:500;margin-top:2px}
    .lang-btn{background:#ffffff0a;border:1px solid #ff8c0059;padding:.55rem 1.1rem;border-radius:14px;color:#fff;font-size:.85rem;font-weight:700;cursor:pointer;backdrop-filter:blur(16px);transition:.3s;display:flex;align-items:center;gap:.5rem;box-shadow:0 4px 20px #0005;flex-shrink:0}.lang-btn:hover{background:#ff8c002e;border-color:var(--orange);box-shadow:0 0 20px var(--orange-glow);transform:translateY(-2px)}
    main{position:relative;z-index:1;width:100%;max-width:540px;padding:clamp(1.8rem,5vw,3rem) 1.2rem;margin:auto 0}.form-card{background:var(--card);border:1px solid var(--border);border-radius:clamp(20px,4vw,28px);padding:clamp(2rem,5vw,2.8rem) clamp(1.4rem,4vw,2.2rem);backdrop-filter:blur(25px);box-shadow:0 30px 60px #000b,inset 0 1px 0 #ffffff1a}
    .form-card h2{font-size:clamp(1.4rem,2.5vw,1.7rem);color:#fff;margin-bottom:.4rem;text-align:center;font-weight:800}.form-card p{color:var(--muted);font-size:clamp(.88rem,1.5vw,.98rem);text-align:center;margin-bottom:2rem}.form-group{margin-bottom:1.3rem}.form-group label{display:block;margin-bottom:.45rem;font-size:.95rem;color:var(--text);font-weight:600}
    .form-control{width:100%;padding:.9rem 1.2rem;background:var(--input);border:1px solid #ffffff1f;border-radius:14px;color:#fff;font-size:1rem;outline:none;transition:.3s;backdrop-filter:blur(10px)}.form-control::placeholder{color:#94a3b8}.form-control:focus{border-color:var(--orange);background:#0f0f19d9;box-shadow:0 0 20px var(--orange-glow)}
    .btn-submit{width:100%;padding:1rem;margin-top:1.2rem;background:linear-gradient(135deg,var(--orange),#ea580c);border:0;border-radius:14px;color:#fff;font-size:1.1rem;font-weight:800;cursor:pointer;transition:.3s;box-shadow:0 6px 25px var(--orange-glow)}.btn-submit:disabled{background:#27272a;color:#71717a;cursor:not-allowed;box-shadow:none;opacity:.65}.btn-submit:not(:disabled):hover{transform:translateY(-2px);box-shadow:0 10px 30px #ff8c00a6}
    .status-msg{margin-top:1.2rem;padding:.9rem;border-radius:12px;text-align:center;font-weight:700;display:none;backdrop-filter:blur(10px)}.status-msg.success{display:block;background:#22c55e26;border:1px solid #22c55e;color:#4ade80}.status-msg.error{display:block;background:#ef444426;border:1px solid #ef4444;color:#fca5a5}
    footer{position:relative;z-index:10;padding:1.5rem;color:var(--muted);font-size:.82rem;text-align:center}
    @media(max-width:640px){header{flex-wrap:wrap;justify-content:space-between}.company-title{order:3;width:100%;margin-top:.5rem;padding-top:.5rem;border-top:1px solid #ffffff14}}
    @media(prefers-reduced-motion:reduce){*,*::before,*::after{animation:none!important;transition:none!important;scroll-behavior:auto!important}}
  </style>
</head>
<body>
  <div class="bg-orbs" aria-hidden="true"><div class="orb orb-1"></div><div class="orb orb-2"></div></div>
  <header>
    <div class="company-logo"><div class="logo-diamond"><span class="logo-symbol">N</span></div><div class="logo-text-wrap"><span class="logo-title">NEW VISION</span><span class="logo-sub">INTERNATIONAL</span></div></div>
    <div class="company-title"><span id="txt-header-title">نيوفيزيون انترناسيونال</span><span id="txt-header-sub">استمارة التسجيل الرسمية</span></div>
    <button type="button" class="lang-btn" id="langToggle" aria-label="تغيير اللغة">🌐 <span id="langLabel">Français</span></button>
  </header>
  <main>
    <section class="form-card">
      <h2 id="txt-form-title">ابدأ خطوتك الأولى الآن</h2><p id="txt-form-subtitle">يرجى إكمال جميع البيانات لتفعيل زر الإرسال</p>
      <form id="registrationForm">
        <div class="form-group"><label for="firstName" id="lbl-firstName">الاسم</label><input type="text" id="firstName" name="firstName" class="form-control" placeholder="أدخل اسمك" autocomplete="given-name" required></div>
        <div class="form-group"><label for="lastName" id="lbl-lastName">اللقب</label><input type="text" id="lastName" name="lastName" class="form-control" placeholder="أدخل لقبك" autocomplete="family-name" required></div>
        <div class="form-group"><label for="phone" id="lbl-phone">رقم الهاتف</label><input type="tel" id="phone" name="phone" class="form-control" placeholder="06XX XX XX XX" autocomplete="tel" inputmode="tel" required></div>
        <div class="form-group"><label for="job" id="lbl-job">ماذا تعمل / المهنة</label><input type="text" id="job" name="profession" class="form-control" placeholder="مثال: مهندس، طالب، تاجر..." autocomplete="organization-title" required></div>
        <button type="submit" id="submitBtn" class="btn-submit" disabled>إرسال البيانات</button>
        <div id="statusMsg" class="status-msg" role="status" aria-live="polite"></div>
      </form>
    </section>
  </main>
  <footer><span id="txt-footer">© 2026 NEW VISION INTERNATIONAL — جميع الحقوق محفوظة.</span></footer>
  <script>
    const form = document.getElementById('registrationForm');
    const submitBtn = document.getElementById('submitBtn');
    const inputs = [...form.querySelectorAll('.form-control')];
    const statusMsg = document.getElementById('statusMsg');
    const langToggle = document.getElementById('langToggle');
    const langLabel = document.getElementById('langLabel');
    const translations = {
      ar:{dir:'rtl',lang:'ar',headerTitle:'نيوفيزيون انترناسيونال',headerSub:'استمارة التسجيل الرسمية',formTitle:'ابدأ خطوتك الأولى الآن',formSubtitle:'يرجى إكمال جميع البيانات لتفعيل زر الإرسال',firstName:'الاسم',phFirstName:'أدخل اسمك',lastName:'اللقب',phLastName:'أدخل لقبك',phone:'رقم الهاتف',phPhone:'06XX XX XX XX',job:'ماذا تعمل / المهنة',phJob:'مثال: مهندس، طالب، تاجر...',submit:'إرسال البيانات',sending:'جاري الإرسال...',success:'✓ تم إرسال معلوماتك بنجاح إلى N-Vision International!',error:'حدث خطأ أثناء الإرسال، يرجى المحاولة لاحقاً.',footer:'© 2026 NEW VISION INTERNATIONAL — جميع الحقوق محفوظة.',btnLang:'Français'},
      fr:{dir:'ltr',lang:'fr',headerTitle:'N-VISION INTERNATIONAL',headerSub:'Formulaire d’inscription officiel',formTitle:'Faites votre premier pas maintenant',formSubtitle:'Veuillez remplir tous les champs pour activer le bouton',firstName:'Prénom',phFirstName:'Entrez votre prénom',lastName:'Nom',phLastName:'Entrez votre nom',phone:'Numéro de téléphone',phPhone:'06XX XX XX XX',job:'Profession / Occupation',phJob:'Ex. : ingénieur, étudiant, commerçant...',submit:'Envoyer les données',sending:'Envoi en cours...',success:'✓ Vos informations ont été envoyées avec succès à N-Vision International !',error:'Une erreur est survenue. Veuillez réessayer plus tard.',footer:'© 2026 NEW VISION INTERNATIONAL — Tous droits réservés.',btnLang:'العربية'}
    };
    let currentLang='ar';
    function setLanguage(lang){
      currentLang=lang;const t=translations[lang];document.documentElement.lang=t.lang;document.documentElement.dir=t.dir;
      document.getElementById('txt-header-title').textContent=t.headerTitle;document.getElementById('txt-header-sub').textContent=t.headerSub;
      document.getElementById('txt-form-title').textContent=t.formTitle;document.getElementById('txt-form-subtitle').textContent=t.formSubtitle;
      document.getElementById('lbl-firstName').textContent=t.firstName;document.getElementById('firstName').placeholder=t.phFirstName;
      document.getElementById('lbl-lastName').textContent=t.lastName;document.getElementById('lastName').placeholder=t.phLastName;
      document.getElementById('lbl-phone').textContent=t.phone;document.getElementById('phone').placeholder=t.phPhone;
      document.getElementById('lbl-job').textContent=t.job;document.getElementById('job').placeholder=t.phJob;
      document.getElementById('txt-footer').textContent=t.footer;langLabel.textContent=t.btnLang;
      if(!submitBtn.dataset.sending)submitBtn.textContent=t.submit;
    }
    function checkInputs(){submitBtn.disabled=!form.checkValidity()||inputs.some(input=>!input.value.trim());}
    function showStatus(type,message){statusMsg.className=`status-msg ${type}`;statusMsg.textContent=message;}
    langToggle.addEventListener('click',()=>setLanguage(currentLang==='ar'?'fr':'ar'));
    inputs.forEach(input=>input.addEventListener('input',()=>{statusMsg.className='status-msg';statusMsg.textContent='';checkInputs();}));
    form.addEventListener('submit',async event=>{
      event.preventDefault();if(!form.checkValidity()){form.reportValidity();return;}
      const t=translations[currentLang];submitBtn.disabled=true;submitBtn.dataset.sending='true';submitBtn.textContent=t.sending;statusMsg.className='status-msg';statusMsg.textContent='';
      try{
        const response=await fetch('https://formspree.io/f/xnppzzrb',{method:'POST',body:new FormData(form),headers:{Accept:'application/json'}});
        if(!response.ok)throw new Error('Form submission failed');
        showStatus('success',t.success);form.reset();
      }catch(error){showStatus('error',t.error);}
      finally{delete submitBtn.dataset.sending;submitBtn.textContent=translations[currentLang].submit;checkInputs();}
    });
    setLanguage('ar');checkInputs();
  </script>
</body>
</html>
