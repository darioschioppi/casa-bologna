# Casa Bologna 🏠

Repository per organizzare la ricerca casa nel Comune di Bologna: mappatura delle agenzie immobiliari sul territorio, contatti, persone da sentire e stato delle visite.

## Struttura

- [`agenzie.json`](./agenzie.json) — elenco delle agenzie immobiliari con contatti e stato di avanzamento.
- [`index.html`](./index.html) — vista card con ricerca e filtri (GitHub Pages).
- [`mappa.html`](./mappa.html) — mappa interattiva con pallini geolocalizzati (GitHub Pages).
- [`zone-bologna.md`](./zone-bologna.md) — elenco dei quartieri/zone del Comune di Bologna, utile per organizzare la ricerca per area.
- [`note-visite.md`](./note-visite.md) — diario delle visite/chiamate fatte, con impressioni e follow-up.

## Come usare `agenzie.json`

È un array di oggetti, uno per agenzia. Campi:

| Campo | Descrizione |
|---|---|
| `nome_agenzia` | Nome dell'agenzia immobiliare |
| `zona` | Quartiere/zona di Bologna in cui opera o ha sede |
| `indirizzo` | Indirizzo della sede (se noto) |
| `telefono` | Numero di telefono |
| `email` | Email di contatto |
| `sito_web` | Sito web / pagina annunci |
| `persona_contatto` | Nome della persona referente (se nota) |
| `stato` | `da contattare` / `contattata` / `appuntamento fissato` / `visitata` / `scartata` |
| `data_ultimo_contatto` | Data dell'ultimo contatto (YYYY-MM-DD) |
| `note` | Note libere (immobili proposti, feedback, prossimi passi) |
| `google_maps_url` | Link Google Maps verificato manualmente (opzionale; se assente, il sito ne calcola uno dalle coordinate geocodificate) |

Esempio di una voce:

```json
{
  "nome_agenzia": "Interim - Immobili di Pregio",
  "zona": "Centro",
  "indirizzo": "Via dell'Indipendenza 63",
  "telefono": "051 241224",
  "email": "info@interimimmobilidipregio.it",
  "sito_web": "https://interimimmobilidipregio.it/",
  "persona_contatto": "Esmeralda",
  "stato": "contattata",
  "data_ultimo_contatto": "2026-09-06",
  "note": "Agente Esmeralda, contatto WhatsApp +39 3290310425.",
  "google_maps_url": "https://maps.app.goo.gl/esempio"
}
```

Puoi modificare il file JSON direttamente su GitHub (editor web) mantenendo la struttura ad array di oggetti.

## Obiettivo

Tenere traccia in modo centralizzato di:
1. Tutte le agenzie immobiliari presenti sul territorio del Comune di Bologna.
2. I contatti e le persone di riferimento per ciascuna.
3. Lo stato di avanzamento (chi è stato contattato, chi va contattato, appuntamenti fissati).
