# ProTech-Support-
ProTech Support  es una aplicación educativa de escuela técnica virtual destinada a estudiantes. La plataforma ofrecerá clases virtuales, horarios, materias, materiales de estudio, actividades, avisos y recursos de apoyo para acompañar a los estudiantes en su aprendizaje.


<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>ProTech Support</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f2f5f8;
            color: #17202a;
        }

        header {
            background: #102a43;
            color: white;
            padding: 25px 18px;
            text-align: center;
        }

        header h1 {
            font-size: 30px;
            margin-bottom: 8px;
        }

        header p {
            font-size: 15px;
        }

        nav {
            background: white;
            padding: 12px;
            display: flex;
            gap: 8px;
            overflow-x: auto;
            position: sticky;
            top: 0;
            z-index: 10;
            box-shadow: 0 2px 8px rgba(0,0,0,0.08);
        }

        nav button {
            border: none;
            background: #e8eef5;
            padding: 11px 15px;
            border-radius: 20px;
            white-space: nowrap;
            cursor: pointer;
            font-weight: bold;
        }

        nav button:hover {
            background: #cddbea;
        }

        main {
            max-width: 900px;
            margin: auto;
            padding: 20px;
        }

        section {
            margin-bottom: 30px;
        }

        .welcome {
            background: white;
            border-radius: 18px;
            padding: 25px;
            margin-bottom: 25px;
            box-shadow: 0 3px 12px rgba(0,0,0,0.08);
        }

        .welcome h2 {
            margin-bottom: 10px;
        }

        .welcome p {
            line-height: 1.6;
            color: #52606d;
        }

        .button {
            display: inline-block;
            margin-top: 18px;
            background: #1976d2;
            color: white;
            text-decoration: none;
            padding: 13px 20px;
            border-radius: 10px;
            border: none;
            cursor: pointer;
            font-weight: bold;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 15px;
        }

        .card {
            background: white;
            border-radius: 16px;
            padding: 20px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.07);
        }

        .card .icon {
            font-size: 32px;
            margin-bottom: 10px;
        }

        .card h3 {
            margin-bottom: 7px;
        }

        .card p {
            color: #627d98;
            font-size: 14px;
            line-height: 1.5;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.07);
        }

        th, td {
            padding: 14px 10px;
            text-align: left;
            border-bottom: 1px solid #e5e7eb;
        }

        th {
            background: #102a43;
            color: white;
        }

        .price {
            font-size: 25px;
            font-weight: bold;
            margin: 12px 0;
        }

        .price-card {
            text-align: center;
        }

        footer {
            background: #102a43;
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 30px;
        }

        @media (max-width: 500px) {
            header h1 {
                font-size: 25px;
            }

            main {
                padding: 14px;
            }

            th, td {
                padding: 10px 7px;
                font-size: 13px;
            }
        }
    </style>
</head>

<body>

<header>
    <h1>⚙️ ProTech Support</h1>
    <p>Escuela Técnica Virtual</p>
</header>

<nav>
    <button onclick="irA('inicio')">Inicio</button>
    <button onclick="irA('materias')">Materias</button>
    <button onclick="irA('horarios')">Horarios</button>
    <button onclick="irA('clases')">Clases</button>
    <button onclick="irA('precios')">Precios</button>
    <button onclick="irA('contacto')">Contacto</button>
</nav>

