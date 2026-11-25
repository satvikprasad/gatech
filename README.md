# gatech

Coursework from Georgia Tech, written in LaTeX.

## Building

Requires a TeX distribution with `latexmk` (e.g. BasicTeX) and these extra packages:

```sh
sudo tlmgr install algorithms algorithmicx bbm bbm-macros cmbright hfbright doublestroke enumitem titling
```

Every file includes the shared `header.tex` at the repo root, so build from inside a course folder with the root on `TEXINPUTS`:

```sh
cd math3235
TEXINPUTS="..:" latexmk -pdf -outdir=build HW10.tex
```

The PDF is written to `build/`.
