<!--

# Hotel
## Ricreare database hotel come da diagramma
Prendere il diagramma e usando phpmyadmin ricreare il database,
inserire dei dati a piacere per poter effettuare le seguenti ricerche
## Ricerche da effettuare sul database
- selezionare tutti gli ospiti
    SELECT * FROM `ospiti`;

- selezionare tutti gli ospiti che sono stati identificati con la carta di identitá
    SELECT * FROM `ospiti` WHERE `documento` = "carta d'identità";

- selezionare tutte le stanze del primo piano
    SELECT * FROM `rooms` WHERE `floor` = 1;

- selezionare tutti gli ospiti che iniziano per E (vedi uso del Like)
    SELECT * FROM `ospiti` WHERE `nome` LIKE 'E%';

- Selezionare tutti gli ospiti che abbiano almeno 30 anni
    SELECT * FROM `ospiti` WHERE `età` >= 30

- selezionare tutte le prenotazioni precedenti ad una data a piacere
    SELECT * FROM prenotazioni WHERE data_prenotazione < '2021-01-01';

## Altre ricerche (opzionali)
- seleziona tutti gli ospiti nati dopo una certa data
    SELECT * FROM ospiti WHERE data_nascita > '1980-01-01'

- calcola il totale degli ordini ricevuti
    SELECT COUNT(id) FROM prenotazioni

- calcola il prezzo massimo pagato


- calcola quanti posti letto ha l'hotel in totale
    SELECT SUM(capacity) as 'posti letto totali' FROM rooms

-->
