# Stockfleth for LaTeX

Works with **XeLaTeX** and **LuaLaTeX** (the engines that read OpenType fonts directly).

1. Put `stockfleth.sty` and the `Stockfleth-*.otf` files from this folder next to your `.tex` file
   (or install the OTFs as system fonts / into your TEXMF tree).
2. In your preamble:

   ```latex
   \usepackage{stockfleth}              % Stockfleth as the typewriter font (\ttfamily, \texttt, verbatim, listings)
   \usepackage[main]{stockfleth}        % ...and as the main text font
   \usepackage[ligatures]{stockfleth}   % keep the fi / fl / ff pairs (off by default, best for code)
   ```

3. Compile with `xelatex` or `lualatex`. `stockfleth-example.tex` shows weights, code, languages and symbols.

Weights are reached with `\fontseries{...}`: `ul` hairline · `el` thin · `l` light · `m` regular · `mb` medium ·
`sb` semibold · `b` bold · `eb` extrabold · `ub` black. `\stockflethultra` gives the heaviest cut, and
`\textstockfleth{...}` sets a run of text in Stockfleth without changing your other fonts.

pdfLaTeX is not supported: it cannot read OpenType fonts without converting them to its older format.

Free for personal and trial use; commercial use needs a licence (see `LICENSE.md`). © 2026 marywildesign.
