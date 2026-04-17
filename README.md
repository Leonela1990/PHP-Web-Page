# CMS Articoli (Locale)

Un progetto in fase di sviluppo per la gestione di articoli, tag e immagini tramite un database MySQL locale.

## Requisiti
- **Server:** XAMPP, WAMP o MAMP.
- **Database:** MySQL/MariaDB (importare lo schema in `db/database_schema.sql` tramite phpMyAdmin).
- **Versione PHP:** 7.4 o superiore.

## Struttura del Database
Il CMS si basa su una struttura relazionale:
* **Articoli:** Tabella centrale con titolo e contenuto.
* **Tag:** Gestiti tramite una tabella separata collegata agli articoli (relazione molti-a-molti).
* **Immagini:** Gestite tramite percorsi salvati nel database.

## Come testare il progetto
1. Avvia Apache e MySQL dal tuo pannello di controllo (es. XAMPP).
2. Crea un database chiamato `nome_tuo_db`.
3. Importa il file `db/database_schema.sql` via phpMyAdmin.
4. Posiziona la cartella del progetto nella root del server (solitamente `htdocs` o `www`).
5. Accedi tramite `http://localhost/nome-cartella`.
