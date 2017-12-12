---
layout: post
title: "Spedizioni da Ordine di Produzione"
description: "Viene illustrato l'utilizzo di carrelli per l'esportazione su tabelle per la predisposizione su terminalini, che permette la creazione di DdT e l'evasione degli ordini di vendita. I carrelli sono confezionati dalla lettura del barcode della riga dell'ordine di produzione."
date: 5 december 2017
tags: spedizioni carrelli
---

I carrelli di Pickup sono uno strumento molto versatile che supporta varie tipologie di esportazione: su file (per l'acquisizione asincrona), su 
tabelle per la predisposizione da terminalini e su tabelle per le proposte di approvvigiornamento. In questo esempio vediamo il caso 
in cui da un carrello è possibile scrivere sulle tabelle per la predisposizione da terminalini e quindi evadere le righe
di Ordini di Vendita (OdV) nella creazione di un Documento di Trasporto (DdT).

{% include image.html name="processi_odp_predisposizione_terminalini.jpg" caption="I due processi per la gestione dei carrelli con il confezionamento 
da riga ordine di produzione e l'esportazione su tabelle per la predisposizione da terminalini." %}

Dal processo '30-Gestione Bancali' mostrato nella prima figura si creano le testate dei carrelli, e selezionando un carrello si passa
alla visualizzazione degli articoli con le quantità relative. L'inserimento degli articoli avviene con la lettura del codice a barre del riferimento
della riga di un Ordine di Produzione (OdP); è possibile attivare il controllo dell'esistenza del riferimento alla riga OdV, per cui se non è presente 
l'inserimento dell'articolo viene bloccato. Quando il carrello è vuoto, l'inserimento del primo articolo tramite lettura del barcode della riga OdP
definisce anche il codice cliente assegnato alla testata del carrello, per cui la lettura di altri barcode OdP genera un errore se il riferimento del cliente
non corrisponde. E' sempre possibile modificare le quantità nei carrelli oppure eliminare articoli dai carrelli.

{% include image.html name="testate_carrello.jpg" caption="Processo '30-Gestione Bancali': le testate di due carrelli; il primo carrello ha già
il riferimento del codice cliente." %}

Nel caso sia presente il controllo del riferimento OdV, viene controllato anche il riferimento dall'indirizzo di consegna, per righe OdP 
collegate ad uno stesso cliente ma con indirizzi di consegna differenti non possono essere inserite nello stesso carrello.
Selezionando il tasto conferma dalla videata con le righe del carrello viene proposta la stampa di un report, che possa servire da etichetta
da apporre sul bancale. Lo stato del carrello viene modificato, passando dallo stato 'In Confezionamento' allo stato 'Da Prelevare'.


{% include image.html name="righe_carrello.jpg" caption="Processo '30-Gestione Bancali': le righe di un carrello; è indicato il codice articolo e la quantità 
con il riferimento alla riga Ordine di Produzione ed Ordine di Vendita." %}

{% include image.html name="stampa_carrello.jpg" caption="Processo '30-Gestione Bancali': videata di stampa dell'etichetta del carrello." %}

Dal processo '32-Chiusura Bancale' è possibile selezionare un carrello e procedere all'esportazione sulle tabelle per la predisposizione da terminalini.
I carrelli chiusi non sono più visibili nei processi di confezionamento e chiusura.

{% include image.html name="esportazione_carrello.jpg" caption="Processo '32-Chiusura Bancale': i carrelli confezionati possono venir confermati
per eseguire l'esportazione sulle tabelle per la predisposizione da terminalini." %}

Nel caso in cui il tipo documento per il DdT sia configurato correttamente, dal menù F11-Altre Funzioni nella creazione dei DdT è possibile
procedere con il caricamento delle righe dei carrelli collegate al cliente ed evadere le righe dell'ordine di vendita collegate tramite il riferimento
inserito nella tabella delle righe per la predisposizione da terminalini.

{% include image.html name="creazione_ddt_altre_funzioni.jpg" caption="Esolver standard: creazione DdT da predisposizione da terminalini ." %}


{% include download.html name="std_odp_predisposizione_terminalini.xml" caption="Scarica il processo in formato xml" %}
