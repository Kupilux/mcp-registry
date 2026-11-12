# App Reviews Intelligence — voce nel registro MCP

Questo repository contiene la definizione (`server.json`) di **App Reviews Intelligence** per il [registro ufficiale MCP](https://registry.modelcontextprotocol.io): un server MCP che offre recensioni da App Store e Google Play con analisi AI su temi, bug e confronti con i competitor.

- **Actor Apify:** [App Reviews Intelligence](https://apify.com/kupilux/app-reviews-intelligence)

## Pubblicare nel registro

1. Apri **Actions** su GitHub.
2. Seleziona il workflow **Publish to MCP Registry**.
3. Clicca **Run workflow** ed eseguilo sul branch desiderato.

L’autenticazione avviene tramite GitHub OIDC: non servono secret nel repository.

## Aggiornare la voce

1. Modifica il campo `version` (e, se necessario, gli altri campi) in `server.json` alla radice del repository.
2. Esegui di nuovo il workflow **Publish to MCP Registry** come sopra.

## Rimuovere o deprecare la voce

1. Apri **Actions** → **Remove from MCP Registry** → **Run workflow**.
2. Scegli lo stato `deprecated` o `deleted`.
3. Nel campo di conferma digita esattamente: `io.github.Kupilux/app-reviews-intelligence`.

Il workflow aggiorna lo stato di tutte le versioni pubblicate per questo server.
