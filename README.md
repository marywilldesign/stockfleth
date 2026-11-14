# stockfleth

A mono font drawn line by line on a 5 × 9 grid: variable, and fluent in Latin-script European languages and every Sámi alphabet.

**Live specimen:** https://marywildesign.com/stockfleth/

## Axes

| axis | tag | range |
|---|---|---|
| weight | `wght` | 100–1000 |
| width | `wdth` | 70–145 |
| *italic* (slant) | `slnt` | 0 to −12° |

Named styles (Google Fonts names): Thin, ExtraLight, Light, Regular, Medium, SemiBold, Bold, ExtraBold, Black, each upright and *italic*. The weight axis runs on to 1000, which the static download includes as ExtraBlack.

## Character set

361 characters: ASCII, the Western European set (Windows-1252 / Latin-1), the Central and Eastern European letters of the Google Fonts Latin Core set (Polish, Czech, Slovak, Hungarian, Romanian, Turkish, Baltic, Maltese, Welsh and more), combining accents, and every Latin-script Sámi alphabet (Northern, Lule, Southern, Ume, Pite, Inari and Skolt: Č Đ Ŋ Ŧ Ʒ Ǯ Ǧ Ǥ Ǩ ʹ): accented letters, curly quotes, dashes, €, £, ©, ™, fractions, arrows, ✓ ✗ and more. Strictly monospaced: every character takes the same width (combining accents take none and sit on the letter before them). The `fi`, `fl`, `ff`, `ft` and `fj` ligatures swap in single-cell alternates that sit a little closer together, and `->`, `=>` and `<-` join into single arrows drawn across their two cells (the Fira Code / JetBrains Mono approach), so columns never shift. Turn them off with `font-variant-ligatures: none` or your editor's ligature setting.

**Small capitals** (`font-variant-caps: small-caps` or `all-small-caps`, OpenType `smcp` / `c2sc`): the capitals redrawn at x-height with full-weight strokes, so they don't look pale like a browser's fake small caps. **Underline and strikethrough** positions and thicknesses are set in the font (80% of the letter stroke) and follow the weight. On the web, browsers draw their own heavier lines unless you add `text-decoration-thickness: from-font`.

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

## About the specimen's "fit" mode

The **fit** button on the specimen page is a feature of the page, not of the font file: a small script picks a width-axis value and size for each line until it fills the box. The downloaded font is variable (weight, width, slant); to get the same fitting elsewhere you would script it the same way.

## Licence

Free for **personal and trial use**. Commercial use needs a separate licence. See [LICENSE.md](LICENSE.md) and get in touch via [marywildesign.com](https://marywildesign.com).

---

by [marywildesign](https://marywildesign.com)
