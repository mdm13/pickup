---
layout: post
title: "Carico prodotto finito"
description: "Illustrazione delle diverse modalità di gestione del magazzino di carico per avanzamenti di produzione con carico del prodotto finito."
date: 13 december 2017
tags: avp
---

Ci sono diverse modalità per controllare im magazzino di destinazione nei movimenti di avanzamento di produzione per il carico del composto, come esemplificato nei nei tre processi disponibili per il download. In tutti e tre i casi il tipo operazione avanzamento di produzione prevede il carico composto e lo scarico dei materiali.

{% include image.html name="tipo-operazione-versamento-scarico.jpg" caption="Parametri per il tipo operazione avanzamento di produzione." %}

Il primo esempio (processo numero 10) utilizza i valori definiti nella riga dell'ordine di produzione, che a loro volta dipendono dal tipo documento ordine di produzione. Il tipo documento avanzamento di produzione non reca alcunaindicazione sul magazzino di carico, come mostrato nella figura.

{% include image.html name="tipo-documento-versamento-consumo.jpg" caption="Tipo documento avanzamento di produzione per il versamento composto e consumo materiali senza indicazione del magazzino di carico." %}

Nel secondo esempio (processo numero 11) il tipo documento avanzamento di produzione contiene l'indicazione del magazzino di carico del composto: tutti i movimenti di carico del prodotto finito andranno a movimentare su questo magazzino, a patto che sia attivata l'apposita opzione nell'attività di apertura delle transazioni del processo Pickup.

{% include image.html name="tipo-documento-versamento-consumo-con-magazzino.jpg" caption="Tipo documento avanzamento di produzione per versamento composto e consumo materiali con l'indicazione del magazzino di carico." %}

Nel terzo esempio (processo numero 9) si prevede la possibilità per l'operatore si scegliere il magazzino di destinazione per il composto al momento della digitazione della quantità del composto. Questa opzione  si attiva nella configurazione del parametro per il codice edit E16 nell'attività di visualizzazione delle transazioni aperte. In particolare si prevede la possibilità di modificare la query di ricerca del magazzino di destinazione del prodotto finito, eventualmente per restringere le possibili scelte per l'operatore.

{% include image.html name="gestione-manuale-magazzino.jpg" caption="Configurazione della scelta manuale del magazzino per il carico del composto." %}

{% include image.html name="selezione-magazzino-carico-arrow.jpg" caption="Nella videata per l'inserimento della quantità prodotta viene attivato il pulsante per la selezione del magazzino di carico del prodotto finito." %}


{% include download.html name="std_avp_carico_composto_magazzini.xml" caption="Scarica i tre processi in formato xml" %}

