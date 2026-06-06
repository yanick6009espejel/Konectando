<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portafolio Konecta</title>
<style>
/* Estilos Globales */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 0;
    color: #333;
    line-height: 1.6;
    scroll-behavior: smooth; /* Desplazamiento suave entre secciones */
}

/* Colores de Konecta (inspirados en las imágenes) */
:root {
    --color-cover: #d4e1f5; /* Azul muy claro de fondo */
    --color-yanick: #1a6d71; /* Teal */
    --color-noe: #888c8f; /* Grey */
    --color-priscila: #c38489; /* Dusty Rose */
    --color-linda: #b26a2e; /* Terracotta Orange */
    --color-levi: #8e2b3f; /* Burgundy Wine */
    --color-waaza: #f0f0f0; /* White/Light Grey */
    --color-text-on-dark: #fff;
    --color-text-on-light: #333;
}

/* Contenedor principal de 'páginas' */
.portfolio-container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

/* Estilo de cada 'página' / sección */
.portfolio-page {
    min-height: 100vh; /* Cada página ocupa el alto de la pantalla */
    padding: 40px;
    margin-bottom: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    background-color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: center; /* Centrar contenido verticalmente */
}

/* Títulos */
h1 { font-size: 3em; margin-bottom: 10px; }
h2 { font-size: 2.2em; margin-top: 30px; margin-bottom: 15px; text-align: center;}
h3 { font-size: 1.5em; margin-top: 20px; margin-bottom: 5px; color: #555;}

/* Párrafos */
p { font-size: 1.1em; margin-bottom: 20px; }
.subtitle { font-style: italic; color: #777; font-size: 1.2em; margin-bottom: 30px; text-align: center; }

/* Estilos Específicos */

/* Página 1: PORTADA */
.page-cover {
    background-color: var(--color-cover);
    text-align: center;
}
.page-cover h1 { color: #2a3f5f; }
.page-cover .logo-placeholder { font-size: 4em; color: #2a3f5f; margin-bottom: 20px; } /* Simulación de logo */

/* Página 2: QUIÉNES SOMOS (Equipo) */
.page-about-team {
    background-color: #f9f9f9;
}
.team-intro { text-align: center; max-width: 800px; margin: 0 auto; }

/* Grid de Miembros del Equipo */
.team-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
    margin-top: 40px;
}

.team-member {
    background: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    text-align: center;
    border-top: 5px solid; /* Borde de color para cada uno */
    transition: transform 0.3s ease;
}
.team-member:hover { transform: translateY(-5px); }
.team-member img {
    max-width: 150px;
    height: auto;
    border-radius: 50%; /* Imagen circular */
    margin-bottom: 15px;
}
.team-member h3 { margin-top: 10px; }
.team-member p.role { font-weight: bold; margin-bottom: 10px; }
.team-member p.bio { font-size: 0.95em; color: #666; text-align: left; }

/* Colores de borde para cada miembro */
.yanick { border-top-color: var(--color-yanick); }
.noe { border-top-color: var(--color-noe); }
.priscila { border-top-color: var(--color-priscila); }
.linda { border-top-color: var(--color-linda); }
.levi { border-top-color: var(--color-levi); }
.waaza { border-top-color: var(--color-noe); } /* El Waaza usa gris por simplicidad */
.supernova { border-top-color: #2a3f5f; } /* Supernova usa azul de portada */

/* Página 3: ENLACE Y STAFF */
.page-staff {
    background-color: #fff;
    text-align: center;
}
.supernova-detail {
    max-width: 700px;
    margin: 30px auto;
    padding: 20px;
    background: #f1f6ff;
    border-radius: 8px;
}
.supernova-detail p { font-weight: bold; }

/* Página 4: CONTACTO */
.page-contact {
    background-color: #fff;
    text-align: center;
}
.contact-info {
    font-size: 1.2em;
    margin-top: 30px;
}
.contact-info p { margin-bottom: 15px; }

/* Navegación Sencilla */
.nav-dots {
    position: fixed;
    right: 20px;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    gap: 10px;
}
.nav-dots a {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #ccc;
    text-decoration: none;
    transition: background-color 0.3s ease;
}
.nav-dots a:hover, .nav-dots a.active {
    background-color: #2a3f5f;
}

</style>
</head>
<body>

<!-- Navegación de puntos fija -->
<div class="nav-dots">
<a href="#cover" class="active" title="Portada"></a>
<a href="#about-team" title="Quiénes Somos"></a>
<a href="#staff" title="Enlace y Staff"></a>
<a href="#contact" title="Contacto"></a>
</div>

<div class="portfolio-container">

<!-- PÁGINA 1: PORTADA -->
<section id="cover" class="portfolio-page page-cover">
    <div class="logo-placeholder">K</div> <!-- Simulación de logo -->
    <h1>Konecta</h1>
    <p class="subtitle">Acompañamiento, Sanación y Claridad Existencial</p>
    <p>Un equipo multidisciplinario dedicado a tu bienestar integral.</p>
    <a href="#about-team" style="text-decoration: none; color: #2a3f5f; font-weight: bold; border: 2px solid #2a3f5f; padding: 10px 20px; border-radius: 5px; margin-top: 20px; display: inline-block;">Conocer al Equipo</a>
</section>

<!-- PÁGINA 2: QUIÉNES SOMOS (Individual y Equipo) -->
<section id="about-team" class="portfolio-page page-about-team">
    <h2>Quiénes Somos</h2>
    <p class="subtitle">Conoce a los profesionales de Konecta</p>

    <div class="team-grid">

        <!-- Yanick -->
        <div class="team-member yanick">
            <img src="image_2.png" alt="Yanick">
            <h3>Yanick</h3>
            <p class="role">Neurobiología y Optimización Conductual</p>
            <p class="bio">Arquitecto del sistema clínico, centrado en la funcionalidad neuropsicológica y la intervención directa sobre la química cerebral.</p>
        </div>

        <!-- Noé -->
        <div class="team-member noe">
            <img src="image_5.png" alt="Noé">
            <h3>Noé</h3>
            <p class="role">Medicina Tradicional y Chamanismo</p>
            <p class="bio">Atención a la dimensión espiritual. Aborda lo que trasciende la ciencia convencional con rigor diagnóstico psicosocial.</p>
        </div>

        <!-- Priscila -->
        <div class="team-member priscila">
            <img src="image_0.png" alt="Priscila">
            <h3>Priscila</h3>
            <p class="role">Acompañamiento y Claridad Existencial</p>
            <p class="bio">Dedicada a proporcionar tranquilidad y entendimiento profundo sobre los procesos de vida, adaptando metodologías espirituales o científicas.</p>
        </div>

        <!-- Linda -->
        <div class="team-member linda">
            <img src="image_4.png" alt="Linda">
            <h3>Linda</h3>
            <p class="role">Reestructuración Psicoespiritual</p>
            <p class="bio">Transformación estructural del individuo para desmantelar dependencias y heridas de la infancia, exigiendo compromiso absoluto.</p>
        </div>

        <!-- Levi -->
        <div class="team-member levi">
            <img src="image_3.png" alt="Levi">
            <h3>Levi</h3>
            <p class="role">Sanación Integral y Encuentro Personal</p>
            <p class="bio">Facilita el retorno del individuo hacia su esencia, enfocándose en la sanación emocional y el amor propio con un enfoque personalizado.</p>
        </div>

        <!-- El Waaza -->
        <div class="team-member waaza">
            <img src="image_1.png" alt="El Waaza">
            <h3>El Waaza</h3>
            <p class="role">Intervención Estratégica y Cambio Humano</p>
            <p class="bio">Articulador táctico que descifra si el propósito de la consulta es la escucha, orientación o reestructuración profunda.</p>
        </div>

    </div>
</section>

<!-- PÁGINA 3: ENLACE Y STAFF -->
<section id="staff" class="portfolio-page page-staff">
    <h2>Enlace y Staff del Equipo</h2>
    <p class="subtitle">La fuerza operativa detrás de Konecta</p>
    
    <p>En Konecta, la eficiencia operativa y la coordinación son fundamentales. Para garantizar la fluidez de nuestros eventos y la conexión directa entre el equipo y el público, contamos con roles de enlace especializados.</p>

    <div class="supernova-detail">
        <img src="image_6.png" alt="Supernova" style="max-width: 150px; border-radius: 50%; margin-bottom: 20px;">
        <h3>super.nova</h3>
        <p>Nuestro enlace vital para eventos.</p>
        <p style="color: #555; font-weight: normal; max-width: 500px; margin: 0 auto;">Coordinador clave que asegura el éxito de cada intervención. super.nova es responsable de la conducción, locación y el enlace para eventos de Konecta.</p>
    </div>

    <p style="margin-top: 30px;">Nuestro equipo de staff trabaja incansablemente para que los profesionales puedan centrarse en lo más importante: <strong>tú</strong>.</p>
</section>

<!-- PÁGINA 4: CONTRA-PORTADA Y CONTACTO -->
<section id="contact" class="portfolio-page page-contact">
    <h2>Konecta</h2>
    <p class="subtitle">Estamos listos para escucharte</p>
    
    <p>Si sientes que es el momento de iniciar tu proceso de sanación, optimización o búsqueda de claridad, nuestro equipo multidisciplinario está aquí para acompañarte. Cada historia es única, y nuestra respuesta también lo será.</p>

    <div class="contact-info">
        <h3>Contacta con nosotros</h3>
        <p><strong>Teléfono/WhatsApp:</strong> +XX XXX XXX XXXX</p>
        <p><strong>Email:</strong> info@konecta-bienestar.com</p>
        <p><strong>Dirección (Atención Presencial):</strong> Calle Armonía #123, Ciudad de México.</p>
        <p><strong>Encuéntranos en Redes:</strong> @KonectaBienestar</p>
    </div>

    <p style="margin-top: 50px; font-size: 0.9em; color: #999;">© 2023 Konecta - Todos los derechos reservados.<br>
    Un enfoque integral para la vida funcional.</p>
</section>

</div>

<script>
// Script sencillo para marcar el punto de navegación activo
window.addEventListener('scroll', () => {
    let current = '';
    const sections = document.querySelectorAll('.portfolio-page');
    const navDots = document.querySelectorAll('.nav-dots a');

    sections.forEach(section => {
        const sectionTop = section.offsetTop;
        const sectionHeight = section.clientHeight;
        if (pageYOffset >= (sectionTop - sectionHeight / 3)) {
            current = section.getAttribute('id');
        }
    });

    navDots.forEach(dot => {
        dot.classList.remove('active');
        if (dot.getAttribute('href') === `#${current}`) {
            dot.classList.add('active');
        }
    });
});
</script>

</body>
</html>
# Konectando
