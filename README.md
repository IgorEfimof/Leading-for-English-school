<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Онлайн-школа английского</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background: #333;
            color: #fff;
            padding: 15px;
            text-align: center;
        }
        .banner {
            width: 100%;
            height: 300px;
            background: url('banner.jpg') no-repeat center center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2em;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
        }
        .nav-links {
            list-style: none;
            display: flex;
        }
        .nav-links li {
            margin: 0 10px;
        }
        .nav-links a {
            color: white;
            text-decoration: none;
        }
        .hero {
            text-align: center;
            padding: 50px;
            background: #f4f4f4;
        }
        form {
            display: flex;
            flex-direction: column;
            max-width: 400px;
            margin: auto;
        }
        input, textarea {
            margin-bottom: 10px;
            padding: 10px;
            font-size: 16px;
        }
        button {
            padding: 10px;
            background: #333;
            color: white;
            border: none;
            cursor: pointer;
        }
        @media (max-width: 768px) {
            .nav-links {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">English School</div>
            <ul class="nav-links">
                <li><a href="#about">О нас</a></li>
                <li><a href="#courses">Курсы</a></li>
                <li><a href="#reviews">Отзывы</a></li>
                <li><a href="#contact">Контакты</a></li>
            </ul>
        </nav>
    </header>
    
    <div class="banner">Добро пожаловать в нашу онлайн-школу!</div>
    
    <section class="hero">
        <h1>Изучайте английский легко и эффективно</h1>
        <p>Запишитесь на бесплатный пробный урок</p>
        <button onclick="scrollToForm()">Записаться</button>
    </section>
    
    <section id="about" class="about">
        <h2>О нас</h2>
        <p>Мы предлагаем качественные онлайн-курсы английского для всех уровней с опытными преподавателями.</p>
    </section>
    
    <section id="courses" class="courses">
        <h2>Наши курсы</h2>
        <ul>
            <li>Английский для начинающих</li>
            <li>Разговорный английский</li>
            <li>Подготовка к экзаменам</li>
            <li>Бизнес-английский</li>
        </ul>
    </section>
    
    <section id="reviews" class="reviews">
        <h2>Отзывы наших студентов</h2>
        <p>Прекрасные курсы! Очень понравилось обучение. - Анна</p>
        <p>Отличный преподавательский состав и удобный формат. - Иван</p>
    </section>
    
    <section id="contact" class="contact">
        <h2>Свяжитесь с нами</h2>
        <form id="contact-form">
            <input type="text" name="name" placeholder="Ваше имя" required>
            <input type="email" name="email" placeholder="Ваш email" required>
            <textarea name="message" placeholder="Ваше сообщение" required></textarea>
            <button type="submit">Отправить</button>
        </form>
    </section>
    
    <footer>
        <p>&copy; 2025 Онлайн-школа английского. Все права защищены.</p>
    </footer>
    
    <script>
        function scrollToForm() {
            document.getElementById('contact-form').scrollIntoView({ behavior: 'smooth' });
        }
    </script>
</body>
</html>
