# Logica di intermittenza

## Scopo

La sequenza alterna due comandi logici quando l'intermittenza è abilitata. Ciascuna posizione ha un
tempo configurabile indipendente. L'implementazione è contenuta nel blocco ciclico `Main [OB1]` e
utilizza timer IEC `TON`.

## Segmenti documentati

| Segmento | Titolo visibile | Funzione |
| --- | --- | --- |
| 1 | Comando Attiva/Disattiva Intermittenza | Gestisce l'abilitazione generale. |
| 2 | Tempo Pos1 Attivato | Imposta o acquisisce il tempo della posizione 1. |
| 3 | Tempo Pos2 Attivato | Imposta o acquisisce il tempo della posizione 2. |
| 4 | Logica Intermittenza Pos1/Pos2 | Alterna i due comandi mediante due timer `TON`. |

## Tag leggibili nello screenshot

| Indirizzo/istanza | Nome visualizzato | Ruolo osservabile |
| --- | --- | --- |
| `%M0.1` | `Intermittenza_Attivata` | Abilitazione della sequenza. |
| `%M0.3` | `Comando-Pos1` | Comando logico della posizione 1. |
| `%M0.4` | `Comando-Pos2` | Comando logico della posizione 2. |
| `%MD8` | `timePos1_ON` | Tempo configurato per la posizione 1. |
| `%MD12` | `timePos2_ON` | Tempo configurato per la posizione 2. |
| `%DB4` | `Pos1_Timer_ON` | Istanza del timer `TON` associato alla posizione 1. |
| `%DB2` | `Pos2_Timer_ON` | Istanza del timer `TON` associato alla posizione 2. |

I nomi e gli indirizzi sono trascritti dalla schermata del 15 agosto 2026. Tipi, valori iniziali e
limiti devono essere confermati nella tabella tag di TIA Portal prima della pubblicazione definitiva.

## Sequenza funzionale attesa

1. Con `Intermittenza_Attivata` disabilitata, la sequenza deve rimanere arrestata.
2. All'abilitazione viene comandata una sola posizione alla volta.
3. Trascorso il tempo della posizione attiva, il comando passa all'altra posizione.
4. L'alternanza prosegue finché l'abilitazione resta attiva.
5. Alla disabilitazione entrambi i comandi devono tornare nello stato sicuro previsto.

I punti precedenti descrivono il comportamento atteso dalla struttura LAD visibile. Devono essere
confermati mediante compilazione e test seguendo `TEST_CHECKLIST.md`.
