<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AsuevsGroup – Umzug & Entrümpelung</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
  function switchLanguage(lang) {
    document.querySelectorAll('[data-lang]').forEach(el => {
      el.style.display = el.dataset.lang === lang ? 'block' : 'none';
    });
    localStorage.setItem('language', lang);
  }
  window.addEventListener('DOMContentLoaded', () => {
    const savedLang = localStorage.getItem('language') || 'de';
    switchLanguage(savedLang);
  });
</script>
  <style>
    .icon-text {
      font-size: 48px;
      line-height: 1;
      margin: 0 auto 1rem;
      animation: float 3s ease-in-out infinite;
    }
    .bulldozer {
      animation: bulldoze 3s ease-in-out infinite;
    }
    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
      100% { transform: translateY(0); }
    }
    @keyframes bulldoze {
      0% { transform: translateX(0); }
      50% { transform: translateX(8px); }
      100% { transform: translateX(0); }
    }
  </style>
</head>
<body class="bg-gray-100 text-gray-900 font-sans transition duration-300" id="body">

  <!-- Language Switch -->
  <div class="flex justify-center items-center gap-4 p-4">
    <button onclick="switchLanguage('de')" class="text-blue-600 font-semibold flex items-center gap-2">
      <img src="https://flagcdn.com/w40/de.png" alt="Deutsch" class="w-5 h-4"> Deutsch
    </button>
    <button onclick="switchLanguage('en')" class="text-blue-600 font-semibold flex items-center gap-2">
      <img src="https://flagcdn.com/w40/gb.png" alt="English" class="w-5 h-4"> English
    </button>
    <button onclick="switchLanguage('ru')" class="text-blue-600 font-semibold flex items-center gap-2">
      <img src="https://flagcdn.com/w40/ru.png" alt="Русский" class="w-5 h-4"> Русский
    </button>
  </div>

  <!-- Header -->
  <header class="bg-white shadow p-6">
    <div class="max-w-6xl mx-auto flex justify-between items-center">
      <div class="flex items-center space-x-4">
        <img src="https://cdn-icons-png.flaticon.com/512/1040/1040230.png" class="w-10 h-10" alt="Logo">
        <h1 class="text-2xl font-bold">AsuevsGroup – Umzug & Entrümpelung</h1>
      </div>
      <div class="space-x-3">
        <a href="mailto:asuevsgroup@gmail.com" class="bg-blue-600 text-white px-4 py-2 rounded-lg hover:bg-blue-700 transition">E-Mail</a>
        <a href="tel:017680584898" class="bg-green-600 text-white px-4 py-2 rounded-lg hover:bg-green-700 transition">Anrufen</a>
      </div>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="py-24">
    <div class="max-w-4xl mx-auto text-center">
      <h2 class="text-5xl font-extrabold mb-4">AsuevsGroup</h2>
      <p data-lang="de" class="text-lg max-w-2xl mx-auto block">Wir sind ein junges, engagiertes Unternehmen mit einem motivierten Team aus ambitionierten, verantwortungsbewussten Fachkräften. Unser Ziel: Umzüge und Entrümpelung einfach, schnell und stressfrei!</p>
      <p data-lang="en" class="text-lg max-w-2xl mx-auto hidden">We are a young, dynamic company with a motivated team of ambitious and responsible workers. Our goal is to make moving and clearing out easy, fast, and stress-free!</p>
      <p data-lang="ru" class="text-lg max-w-2xl mx-auto hidden">Мы — молодая, амбициозная компания с мотивированной и ответственной командой. Наша цель — сделать переезд и уборку лёгкими, быстрыми и без стресса!</p>
    </div>
  </section>

  <!-- Services -->
  <section class="py-12">
    <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-6 text-center">
      <div class="p-6 border rounded-xl shadow bg-white">
        <div class="icon-text">📦</div>
        <h3 class="text-xl font-semibold mb-2 block" data-lang="de">Umzug</h3>
        <h3 class="text-xl font-semibold mb-2 hidden" data-lang="en">Moving</h3>
        <h3 class="text-xl font-semibold mb-2 hidden" data-lang="ru">Переезд</h3>
        <p data-lang="de" class="block">Privat- & Firmenumzüge sicher und effizient.</p>
        <p data-lang="en" class="hidden">Private & business moves – fast and reliable.</p>
        <p data-lang="ru" class="hidden">Частные и коммерческие переезды — быстро и надёжно.</p>
      </div>
      <div class="p-6 border rounded-xl shadow bg-white">
        <div class="icon-text">🚛</div>
        <h3 class="text-xl font-semibold mb-2 block" data-lang="de">Entrümpelung</h3>
        <h3 class="text-xl font-semibold mb-2 hidden" data-lang="en">Clear-out</h3>
        <h3 class="text-xl font-semibold mb-2 hidden" data-lang="ru">Расчистка</h3>
        <p data-lang="de" class="block">Häuser, Wohnungen, Keller & Büros professionell geräumt.</p>
        <p data-lang="en" class="hidden">Houses, flats, basements & offices professionally cleared.</p>
        <p data-lang="ru" class="hidden">Дома, квартиры, подвалы и офисы — профессиональная расчистка.</p>
      </div>
      <div class="p-6 border rounded-xl shadow bg-white">
        <div class="icon-text bulldozer">🛋️</div>
        <h3 class="text-xl font-semibold mb-2 block" data-lang="de">Haushaltsauflösung</h3>
        <h3 class="text-xl font-semibold mb-2 hidden" data-lang="en">House Clearance</h3>
        <h3 class="text-xl font-semibold mb-2 hidden" data-lang="ru">Ликвидация хозяйства</h3>
        <p data-lang="de" class="block">Diskret & zuverlässig – alles aus einer Hand.</p>
        <p data-lang="en" class="hidden">Discrete & reliable – all from one source.</p>
        <p data-lang="ru" class="hidden">Деликатно и надёжно – всё под ключ.</p>
      </div>
    </div>
  </section>

  <!-- Kontaktformular -->
  <section id="kontakt" class="bg-white py-12">
    <div class="max-w-xl mx-auto px-4">
      <h2 class="text-3xl font-bold mb-4 text-center" data-lang="de">Kontaktieren Sie uns</h2>
      <h2 class="text-3xl font-bold mb-4 text-center hidden" data-lang="en">Contact us</h2>
      <h2 class="text-3xl font-bold mb-4 text-center hidden" data-lang="ru">Свяжитесь с нами</h2>
      <form class="grid grid-cols-1 gap-4 bg-gray-50 p-6 rounded-lg shadow">
        <input type="text" placeholder="Name / Имя" class="border p-3 rounded-md" required />
        <input type="email" placeholder="E-Mail" class="border p-3 rounded-md" required />
        <textarea data-lang="de" placeholder="Ihre Nachricht..." rows="4" class="border p-3 rounded-md block" required></textarea>
        <textarea data-lang="en" placeholder="Your message..." rows="4" class="border p-3 rounded-md hidden" required></textarea>
        <textarea data-lang="ru" placeholder="Ваше сообщение..." rows="4" class="border p-3 rounded-md hidden" required></textarea>
        <button type="submit" class="bg-blue-600 text-white py-2 rounded-md hover:bg-blue-700 transition" data-lang="de">Absenden</button>
        <button type="submit" class="bg-blue-600 text-white py-2 rounded-md hover:bg-blue-700 transition hidden" data-lang="en">Send</button>
        <button type="submit" class="bg-blue-600 text-white py-2 rounded-md hover:bg-blue-700 transition hidden" data-lang="ru">Отправить</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-800 text-white py-6 text-sm">
    <div class="max-w-4xl mx-auto flex flex-col md:flex-row justify-between items-center space-y-2 md:space-y-0 px-4">
      <p>&copy; 2025 AsuevsGroup</p>
      <div class="text-center md:text-right">
        <p>Email: asuevsgroup@gmail.com</p>
        <p>Telefon: 0176 80584898, 0176 61256216</p>
      </div>
    </div>
  </footer>

</body>
</html>
