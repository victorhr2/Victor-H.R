<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Víctor H.R. - Regulación de Mercados</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary-color: #1e3a8a; /* Azul oscuro elegante */
            --secondary-color: #3b82f6; /* Azul brillante */
            --bg-color: #f3f4f6; /* Gris muy claro */
            --card-bg: #ffffff;
            --text-main: #1f2937;
            --text-muted: #6b7280;
            --accent: #f59e0b; /* Acento ámbar/dorado */
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 40px 20px;
        }

        .container {
            width: 100%;
            max-width: 900px;
            background: var(--card-bg);
            border-radius: 16px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            overflow: hidden;
            border: 1px solid #e5e7eb;
        }

        /* Encabezado con Gradiente */
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 50px 40px;
            text-align: center;
            position: relative;
        }

        header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 6px;
            background-color: var(--accent);
        }

        h1 {
            font-size: 36px;
            margin-bottom: 10px;
            letter-spacing: 1px;
            font-weight: 800;
        }

        .subtitle {
            font-size: 18px;
            font-weight: 400;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }

        /* Contenedor de las tarjetas */
        .content {
            padding: 40px;
        }

        .intro-text {
            text-align: center;
            margin-bottom: 40px;
            font-size: 16px;
            color: var(--text-muted);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        /* Tarjetas de Control */
        .card {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 30px 25px;
            text-decoration: none;
            color: var(--text-main);
            border: 1px solid #e5e7eb;
            box-shadow: 0 4px 6px rgba(0,0,0,0.04);
            transition: all 0.3s ease;
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            overflow: hidden;
        }

        .card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background-color: var(--secondary-color);
            transform: scaleX(0);
            transition: transform 0.3s ease;
            transform-origin: left;
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
            border-color: #d1d5db;
        }

        .card:hover::before {
            transform: scaleX(1);
        }

        .card-icon {
            font-size: 40px;
            color: var(--secondary-color);
            margin-bottom: 20px;
        }

        .card h2 {
            font-size: 20px;
            margin-bottom: 12px;
            color: var(--primary-color);
        }

        .card p {
            font-size: 14px;
            color: var(--text-muted);
            margin-bottom: 20px;
            flex-grow: 1;
        }

        .btn-start {
            display: inline-block;
            padding: 10px 20px;
            background-color: var(--bg-color);
            color: var(--secondary-color);
            border-radius: 6px;
            font-weight: 600;
            font-size: 14px;
            transition: all 0.2s;
            border: 1px solid transparent;
        }

        .card:hover .btn-start {
            background-color: var(--secondary-color);
            color: white;
        }

        /* Pie de página */
        footer {
            text-align: center;
            padding: 30px;
            background-color: #f8fafc;
            border-top: 1px solid #e5e7eb;
            color: var(--text-muted);
            font-size: 14px;
        }

        footer i {
            color: var(--accent);
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Víctor H.R.</h1>
            <div class="subtitle">Portal Académico de Controles Interactivos<br>Cátedra: Regulación de Mercados</div>
        </header>

        <div class="content">
            <p class="intro-text">Selecciona un módulo para acceder a las evaluaciones prácticas. Cada control está calibrado para responderse con tiempo límite.</p>
            
            <div class="grid">
                <!-- Tarjeta 1 -->
                <a href="Control_Unidad_1_Alumnos.html" class="card">
                    <i class="fas fa-chart-line card-icon"></i>
                    <h2>Unidad I</h2>
                    <p>Fundamentos, Geometría de Mercado, Costos y Doctrina Regulatoria.</p>
                    <span class="btn-start">Iniciar Control <i class="fas fa-arrow-right"></i></span>
                </a>
                
                <!-- Tarjeta 2 -->
                <a href="Control_Unidad_2_Alumnos_Diseño_UI.html" class="card">
                    <i class="fas fa-leaf card-icon"></i>
                    <h2>Unidad II</h2>
                    <p>Externalidades, Tarificación, Monopolios Naturales y Jurisprudencia Ambiental.</p>
                    <span class="btn-start">Iniciar Control <i class="fas fa-arrow-right"></i></span>
                </a>

                <!-- Tarjeta 3 -->
                <a href="Control_Unidad_3_Alumnos.html" class="card">
                    <i class="fas fa-balance-scale card-icon"></i>
                    <h2>Unidad III</h2>
                    <p>Libre Competencia, Cárteles, Mercado Relevante y Disuasión de Becker.</p>
                    <span class="btn-start">Iniciar Control <i class="fas fa-arrow-right"></i></span>
                </a>
            </div>
        </div>

        <footer>
            <p>Diseñado y desarrollado por <strong>Víctor Ignacio Huaiquián Rebolledo</strong> <i class="fas fa-code"></i> 2026</p>
        </footer>
    </div>

</body>
</html>
