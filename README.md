# stockfleth

A variable monospace typeface drawn on a 5 × 9 module grid.

**Live specimen:** https://marywildesign.com/stockfleth/

## Axes

| axis | tag | range |
|---|---|---|
| weight | `wght` | 100–1000 |
| width | `wdth` | 70–145 |
| italic (slant) | `slnt` | 0 to −12° |

Named styles: Hairline, Thin, Light, Regular, Medium, Semibold, Bold, Extrabold, Black, Ultra, each upright and italic.

## Character set

219 characters: ASCII plus the Western European set (Windows-1252 / Latin-1): accented letters, curly quotes, dashes, €, £, ©, ™, fractions and more. Standard ligatures `fi`, `fl` and `ff` each take exactly two cells, so the grid holds.

## Files

| file | use |
|---|---|
| `fonts/Stockfleth-VF.ttf` | variable font for desktop apps (Figma, Adobe, macOS, Windows) |
| `fonts/Stockfleth-VF.woff2` | variable font for the web |
| `fonts/Stockfleth-static-otf.zip` | 20 static OTFs for apps without variable-font support |

### Web use

```css
@font-face {
  font-family: Stockfleth;
  src: url(Stockfleth-VF.woff2) format("woff2");
  font-weight: 100 1000;
  font-stretch: 70% 145%;
}
.headline { font-family: Stockfleth, ui-monospace, monospace; font-variation-settings: "wght" 700, "wdth" 120, "slnt" 0; }
```
