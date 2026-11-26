# Prompting — cel cartoon a inchiostro

## Grammatica

1. **Medium**: `cartoon cel-shaded illustration, 1990s urban style, bold black outlines`
2. **Scena**: chi è, cosa fa, cosa è andato storto
3. **Inquadratura**: `high angle` + `foreground element cropped at the edge`
4. **Livelli di tratto**: `9px silhouette, 4px structure, 2px surface, 1px micro-marks`
5. **Ombre**: `cast shadows as flat geometric shapes with crisp borders, same direction for every object, occlusion crescents at neck, armpits, jersey hem and between fingers`
6. **Ambiente**: `street environment: cracked asphalt, pavement joints, drain cover, gum spots, stickers, brick wall, shutter`
7. **Proporzioni**: `stubby cartoon proportions, big head, short thick limbs, mitt hands`
8. **Dettagli**: lista dei segni per oggetto (`depth-details.md` §8) + micro-segni dal budget (§9)
9. **Negativi fissi, sempre**: `no gradients, no soft shadows, no blurred edges, no texture overlay, no halftone dots, no 3D, no text, no empty floor`
10. **Palette** con hex e **formato** 1:1 / 4:5 / 3:4 / 2:3 / 16:9

## Regole

- **Indumenti e accessori nominati con volume**: `baggy jersey hanging loose`, `thick gold chain necklace hanging forward`.
- **I dettagli si elencano come segni, non come aggettivi**: "molto dettagliato" non produce nulla; `metal eyelets, stitched collar band, one missing brick` sì.
- **I punti di volume si elencano**: collo, ascelle, orlo, fra le dita.
- **Micro-segni dentro le aree piatte**, mai sul contorno; densità che sale verso il punto focale.
- **Spessori in pixel** quando serve precisione.
- **Per una UI** non si chiede prospettiva: si chiedono pannelli piatti, ombra di stack, schermi incassati e tacche sulle manopole (`depth-details.md` §10).

## Esempi

### Scena street con jersey, catena e ombre geometriche (riferimento)
```
Cartoon cel-shaded illustration, 1990s urban sneaker culture style: a chunky anthropomorphic pigeon sneakerhead crouching on cracked asphalt, wearing a baggy white football jersey with red numbers and a thick gold chain necklace hanging forward, cleaning a red sneaker with a rag, tongue out in concentration, sweat drops. High angle, top-down view. Foreground: a huge yellow shop-frame corner and a drain cover cropped at the bottom edge, in flat silhouette shadow. Midground: the bird, an open sneaker box with tissue paper, a tipped blue soda can with a flat spill shape, a crumpled receipt, three cigarette butts, a gum spot, an oil stain as a flat black shape, a paper bag. Background: flat grey asphalt with pavement joints and a cracked patch, brick wall with a torn poster, grey roller shutter with a single-line graffiti tag, strip of pale blue sky. Thick closed black outlines with varied line weight (5px silhouette, 3px interior shapes, 1.5px details on laces, stitching, chain links and cracks), flat saturated cel colors, exactly one hard-edged shadow tone per form with no blending, cast shadows as flat geometric shapes with crisp borders and the same direction for every object, hard contact shadows under every object, occlusion crescents at neck, armpits, jersey hem and between fingers, white rim highlight strokes. Clean digital cartoon look, no gradients, no soft shadows, no blurred edges, no paper texture, no halftone, no text. Palette: black #121014, white #F8F7F2, asphalt #4A4C4B, cement #6F7175, red #CB2027, yellow #F6D22C, gold #E1A72B, brick #8E4A3A.
```
Perché funziona: `varied line weight` con i pixel dichiarati dà spessore; `one hard-edged shadow tone with no blending` + `flat geometric shapes` bloccano le sfumature; `same direction for every object` tiene insieme la scena; le occlusioni colpiscono i punti dove il volume si appiattisce; i capi sono nominati con volume.

### Blocco dettagli al massimo (da incollare in qualsiasi prompt)
```
Details, one object at a time: fur tufts at the neck and pointed tips along the silhouette; eye with pupil, white highlight, lid crease and brow hairs; mitt hands with knuckles, nails with pale moons and wrist folds; jersey with stitched shoulder seams, ribbed collar band, curled hem, armpit wedge folds and inner label; shorts with drawstring tips, side seam and knee folds; sneakers with laces one by one through metal eyelets, double stitching, tread blocks and worn heel; chain links drawn individually with a clasp and star glints; soda can with pull-tab ring, band as a line and one drip; crumpled paper bag with creased corners and a torn edge; box with tape strip, bubbles and a crooked label; drain cover with individual grate bars and one bent; staggered brick joints with chipped mortar and one missing brick; layered torn posters with peeling corners; fire escape with bolted treads, welds and rust patches; asphalt with branching cracks, a darker patched square and grass tufts in the cracks; cigarette butts with crushed filters, gum spots flattened. Micro-marks sit inside flat color areas, never on the outline; detail thickens at the face, hands, shoes and foreground, and thins toward the edges.
```

## Correzioni

| Problema | Aggiungi |
|---|---|
| Sfumature o 3D | `flat cel colors, hard-edged shadow shape, no gradients, no rendering` |
| **Ombre morbide** | `cast shadows as flat geometric shapes with crisp borders, no soft shadows, no blurred edges, no blending` |
| Sembra una stampa vecchia | `clean digital cartoon look, no paper grain, no halftone dots` |
| Colori spenti | `saturated primary accents, clean flat fills` |
| Personaggio realistico | `stubby proportions, big head, short thick limbs, mitt hands` |
| Posa da catalogo | `caught mid-action, comic expression, props scattered around` |
| Contorno debole | `very thick uniform black outlines, closed shapes` |
| Disegno piatto | `varied line weight, occlusion shadows where forms meet, hard contact shadows, overlapping double lines` |
| **Indumenti spariti** | `one garment of each type, worn, baggy fit, folds drawn with wedge shadows` |
| **Oggetti lisci o finti** | elenca i segni: `metal eyelets, stitched seams, chain links individually, creased paper, grate bars, one missing brick` |
| **Dettaglio uniforme** | `detail thickens at the focal point and thins toward the edges, micro-marks inside flat color` |
| **UI piatta o 3D** | `flat 2D interface, panels as stacked sheets with a solid offset shadow, recessed screens, ink tick marks on knobs, no perspective, no glossy highlights` |
| Ambiente vuoto | `cracked pavement with joints, drain cover, gum spots, brick wall, torn posters, foreground object at edge` |
| Troppo pieno | `60% calm surface, medium detail midground, fine detail only near the focal point` |
| Testo storpiato | `no lettering, no text, blank label areas` |
