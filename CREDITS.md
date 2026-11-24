# Credits

## LaTeX template

The CV's layout (centered bold section headings, `\hfill`-aligned dates,
compact `itemize` lists, and the page margins) started from this Overleaf
template:

- **Title:** CV - Harvard-like
- **Author:** Aline R. Antunes
- **Source:** https://www.overleaf.com/latex/templates/cv-harvard-like/mdwdzhtvvbhs
- **License:** [LaTeX Project Public License 1.3c](https://www.latex-project.org/lppl/lppl-1-3c/)
- **Imported:** November 2026 (the `Initial Overleaf Import` commit, `d858717`)

The template describes itself as "CV template similar to harvad CV".

### What changed from the template

- All CV content is Andrew Masker's; none of the template's sample text remains.
- The single `main.tex` was split into `preamble.tex` and `sections/*.tex`.
- Removed template packages this CV doesn't use: `graphicx`, `lipsum`
  (placeholder text), `inputenc` (UTF-8 is the LaTeX default), and
  `babel` with the `brazil` option (Brazilian Portuguese, which also
  applied Portuguese hyphenation to English text).
- Added `etaremune` for the reverse-numbered publication lists.

LPPL 1.3c asks that modified versions say they've been changed and where
the original came from; this file and the comment at the top of `main.tex`
cover that.

## Removed reference material

`tipsforCV.pdf`, which came in with the Overleaf import, was the Dartmouth
College Center for Professional Development *Resume Guide* (28 pages,
dated 2015–2017). It was removed because it's third-party material, not
part of the CV. It's still in this repo's history at commit `d858717`, and
Dartmouth's current guides are at https://careerdesign.dartmouth.edu/resources/.
