# portafolio.com
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pau Izquierdo | IT & Marketing</title>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #0f172a;
            --accent: #2563eb;
            --bg: #ffffff;
            --card-bg: #f8fafc;
            --text: #1e293b;
            --text-light: #64748b;
            --transition: all 0.3s ease;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
        }

        /* --- NAVEGACIÓN --- */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 8%;
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo { font-size: 1.4rem; font-weight: 800; color: var(--primary); letter-spacing: -0.5px; }

        .nav-links { display: flex; list-style: none; gap: 2.5rem; }
        .nav-links a { text-decoration: none; color: var(--text); font-weight: 500; transition: var(--transition); }
        .nav-links a:hover { color: var(--accent); }

        /* --- DROPDOWN PROYECTOS --- */
        .dropdown { position: relative; }
        .dropdown-content {
            display: none;
            position: absolute;
            background: white;
            min-width: 180px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            border-radius: 10px;
            top: 100%;
            padding: 0.5rem 0;
            border: 1px solid #f1f5f9;
        }
        .dropdown-content a { padding: 12px 20px; display: block; font-size: 0.9rem; }
        .dropdown-content a:hover { background: #f1f5f9; color: var(--accent); }
        .dropdown:hover .dropdown-content { display: block; }

        /* --- HERO --- */
        .hero {
            padding: 100px 8% 60px;
            text-align: center;
            background: radial-gradient(circle at top right, #f1f5f9, #ffffff);
        }
        .hero h1 { font-size: 2.8rem; color: var(--primary); margin-bottom: 15px; }
        .hero p { color: var(--text-light); font-size: 1.2rem; max-width: 600px; margin: 0 auto; }

        /* --- SECCIÓN EXPERIENCIA --- */
        .experience-section { padding: 40px 8% 100px; }
        .container { max-width: 900px; margin: 0 auto; }

        .job-card {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            border-left: 6px solid var(--accent);
            transition: var(--transition);
        }

        .job-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            flex-wrap: wrap;
            gap: 10px;
        }

        .company-name {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
        }

        .job-tag {
            background: #dbeafe;
            color: var(--accent);
            padding: 6px 16px;
            border-radius: 30px;
            font-size: 0.85rem;
            font-weight: 700;
            text-transform: uppercase;
        }

        .job-list {
            list-style: none;
            margin-top: 20px;
        }

        .job-list li {
            position: relative;
            padding-left: 25px;
            margin-bottom: 12px;
            color: var(--text);
            font-size: 1.05rem;
        }

        .job-list li::before {
            content: "→";
            position: absolute;
            left: 0;
            color: var(--accent);
            font-weight: bold;
        }

        footer { text-align: center; padding: 60px; color: var(--text-light); font-size: 0.9rem; border-top: 1px solid #f1f5f9; }
    </style>
</head>
<body>

<nav>
    <div class="logo">PAU IZQUIERDO</div>
    <ul class="nav-links">
        <li><a href="#">Inicio</a></li>
        <li class="dropdown">
            <a href="#">Proyectos ▾</a>
            <div class="dropdown-content">
                <a href="#">Programación</a>
                <a href="#">Hardware</a>
            </div>
        </li>
        <li><a href="#">Sobre mí</a></li>
        <li><a href="#">Contacto</a></li>
    </ul>
</nav>

<header class="hero">
    <h1>Experiencia Profesional</h1>
    <p>Perfil técnico especializado en gestión de infraestructuras IT y soporte administrativo.</p>
</header>

<section class="experience-section">
    <div class="container">
        
        <div class="job-card">
            <div class="job-header">
                <span class="company-name">Kouten</span>
                <span class="job-tag">Sistemas y Redes</span>
            </div>
            <ul class="job-list">
                <li>Mantenimiento preventivo y correctivo de infraestructuras tecnológicas.</li>
                <li>Gestión y monitorización de redes locales para asegurar la conectividad.</li>
                <li>Instalación de sistemas y configuración de equipamiento IT corporativo.</li>
                <li>Resolución de incidencias técnicas en instalaciones físicas.</li>
            </ul>
        </div>

        <div class="job-card">
            <div class="job-header">
                <span class="company-name">Ocasionagestio</span>
                <span class="job-tag">Administración y Marketing</span>
            </div>
            <ul class="job-list">
                <li>Gestión de tareas administrativas y soporte organizativo interno.</li>
                <li>Desarrollo de acciones de marketing para la promoción de servicios.</li>
                <li>Atención al cliente y gestión de documentación comercial.</li>
                <li>Apoyo en la visibilidad digital y comunicación de la empresa.</li>
            </ul>
        </div>

    </div>
</section>

<footer>
    <p>&copy; 2026 Pau Izquierdo. Diseñado con enfoque en IT & Estrategia.</p>
</footer>

</body>
</html>
