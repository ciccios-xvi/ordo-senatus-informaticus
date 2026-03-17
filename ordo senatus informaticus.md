<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Senato Accademico di Informatica</title>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;700&family=Fauna+One&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #c5a059;
            --deep-red: #800020;
            --dark-bg: #0a0a0a;
            --parchment: #f4e4bc;
            --text-light: #e0e0e0;
        }

        body {
            font-family: 'Fauna One', serif;
            background-color: var(--dark-bg);
            color: var(--text-light);
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.8)), url('tua-immagine.jpg');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border-bottom: 3px solid var(--gold);
            text-align: center;
        }

        header h1 {
            font-family: 'Cinzel', serif;
            font-size: 4rem;
            margin: 0;
            color: var(--gold);
            letter-spacing: 8px;
            text-shadow: 3px 3px 15px rgba(0,0,0,0.9);
        }

        .motto {
            font-style: italic;
            color: var(--gold);
            letter-spacing: 2px;
            margin-top: 10px;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* SEZIONE MANIFESTO */
        .manifesto {
            background-color: #1a1a1a;
            border: 2px solid var(--gold);
            padding: 40px;
            margin-bottom: 60px;
            position: relative;
            box-shadow: 0 0 30px rgba(197, 160, 89, 0.2);
        }

        .manifesto h2 {
            font-family: 'Cinzel', serif;
            color: var(--gold);
            text-align: center;
            font-size: 2rem;
            margin-top: 0;
        }

        .manifesto-text {
            font-size: 1.1rem;
            text-align: justify;
            color: #ccc;
            columns: 2;
            column-gap: 40px;
            column-rule: 1px solid var(--gold);
        }

        /* GRIGLIA SENATORI */
        .senators-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .senator-card {
            background: linear-gradient(145deg, #1a1a1a, #252525);
            border-top: 4px solid var(--gold);
            padding: 30px;
            text-align: center;
            border-radius: 0 0 10px 10px;
        }

        .senator-card h3 {
            font-family: 'Cinzel', serif;
            color: var(--gold);
            margin-bottom: 5px;
            font-size: 1.5rem;
        }

        .role-title {
            color: var(--deep-red);
            font-weight: bold;
            text-transform: uppercase;
            font-size: 0.85rem;
            letter-spacing: 1px;
            margin-bottom: 15px;
            display: block;
        }

        .role-desc {
            font-size: 0.95rem;
            min-height: 80px;
            margin-bottom: 20px;
        }

        .upload-btn {
            background-color: transparent;
            border: 1px solid var(--gold);
            color: var(--gold);
            padding: 10px 20px;
            cursor: pointer;
            transition: 0.3s;
            text-transform: uppercase;
            font-weight: bold;
        }

        .upload-btn:hover {
            background-color: var(--gold);
            color: black;
        }

        footer {
            text-align: center;
            padding: 50px;
            border-top: 1px solid #333;
            font-family: 'Cinzel', serif;
            color: #555;
        }

        @media (max-width: 768px) {
            .manifesto-text { columns: 1; }
            header h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>

<header>
    <h1>SENATO</h1>
    <div class="motto">Collaborazione • Disciplina • Progresso</div>
</header>

<div class="container">
    
    <section class="manifesto">
        <h2>Atto Solenne di Fondazione</h2>
        <div class="manifesto-text">
            <p>Con il presente atto si proclama solennemente la fondazione del consesso denominato <strong>Senato</strong>, istituzione collegiale istituita con lo scopo di favorire la cooperazione intellettuale e l’assistenza reciproca nell’ambito dell’informatica. Il Senato nasce quale organo di coordinamento volto a promuovere ordine metodologico e rigore logico.</p>
            <p>In un contesto accademico caratterizzato da richieste esigenti, tale assemblea si pone quale baluardo di collaborazione, affinché nessun senatore sia lasciato solo nell’affrontare le difficoltà dello studio. L’azione congiunta consente di affrontare con sicurezza la "tirannia" delle eccessive difficoltà imposte dalle verifiche.</p>
        </div>
    </section>

    <div class="senators-grid">
        
        <div class="senator-card">
            <h3>Fogliana</h3>
            <span class="role-title">Redattore degli Elaborati</span>
            <p class="role-desc">Incaricato della formulazione e strutturazione iniziale degli esercizi. Predispone le fondamenta del lavoro collettivo.</p>
            <input type="file" id="upload-fogliana" hidden>
            <button class="upload-btn" onclick="document.getElementById('upload-fogliana').click()">Deposita Documento</button>
        </div>

        <div class="senator-card">
            <h3>Poma</h3>
            <span class="role-title">Garante della Correttezza</span>
            <p class="role-desc">Verificatore tecnico e metodologico. Esamina la validità logica e assicura il rispetto degli standard di precisione.</p>
            <input type="file" id="upload-poma" hidden>
            <button class="upload-btn" onclick="document.getElementById('upload-poma').click()">Deposita Documento</button>
        </div>

        <div class="senator-card">
            <h3>Savalli</h3>
            <span class="role-title">Revisore e Correttore</span>
            <p class="role-desc">Perfeziona e apporta i miglioramenti finali ai contenuti, elevando la qualità complessiva dell'opera del Senato.</p>
            <input type="file" id="upload-savalli" hidden>
            <button class="upload-btn" onclick="document.getElementById('upload-savalli').click()">Deposita Documento</button>
        </div>

    </div>
</div>

<footer>
    AD MAIORA • SENATO ACCADEMICO INFORMATICO • 2026
</footer>

</body>
</html>
