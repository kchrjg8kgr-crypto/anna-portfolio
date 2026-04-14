# anna-portfolio
<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Anna | UGC Creator</title>

<style>
body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  background: #ffffff;
  color: #111;
}

.container {
  width: 90%;
  max-width: 1100px;
  margin: auto;
}

/* HERO */
.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  animation: fadeIn 1.5s ease;
}

h1 {
  font-size: 56px;
  margin: 0;
}

.subtitle {
  font-size: 20px;
  color: #555;
  margin-top: 10px;
}

.btn {
  margin-top: 30px;
  display: inline-block;
  padding: 14px 28px;
  background: #111;
  color: white;
  text-decoration: none;
  transition: 0.3s;
}

.btn:hover {
  background: #333;
}

/* SECTIONS */
section {
  padding: 100px 0;
  opacity: 0;
  transform: translateY(40px);
  transition: 1s;
}

section.visible {
  opacity: 1;
  transform: translateY(0);
}

/* GRID */
.grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.card {
  height: 250px;
  background: #f5f5f5;
  transition: 0.4s;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #aaa;
  font-size: 14px;
}

.card:hover {
  transform: scale(1.03);
}

/* TEXT */
h2 {
  font-size: 32px;
  margin-bottom: 20px;
}

p {
  font-size: 18px;
  color: #555;
  line-height: 1.6;
}

/* FOOTER */
footer {
  text-align: center;
  padding: 60px 0;
  color: #777;
}

/* ANIMATION */
@keyframes fadeIn {
  from {opacity: 0; transform: translateY(30px);}
  to {opacity: 1; transform: translateY(0);}
}
</style>
</head>

<body>

<div class="container hero">
  <h1>Anna — UGC Creator</h1>
  <div class="subtitle">Стильний контент, який продає</div>
  <div class="subtitle">Чехія 🇨🇿 | Україна 🇺🇦</div>
  <a href="#contact" class="btn">Співпраця</a>
</div>

<section class="container">
  <h2>Про мене</h2>
  <p>
    Мене звати Анна — я UGC creator, яка створює естетичний та автентичний контент для брендів.
    Я допомагаю бізнесам виглядати сучасно, викликати довіру та продавати через візуал.
  </p>
</section>

<section class="container">
  <h2>Послуги</h2>
  <p>UGC відео • Lifestyle контент • Рекламні інтеграції • Контент для TikTok та Reels</p>
</section>

<section class="container">
  <h2>Портфоліо</h2>
  <div class="grid">
    <div class="card">Ваше відео</div>
    <div class="card">Ваше відео</div>
    <div class="card">Ваше відео</div>
    <div class="card">Ваше відео</div>
  </div>
</section>

<section class="container">
  <h2>Мій стиль</h2>
  <p>
    Мінімалізм. Естетика. Натуральність.  
    Я створюю контент, який виглядає дорого, але залишається живим і близьким для аудиторії.
    Кожна деталь працює на результат.
  </p>
</section>

<section class="container">
  <h2>Переваги</h2>
  <p>
    • Контент, що продає  
    • Сучасний стиль і тренди  
    • Робота з брендами в Європі  
    • Швидка комунікація та відповідальність  
  </p>
</section>

<section id="contact" class="container">
  <h2>Контакти</h2>
  <p>Instagram: @ugc.form</p>
  <p>Email: your@email.com</p>
</section>

<footer>
  © 2026 Anna UGC Creator
</footer>

<script>
const sections = document.querySelectorAll("section");

window.addEventListener("scroll", () => {
  sections.forEach(sec => {
    const top = sec.getBoundingClientRect().top;
    if (top < window.innerHeight - 100) {
      sec.classList.add("visible");
    }
  });
});
</script>

</body>
</html>
