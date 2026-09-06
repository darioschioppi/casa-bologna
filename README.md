# Casa Bologna 🏠

Repository per organizzare la ricerca casa nel Comune di Bologna: mappatura delle agenzie immobiliari sul territorio, contatti, persone da sentire e stato delle visite.

## Struttura

- [`agenzie.csv`](./agenzie.csv) — elenco delle agenzie immobiliari con contatti e stato di avanzamento.
- [`zone-bologna.md`](./zone-bologna.md) — elenco dei quartieri/zone del Comune di Bologna, utile per organizzare la ricerca per area.
- [`note-visite.md`](./note-visite.md) — diario delle visite/chiamate fatte, con impressioni e follow-up.

## Come usare `agenzie.csv`

Colonne:

| Colonna | Descrizione |
|---|---|
| `nome_agenzia` | Nome dell'agenzia immobiliare |
| `zona` | Quartiere/zona di Bologna in cui opera o ha sede |
| `indirizzo` | Indirizzo della sede (se nota) |
| `telefono` | Numero di telefono |
| `email` | Email di contatto |
| `sito_web` | Sito web / pagina annunci |
| `persona_contatto` | Nome della persona referente (se nota) |
| `stato` | `da contattare` / `contattata` / `appuntamento fissato` / `visitata` / `scartata` |
| `data_ultimo_contatto` | Data dell'ultimo contatto (YYYY-MM-DD) |
| `note` | Note libere (immobili proposti, feedback, prossimi passi) |

Puoi aprire il CSV con Excel/Google Sheets/Numbers oppure modificarlo direttamente su GitHub.

## Obiettivo

Tenere traccia in modo centralizzato di:
1. Tutte le agenzie immobiliari presenti sul territorio del Comune di Bologna.
2. I contatti e le persone di riferimento per ciascuna.
3. Lo stato di avanzamento (chi è stato contattato, chi va contattato, appuntamenti fissati).
