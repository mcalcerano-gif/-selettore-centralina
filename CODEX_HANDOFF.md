# Codex handoff — Selettore centralina

Aggiornato: 5 settembre 2026.

## Stato verificato

- Prototipo statico pubblico ospitato da GitHub Pages.
- Nessun database D1, Worker Cloudflare, servizio AI, cron, backend, cookie di
  autenticazione o dato cliente nel repository.
- Nessun workflow definito nel repository e nessun deploy automatico osservato
  dopo il build iniziale del sito (8 agosto 2026). GitHub espone soltanto il
  workflow Pages gestito dalla piattaforma.
- Il repository non ha partecipato all'anomalia D1 Cloudflare del 4 settembre
  2026 e non può generare letture D1 o costi AI.

## Regole per le prossime chat/agenti

Leggere integralmente `README.md` e `AI_DATA_GOVERNANCE.md` prima di modificare.
Conservare il progetto come calcolatore statico finché un backend non viene
progettato e approvato esplicitamente. Qualunque futura API, AI, telemetria,
raccolta dati o automazione deve partire disabilitata, avere budget e rate limit
hard, minimizzazione dei dati e deploy manuale verificato.

Non inserire dati clienti, credenziali o documentazione riservata nel repository
pubblico.
