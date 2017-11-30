---
layout: post
title: "Gestione PIN operatore"
date: 30 november 2017
---

Tra le attività più comuni nei processi di Pickup troviamo la selezione della risorsa, sia essa risorsa
umana oppure di produzione; in alcuni casi è necessario verificare l'identità della risorsa, e a questo 
scopo sono stati introdotti dei parametri specifici nell'azione di selezione (codice S05): 
è possibile attivare il controllo del PIN dell'utente, con l'ulteriore opzione di ignorare il controllo
del PIN nel caso in cui la selezione sia collegata alla lettura di un codice a barre.

{% include image.html name="parametri_S05.jpg" caption="Definizione dei parametri per l'azione di selezione delle risorse." %}


Una volta attivata la gestione del PIN, con la selezione della risorsa tramite la pressione del bottone corrispondente, si apre la videata di inserimento del PIN, che se corretto permette di proseguire
con le attività del processo.

L'amministrazione dei PIN delle risorse avviene tramite un processo di Pickup dedicato, incluso nel modulo Presenze; si seleziona la risorsa e si inserisce il PIN dell'operatore (fino a 12 cifre); 
il valore viene salvato in forma
criptata come codice esterno nell'anagrafica risorse di Esolver, per cui non è possibile carpire il PIN di un operatore una volta inserito nel database di Esolver. Nel caso l'operatore smarrisca il PIN questo dovrà richiederne uno nuovo, ed il processo di aggiornamento di un nuovo PIN annullerà quello non più in uso; infine non è permessa la duplicazione dei PIN o il riutilizzo di PIN non più in uso.

{% include image.html name="codici-esterni-risorse.jpg" caption="Elenco dei codici esterni associati ad una risorsa dalla gestione risorse di Esolver." %}


{% include download.html name="std_gestione_pin_risorsa.xml" caption="Scarica il processo in formato xml" %}
