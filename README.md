<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Corazón de Mezcal – Banquetes Guelaguetza</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: 'Segoe UI', sans-serif;
}

body{
    background:#f5f1eb;
    color:#333;
}

/* NAV */
nav{
    position:fixed;
    width:100%;
    background:#000;
    color:#fff;
    padding:15px;
    display:flex;
    justify-content:space-between;
    z-index:1000;
}

nav a{
    color:#fff;
    margin-left:15px;
    text-decoration:none;
}

/* HERO */
.hero{
    height:100vh;
    background:url('https://images.unsplash.com/photo-1555244162-803834f70033') center/cover;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    color:#fff;
}

.hero h1{
    font-size:3rem;
}

.hero p{
    margin:20px 0;
}

.btn{
    padding:12px 25px;
    margin:5px;
    background:#c0392b;
    color:#fff;
    border:none;
    cursor:pointer;
}

/* SECTIONS */
section{
    padding:80px 20px;
    text-align:center;
}

.cards{
    display:flex;
    flex-wrap:wrap;
    gap:20px;
    justify-content:center;
}

.card{
    background:#fff;
    padding:20px;
    width:300px;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,0.1);
}

/* GALERIA */
.gallery img{
    width:100%;
    max-width:300px;
    margin:10px;
    border-radius:10px;
}

/* FOOTER */
footer{
    background:#000;
    color:#fff;
    padding:20px;
}

/* WHATSAPP */
.whatsapp{
    position:fixed;
    bottom:20px;
    right:20px;
    background:#25d366;
    color:#fff;
    padding:15px;
    border-radius:50%;
    font-size:20px;
    text-decoration:none;
}

/* RESPONSIVE */
@media(max-width:768px){
    .hero h1{
        font-size:2rem;
    }
}
</style>
</head>

<body>

<nav>
    <div>Corazón de Mezcal</div>
    <div>
        <a href="#paquetes">Paquetes</a>
        <a href="#menu">Menú</a>
        <a href="#contacto">Contacto</a>
    </div>
</nav>

<div class="hero">
    <div>
        <h1>Vive la Guelaguetza en tu Evento</h1>
        <p>Tradición, cultura y el espíritu del agave en cada montaje</p>
        <button class="btn" onclick="scrollToSection('contacto')">Reservar ahora</button>
        <button class="btn" onclick="scrollToSection('paquetes')">Ver paquetes</button>
        <p>@corazonde_mezcal</p>
    </div>
</div>

<section>
    <h2>Sobre Nosotros</h2>
    <p>Un viaje sensorial inspirado en la Guelaguetza que une gastronomía, mezcal y tradición oaxaqueña.</p>
</section>

<section>
    <h2>Experiencias</h2>
    <div class="cards">
        <div class="card">Bodas temáticas</div>
        <div class="card">Eventos privados</div>
        <div class="card">Corporativos</div>
        <div class="card">Show Guelaguetza</div>
    </div>
</section>

<section id="paquetes">
    <h2>Paquetes</h2>
    <div class="cards">
        <div class="card">
            <h3>Calenda</h3>
            <p>$800</p>
            <p>Buffet + bebida + música</p>
        </div>
        <div class="card">
            <h3>Flor de Piña</h3>
            <p>$1,300</p>
            <p>3 tiempos + mezcal + baile</p>
        </div>
        <div class="card">
            <h3>Monte Albán</h3>
            <p>$1,950</p>
            <p>4 tiempos + barra libre + show</p>
        </div>
    </div>
</section>

<section id="menu">
    <h2>Menú</h2>
    <p>Mole negro · Tlayudas · Tasajo · Memelas · Alegrías · Nicuatole</p>
</section>

<section class="gallery">
    <h2>Galería</h2>
    <img src="https://images.unsplash.com/photo-1528605248644-14dd04022da1">
    <img src="https://images.unsplash.com/photo-1544025162-d76694265947">
    <img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
</section>

<section>
    <h2>Testimonios</h2>
    <p>"Una experiencia increíble, totalmente diferente"</p>
    <p>"El mejor evento que hemos tenido"</p>
    <p>"Elegancia y tradición en un solo lugar"</p>
</section>

<section id="contacto">
    <h2>Reservaciones</h2>
    <p>Tel: 9532765754</p>
    <form>
        <input type="text" placeholder="Nombre"><br><br>
        <input type="text" placeholder="Tipo de evento"><br><br>
        <input type="date"><br><br>
        <input type="number" placeholder="Personas"><br><br>
        <button class="btn">Enviar</button>
    </form>
</section>

<footer>
    <p>© Corazón de Mezcal</p>
    <p>Síguenos en Instagram: @corazonde_mezcal</p>
</footer>

<a class="whatsapp" href="https://wa.me/529532765754" target="_blank">💬</a>

<script>
function scrollToSection(id){
    document.getElementById(id).scrollIntoView({behavior:'smooth'});
}
</script>

</body>
</html>
