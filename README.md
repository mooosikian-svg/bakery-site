# bakery-site
Здесь вы найдёте проверенные рецепты хлеба, пирогов, печенья и круассанов. От простого дрожжевого теста до сложных французских десертов. Каждый рецепт сопровождается пошаговыми фото и советами.
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Домашняя пекарня — выпечка с любовью</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Шапка -->
    <header>
        <div class="container">
            <h1 class="logo">🍞 Домашняя пекарня</h1>
            <nav>
                <a href="#">Главная</a>
                <a href="#">Рецепты</a>
                <a href="#">О нас</a>
            </nav>
        </div>
    </header>

    <!-- Герой-секция (первый экран) -->
    <section class="hero">
        <div class="container">
            <h2>Печём с душой</h2>
            <p>Проверенные рецепты хлеба, пирогов и круассанов<br> для домашнего уюта</p>
            <a href="#" class="btn">Смотреть рецепты</a>
        </div>
    </section>

    <!-- Карточки рецептов -->
    <section class="recipes">
        <div class="container">
            <h3 class="section-title">Популярные рецепты</h3>
            <div class="card-grid">
                <div class="card">
                    <img src="photo-placeholder.jpg" alt="Яблочный пирог">
                    <h4>Яблочный пирог</h4>
                    <p>Нежный, с кислинкой и корицей</p>
                </div>
                <div class="card">
                    <img src="photo-placeholder.jpg" alt="Хлеб на закваске">
                    <h4>Хлеб на закваске</h4>
                    <p>Хрустящая корочка, воздушный мякиш</p>
                </div>
                <div class="card">
                    <img src="photo-placeholder.jpg" alt="Круассаны">
                    <h4>Круассаны</h4>
                    <p>Слоёные, масляные, французские</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Подвал -->
    <footer>
        <div class="container">
            <p>© 2025 Домашняя пекарня. Печём с любовью ❤️</p>
        </div>
    </footer>

</body>
</html>
/* Подключаем шрифты */
@import url('https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,600&family=Playfair+Display:wght@700&display=swap');

/* Цветовая палитра */
:root {
    --vanilla: #FFF9F4;
    --chocolate: #3E2A24;
    --caramel: #D98A5B;
    --sage: #A3B18A;
    --cream: #EADBC6;
}

/* Общие стили */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', sans-serif;
    background-color: var(--vanilla);
    color: var(--chocolate);
    line-height: 1.5;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Шапка */
header {
    background-color: var(--vanilla);
    border-bottom: 2px solid var(--cream);
    padding: 20px 0;
    position: sticky;
    top: 0;
    background-color: rgba(255, 249, 244, 0.95);
    backdrop-filter: blur(5px);
}

header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

.logo {
    font-family: 'Playfair Display', serif;
    font-size: 28px;
    color: var(--caramel);
}

nav a {
    color: var(--chocolate);
    text-decoration: none;
    margin-left: 30px;
    font-weight: 500;
    transition: color 0.3s;
}

nav a:hover {
    color: var(--caramel);
}

/* Герой-секция */
.hero {
    background: linear-gradient(135deg, var(--vanilla) 0%, var(--cream) 100%);
    text-align: center;
    padding: 100px 20px;
    border-radius: 0 0 40px 40px;
    margin-bottom: 60px;
}

.hero h2 {
    font-family: 'Playfair Display', serif;
    font-size: 48px;
    margin-bottom: 20px;
}

.hero p {
    font-size: 18px;
    margin-bottom: 30px;
    color: #5a3a32;
}

.btn {
    display: inline-block;
    background-color: var(--caramel);
    color: white;
    padding: 12px 32px;
    border-radius: 40px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    box-shadow: 0 4px 10px rgba(0,0,0,0.05);
}

.btn:hover {
    background-color: #c27a4e;
    transform: translateY(-2px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.1);
}

/* Секция рецептов */
.section-title {
    font-family: 'Playfair Display', serif;
    font-size: 36px;
    text-align: center;
    margin-bottom: 40px;
}

.card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
    margin-bottom: 60px;
}

.card {
    background: white;
    border-radius: 24px;
    overflow: hidden;
    box-shadow: 0 8px 20px rgba(0,0,0,0.05);
    transition: all 0.3s ease;
    text-align: center;
    padding-bottom: 20px;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
}

.card img {
    width: 100%;
    height: 220px;
    object-fit: cover;
    display: block;
}

.card h4 {
    font-size: 22px;
    margin: 15px 0 8px;
    color: var(--caramel);
}

.card p {
    padding: 0 15px;
    color: #5a3a32;
}

/* Подвал */
footer {
    background-color: var(--chocolate);
    color: var(--cream);
    text-align: center;
    padding: 30px 0;
    margin-top: 40px;
    border-radius: 30px 30px 0 0;
}

/* Адаптивность (мобильные) */
@media (max-width: 768px) {
    .hero h2 {
        font-size: 32px;
    }
    
    .section-title {
        font-size: 28px;
    }
    
    header .container {
        flex-direction: column;
        gap: 15px;
    }
    
    nav a {
        margin: 0 15px;
    }
}
apple-pie.jpg
sourdough-bread.jpg
croissant.jpg
