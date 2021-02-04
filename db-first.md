<!-- db-first
Istruzioni:
Create un file di testo per descrivere un database di un negozio di videogiochi.
Strutturate il file come fatto oggi in classe.  Specificate: il nome del database, la tabella e le potenziali colonne con i tipi di dato. -->

# GAME-POP

## Videogames

---

-   id | BIGINT | PRIMARY KEY
-   titolo | VARCHAR(50) | NOTNULL
-   descrizione | TEXT | NULL
-   piattaforma | VARCHAR(20) | NOTNULL <!-- ps4, xbox, pc, ecc. -->
-   PEGI | TINYINT | NULL
-   data_di_rilascio | DATE | NULL
-   categoria | VARCHAR(20) | NULL <!-- simulazione, rompicapi, arcade, ecc. -->
-   prezzo | FLOAT(3,2) | NOTNULL
-   acquisti_in_game | TINYINT | NULL <!-- è un boolean, presenti o no -->
-   produttore | VARCHAR(20) | NULL
-   quantità | SMALLINT | NULL
-   ratings | VARCHAR() | NULL <!-- link al sito x che raccoglie le valutazioni dei gamers su quel gioco - es. metacritic -->
-   img_copertina | VARCHAR() | NULL <!-- link a img -->
-   dimensione_in_MB | SMALLINT | NULL
-   voto_utenti | TINYINT | NULL <!-- immaginiamo un sito interattivo del negozio con gli utenti che possono valutare il gioco su una scala a 5 -->
-   nuovo | TINYINT | NOTNULL <!-- nuovo o usato? abbiamo un boolean - se vero il gioco è nuovo -->
