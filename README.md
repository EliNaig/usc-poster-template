<div align="center">

<img src="assets/usc-seal.png" alt="University of South Carolina seal" width="120">

# Unofficial University of South Carolina Research Poster Template

![University of South Carolina](https://img.shields.io/badge/University%20of%20South%20Carolina-73000A?style=flat-square&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)
![LuaLaTeX](https://img.shields.io/badge/Compiler-LuaLaTeX-2C5F8A?style=flat-square)
![Size](https://img.shields.io/badge/Size-48in%20x%2036in-BFA15A?style=flat-square)
![License: MIT](https://img.shields.io/badge/License-MIT-3DA639?style=flat-square)

</div>

A LaTeX [beamerposter] template in USC branding, based on the [Gemini] theme.

<p align="center">
<a href="poster.pdf">
<img src="preview.png" alt="Compiled poster preview" width="720">
</a>
</p>

## Files

| File | Purpose |
| --- | --- |
| `poster.tex` | The poster: title, authors, footer, content blocks |
| `beamercolorthemeusc.sty` | USC colors |
| `beamerthemegemini.sty` | Gemini layout theme |
| `logos/` | White USC logo and NSF logo |
| `poster.bib` | Bibliography |
| `.latexmkrc` | Selects LuaLaTeX for latexmk |

## Requirements

A **full** TeX Live 2024 or newer: it includes LuaLaTeX and `latexmk` (both
required; the theme's `fontspec` breaks pdflatex) and the Raleway/Lato fonts.

- **macOS:** [MacTeX] (`brew install --cask mactex`)
- **Windows:** [TeX Live] (full scheme)
- **Linux:** `texlive-full`

Or skip installing entirely and use [Overleaf](#use-on-overleaf).

## Build

```sh
latexmk poster.tex
```

## Use on Overleaf

Upload the repo ZIP as a new project and set the compiler to **LuaLaTeX**.
This GitHub repo is the canonical version.

## Customizing

- **Title, authors, footer:** top of `poster.tex`.
- **Size:** preset to 48in x 36in landscape (set in cm).
- **Colors:** `beamercolorthemeusc.sty`, using the official [USC brand colors].
- **Logos:** in the header via `\logoleft` and `\logoright` (drop the NSF
  logo if not NSF-funded); more variants in the [USC toolbox][USC logos].
- **Printing:** print from the PDF, and confirm the board size with your event.

## License

MIT (see [LICENSE.md](LICENSE.md)). Unofficial; not endorsed by the
University of South Carolina. Logos remain subject to USC brand guidelines.

[beamerposter]: https://github.com/deselaers/latex-beamerposter
[Gemini]: https://github.com/anishathalye/gemini
[MacTeX]: https://www.tug.org/mactex/
[TeX Live]: https://www.tug.org/texlive/
[USC brand colors]: https://sc.edu/about/offices_and_divisions/communications/toolbox/colors/
[USC logos]: https://sc.edu/about/offices_and_divisions/communications/toolbox/logos/
