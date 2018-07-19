---
layout: post
title: "Visualizzazione messaggi"
description: "Visualizzazione messaggi personalizzati"
date: 19 July 2018
tags: avp  messaggi custom
rifdemo: DEMOGLA_1010
---

L'Attività di tipo Custom è stata introdotta per poter gestire funzionalità che non
rientrano in quelle più comuni (come ad esempio la selezione di elementi da una lista - Attività di Raccolta Dati, o
l'indicazione di una data - Attività di Input). La funzionalità specifica è determinata dal codice dell'Attività Custom.

Il codice Custom C19, in particolare, permette di visualizzare dei messaggi di testo che possano essere utili per l'operatore, con la possibilità
di inoltrare lo stesso messaggio ad un indirizzo email. L'attivazione del messaggio è calcolata in base ad una query configurabile
dall'utente, così come il contenuto del messaggio.

Un esempio di utilizzo è la visualizzazione di messaggi di allerta
per il versamento di scarti nell'avanzamento di produzione;   dal riferimento della riga dell'ordine di produzione è possibile
ricavare quanti pezzi sono stati ordinati e quanti sono stati versati nel magazzino di scarto per la stessa riga dell'
ordine di produzione; dal rapporto tra i due valori si ricava la percentuale di scarto e si può decidere di attivare il messaggio
di allerta in base ad una soglia fissa o configurabile dall'anagrafica dell'articolo.

Nel processo di AVP allegato sono inserite due Attività di tipo Custom con codice C19 per la visualizzazione di messaggi personalizzati.

{% include download.html name="DEMOGLA_1010.xml" caption="Scarica il processo in formato xml" %}

