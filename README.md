# Nasdaq_App

Ho creato questa piccola App utilizzando la libreria ReactJS con un approccio Class Component

Si tratta di una App che simula il monitoraggio dell'andamento della borsa americana

Per rendere la simulazione quanto più realistica mi sono servita di due API di test create appositamente con Laravel.

La prima API viene interrogata tramite keywords immesse dentro una barra di ricerca e mi recupera la lista delle azioni 
(essendo tale API solamente un test ho inserito soltanto come aziende cercabili Amazon e Apple). 

La seconda mi restituisce l'andamento (in guadagno o perdita) del mercato in tempo reale all'attivazione di un pulsante di checkbox
sull'interfaccia di dettaglio di ogni singola azione.

Ho inoltre implementato un grafico utilizzando il servizio di Recharts.org al fine di rendere realistica la consultazione dei dati.

Per riuscire a simulare le perdite e i guadagni delle singole aziende ho implementato un metodo di Random Javascript 
e inoltre, con un operatore ternario ho simulato gli orari di apertura e di chiusura della borsa, in modo tale che oltre una certa fascia di orario 
(quella che va dalle 09:00 alle 16:00) i dati non sono più consultabili, ovvero il pulsante di checkbox che mostra i punti e le percentuali di perdita o guadagno, 
risulta disabilitato.

App testabile al seguente link:
