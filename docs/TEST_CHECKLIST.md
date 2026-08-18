# Checklist di verifica TIA Portal

Compilatore: ____________________

Versione TIA Portal: ____________________

Data: ____________________

Tecnico: ____________________

## Preparazione

- [ ] Lavorare su una copia del progetto.
- [ ] Verificare TIA Portal V18 Update 5 o compatibilità esplicita.
- [ ] Confermare CPU 1511-1 PN, articolo e firmware.
- [ ] Verificare indirizzi e tipi dei tag elencati in `LOGIC.md`.
- [ ] Sostituire eventuali indirizzi fisici con tag sicuri per la simulazione.

## Compilazione

- [ ] Compilazione hardware completata senza errori.
- [ ] Compilazione software completata senza errori.
- [ ] Warning esaminati e annotati.
- [ ] Nessuna protezione, credenziale o dato di impianto presente nel pacchetto pubblico.

## Test funzionale

- [ ] Stato iniziale sicuro con intermittenza disabilitata.
- [ ] Avvio della sequenza tramite `Intermittenza_Attivata`.
- [ ] Una sola posizione attiva alla volta.
- [ ] Durata posizione 1 coerente con `timePos1_ON`.
- [ ] Durata posizione 2 coerente con `timePos2_ON`.
- [ ] Alternanza ripetuta per almeno dieci cicli senza sovrapposizioni.
- [ ] Arresto durante la posizione 1.
- [ ] Arresto durante la posizione 2.
- [ ] Riavvio dopo arresto e dopo reset della CPU.
- [ ] Verifica con valori temporali minimo, nominale e massimo ammesso.

## Esito

- [ ] Superato
- [ ] Non superato

Note:

```text

```
