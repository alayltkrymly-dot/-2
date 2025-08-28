
صــدقة جــارية لــــــكسروي محمد   ــوــ   لأمواتنا أجمــعيـــن 2
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  
  <title>صدقة جارية | إهداء للمرحوم كسروي</title>
  <meta name="description" content="صدقة جارية إهداء إلى روح المرحوم كسروي وجميع أموات المسلمين، موقع للاستماع إلى القرآن الكريم كاملاً مع الدعاء للفقيد.">
  <meta name="keywords" content="صدقة جارية, قرآن كريم, المرحوم كسروي, دعاء للميت, استماع للقرآن, موقع ديني">
  <meta name="robots" content="index, follow">

  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: "Tajawal", sans-serif;
      background: #000;
      color: #fff;
      text-align: center;
      overflow-x: hidden;
    }

    /* الخلفية صور متغيرة مع fade */
    body::before {
      content: "";
      position: fixed;
      top:0; left:0; width:100%; height:100%;
      background-size: cover;
      background-position: center;
      z-index: -1;
      animation: bgFade 18s infinite;
      transition: background-image 1s ease-in-out;
    }

    @keyframes bgFade {
      0% { background-image: url("photo1.jpg"); }
      33% { background-image: url("photo2.jpg"); }
      66% { background-image: url("photo3.jpg"); }
      100% { background-image: url("photo1.jpg"); }
    }

    .overlay {
      position: relative;
      z-index: 2;
      padding: 20px;
      background: rgba(0,0,0,0.6);
      border-radius: 12px;
      margin: 40px auto;
      width: 90%;
      max-width: 700px;
    }

    h1 {
      font-size: 2em;
      color: #ffd700;
      margin-bottom: 10px;
      animation: glowText 2s infinite alternate;
    }

    p {
      font-size: 1.2em;
      margin-bottom: 20px;
      animation: glowText 2s infinite alternate;
    }

    @keyframes glowText {
      0% { text-shadow: 0 0 5px #00ffcc, 0 0 10px #00ffcc; }
      50% { text-shadow: 0 0 15px #ffd700, 0 0 25px #ffd700; }
      100% { text-shadow: 0 0 5px #00ffcc, 0 0 10px #00ffcc; }
    }

    .quran-list {
      margin-top: 20px;
    }

    .quran-list button {
      display: block;
      margin: 10px auto;
      padding: 12px 25px;
      background: #00ffcc;
      border: none;
      border-radius: 10px;
      font-size: 1em;
      cursor: pointer;
      transition: 0.3s, box-shadow 1s;
      animation: glowButton 2s infinite alternate;
    }

    @keyframes glowButton {
      0% { box-shadow: 0 0 5px #00ffcc; }
      50% { box-shadow: 0 0 20px #ffd700; }
      100% { box-shadow: 0 0 5px #00ffcc; }
    }

    .quran-list button:hover {
      transform: scale(1.1);
      color: #000;
    }

    /* الفوتر */
    footer {
      position: fixed;
      bottom: 10px;
      width: 100%;
      text-align: center;
      font-size: 1em;
      color: #00ffcc;
      z-index: 2;
    }

    footer a {
      margin: 0 10px;
      display: inline-block;
      transition: transform 0.3s, filter 0.3s;
    }

    footer a img {
      width: 28px;
      height: 28px;
    }

    footer a:hover img {
      transform: scale(1.3);
    }

    /* glow حسب اللون لكل منصة */
    footer a[href*="facebook.com"] img:hover {
      filter: drop-shadow(0 0 6px #1877F2);
    }

    footer a[href*="wa.me"] img:hover {
      filter: drop-shadow(0 0 6px #25D366);
    }

    footer a[href*="instagram.com"] img:hover {
      filter: drop-shadow(0 0 6px #C13584);
    }

    audio {
      margin-top: 15px;
      width: 90%;
      max-width: 500px;
    }

  </style>
</head>
<body>
  <div class="overlay">
    <h1>إهداء إلى روح المرحوم كسروي وجميع أموات المسلمين</h1>
    <p>اللهم اغفر له وارحمه واجعل قبره روضة من رياض الجنة</p>

    <!-- مشغل صوت مع mute أولي -->
    <audio id="player" controls muted>
      <source src="yasin2.mp3" type="audio/mpeg">
      متصفحك لا يدعم تشغيل الصوت
    </audio>

    <!-- أربع أزرار فقط "صدقة جارية" -->
    <div class="quran-list">
      <button onclick="playSurah('fatiha1.mp3')">صدقة جارية</button>
      <button onclick="playSurah('yasin2.mp3')">صدقة جارية</button>
      <button onclick="playSurah('baqara1.mp3')">صدقة جارية</button>
      <button onclick="playSurah('mulk1.mp3')">صدقة جارية</button>
    </div>
  </div>

  <footer>
    أنشئ بواسطة م.محمد رمضان كسروي | تقبل الله هذا العمل وجعله في ميزان حسناتنا
    <br>
    <!-- أيقونات التواصل -->
    <a href="https://www.facebook.com/profile.php?id=100070530433568" target="_blank">
      <img src="https://cdn-icons-png.flaticon.com/512/733/733547.png" alt="Facebook">
    </a>
    <a href="https://wa.me/201157394843" target="_blank">
      <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp">
    </a>
    <a href="https://www.instagram.com/اسم_الحساب/" target="_blank">
      <img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram">
    </a>
  </footer>

  <script>
    const player = document.getElementById("player");
    let firstInteraction = false;

    function playSurah(file) {
      player.src = file;
      player.muted = false; // يشغل الصوت الحقيقي بعد التفاعل
      player.play();
    }

    // لتفعيل الصوت بعد أول تفاعل مع الصفحة
    document.body.addEventListener("click", () => {
      if (!firstInteraction) {
        player.muted = false;
        player.play();
        firstInteraction = true;
      }
    }, { once: true });
  </script>
</body>
</html>
