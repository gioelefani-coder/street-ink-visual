# street-ink-visual

Skill estetica per agenti AI: **cartone animato a inchiostro con cel shading**, cultura sneaker/street anni '90. Un sistema, non un elenco di ricette — vale per illustrazioni, card, poster, loghi, icone, etichette, social, merch e UI.

Non è una skill di processo: fornisce lo strato visivo (identità, palette, gerarchia dei tratti, ambiente, catalogo dei dettagli, specifiche per supporto) da innestare in un brief prodotto altrove.

## File

| File | Contenuto |
|---|---|
| `SKILL.md` | nucleo: identità, palette, dettaglio per scala, composizione, ambiente, profondità, soggetti, prompt, anti-pattern, workflow |
| `depth-details.md` | gerarchia 3:2:1, le quattro ombre, regola del gancio, catalogo dei dettagli per oggetto, quattro livelli (L1–L4) e budget dei segni, profondità nelle UI piatte |
| `prompting.md` | grammatica del prompt, esempio di riferimento completo, blocco "dettagli al massimo", tabella correzioni |
| `street-environment.md` | i tre strati, vocabolario dei segni per ambiente, sei ricette di scena, palette ambiente, densità 60/30/10 |
| `supporti.md` | tabella palette con hex, adattamenti per supporto (logo, icone, poster, social, merch, sticker, UI…), pipeline della character card |

## Regole non negoziabili

- Contorno nero pieno e chiuso, spessori gerarchici 3:2:1 (poi L1–L4 per il massimo dettaglio).
- Colori piatti e saturi, max 5 oltre a nero e bianco; un solo accento caldo dominante.
- Ombre geometriche piene a bordo netto, una sola direzione; ombre di contatto e occlusioni.
- Nessuna texture sovrapposta: niente gradienti, blur, retino, grana, 3D.
- L'ambiente non è mai vuoto: densità 60/30/10.
- Il testo non si genera mai nell'immagine: si compone a parte in HTML/CSS/SVG.

## Installazione

Come skill di progetto, copia la cartella in `.agents/skills/street-ink-visual/` (oppure carica `SKILL.md` come skill dell'account). I quattro file di riferimento restano accanto a `SKILL.md`.

## Licenza

MIT.
