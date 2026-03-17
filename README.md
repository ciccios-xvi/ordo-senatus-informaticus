
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
            --card-bg: #1a1a1a;
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
            height: 60vh;
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

        .container {
            max-width: 1100px;
            margin: -40px auto 60px auto;
            padding: 0 20px;
        }

        .manifesto {
            background-color: var(--card-bg);
            border: 2px solid var(--gold);
            padding: 30px;
            margin-bottom: 50px;
            box-shadow: 0 0 30px rgba(197, 160, 89, 0.1);
        }

        .senators-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 25px;
            margin-bottom: 60px;
        }

        .senator-card {
            background: linear-gradient(145deg, #1a1a1a, #222);
            border-top: 4px solid var(--gold);
            padding: 30px;
            text-align: center;
            border-radius: 0 0 10px 10px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
        }

        .role-title {
            color: var(--deep-red);
            font-weight: bold;
            text-transform: uppercase;
            font-size: 0.8rem;
            display: block;
            margin-bottom: 15px;
        }

        /* Pulsanti Doppi */
        .btn-group {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 20px;
        }

        .btn {
            padding: 10px 15px;
            text-decoration: none;
            font-weight: bold;
            font-size: 0.85rem;
            text-transform: uppercase;
            cursor: pointer;
            transition: 0.3s;
            border: 1px solid var(--gold);
            font-family: 'Cinzel', serif;
        }

        .btn-deposit {
            background: transparent;
            color: var(--gold);
        }

        .btn-folder {
            background: var(--gold);
            color: black;
        }

        .btn:hover {
            filter: brightness(1.2);
            transform: scale(1.02);
        }

        /* Registro */
        .history-section { background: var(--card-bg); padding: 30px; border: 1px solid #333; }
        table { width: 100%; border-collapse: collapse; margin-top: 20px; }
        th { color: var(--gold); text-align: left; border-bottom: 2px solid var(--gold); padding: 12px; font-family: 'Cinzel', serif; }
        td { padding: 12px; border-bottom: 1px solid #333; font-size: 0.9rem; }
        .status-pill { padding: 4px 10px; border-radius: 20px; font-size: 0.75rem; font-weight: bold; }
        .done { background: #1b4332; color: #74c69d; }

        footer { text-align: center; padding: 40px; color: #555; font-family: 'Cinzel', serif; }
    </style>
</head>
<body>

<header>
    <h1>SENATO</h1>
    <p style="color: var(--gold); letter-spacing: 3px;">ORDINE • RIGORE • COLLABORAZIONE</p>
</header>

<div class="container">
    
    <section class="manifesto">
        <h2 style="font-family:'Cinzel'; color:var(--gold); text-align:center; margin-top:0;">Atto di Fondazione</h2>
        <p style="text-align: justify; color: #bbb; font-size: 0.95rem;">
            Il Senato opera come organismo armonico e coordinato, nel quale ogni membro contribuisce secondo le proprie mansioni al progresso collettivo. L'unione dei senatori è il baluardo contro le insidie dello studio accademico.
        </p>
    </section>

    <div class="senators-grid">
        <div class="senator-card">
            <h3 style="font-family:'Cinzel'; color:var(--gold); margin-bottom:5px;">Fogliana</h3>
            <span class="role-title">Redattore degli Elaborati</span>
            <div class="btn-group">
                <input type="file" id="file-fogliana" style="display:none">
                <button class="btn btn-deposit" onclick="document.getElementById('file-fogliana').click()">Deposita Documento</button>
                <a href="https://drive.google.com/drive/folders/1wR8Nr0_dXi_75lryF4BsB1I5MF05-LVh?usp=drive_link" target="_blank" class="btn btn-folder">Apri Cartella</a>
            </div>
        </div>

        <div class="senator-card">
            <h3 style="font-family:'Cinzel'; color:var(--gold); margin-bottom:5px;">Poma</h3>
            <span class="role-title">Garante della Correttezza</span>
            <div class="btn-group">
                <input type="file" id="file-poma" style="display:none">
                <button class="btn btn-deposit" onclick="document.getElementById('file-poma').click()">Deposita Documento</button>
                <a href="https://drive.google.com/drive/folders/12W-AwTWb6hNMAYm21ghprxpxml_3kc6b?usp=drive_link" target="_blank" class="btn btn-folder">Apri Cartella</a>
            </div>
        </div>

        <div class="senator-card">
            <h3 style="font-family:'Cinzel'; color:var(--gold); margin-bottom:5px;">Savalli</h3>
            <span class="role-title">Revisore e Correttore</span>
            <div class="btn-group">
                <input type="file" id="file-savalli" style="display:none">
                <button class="btn btn-deposit" onclick="document.getElementById('file-savalli').click()">Deposita Documento</button>
                <a href="https://drive.google.com/drive/folders/1ZM9s2FH4D4l8hnaC82FNYreW-RQq_jYF?usp=drive_link" target="_blank" class="btn btn-folder">Apri Cartella</a>
            </div>
        </div>
    </div>

    <section class="history-section">
        <h2 style="font-family:'Cinzel'; color:var(--gold); text-align:center;">Registro Storico</h2>
        <table>
            <thead>
                <tr>
                    <th>Data</th>
                    <th>Documento</th>
                    <th>Stato</th>
                </tr>
            </thead>
            <tbody>
                <tr><td>17/03/2026</td><td>Analisi Consumi C++</td><td><span class="status-pill done">Archiviato</span></td></tr>
                <tr><td>17/03/2026</td><td>Gestione Cinema</td><td><span class="status-pill done">Archiviato</span></td></tr>
            </tbody>
        </table>
    </section>
</div>

<footer>AD MAIORA • SENATO ACCADEMICO • 2026</footer>

</body>
</html>
