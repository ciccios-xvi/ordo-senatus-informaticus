
<html lang="it">
<head>
    <meta charset="UTF-8">
    <title>Registro Storico</title>
    <style>
        /* Stili Generali (per l'ambiente di test) */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #121212; /* Fondo molto scuro del sito */
            color: #d8c3a5; /* Colore testo generale chiaro/dorato */
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        /* Contenitore Principale (scuro come nell'immagine) */
        .registro-container {
            background-color: #1a1a1a; /* Leggermente più chiaro dello sfondo per profondità */
            border-radius: 8px;
            padding: 40px;
            width: 80%;
            max-width: 900px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }

        /* Titolo della Sezione */
        .registro-container h2 {
            text-align: center;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: #d8c3a5; /* Testo dorato scuro */
            margin-top: 0;
            margin-bottom: 20px;
        }

        /* Linea Separatoria Dorata */
        .registro-container hr {
            border: none;
            border-top: 1px solid #7d6b53; /* Linea sottile dorata scura */
            margin-bottom: 30px;
        }

        /* Stile della Tabella */
        .storico-table {
            width: 100%;
            border-collapse: collapse; /* Rimuove lo spazio tra i bordi delle celle */
            color: #eae0d5; /* Testo dei dati chiaro e caldo */
        }

        /* Intestazione Tabella */
        .storico-table thead th {
            text-align: left;
            padding: 15px 20px;
            text-transform: uppercase;
            font-size: 0.85rem;
            color: #d8c3a5; /* Testo intestazione dorato scuro */
            border-bottom: 1px solid #7d6b53; /* Linea sotto intestazione */
        }

        /* Corpo Tabella - Sfondo Scuro per Leggibilità */
        .storico-table tbody {
            background-color: #212121; /* Sfondo scuro per il blocco dati */
        }

        /* Righe del Corpo Tabella */
        .storico-table tbody tr {
            border-bottom: 1px solid #333; /* Linee divisorie orizzontali scure */
        }

        /* Ultima riga senza bordo inferiore */
        .storico-table tbody tr:last-child {
            border-bottom: none;
        }

        /* Celle della Tabella */
        .storico-table tbody td {
            padding: 15px 20px;
            font-size: 0.95rem;
        }

        /* Colonna Data - Tono leggermente più neutro */
        .storico-table tbody td.data-col {
            color: #b0a99f;
        }

        /* Badge Stato 'Archiviato' */
        .status-badge {
            display: inline-block;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
            text-transform: uppercase;
            color: white; /* Testo bianco sul badge */
        }

        /* Colore specifico per Stato 'Archiviato' (Verde Scuro Profondo) */
        .status-badge.archiviato {
            background: linear-gradient(135deg, #0f5132, #072a1a); /* Gradiente per profondità */
            box-shadow: 1px 1px 3px rgba(0,0,0,0.3);
        }

    </style>
</head>
<body>

<div class="registro-container">
    <h2>Registro Storico</h2>
    <hr>

    <table class="storico-table">
        <thead>
            <tr>
                <th>Data</th>
                <th>Documento</th>
                <th>Stato</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td class="data-col">17/03/2026</td>
                <td>Analisi Consumi C++</td>
                <td><span class="status-badge archiviato">Archiviato</span></td>
            </tr>
            <tr>
                <td class="data-col">17/03/2026</td>
                <td>Gestione Cinema</td>
                <td><span class="status-badge archiviato">Archiviato</span></td>
            </tr>
        </tbody>
    </table>
</div>

</body>
</html>
