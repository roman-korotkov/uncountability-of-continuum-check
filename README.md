# Uncountability of continuum, check

[![DOI](https://zenodo.org/badge/1463618412.svg)](https://doi.org/10.5281/zenodo.24361601)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Preface

This is the opening article in the series Uncountability of the Continuum. Its character is deliberately investigational: rather than offering a finished, self-contained solution, it traces a path of inquiry and invites the reader to follow the same line of thought.

What first drew me to the subject was a simple but persistent question: why has Cantor’s theorem on the uncountability of the continuum attracted so many attempts at refutation? The usual reply - "only cranks question it" - strikes me as unhelpfully dismissive and, in a certain sense, chauvinistic. No comparable resistance is directed at the Pythagorean theorem or the fundamental theorem of arithmetic. The sheer volume and longevity of the dissent therefore call for a more careful explanation.

When one returns to Cantor’s original writings, a striking fact emerges. His arguments rest on a number of additional, often tacit, prerequisites that have largely disappeared from the modern textbook presentations. These conditions are not accidental ornaments; they point toward a coherent alternative perspective on the foundational assumptions that underlie contemporary axiomatic set theory. Exploring that perspective is the central task of the series.

## Abstract

The paper critically re-examines the classical proof of the uncountability of the continuum via Cantor’s diagonal argument. Returning to naive mathematics, the author distinguishes potential and actual infinity and introduces two constructive sets on the unit interval: the potentially infinite C[0, 1] (the union of all finite binary expansions) and the actually infinite U[0, 1] (the set in which every digit position is defined). It is shown that, under potential infinity, the diagonal construction either never terminates or yields only a countable collection of limits, and therefore cannot establish the existence of a real outside the original set. Under actual infinity the applicability of the diagonal method hinges on further assumptions about the morphology of infinity - its universality, totality, and degree of reflexivity. A distinction is drawn between strong and weak interpretations of one-to-one correspondence. Analysis of Cantor’s original 1891 formulation reveals that the argument relies on the fixation of a universal, totally ordered coordinate system and is not generally valid outside these presuppositions. The author concludes that the diagonal argument by itself supplies no structural information about the relation between ℕ and ℝ; its correctness is determined by the adopted morphology of infinity.

## Repository Structure

```text
.
├── article_ru.tex      # Main LaTeX source file in Russian
├── article_ru.bib      # BibTeX bibliography
├── CITATION.cff        # Citation metadata for GitHub and Zenodo
├── LICENSE             # CC BY 4.0 license text
└── README.md           # Project overview and build instructions
```

## Compiling the Paper

To compile the PDF locally using `latexmk` (recommended, handles bibliography passes automatically):

```bash
latexmk -pdf article_ru.tex
```

Alternatively, run `pdflatex` and `bibtex` manually:

```bash
pdflatex article_ru.tex
bibtex article_ru
pdflatex article_ru.tex
pdflatex article_ru.tex
```

## How to Cite

If you reference this work, please cite it via Zenodo or use the following BibTeX entry (update the DOI after publishing your first GitHub release):

```bibtex
@misc{korotkov2026continuum,
  author       = {Korotkov, Roman},
  title        = {Uncountability of continuum, check},
  year         = {2026},
  publisher    = {Zenodo},
  version      = {v0.9.0},
  doi          = {10.5281/zenodo.24361601},
  url          = {https://doi.org/10.5281/zenodo.24361601}
}
```

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
