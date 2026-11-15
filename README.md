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

**Which weights for which sizes:** Thin and ExtraLight are display weights, for 24 px / 18 pt and up. For text below about 16 px / 12 pt use Light or heavier; Regular and Medium suit body text and code.

## Character set

365 characters: ASCII, the Western European set (Windows-1252 / Latin-1), the Central and Eastern European letters of the Google Fonts Latin Core set (Polish, Czech, Slovak, Hungarian, Romanian, Turkish, Baltic, Maltese, Welsh and more), combining accents, and every Latin-script Sámi alphabet (Northern, Lule, Southern, Ume, Pite, Inari and Skolt: Č Đ Ŋ Ŧ Ʒ Ǯ Ǧ Ǥ Ǩ ʹ): accented letters, curly quotes, dashes (hyphen, en dash, and an em dash that runs edge to edge so a row of them makes one line), €, £, ©, ™, ≠ ≤ ≥ ∞, fractions, arrows, ✓ ✗ and more. Strictly monospaced: every character takes the same width (combining accents take none and sit on the letter before them, rising above capitals and tall letters like b, d, h, k and l). The f is centred on its stem like i, l and t, so words such as "fifty" and "if" space evenly with no f-ligatures needed. `->`, `=>` and `<-` join into single arrows drawn across their two cells (the Fira Code / JetBrains Mono approach), so columns never shift. Turn them off with `font-variant-ligatures: none` or your editor's ligature setting.

**Small capitals** (`font-variant-caps: small-caps` or `all-small-caps`, OpenType `smcp` / `c2sc`): the capitals redrawn at x-height with full-weight strokes, so they don't look pale like a browser's fake small caps. Every accented and Sámi letter has one too (á, č, đ, ŋ, ø, æ...), so small-caps words never fall back to a lowercase letter. **Underline and strikethrough** positions and thicknesses are set in the font (80% of the letter stroke) and follow the weight. On the web, browsers draw their own heavier lines unless you add `text-decoration-thickness: from-font`.

## Metrics

Units per em: 1000. The outer edges of the strokes stay on these lines at every weight and width; heavier weights grow inward.

| line | height |
|---|---|
| ascender (b, d, f, h, k, l, t) | 750 |
| cap height and figures | 700 |
| x-height | 500 |
| maths axis (+ − = × ÷ ¬ ·, dashes, arrows) | 350 |
| baseline | 0 |
| descender | −200 |

Round letters overshoot each line by 10 (1% of the em), and pointed ones (v, w, V, W, arrow tips) a little more, so they look the same size as the flat letters. Superior figures hang from the cap height (330–700), as do the ordinals ª º (470–700). Every character is one cell wide: 600 units at width 100, from 420 at width 70 to 870 at width 145.

## Works everywhere

- **Design apps** (Figma, Adobe, Affinity, Sketch, Canva uploads): the variable TTF, or any static style.
- **Word, PowerPoint, Excel, Pages, Keynote**: install the static TTFs. Office has limited variable-font support, and on Windows it only embeds TrueType fonts in documents.
- **PDFs and shared documents**: the fonts allow editable embedding, so exported PDFs and saved Word, PowerPoint or Keynote files carry the font and stay editable for whoever opens them.
- **Websites**: the WOFF2 (see below).
- **Google Docs and Slides**: only offer Google's own font library, so no custom font can be used there.

## Files

| file | use |
|---|---|
| `fonts/Stockfleth-VF.ttf` | variable font for desktop apps (Figma, Adobe, macOS, Windows) |
| `fonts/Stockfleth-VF.woff2` | variable font for the web |
| `fonts/Stockfleth-static.zip` | the 20 static styles (Thin to ExtraBlack, upright and italic), as OTF and TTF. Use the TTFs in Word, PowerPoint and other Office apps: they embed in documents. |

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

## Character inspector

On the specimen page, hover over any character in the grid (or tap it on a tablet) to see it large against the lines above: ascender, cap height, x-height, baseline and descender, with dashed lines marking the edges of its cell. Alongside are its glyph name, Unicode name and code (decimal and hex), and the OpenType feature for small caps and ligatures. It follows the weight, width and slant sliders, and draws in the font's own units, so what it shows is where the font really puts each line. With a mouse or trackpad, click any character to copy it (the cursor turns into a +); a combining accent copies on its own, without the dotted circle. Combining accents are shown on a dotted circle; typed after a letter, they sit on that letter. On desktop the inspector sits to the right of the grid and stays in view as you scroll; phones show the grid on its own.

## About the specimen's "fit" mode

The **fit** button on the specimen page is a feature of the page, not of the font file: a small script picks a width-axis value and size for each line until it fills the box. The downloaded font is variable (weight, width, slant); to get the same fitting elsewhere you would script it the same way.

## Licence

Free for **personal and trial use**. Commercial use needs a separate licence. See [LICENSE.md](LICENSE.md) and get in touch via [marywildesign.com](https://marywildesign.com).

---

by [marywildesign](https://marywildesign.com)
