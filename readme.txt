========================================================================
       ISTRUZIONI PER L'AVVIO DELLA DASHBOARD DI ANALISI BI
========================================================================

Questo pacchetto contiene l'applicazione standalone per l'analisi dei 
dati del mercato del lavoro rlativi ald un .csv MICRODATI, o subset. 
Non è necessario installare Python o altre
librerie sul computer: tutto il motore software è integrato nell'eseguibile.

L'ho testato in una crtella vuota sul mio portatile e funziona, d'altra parte 
ero all'interno di un ambiente virtuale di sviluppo. È da verificare nella "vita reale" 
(ammesso, naturalmente, che sia reale una cartella vuota nella memoria di un notebook).

------------------------------------------------------------------------
1. REQUISITI PER IL FUNZIONAMENTO
------------------------------------------------------------------------
Per far funzionare l'applicazione sono necessari solo due file, che 
devono risiedere SEMPRE all'interno della stessa identica cartella vuota 
(crearne una nuova):

  1. app.exe            (L'applicazione della Dashboard)
  2. dati_mercato.csv   (Il file contenente i dati da analizzare)

NOTA SUL FILE DATI: Se il file del database ha un nome diverso, rinominalo 
esattamente in "dati_mercato.csv" prima di avviare il programma.

Il primo avvio comporta del tempo di attesa di caricamento, come la prima lettura del Dashboard

È stato testato con un file di circa 1 giga di grandezza con successo. 

------------------------------------------------------------------------
2. PROCEDURA DI AVVIO (PASSO-PASSO)
------------------------------------------------------------------------
Segui questi semplici passaggi per consultare i grafici:

  [Passo 1] Fai doppio clic sul file "app.exe".
  
  [Passo 2] Si aprirà una finestra nera del Terminale. Non chiuderla! 
            L'applicazione sta caricando il database in memoria. 
            Dato che il file supera il milione di righe, attendi qualche
            secondo finché non vedi comparire la scritta:
            "--> Caricamento completato con successo!"

  [Passo 3] Apri il tuo browser internet (Chrome, Edge o Firefox) e 
            digita o copia questo indirizzo nella barra di ricerca:
            
            http://127.0.0.1:8062

  [Passo 4] La Dashboard si aprirà immediatamente sul form di setup.

------------------------------------------------------------------------
3. PRIMO ACCESSO: MAPPATURA DEI CAMPI
------------------------------------------------------------------------
Se i nomi delle colonne del tuo file differiscono da quelli standard, 
non c'è problema:
  - Usa i menu a tendina del pannello iniziale per associare i campi 
    richiesti alle colonne effettive del tuo file CSV.
  - Clicca sul pulsante verde "Attiva Dashboard".
  - I grafici e i trend si genereranno istantaneamente adattandosi 
    alla struttura del tuo database.

------------------------------------------------------------------------
4. COME CHIUDERE L'APPLICAZIONE
------------------------------------------------------------------------
Quando hai terminato l'analisi:
  1. Chiudi semplicemente la scheda del browser.
  2. Torna sulla finestra nera del Terminale e premi la combinazione 
     di tasti "CTRL + C" sulla tastiera, oppure clicca sulla "X" in 
     alto a destra per chiudere definitivamente il programma.

------------------------------------------------------------------------
Risoluzione dei problemi:
Se al doppio clic l'app viene bloccata dall'antivirus aziendale (SmartScreen), 
clicca su "Maggiori informazioni" e poi su "Esegui comunque". L'avviso 
compare solo perché l'eseguibile è stato generato internamente e non 
dispone di una firma digitale commerciale.
========================================================================