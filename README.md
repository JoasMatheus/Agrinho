# Agrinho
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Agro Forte • Futuro Sustentável</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    background:#7ec850;
    color:#2d2d2d;
    font-family:'Poppins', sans-serif;
    overflow-x:hidden;
}

/* ===== BARRA SUPERIOR ===== */

header{
    background:#6b3f1f;
    border-bottom:6px solid #3d210e;
    position:fixed;
    width:100%;
    top:0;
    z-index:999;
    box-shadow:0 4px 0 #2c1608;
}

.menu{
    width:90%;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 0;
}

.logo{
    font-family:'Press Start 2P', cursive;
    color:#ffe680;
    font-size:14px;
}

nav a{
    color:#fff4c7;
    text-decoration:none;
    margin-left:25px;
    font-weight:600;
    transition:0.3s;
}

nav a:hover{
    color:#ffe680;
}

/* ===== HERO ===== */

.hero{
    height:100vh;

    background:
    linear-gradient(rgba(0,0,0,0.35), rgba(0,0,0,0.35)),
    url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1600&q=80');

    background-size:cover;
    background-position:center;

    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.hero-box{
    background:#fff4c7;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    padding:50px;
    max-width:900px;
    border-radius:10px;
}

.hero h1{
    font-family:'Press Start 2P', cursive;
    font-size:2.4rem;
    color:#4b7f28;
    margin-bottom:30px;
    line-height:1.5;
}

.hero p{
    font-size:1.1rem;
    margin-bottom:30px;
    color:#4d3b2f;
}

.btn{
    display:inline-block;
    background:#4b7f28;
    color:white;
    text-decoration:none;
    padding:16px 35px;
    border-radius:8px;
    border:4px solid #2d4f18;
    font-weight:600;
    transition:0.2s;
}

.btn:hover{
    transform:translateY(-4px);
    background:#5f9c34;
}

/* ===== SEÇÕES ===== */

section{
    padding:100px 10%;
}

.titulo{
    text-align:center;
    margin-bottom:60px;
}

.titulo h2{
    font-family:'Press Start 2P', cursive;
    font-size:1.5rem;
    color:#fff4c7;
    margin-bottom:25px;
    text-shadow:3px 3px #3d210e;
}

.titulo p{
    color:white;
    max-width:700px;
    margin:auto;
}

/* ===== SOBRE ===== */

.sobre{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.sobre img{
    width:100%;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    border-radius:10px;
}

.sobre-texto{
    background:#fff4c7;
    padding:40px;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    border-radius:10px;
}

.sobre-texto h3{
    font-family:'Press Start 2P', cursive;
    font-size:1rem;
    margin-bottom:25px;
    color:#4b7f28;
}

.sobre-texto p{
    margin-bottom:20px;
}

/* ===== CARDS ===== */

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(250px, 1fr));
    gap:30px;
}

.card{
    background:#fff4c7;
    padding:35px;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    border-radius:10px;
    transition:0.3s;
}

.card:hover{
    transform:translateY(-8px);
}

.card h3{
    color:#4b7f28;
    margin-bottom:20px;
    font-family:'Press Start 2P', cursive;
    font-size:0.9rem;
    line-height:1.6;
}

/* ===== IMPACTO ===== */

.impacto{
    background:#4b7f28;
    border-top:8px solid #2d4f18;
    border-bottom:8px solid #2d4f18;
}

.impacto-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(220px,1fr));
    gap:30px;
    text-align:center;
}

.impacto-item{
    background:#fff4c7;
    padding:40px 20px;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    border-radius:10px;
}

.impacto-item h2{
    font-family:'Press Start 2P', cursive;
    color:#4b7f28;
    font-size:1.8rem;
    margin-bottom:20px;
}

/* ===== GALERIA ===== */

.galeria{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(300px, 1fr));
    gap:20px;
}

.galeria img{
    width:100%;
    height:250px;
    object-fit:cover;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    border-radius:10px;
}

/* ===== CONTATO ===== */

.contato-box{
    background:#fff4c7;
    padding:50px;
    border:8px solid #6b3f1f;
    box-shadow:0 8px 0 #3d210e;
    border-radius:10px;
    max-width:700px;
    margin:auto;
}

form{
    display:flex;
    flex-direction:column;
    gap:20px;
}

input,
textarea{
    padding:16px;
    border:4px solid #6b3f1f;
    border-radius:8px;
    background:#fffdf2;
    font-size:1rem;
}

textarea{
    resize:none;
    height:150px;
}

button{
    border:none;
    cursor:pointer;
}

/* ===== FOOTER ===== */

footer{
    background:#6b3f1f;
    color:#fff4c7;
    text-align:center;
    padding:30px;
    border-top:6px solid #3d210e;
}

/* ===== RESPONSIVO ===== */

