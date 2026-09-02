# AI, dati e rilascio — policy obbligatoria

Questa policy è un **gate di rilascio**, non un parere legale. Si applica a
sviluppo, test, produzione e a ogni futuro agente che modifica il progetto.

## Regole non derogabili

1. I deploy in produzione sono solo manuali, dopo test, revisione del diff e
   conferma esplicita del proprietario. Un push Git non deve distribuire.
2. Cron, agenti autonomi e servizi AI a consumo restano disabilitati per
   impostazione predefinita. Riattivarli richiede limite di spesa, frequenza,
   arresto automatico e approvazione documentata.
3. Password, token, chiavi API, cookie, OTP, SPID, dati di pagamento e
   credenziali operative non entrano in Git, prompt, telemetria o log.
4. Dati personali, clienti, vendite e documenti aziendali possono raggiungere
   un modello esterno soltanto dopo approvazione esplicita, minimizzazione,
   informativa/base giuridica, accordi con il fornitore, retention definita,
   logging dei payload disabilitato e DPIA quando richiesta.
5. Nessun outreach commerciale autonomo. Ogni messaggio richiede revisione
   umana, base giuridica verificata, lista di esclusione e opt-out.
6. Nessun aggiramento di login, paywall, CAPTCHA o limiti tecnici. La raccolta
   usa solo fonti consentite e registra provenienza, licenza/termini, robots,
   data, quota e retention. Niente estrazione sistematica non autorizzata.
7. Trading, modifiche di rete/domotica, cancellazioni, acquisti e altre azioni
   con effetto reale richiedono autorizzazione umana specifica. DEMO e REAL
   devono essere separati e REAL non può riarmarsi al boot o al deploy.
8. Gli utenti devono sapere quando interagiscono con AI e poter ottenere una
   revisione umana. Output e inferenze non diventano fatti senza evidenza.
9. Accesso minimo necessario, cifratura, audit senza payload sensibili,
   backup/rollback testati e procedura incidenti sono prerequisiti di
   produzione.
10. Una modifica a modello, provider, fonti, dati, finalità, paesi, costi o
    automazioni riapre questa verifica prima del rilascio.

## Stato sicuro predefinito

In assenza di una decisione registrata il sistema deve fallire chiuso:
nessun deploy automatico, nessun cron a consumo, nessun dato personale verso
AI, nessun contatto automatico e nessuna azione reale.

Queste regole sono versionate nel repository. Non possono garantire conformità
“per sempre”: ogni rilascio deve rieseguire il gate rispetto a codice, uso e
normativa correnti.
