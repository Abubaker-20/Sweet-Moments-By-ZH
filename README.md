
```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sweet Moments Bey ZH</title>
    <style>
        body { font-family: Arial; margin: 0; padding: 0; }
        .hidden { display: none; }
        header { background: #f8e8e8; padding: 20px; text-align: center; }
        .logo { color: #d85a7f; font-size: 2rem; font-weight: bold; }
        .language-switcher { margin: 15px 0; }
        .language-btn { background: none; border: 1px solid #d85a7f; padding: 5px 15px; margin: 0 5px; border-radius: 20px; cursor: pointer; }
        nav { background: #d85a7f; padding: 15px; }
        nav ul { list-style: none; padding: 0; margin: 0; display: flex; justify-content: center; }
        nav ul li { margin: 0 15px; }
        nav ul li a { color: white; text-decoration: none; }
        .hero { padding: 40px 20px; text-align: center; background: #fff5f7; }
        section { padding: 40px 20px; }
        footer { background: #333; color: white; padding: 20px; text-align: center; }
        .rtl { direction: rtl; }
        .ltr { direction: ltr; }
    </style>
</head>
<body class="rtl">
    <header>
        <div class="logo">Sweet Moments Bey ZH</div>
        <div class="language-switcher">
            <button class="language-btn active" onclick="switchLanguage('ar')">🇸🇦 العربية</button>
            <button class="language-btn" onclick="switchLanguage('de')">🇩🇪 Deutsch</button>
        </div>
    </header>
    
    <nav>
        <ul id="nav-ar">
            <li><a href="#about">عنّا</a></li>
            <li><a href="#products">منتجاتنا</a></li>
            <li><a href="#order">اطلب الآن</a></li>
            <li><a href="#contact">تواصل معنا</a></li>
        </ul>
        <ul id="nav-de" class="hidden">
            <li><a href="#about">Über uns</a></li>
            <li><a href="#products">Unsere Produkte</a></li>
            <li><a href="#order">Jetzt bestellen</a></li>
            <li><a href="#contact">Kontakt</a></li>
        </ul>
    </nav>
    
    <section class="hero">
        <div id="hero-ar">
            <h1>🎂 مرحبًا بكم في Sweet Moments Bey ZH</h1>
            <p>نقدم لكم أجمل اللحظات الحلوة من خلال أشهى أنواع التورتات والمخبوزات</p>
        </div>
        <div id="hero-de" class="hidden">
            <h1>🎂 Willkommen bei Sweet Moments Bey ZH</h1>
            <p>Wir bieten Ihnen süße Momente mit handgemachten Torten und Desserts</p>
        </div>
    </section>
    
    <section id="contact">
        <div id="contact-ar">
            <h2>تواصل معنا</h2>
            <p>واتساب: +41 12 345 6789</p>
        </div>
        <div id="contact-de" class="hidden">
            <h2>Kontakt</h2>
            <p>WhatsApp: +41 12 345 6789</p>
        </div>
    </section>
    
    <footer>
        <div id="footer-ar">© 2023 Sweet Moments Bey ZH</div>
        <div id="footer-de" class="hidden">© 2023 Sweet Moments Bey ZH</div>
    </footer>

    <script>
        function switchLanguage(lang) {
            // Arabic
            if (lang === 'ar') {
                document.body.className = 'rtl';
                document.querySelectorAll('[id$="-ar"]').forEach(el => el.classList.remove('hidden'));
                document.querySelectorAll('[id$="-de"]').forEach(el => el.classList.add('hidden'));
                document.querySelector('.language-btn[onclick*="ar"]').classList.add('active');
                document.querySelector('.language-btn[onclick*="de"]').classList.remove('active');
            }
            // German
            else {
                document.body.className = 'ltr';
                document.querySelectorAll('[id$="-ar"]').forEach(el => el.classList.add('hidden'));
                document.querySelectorAll('[id$="-de"]').forEach(el => el.classList.remove('hidden'));
                document.querySelector('.language-btn[onclick*="ar"]').classList.remove('active');
                document.querySelector('.language-btn[onclick*="de"]').classList.add('active');
            }
        }
    </script>
</body>
</html>
```
   ```html
   <img src="images/cake.jpg" alt="تورتة الشوكولاتة" width="300">
   ```
```css
@media (max-width: 600px) {
    nav ul { flex-direction: column; }
    nav ul li { margin: 5px 0; }
}
```
