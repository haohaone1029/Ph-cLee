
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Phúc Lee | Profile</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: 'Segoe UI', sans-serif;
      background: black;
      overflow-x: hidden;
      color: #fff;
    }

    canvas#galaxy {
      position: fixed;
      top: 0;
      left: 0;
      z-index: 0;
    }

    .container {
      position: relative;
      z-index: 2;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 20px;
    }

    .avatar {
      width: 160px;
      height: 160px;
      border-radius: 50%;
      border: 4px solid cyan;
      box-shadow: 0 0 30px cyan;
      margin-bottom: 20px;
      transition: transform 0.3s ease;
    }

    .avatar:hover {
      transform: scale(1.05);
    }

    h1 {
      font-size: 2.8rem;
      color: cyan;
      text-shadow: 0 0 10px cyan;
      margin: 0;
    }

    h2 {
      font-size: 1.2rem;
      color: #aaa;
      margin: 10px 0 30px;
    }

    .social {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
      margin-bottom: 30px;
    }

    .social a {
      padding: 10px 20px;
      background-color: transparent;
      border: 2px solid cyan;
      border-radius: 30px;
      color: cyan;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
      box-shadow: 0 0 10px cyan;
    }

    .social a:hover {
      background-color: cyan;
      color: black;
      box-shadow: 0 0 20px cyan;
    }

    .tagline {
      margin-top: 20px;
      font-style: italic;
      font-size: 1.1rem;
      color: #b3ffff;
      min-height: 24px;
    }

    .skills, .projects {
      margin-top: 40px;
      max-width: 600px;
      text-align: left;
    }

    .skills h3, .projects h3 {
      color: cyan;
      margin-bottom: 10px;
      text-align: center;
    }

    .skills ul, .projects ul {
      list-style: none;
      padding: 0;
    }

    .skills li, .projects li {
      background: rgba(0, 255, 255, 0.1);
      padding: 8px 15px;
      margin: 5px 0;
      border-left: 4px solid cyan;
      border-radius: 6px;
    }

    .projects a {
      color: #00ffff;
      text-decoration: none;
    }

    .projects a:hover {
      text-decoration: underline;
    }

    #toggleMusicBtn {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: cyan;
      color: black;
      border: none;
      border-radius: 30px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 0 10px cyan;
    }

    #toggleMusicBtn:hover {
      box-shadow: 0 0 20px cyan;
    }

    #clock {
      margin-top: 15px;
      font-size: 1.2rem;
      color: #0ff;
      text-shadow: 0 0 5px #0ff;
    }

    /* Footer ảnh */
    .footer-images {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 30px;
      margin-bottom: 15px;
      gap: 25px;
    }

    .footer-images img {
      border-radius: 12px;
      box-shadow: 0 0 20px cyan;
      transition: transform 0.3s ease;
      cursor: pointer;
    }

    .footer-images img:hover {
      transform: scale(1.05);
    }

    .footer-images .small-images {
      display: flex;
      gap: 25px;
      justify-content: center;
      width: 100%;
      max-width: 650px;
    }

    .footer-images .large-image {
      max-width: 300px;
      width: 100%;
    }

    .footer-images .small-images img {
      max-width: 150px;
      width: 100%;
      box-shadow: 0 0 15px cyan;
    }

    /* Chủ quyền cuối trang */
    .footer-copyright {
      margin-top: 15px;
      font-weight: bold;
      font-size: 1.1rem;
      color: #33ffff;
      text-shadow: 0 0 10px #33ffff;
      user-select: none;
    }
  </style>
