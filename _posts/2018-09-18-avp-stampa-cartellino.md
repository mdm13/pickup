---
layout: post
title: "Avanzamento di produzione con stampa cartellino"
description: "Stampa cartellino in un processo di avanzamento di produzione"
date: 18 September 2018
tags: avp stampa
rifdemo: DEMOGLA_1400
---

Presentiamo, in questo esempio, la possibilità di effettuare una registrazione di avanzamento con stampa 
del cartellino di lavoro. La registrazione delle ore è in modalità start-stop, per cui il tempo viene calcolato 
automaticamente. La prima attività prevede la selezione della risorsa umana.
Nel caso non ci siano transazioni aperte dalla risorsa selezionata, viene richiesta la selezione della fase il 
cui riferimento alla riga fase viene letto con un codice a barre.
Dopo la selezione della fase viene visualizzata la schermata di stampa.

{% include image.html name="videata-stampa.png" caption="Videata di stampa su tablet" %}

Attraverso i tasti in alto a destra si potrà scegliere se stampare o visualizzare l’anteprima della stampa.

Una volta completata la lavorazione, l’operatore rientra nel processo selezionando la propria risorsa, per cui viene 
presentata la videata di imputazione della quantità lavorata. Il documento creato tramite l’acquisizione dati riporterà una riga di 
avanzamento di fase con la quantità digitata ed una riga con le ore lavorate per la risorsa di produzione selezionata. 
Questo dipende dalla configurazione dei tipi operazione avanzamento operazione nell’attività di apertura delle transazioni: 
sono indicate sia il tipo operazione per avanzamento/materiali che per le ore lavorate.
Nel processo le impostazioni da seguire per poter stampare il cartellino sono le seguenti

{% include image.html name="videata-stampa2.png" caption="Impostazioni per stampa di un cartellino" %}


{% include download.html name="std_AVP_fase_con_stampa.xml" caption="Scarica il processo in formato xml" %}

