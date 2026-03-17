# Projeto-em-CSS
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Agora | Grécia Antiga</title>
    <style>
        :root {
            --gold: #d4af37;
            --marble: #f5f5f5;
            --deep-blue: #0a192f;
            --text-gray: #a8b2d1;
            --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--deep-blue);
            color: var(--marble);
            line-height: 1.6;
            overflow-x: hidden;
        }

        header {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(rgba(10, 25, 47, 0.8), rgba(10, 25, 47, 0.8)), 
                        url('https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?auto=format&fit=crop&q=80&w=1000');
            background-size: cover;
            border-bottom: 4px solid var(--gold);
        }

        header h1 {
            font-size: clamp(3rem, 10vw, 5rem);
            text-transform: uppercase;
            letter-spacing: 10px;
            color: var(--gold);
            text-shadow: 2px 2px 10px rgba(0,0,0,0.5);
        }

        header p {
            font-style: italic;
            color: var(--text-gray);
            font-size: 1.2rem;
        }

        .container {
            max-width: 1100px;
            margin: -50px auto 50px;
            padding: 20px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .card {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(212, 175, 55, 0.2);
            padding: 30px;
            border-radius: 12px;
            transition: var(--transition);
            position: relative;
            cursor: pointer;
        }

        .card:hover {
            transform: translateY(-10px);
            background: rgba(255, 255, 255, 0.1);
            border-color: var(--gold);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }

        .card h2 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
        }

        .card h2::before {
            content: '🏛️';
            margin-right: 10px;
            font-size: 1.2rem;
        }

        .card p {
            color: var(--text-gray);
            font-size: 0.95rem;
        }

        .badge {
            display: inline-block;
            background: var(--gold);
            color: var(--deep-blue);
            padding: 2px 10px;
            border-radius: 20px;
            font-weight: bold;
            font-size: 0.7rem;
            margin-bottom: 10px;
            text-transform: uppercase;
        }

        footer {
            text-align: center;
            padding: 40px;
            color: var(--text-gray);
            font-size: 0.8rem;
            border-top: 1px solid rgba(255,255,255,0.1);
        }

        /* Responsive adjustments */
        @media (max-width: 600px) {
            header h1 { font-size: 2.5rem; }
            .container { margin-top: 20px; }
        }
    </style>
</head>
<body>

    <header>
        <h1>The Agora</h1>
        <p>Onde o pensamento ocidental começou a ser codificado.</p>
    </header>

    <div class="container">
        <div class="grid">
            <div class="card">
                <span class="badge">Mindset</span>
                <h2>Filosofia</h2>
                <p>Esqueça o "porque sim". Sócrates, Platão e Aristóteles hackearam a mente humana para entender a ética, a política e a própria realidade.</p>
            </div>

            <div class="card">
                <span class="badge">Lore</span>
                <h2>Mitologia</h2>
                <p>Deuses com falhas humanas, heróis em jornadas épicas e monstros que representam nossos medos. É o roteiro original de todo o entretenimento moderno.</p>
            </div>

            <div class="card">
                <span class="badge">Social Tech</span>
                <h2>Democracia</h2>
                <p>A primeira versão de um sistema operacional político onde o "usuário" (cidadão) tinha voz ativa na gestão da cidade-estado.</p>
            </div>

            <div class="card">
                <span class="badge">Engineering</span>
                <h2>Ciência & Arte</h2>
                <p>Da geometria de Pitágoras à proporção áurea na arquitetura. Eles não apenas construíram prédios; eles descobriram as leis do design universal.</p>
            </div>
        </div>
    </div>

    <footer>
        &copy; 2026 Hellenic Hub - Criado para mentes curiosas.
    </footer>

</body>
</html>
