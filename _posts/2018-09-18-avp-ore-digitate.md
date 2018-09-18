---
layout: post
title: "Avanzamento di produzione con ore digitate"
description: "processo di Avanzamento di produzione con ore digitate (NO START - STOP)"
date: 18 September 2018
tags: avp
rifdemo: DEMOGLA_1402
---

Presentiamo, in questo esempio, la possibilità di effettuare una registrazione di avanzamento digitando le ore. 
La registrazione delle ore è quindi in modalità manuale. La prima attività prevede la selezione della risorsa umana.
Viene richiesta la selezione della fase il cui riferimento alla riga fase viene letto con un codice a barre.
In questo caso non si effettuano controlli su transazioni eventualmente aperte dalla risorsa selezionata in quanto il processo 
chiude direttamente la transazione una volta imputata la quantità di ore lavorate. 
Dopo aver selezionato la fase viene mostrata la schermata di imputazione delle ore lavorate.
Il documento creato tramite l’acquisizione dati riporterà un’unica riga di avanzamento di fase con le ore lavorate per la risorsa 
di produzione selezionata. Questo dipende dalla configurazione dei tipi operazione avanzamento operazione nell’attività di apertura delle 
transazioni: va indicata solo il tipo operazione per le ore lavorate.

{% include image.html name="AVP_ore_digitate.png" caption="Configurazione tipi operazioni sul processo" %}

Attraverso i tasti in alto a destra si potrà scegliere se stampare o visualizzare l’anteprima della stampa.

Una volta completata la lavorazione, l’operatore rientra nel processo selezionando la propria risorsa, per cui viene 
presentata la videata di imputazione della quantità lavorata. Il documento creato tramite l’acquisizione dati riporterà una riga di 
avanzamento di fase con la quantità digitata ed una riga con le ore lavorate per la risorsa di produzione selezionata. 
Questo dipende dalla configurazione dei tipi operazione avanzamento operazione nell’attività di apertura delle transazioni: 
sono indicate sia il tipo operazione per avanzamento/materiali che per le ore lavorate.
Nel processo le impostazioni da seguire per poter stampare il cartellino sono le seguenti

{% include image.html name="AVP_ore_digitate2.png" caption="Configurazione Attività di Visualizzazione Transazioni" %}


{% include download.html name="std_AVP_ore_digitate.xml" caption="Scarica il processo in formato xml" %}

