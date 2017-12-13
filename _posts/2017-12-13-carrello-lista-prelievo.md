---
layout: post
title: "Carrello lista prelievo"
description: "Creazione di un carrello con codice magazzino e cliente in testata; inserimento di articolo con la ricerca per codice articolo e stampo dell'elenco degli articoli nel carrello."
date: 13 december 2017
tags: carrelli
---

Riportiamo un esempio di un utilizzo molto semplice dei carrelli in Pickup: i carrelli vengono creati nella videata di visualizzazione delle testate dei carrelli, e gli articoli vengono inseriti leggendo il codice dell'articolo con il barcode oppure selezionando gli articoli da una ricerca in base ai primi caratteri del codice articolo. 

{% include image.html name="visualizzazione-articoli-carrello.jpg" caption="Visualizzazione degli articoli nel carrello." %}

Confermando la composizione del carrello dalla videata articoli viene proposta l'attività di stampa collegata al report PK_CARRELLO_LIS_PRE incluso nel pacchetto di installazione di {{ site.pickup }}. 

{% include image.html name="stampa-anteprima.jpg" caption="Anteprima della stampa degli articoli nel carrello dal formato PK_CARRELLO_LIS_PRE." %}


{% include download.html name="std_carrelli_lista_prelievo.xml" caption="Scarica il processo in formato xml" %}