<main>

    <section id="inicio" class="welcome">
        <h2>Bienvenido/a a ProTech Support 👋</h2>

        <p>
            Somos una escuela técnica virtual pensada para acompañar
            a estudiantes de primer año en sus materias y actividades.
        </p>

        <p style="margin-top:10px;">
            Encontrá tus materias, horarios, clases virtuales,
            materiales y actividades en un solo lugar.
        </p>

        <button class="button" onclick="irA('materias')">
            Ver materias
        </button>
    </section>


    <section id="materias">
        <h2>📚 Materias</h2>

        <div class="grid">

            <div class="card">
                <div class="icon">📐</div>
                <h3>Dibujo Técnico</h3>
                <p>
                    Vistas, perspectivas, escalas, acotación
                    y representación técnica.
                </p>
            </div>

            <div class="card">
                <div class="icon">➗</div>
                <h3>Matemática</h3>
                <p>
                    Números, operaciones, ecuaciones,
                    geometría y resolución de problemas.
                </p>
            </div>

            <div class="card">
                <div class="icon">🇬🇧</div>
                <h3>Inglés Técnico</h3>
                <p>
                    Vocabulario técnico, lectura y
                    comprensión de textos.
                </p>
            </div>

            <div class="card">
                <div class="icon">⚡</div>
                <h3>Electricidad</h3>
                <p>
                    Conceptos básicos de electricidad,
                    circuitos y seguridad.
                </p>
            </div>

            <div class="card">
                <div class="icon">💻</div>
                <h3>Informática</h3>
                <p>
                    Herramientas digitales y conceptos
                    básicos de tecnología.
                </p>
            </div>

            <div class="card">
                <div class="icon">🔧</div>
                <h3>Taller Técnico</h3>
                <p>
                    Introducción a herramientas,
                    materiales y procesos técnicos.
                </p>
            </div>

        </div>
    </section>


    <section id="horarios">
        <h2>🗓️ Horarios</h2>

        <table>
            <tr>
                <th>Día</th>
                <th>Materia</th>
                <th>Horario</th>
            </tr>

            <tr>
                <td>Lunes</td>
                <td>Matemática</td>
                <td>18:00 - 19:00</td>
            </tr>

            <tr>
                <td>Martes</td>
                <td>Dibujo Técnico</td>
                <td>18:00 - 19:00</td>
            </tr>

            <tr>
                <td>Miércoles</td>
                <td>Inglés Técnico</td>
                <td>18:00 - 19:00</td>
            </tr>

            <tr>
                <td>Jueves</td>
                <td>Electricidad</td>
                <td>18:00 - 19:00</td>
            </tr>

            <tr>
                <td>Viernes</td>
                <td>Taller Técnico</td>
                <td>18:00 - 19:00</td>
            </tr>
        </table>
    </section>


    <section id="clases">
        <h2>🎥 Clases virtuales</h2>

        <div class="card">
            <h3>Próxima clase</h3>

            <p style="margin-top:10px;">
                Matemática - Primer Año
            </p>

            <p style="margin-top:5px;">
                Lunes - 18:00 hs
            </p>

            <button class="button" onclick="alert('El enlace de la clase se agregará próximamente.')">
                Entrar a clase
            </button>
        </div>
    </section>


    <section id="precios">
        <h2>💰 Planes</h2>

        <div class="grid">

            <div class="card price-card">
                <h3>Clase individual</h3>
                <div class="price">$2.000</div>
                <p>Una clase virtual de una materia.</p>
                <button class="button" onclick="contactar()">
                    Consultar
                </button>
            </div>

            <div class="card price-card">
                <h3>Pack mensual</h3>
                <div class="price">$7.000</div>
                <p>Cuatro clases durante el mes.</p>
                <button class="button" onclick="contactar()">
                    Consultar
                </button>
            </div>

            <div class="card price-card">
                <h3>Plan completo</h3>
                <div class="price">$12.000</div>
                <p>Acceso a todas las materias.</p>
                <button class="button" onclick="contactar()">
                    Consultar
                </button>
            </div>

        </div>
    </section>


    <section id="contacto">
        <h2>📞 Contacto</h2>

        <div class="card">
            <h3>¿Querés inscribirte?</h3>

            <p style="margin-top:10px;">
                Comunicate con ProTech Support para consultar
                disponibilidad, horarios e inscripción.
            </p>

            <button class="button" onclick="contactar()">
                Contactar
            </button>
        </div>
    </section>

</main>


<footer>
    <p>⚙️ ProTech Support</p>
    <p style="margin-top:7px;">
        Escuela Técnica Virtual
    </p>
</footer>


<script>

    function irA(id) {
        document.getElementById(id).scrollIntoView({
            behavior: "smooth"
        });
    }

    function contactar() {
        alert("Acá vamos a colocar tu número de WhatsApp cuando terminemos la aplicación.");
    }

</script>

</body>
</html>