@media(max-width:900px){

    .hero h1{
        font-size:1.5rem;
    }

    .sobre{
        grid-template-columns:1fr;
    }

    .menu{
        flex-direction:column;
        gap:20px;
    }

    nav a{
        margin:0 10px;
    }

}

</style>
</head>

<body>

<!-- MENU -->

<header>

<div class="menu">

<div class="logo">
AGRO PIXEL
</div>

<nav>
<a href="#inicio">Início</a>
<a href="#sobre">Sobre</a>
<a href="#solucoes">Soluções</a>
<a href="#impacto">Impacto</a>
<a href="#contato">Contato</a>
</nav>

</div>

</header>

<!-- HERO -->

<section class="hero" id="inicio">

<div class="hero-box">

<h1>
AGRO FORTE,<br>
FUTURO SUSTENTÁVEL
</h1>

<p>
Cultivar alimentos, proteger a natureza e construir um futuro melhor.
Inspirado na estética acolhedora de Stardew Valley, este projeto mostra
como tecnologia, agricultura e meio ambiente podem trabalhar juntos.
</p>

<a href="#sobre" class="btn">
Explorar Fazenda
</a>

</div>

</section>

<!-- SOBRE -->

<section id="sobre">

<div class="titulo">

<h2>
VIDA NO CAMPO
</h2>

<p>
A sustentabilidade transforma pequenas ações em grandes resultados.
</p>

</div>

<div class="sobre">

<img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?auto=format&fit=crop&w=1200&q=80">

<div class="sobre-texto">

<h3>
PLANTAR COM RESPONSABILIDADE
</h3>

<p>
Assim como em Stardew Valley, o equilíbrio da fazenda depende do cuidado
com a terra, da preservação das florestas e do respeito aos ciclos naturais.
</p>

<p>
A agricultura sustentável promove produtividade sem destruir os recursos
naturais, garantindo alimentos saudáveis e um futuro mais verde.
</p>

<a href="#" class="btn">
Conhecer Projeto
</a>

</div>

</div>

</section>

<!-- SOLUÇÕES -->

<section id="solucoes">

<div class="titulo">

<h2>
SOLUÇÕES VERDES
</h2>

<p>
Tecnologia e consciência ambiental trabalhando lado a lado.
</p>

</div>

<div class="cards">

<div class="card">

<h3>
🌱 SOLO VIVO
</h3>

<p>
Práticas regenerativas recuperam nutrientes e fortalecem a biodiversidade.
</p>

</div>

<div class="card">

<h3>
💧 ÁGUA LIMPA
</h3>

<p>
Sistemas inteligentes evitam desperdícios e melhoram a irrigação.
</p>

</div>

<div class="card">

<h3>
🚜 TECNOLOGIA
</h3>

<p>
Sensores, drones e monitoramento digital ajudam produtores rurais.
</p>

</div>

<div class="card">

<h3>
☀ ENERGIA LIMPA
</h3>

<p>
Fontes renováveis reduzem impactos ambientais e custos agrícolas.
</p>

</div>

</div>

</section>

<!-- IMPACTO -->

<section class="impacto" id="impacto">

<div class="titulo">

<h2>
IMPACTO POSITIVO
</h2>

<p>
Pequenas atitudes criam grandes colheitas para o futuro.
</p>

</div>

<div class="impacto-grid">

<div class="impacto-item">
<h2>70%</h2>
<p>Menos desperdício de água</p>
</div>

<div class="impacto-item">
<h2>45%</h2>
<p>Maior eficiência agrícola</p>
</div>

<div class="impacto-item">
<h2>100%</h2>
<p>Compromisso sustentável</p>
</div>

<div class="impacto-item">
<h2>+500</h2>
<p>Famílias beneficiadas</p>
</div>

</div>

</section>

<!-- GALERIA -->

<section>

<div class="titulo">

<h2>
NATUREZA & COLHEITAS
</h2>

<p>
A beleza do campo inspira um futuro mais sustentável.
</p>

</div>

<div class="galeria">

<img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?auto=format&fit=crop&w=1200&q=80">

<img src="https://images.unsplash.com/photo-1472396961693-142e6e269027?auto=format&fit=crop&w=1200&q=80">

<img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1200&q=80">

</div>

</section>

<!-- CONTATO -->

<section id="contato">

<div class="titulo">

<h2>
FALE COM A FAZENDA
</h2>

<p>
Participe dessa jornada por um agro mais sustentável.
</p>

</div>

<div class="contato-box">

<form>

<input type="text" placeholder="Seu nome">

<input type="email" placeholder="Seu e-mail">

<textarea placeholder="Digite sua mensagem"></textarea>

<button class="btn">
Enviar Carta
</button>

</form>

</div>

</section>

<!-- FOOTER -->

<footer>

<p>
© 2026 • Agro Forte • Inspirado na estética pixelada de Stardew Valley
</p>

</footer>

</body>
</html>
