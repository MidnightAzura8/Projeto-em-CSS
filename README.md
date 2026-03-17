<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Agora | Ancient Greece</title>
    <style>
        /* Resets de CSS para evitar bugs de margem */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', 'Segoe UI', sans-serif;
        }

        :root {
            --gold: #d4af37;
            --deep-blue: #050c18;
            --card-bg: rgba(255, 255, 255, 0.03);
            --text-main: #e0e0e0;
        }

        body {
            background-color: var(--deep-blue);
            color: var(--text-main);
            overflow-x: hidden;
        }

        /* Hero Section ajustada */
        header {
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
            background: linear-gradient(rgba(5, 12, 24, 0.7), rgba(5, 12, 24, 0.9)), 
                        url('https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?q=80&w=2000') no-repeat center center;
            background-size: cover;
            border-bottom: 2px solid var(--gold);
        }

        header h1 {
            font-size: clamp(2.5rem, 8vw, 5rem);
            color: var(--gold);
            text-transform: uppercase;
            letter-spacing: 8px;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.2rem;
            color: #888;
            max-width: 600px;
        }

        /* Grid de Conteúdo */
        .container {
            max-width: 1200px;
            margin: -60px auto 60px;
            padding: 0 20px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .card {
            background: var(--card-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(212, 175, 55, 0.1);
            padding: 30px;
            border-radius: 15px;
            transition: all 0.4s ease;
        }

        .card:hover {
            transform: translateY(-12px);
            border-color: var(--gold);
            box-shadow: 0 15px 35px rgba(0,0,0,0.5);
        }

        .badge {
            background: var(--gold);
            color: #000;
            padding: 4px 12px;
            font-size: 0.7rem;
            font-weight: 900;
            border-radius: 4px;
            text-transform: uppercase;
            margin-bottom: 20px;
            display: inline-block;
        }

        .card h2 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.6rem;
        }

        .card p {
            color: #aaa;
            font-size: 0.95rem;
            line-height: 1.6;
        }

        footer {
            text-align: center;
            padding: 40px;
            opacity: 0.5;
            font-size: 0.8rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>THE AGORA</h1>
        <p>A "Deep Web" do conhecimento clássico. Onde os hackers da lógica criaram o mundo moderno.</p>
    </header>

    <div class="container">
        <div class="grid">
            <div class="card">
                <span class="badge">Legacy</span>
                <h2>Filosofia</h2>
                <p>Sócrates não tinha Wi-Fi, mas conectou mentes. Ele ensinou que questionar é o código-fonte da sabedoria.</p>
            </div>
            <div class="card">
                <span class="badge">Lore</span>
                <h2>Mitologia</h2>
                <p>Deuses, monstros e heróis. A mitologia grega é o Universo Cinematográfico original, mas com muito mais drama.</p>
            </div>
            <div class="card">
                <span class="badge">Politics</span>
                <h2>Democracia</h2>
                <p>O primeiro sistema operacional social. Direto de Atenas: um governo feito de cidadãos para cidadãos.</p>
            </div>
        </div>
    </div>

    <footer>
        &copy; 2026 - Debugando a História
    </footer>

</body>
</html>
