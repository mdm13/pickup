---
layout: post
title: "Ordine di spedizione"
date: 10 november 2017
---

Tra i processi rilevanti per la logistica di Pickup abbiamo la possibilità di gestire il picking negli ordini di spedizione.
Nella prima videata sono visualizzate le testate degli ordini di spedizione, con il colore del pulsante (visualizzazione tablet) o 
della riga della griglia (visualizzazione terminalino) associato allo stato dell'ordine di spedizione. Selezionando la testata dell'ordine di spedizione (OdS) per cui si desidera effettuare il picking, 
si passa alla visualizzazione delle righe dell'OdS sotto forma di bottone (visualizzazione tablet) oppure di righe della griglia (visualizzazione terminalino).

{% include image.html name="testate-ods.jpg" caption="Videata tablet con la visualizzazione delle testate degli ordini di spedizione." %}

{% include image.html name="righe-ods.jpg" caption="Videata tablet con la visualizzazione delle righe di un ordine di spedizione." %}

{% include image.html name="testate-ods-terminalini.jpg" caption="Videata terminalini con la visualizzazione delle testate degli ordini di spedizione." %}

A differenza di altri processi Pickup, per cui l'interazione con Esolver avviene generalmente in modo asincrono con files di esportazione, la gestione degli OdS interagisce le tabelle transitorie del database ed attiva i blocchi del documento come da standard Esolver.

{% include image.html name="blocco-ods.jpg" caption="Blocco dell'ordine di spedizione durante la variazione tramite processo di picking di Pickup." %}

L'operazione di picking consiste nell'indicare la quantità prelevata per ciascuna riga dell'ordine di spedizione; questa operazione si può effettuare selezionando la riga e digitando la quantità prelevata, con la possibilità di selezionare le matricole nel caso l'articolo ne preveda la gestione. Nel caso si lavori con l'interfaccia a terminalino è senz'altro preferibile l'utilizzo del barcode, per cui l'operatore legge il codice a barre di un articolo oppure la matricola, e la quantità prelevata viene automaticamente valorizzata per la riga dell'OdS non ancora a saldo.

{% include image.html name="prelilevo-matricola.jpg" caption="Selezione della matricola nel picking su una riga di un ordine di spedizione." %}


{% include download.html name="std_spedizioni_picking.xml" caption="Scarica il processo in formato xml: spedizioni con e senza selezione cliente." %}