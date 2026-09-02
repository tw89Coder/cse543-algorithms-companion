# CSE543 Algorithms Companion

A Feynman-style course companion and reference for **CSE543: Advanced
Algorithms for Communications and Information Security** at National Sun
Yat-sen University.

The book develops the five syllabus topics—metaheuristics, algorithms review,
mathematical optimization, approximation algorithms, and randomized
algorithms—through intuition, concrete examples, formal models, proofs,
counterexamples, exercises, and Feynman checks. Additional material is divided
into clearly marked appendix groups: complexity, security, and systems;
followed by limited-information algorithms and parallel/distributed heuristic
search.

> **Unofficial material.** This repository is maintained independently by YHL.
> It does not represent an official publication or position of National Sun
> Yat-sen University, its Department of Computer Science and Engineering, or
> the course instructor.

## Files

- `CSE543_feynman_preview.tex` — main XeLaTeX source
- `style/cse543book.sty` — centralized typography and visual styles
- `CSE543_feynman_preview.pdf` — compiled textbook

## Build

The project targets XeLaTeX and common Ubuntu TeX Live / Overleaf packages.
No shell escape is required.

```bash
latexmk -xelatex -interaction=nonstopmode -file-line-error CSE543_feynman_preview.tex
```

To remove generated intermediate files:

```bash
latexmk -C CSE543_feynman_preview.tex
```

## Typography

The preferred Chinese fonts are Noto Serif CJK TC and Noto Sans CJK TC, with
the TeX Live Fandol family used only as an explicit fallback. English prose and
mathematics use Libertinus Serif and Libertinus Math. The document is designed
for A4 single-page reading and continuous tablet scrolling.

## Status

Release candidate, dated September 2026. The compiled edition currently has
173 pages.

## License

Copyright © 2026 YHL.

- The textbook content—including `CSE543_feynman_preview.tex`, the compiled
  PDF, original figures, tables, and exercises—is licensed under the
  [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
  License](https://creativecommons.org/licenses/by-nc-sa/4.0/)
  (**CC BY-NC-SA 4.0**), except where otherwise noted.
- The standalone typography and build code in `style/cse543book.sty`, and any
  future helper scripts explicitly identified as code, are licensed under the
  MIT License.

When redistributing or adapting the textbook, give appropriate credit, link to
the CC license, indicate whether changes were made, and distribute adaptations
under the same license. The course title, course code, and public syllabus
information are used only for identification and curriculum alignment; no
endorsement by the university, department, or instructor is implied.

See [LICENSE.md](LICENSE.md) for scope and attribution guidance and
[LICENSE-CODE](LICENSE-CODE) for the code license.
