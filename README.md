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

No reuse license has been selected yet. Until one is added, please do not
assume permission to redistribute or modify the material.
