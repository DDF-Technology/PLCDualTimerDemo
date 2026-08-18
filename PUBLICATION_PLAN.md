# Piano di pubblicazione

## Modello di distribuzione

PLCDualTimerDemo sarà pubblicato gratuitamente, in forma completa e sotto licenza MIT. Non sono
previste varianti ridotte, timeout, watermark funzionali o uscite disabilitate.

## Materiale pronto

- progetto TIA Portal V18 originale;
- licenza MIT e avvisi relativi a Siemens;
- schermata del blocco `Main [OB1]` in LAD;
- descrizione della sequenza e dei tag leggibili;
- checklist riproducibile per compilazione e collaudo.

## Verifiche prima della release pubblica

1. Aprire una copia con TIA Portal V18 Update 5.
2. Compilare hardware e software e registrare l'esito.
3. Eseguire la simulazione con PLCSIM o il test controllato su CPU compatibile.
4. Provare avvio, arresto, riavvio e alternanza delle due uscite.
5. Provare valori temporali validi, limite e non validi.
6. Confermare o aggiornare la tabella dei tag in `docs/LOGIC.md`.
7. Esportare il blocco in un formato leggibile e reimportabile, se disponibile.
8. Verificare nuovamente l'assenza di dati di cliente o impianto.
9. Controllare i termini Siemens applicabili ai file generati dalla toolchain.

## Criterio di pubblicazione

La release candidata può essere distribuita come materiale didattico, ma non deve essere presentata
come validata finché la checklist non è stata completata. La pubblicazione sul sito dovrà mantenere
ben visibili lo stato di prerelease e l'assenza di validazione su PLCSIM o hardware.
