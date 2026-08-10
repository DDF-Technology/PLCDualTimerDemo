# PLCDualTimerDemo

Archivio dimostrativo PLC dedicato a una logica di intermittenza ottenuta alternando due timer.
Il repository conserva il progetto e i relativi metadati dell'ambiente di sviluppo come materiale
didattico e storico.

## Contenuto

- `IntermittenzaDoppioTimer.ap18`: progetto principale;
- `AdditionalFiles/` e `UserFiles/`: allegati e file utente;
- `System/`, `IM/`, `Vci/` e `XRef/`: configurazione, indici e riferimenti incrociati;
- `Logs/` e `TMP/`: dati storici generati dall'ambiente;
- archivio PLCM aggiuntivo incluso nel progetto.

## Apertura e verifica

Il formato `.ap18` e la struttura delle cartelle indicano un progetto Automation Studio, ma la
versione esatta dell'IDE e il target hardware devono essere confermati. Prima di aprirlo, creare una
copia di lavoro per evitare migrazioni automatiche irreversibili del formato.

La logica va compilata e simulata con il target corretto. Prima del download su PLC reale verificare
mapping I/O, tempi, stato iniziale, arresto sicuro e comportamento al riavvio.

## Stato e limiti

Archivio tecnico non validato su hardware. Mancano una descrizione dettagliata delle variabili, una
procedura di simulazione riproducibile e l'identificazione definitiva di CPU e runtime.

## Proprietà e licenza

Copyright © 2026 Fabio De Deo — [www.ddf.technology](https://www.ddf.technology/). Tutti i
diritti riservati. Consultare [LICENSE](LICENSE).
