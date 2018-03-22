## Lantian theme

---

Forked from the [Metropolis repository](https://github.com/matze/mtheme). This is my own lightly customized version of the Metropolis beamer theme so I can keep the Metropolis theme installed alongside my customizations. It is bloated with custom math and tikz commands so not recommended for quick, lightweight presentations.

## Installation

Installing lantian from source, like any Beamer theme, involves four easy
steps:

1. **Download the source** with a `git clone` of the [Lantian repository](https://github.com/Stefan-Endres/mtheme) or as a [zip archive](https://github.com/Stefan-Endres/mtheme/archive/master.zip) of the latest development version.

2. **Compile the style files** by running `make sty` inside the downloaded
    directory. (Or run LaTeX directly on `source/lantiantheme.ins`.)

3. **Move the resulting `*.sty` files** to the folder containing your
   presentation. To use Metropolis with many presentations, run `make install`
   or move the `*.sty` files to a folder in your TeX path instead (might require
   `sudo` rights).

4. **Use the theme for your presentation** by declaring `\usetheme{lantian}` in the preamble of your Beamer document.

5. On Arch linux, to install in shared tex libraries run
`# sudo bash install`
`# mktexlsr`

## Usage

The following code shows a minimal example of a Beamer presentation using
Lantian.

```latex
\documentclass{beamer}
\usetheme{lantian}           % Use metropolis theme
\title{A minimal example}
\date{\today}
\author{Matthias Vogelgesang and Stefan Endres}
\institute{Centre for Modern Beamer Themes}
\begin{document}
  \maketitle
  \section{First Section}
  \begin{frame}{First Frame}
    Hello, world!
  \end{frame}
\end{document}
```

## License
(Copyright 2015 Matthias Vogelgesang)

The theme itself is licensed under a [Creative Commons Attribution-ShareAlike
4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/). This means that if you change the theme and re-distribute it, you *must* retain the copyright notice header and license it under the same CC-BY-SA license. This does not affect the presentation that you create with the theme.
