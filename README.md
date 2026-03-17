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
            height: 65vh;
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

        /* MANIFESTO */
        .manifesto {
            background-color: var(--card-bg);
            border: 2px solid var(--gold);
            padding: 40px;
            margin-bottom: 50px;
            box-shadow: 0 0 30px rgba(197, 160, 89, 0.1);
        }

        .manifesto h2 {
            font-family: 'Cinzel', serif;
            color: var(--gold);
            text-align: center;
            margin-top: 0;
        }

        /* GRIGLIA SENATORI */
        .senators-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-bottom: 60px;
        }

        .senator-card {
            background: linear-gradient(145deg, #1a1a1a, #222);
            border-top: 4px solid var(--gold);
            padding: 30px;
            text-align: center;
            border-radius: 0 0 10px 10px;
            transition: 0.3s;
        }

        .senator-card:hover { transform: translateY(-5px); }

        .role-title {
            color: var(--deep-red);
            font-weight: bold;
            text-transform: uppercase;
            font-size: 0.8rem;
            display: block;
            margin-bottom: 15px;
        }

        .drive-link {
            display: inline-block;
            background: transparent;
            border: 1px solid var(--gold);
            color: var(--gold);
            padding: 10px 20px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
            margin-top: 15px;
        }

        .drive-link:hover {
            background: var(--gold);
            color: black;
        }

        /* CRONOLOGIA */
        .history-section {
            background: var(--card-bg);
            padding: 30px;
            border: 1px solid #333;
        }

        table {
