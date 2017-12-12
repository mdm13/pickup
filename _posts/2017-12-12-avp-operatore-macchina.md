---
layout: post
title: "AVP operatore macchina"
description: "Un esempio di avanzamento di produzione con risorse multiple, con consuntivazione ore in modalita' start-stop
e imputazione quantita' di fase."
date: 12 december 2017
tags: avp start-stop
---

Tra le numerose variazioni sul tema dell'avanzamento di produzione, presentiamo in questo esempio la possibilita' di effettuare una registrazione di avanzamento con consuntivazione delle ore per piu' risorse contestualmente all'avanzamento di una quantita' di fase per il prodotto finito. La registrazione delle ore e' in modalita' start-stop, per cui il tempo viene calcolato automaticamente.
La prima attivita' prevede la selezione della risorsa umana; quindi, nel caso non ci siano transazioni aperte dalla risorsa selezionata, viene richiesta la selezione della macchina; per questa attivita' e' abilitata la selezione multipla. Il riferimento alla riga fase viene quindi letto con un codice a barre. 
Una volta completata la lavorazione, l'operatore rientra nel processo selezionando la propria risorsa, per cui viene presentata la videata di imputazione della quantita' lavorata. Il documento creato tramite l'acquisizione dati riportera' una riga di avanzamento di fase con la quantita' digitata ed una riga con le ore lavorate per ogni risorsa di produzione selezionata. Questo dipende dalla configurazione dei tipi operazione avanzamento operazione nell'attivita' di apertura delle transazioni: sono indicate sia il tipo operazione per avanzamento/materiali che per le ore lavorate.

{% include image.html name="config-apertura-transazioni.jpg" caption="Configurazione attivita' di apertura transazioni." %}


Evidenziamo la configurazione del flag "Risorsa di Supporto Materiali" nell'attivita' di selezione della risorsa macchina; attivando questo flag si disabilita l'inserimento di righe di aggiuntive avanzamento quantita' per ogni risorsa macchina. 

{% include image.html name="risorsa-di-supporto-materiali.jpg" caption="Configurazione attivita' di selezione risorse di produzione/macchina: il flag 'Risorsa di Supporto Materiali' e' attivo per evitare l'inserimento multiplo della quantita'." %}


{% include download.html name="std_avp_operatore_macchine_rsu.xml" caption="Scarica il processo in formato xml" %}


