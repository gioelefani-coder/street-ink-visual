# Supporti, palette, card

## Palette

| Nome | Hex | Uso |
|---|---|---|
| Inchiostro | `#121014` | contorni, neri pieni, ombre di contatto |
| Bianco | `#F8F7F2` | luci, jersey, occhi, muri |
| Cemento | `#6F7175` | marciapiede chiaro, pavimento |
| Asfalto | `#4A4C4B` | strada, cortile |
| Giunto | `#2E3030` | fughe, crepe, ombre |
| Crema | `#F0E3C4` | fondi per tavole e card |
| Cielo | `#86C8E4` | cielo, vetrine |
| Mattone | `#8E4A3A` | muri, cortili |
| Saracinesca | `#9AA0A0` | serrande, lamiere |
| Vetro | `#B9D6DE` | vetrine, finestre |

Accenti (2–3): rosso `#CB2027`, giallo `#F6D22C`, blu `#23509E`, verde `#2F6B3D`, oro `#E1A72B`, arancio `#E0662A`. Pelo: `#C07C3C` / `#8A5326` / `#A9ABA8`.
Combinazioni: marciapiede (cemento, bianco, rosso, giallo, oro) · vetrina (crema, blu, rosso, cielo) · tuta (asfalto, verde, giallo) · notte (asfalto, oro, rosso) · cortile (mattone, muschio, crema) · due colori (crema, nero + un accento).
Regole: max 5 colori oltre a nero e bianco; un solo accento caldo dominante; fondo neutro e desaturato; ombre col tono base più scuro, nero pieno solo per contatti e inchiostro; testo bianco su nero o nero su crema/giallo.

## Adattamenti per supporto

- **Logo**: silhouette chiusa, contorno 4 px, 2 colori + nero, leggibile a 24 px, senza ambiente.
- **Icone**: griglia 24 px, stroke 2 px, forme chiuse, un solo dettaglio pieno, luce da un lato, nessuna ombra di contatto.
- **Poster**: 2:3 o 3:4, tre strati, quattro livelli di tratto se stampa grande, titolo composto a parte mai sopra il viso.
- **Etichetta**: bande piatte, telaio nero, 3 colori + nero, testo minimo 8 pt.
- **Editoriale**: una scena comica che spiega il concetto in 2 secondi, con ambiente riconoscibile e spazio per il titolo.
- **Social**: 1:1 o 4:5, 9:16 storie, soggetto nel 55% centrale, leggibile in thumbnail a 200 px.
- **Merch**: grafica 30–35 cm, max 4 colori, funziona su nero (contorni in panna) e su bianco.
- **Sticker**: bordo bianco 8 px + contorno nero, ombra netta offset, 3 colori.
- **Pattern**: 5–9 elementi a due scale su fondo neutro piatto.
- **UI / empty state**: 1 colore + 1 accento, contorno 2–3 px, fondo trasparente o crema. Per una schermata completa: fondo finestra, pannelli con ombra di stack, schermi incassati, manopole con tacca (vedi `depth-details.md` §10).
- **Infografica**: blocchi a bordo nero 3 px, numeri grossi, colore solo sul dato chiave.

## Character card (pipeline ibrida)

L'immagine generata è **solo la figura**: anagrafica, statistiche, griglia e firma si compongono in HTML/CSS/SVG con testi veri. Test reale: in un colpo solo escono testo storpiato, 18 scarpe identiche, capi duplicati, corpo umano con testa animale.

1. **Tavola** su fondo crema piatto o muro street a linea, senza testo.
2. **Un oggetto per immagine**, fondo crema, poi ritaglio.
3. **Icone** SVG a linea.
4. **Pannello** 1024×1024: margine 24, cornice nera 4, colonna sinistra 300 (ritratto 300×240, anagrafica 300×170, statistiche 300×175 con 1–20, griglia 2×3) e colonna destra 636 con figura alta 460–520 e linee di richiamo 1 px.
5. Tipografia condensata 700 maiuscola, minimo 13 px. Firma in basso a destra, ruotata −2°.

Controllo: oggetti tutti diversi, etichette corrette, corpo animale completo, contorni gerarchici, ombre di contatto, riduzione al 25% leggibile.
