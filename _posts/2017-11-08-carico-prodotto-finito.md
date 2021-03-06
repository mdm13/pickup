---
layout: post
title: "Carico prodotto finito"
description: "Carico del prodotto finito nell'avanzamento di produzione con la gestione del lotto."
date: 8 november 2017
tags: avp lotti
---

Consideriamo il caso del carico a magazzino del prodotto finito dal riferimento della riga 
di un ordine di produzione, con la gestione del lotto. Il lotto è inserito nella riga dell'ordine, e questo
viene visualizzato al momento dell'inserimento della quantità da versare.
Nel caso in cui non sia stato indicato il lotto del prodotto finito l'operatore è costretto a 
correggere l'impostazione dell'ordine di produzione direttamente da Esolver. Questo evita la creazione di movimenti
errati, dal momento che l'indicazione del lotto è obbligatoria.


{% include image.html name="editazione_quantita.jpg" caption="Videata di editazione quantità con visualizzazione del riferimento del lotto per il prodotto finito." %}

Nel dettaglio il processo segue i seguenti steps, secondo la sequenza delle attività:

1. Selezione operatore
2. Inserimento riferimento riga ordine di produzione da barcode
3. Visualizzazione riga ordine di produzione; l'operatore procede con l'editazione della quantità da versare, il lotto è precaricato dal riferimento della riga ODP
6. Creazione file di esportazione per l'acquisizione asincrona (DAS) di Esolver.

 
{% include download.html name="std_avp_carico_prodotto_finito.xml" caption="Scarica il processo in formato xml" %}