</head>
<body>
  <canvas id="galaxy"></canvas>

  <div class="container">
    <img class="avatar" src="https://i.imgur.com/EWKPif6.jpeg" alt="Mun Avatar" />
    <h1>🟢 Phúc Lee</h1>
    <h2>💻 THU SLL PET - CANDY GAG</h2>

    <div class="social">
      <a href="https://www.facebook.com/phuc.channel.372#" target="_blank">📘 Facebook</a>
      <a href="https://zalo.me/0938605298" target="_blank">📱 Zalo</a>
      <a href="https://www.tiktok.com/@phuclees?is_from_webapp=1&sender_device=pc" target="_blank">🎵 TikTok</a>
    </div>

    <button id="toggleMusicBtn">🔊 Tắt nhạc</button>

    <p class="tagline" id="typewriter"></p>
    <p id="clock"></p>

    <div class="skills">
      <h3>Kỹ năng nổi bật</h3>
      <ul>
        <li>✅ UY TÍN CHẤT LƯỢNG</li>
        <li>✅ GDTG - ĐT PHÍ RẺ</li>
        <li>✅ SEO & Tối ưu hóa Web</li>
        <li>✅ KĨ NĂNG KINH DOANH CAO</li>
      </ul>
    </div>

    <div class="projects">
      <h3>Các dịch vụ nổi bật</h3>
      <ul>
        <li><a href="#">🔹 THU MUA ACC GAME</a></li>
        <li><a href="#">🔹 SELL UGPHONE</a></li>
        <li><a href="#">🔹 SELL DỊCH VỤ ROBLOX - CÀY THUÊ</a></li>
      </ul>
    </div>

    <div class="footer-images">
      <img class="large-image" src="https://i.imgur.com/mfvIwkp.png" alt="Ảnh lớn chủ quyền" />
      <div class="small-images">
      </div>
    </div>

    <div class="footer-copyright">
       © 2025 Chủ quyền Website By TRẦN HÀO | DARKSTACK TEAM
    </div>

  </div>

  <!-- Nhạc nền ẩn bằng thẻ audio -->
  <audio id="backgroundAudio" loop autoplay preload="auto" style="display:none">
    <source src="https://pomf2.lain.la/f/l5nv41b6.mp3" type="audio/mpeg" />
    Trình duyệt của bạn không hỗ trợ phần tử audio.
  </audio>

  <script>
    // Galaxy stars
    const canvas = document.getElementById('galaxy');
    const ctx = canvas.getContext('2d');
    let stars = [];

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }

    function createStars(count) {
      stars = [];
      for (let i = 0; i < count; i++) {
        stars.push({
          x: Math.random() * canvas.width,
          y: Math.random() * canvas.height,
          radius: Math.random() * 1.5,
          velocity: Math.random() * 0.5 + 0.2
        });
      }
    }

    function drawStars() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      ctx.fillStyle = "#ffffff";
      stars.forEach(star => {
        ctx.beginPath();
        ctx.arc(star.x, star.y, star.radius, 0, Math.PI * 2);
        ctx.fill();
      });
    }

    function animateStars() {
      stars.forEach(star => {
        star.y += star.velocity;
        if (star.y > canvas.height) {
          star.y = 0;
          star.x = Math.random() * canvas.width;
        }
      });
      drawStars();
      requestAnimationFrame(animateStars);
    }

    window.addEventListener('resize', () => {
      resizeCanvas();
      createStars(150);
    });

    resizeCanvas();
    createStars(150);
    animateStars();

    // Quotes
    const quotes = [
      "Uy tín làm nên thương hiệu.",
      "Nơi khẳng định chính mình.",
      "Không cần nổi tiếng, chỉ cần uy tín.",
      "Tiền không tự chảy, phải biết cày và xoay."
    ];
    function rotateQuotes() {
      const quote = quotes[Math.floor(Math.random() * quotes.length)];
      document.getElementById("typewriter").innerHTML = quote;
    }
    setInterval(rotateQuotes, 5000);
    rotateQuotes();

    // Clock
    function updateClock() {
      const now = new Date();
      const h = now.getHours().toString().padStart(2, "0");
      const m = now.getMinutes().toString().padStart(2, "0");
      const s = now.getSeconds().toString().padStart(2, "0");
      document.getElementById("clock").textContent = `🕒 ${h}:${m}:${s}`;
    }
    setInterval(updateClock, 1000);
    updateClock();

    // Music toggle
    const audio = document.getElementById('backgroundAudio');
    const btn = document.getElementById('toggleMusicBtn');
    btn.addEventListener('click', () => {
      if (audio.paused) {
        audio.play();
        btn.textContent = '🔊 Tắt nhạc';
      } else {
        audio.pause();
        btn.textContent = '🔈 Bật nhạc';
      }
    });
  </script>
</body>
</html>
