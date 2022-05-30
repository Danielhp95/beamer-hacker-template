# Beamer hacker template

Beamer template derived from [DarkConsoleTheme](https://www.overleaf.com/latex/templates/darkconsole-beamer-theme/yrqyrpvxzjvj), but cooler, in my opinion.

**NOTE:** `pdflatex` won't work with this template, I recommend using`lualatex`.

## Template structure:
+ `kmbeamer_color.sty`: Defines colors used throughout template (i.e: `\definecolor{lightorange}{HTML}{FFAF24}`)
+ `beamerthemeDarkConsole.sty`: Defines template layout (i.e footnotes, title page)
+ `beamercolorthemeDarkConsole.sty`: Defines colours for certain latex elements.


## Images

#### Title

![Title]{./sample_images/title.png)

#### Random frame

![random_frame]{./sample_images/math.png)

## Usage

1. Clone repo: `git clone https://github.com/Danielhp95/beamer-hacker-template`
2. Create latex entrypoint, or used provided file in `beamer-hacker-template/presentation.tex`:

```latex

% Aspect ratio is tweaked to fit more modern screen ratios
\documentclass[xcolor=dvipsnames, compress, aspectratio=169]{beamer}
\usetheme{DarkConsole}

\title{Presentation title}
\author{\textbf{Yours Truly}}

\begin{document}
\maketitle
% Your content goes here
\end{document}
```
3 - Compile using `lualatex presentation.tex`
