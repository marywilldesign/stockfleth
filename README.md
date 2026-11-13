# stockfleth

A mono font drawn line by line on a 5 × 9 grid: variable, adaptive, and fluent in the Nordic languages and every Latin-script Sámi language.

**Live specimen:** https://marywildesign.com/stockfleth/

## Axes

| axis | tag | range |
|---|---|---|
| weight | `wght` | 100–1000 |
| width | `wdth` | 70–145 |
| italic (slant) | `slnt` | 0 to −12° |

Named styles: Hairline, Thin, Light, Regular, Medium, Semibold, Bold, Extrabold, Black, Ultra, each upright and italic.

## Character set

246 characters: ASCII, the Western European set (Windows-1252 / Latin-1) and every Latin-script Sámi alphabet (Northern, Lule, Southern, Ume, Pite, Inari and Skolt: Č Đ Ŋ Ŧ Ʒ Ǯ Ǧ Ǥ Ǩ ʹ): accented letters, curly quotes, dashes, €, £, ©, ™, fractions, arrows, ✓ ✗ and more. Strictly monospaced: every glyph has the same advance width. The `fi`, `fl` and `ff` ligatures swap in single-cell alternates that sit a little closer together (the Fira Code / JetBrains Mono approach), so columns never shift; turn them off with `font-variant-ligatures: none` or your editor's ligature setting.

## Files

| file | use |
|---|---|
| `fonts/Stockfleth-VF.ttf` | variable font for desktop apps (Figma, Adobe, macOS, Windows) |
| `fonts/Stockfleth-VF.woff2` | variable font for the web |
| `fonts/Stockfleth-static-otf.zip` | 20 static OTFs for apps without variable-font support |
| `fonts/Stockfleth-latex.zip` | LaTeX package (`\usepackage{stockfleth}`, XeLaTeX / LuaLaTeX), example and the 20 OTFs |

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

## Licence

Free for **personal and trial use**. Commercial use needs a separate licence. See [LICENSE.md](LICENSE.md) and get in touch via [marywildesign.com](https://marywildesign.com).

---

by [marywildesign](https://marywildesign.com)
