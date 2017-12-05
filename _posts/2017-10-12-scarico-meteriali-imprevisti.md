---
layout: post
title: "Scarico materiali imprevisti"
date: 12 october 2017
tags: avp
---

Nel contesto dell'avanzamento di produzione, è possibile collegare lo scarico di materiali impevisti 
alle righe di prodotto finito indicando l'articolo e il riferimento alla riga ODP, entrambe letti tramite barcode
da un cartellino di produzione. L'operatore viene guidato alla videata di imputazione della quantità, nella quale è stata aggiunta
la gestione della seconda unità di misura. Se il materiale è gestito a lotto, l'operatore deve selezionare il lotto da scaricare, 
è prevista la possibilità di selezionare più lotti.


{% include image.html name="editazione-avp.jpg" caption="Videata di editazione quantità:
 inserendo il valore nell'unità di misura secondaria viene automaticamente aggiornato quello nell'unità di misura del documento." %}

Nel dettaglio il processo segue i seguenti steps, seguendo la sequenza delle attività:

1. Selezione operatore
2. Inserimento codice articolo da barcode
3. Visualizzazione articolo, il materiale imprevisto che si intende scaricare
4. Inserimento riferimento riga ordine di produzione da barcode
5. Visualizzazione riga ordine di produzione; l'operatore procede con l'editazione della quantità prelevata selezionando la riga ODP
6. Creazione file di esportazione per l'acquisizione asincrona (DAS) di Esolver.

 
{% include download.html name="std_materiale_imprevisto_con_um2.xml" caption="Scarica il processo in formato xml" %}

