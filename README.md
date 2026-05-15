# Exercise 5 — Linear Systems and Stationary Iterative Methods

Numerical Analysis 2026 / Lecture 5 assignment bundle.

This repository contains **Ex 5.0--5.3**. The handout is shared with
Lecture 6, but this repository and deadline are separate from Exercise 6.

---

## Files

| File | Topic |
|---|---|
| `linear-equations-handout.qmd` | **Ex 5.0** — your edited copy of the shared Lectures 5--6 handout (>= 3 Q&A blocks, focused on Sections 1--9) |
| `ex5-1.qmd` | **Ex 5.1** — explain matrix condition numbers and create well/ill-conditioned matrices |
| `ex5-2.qmd` | **Ex 5.2** — use those matrices to compare direct solvers: `solve` vs `inv` |
| `ex5-3.qmd` | **Ex 5.3** — implement Jacobi and Gauss-Seidel, then observe their behavior on prepared matrices |
| `requirements.txt` | Python packages used in the exercises |

For Ex 5.0, copy
[`050/linear-equations-handout.qmd`](https://github.com/waseda-num-analysis-2026/materials/blob/main/050/linear-equations-handout.qmd)
from the `materials` repository into the root of this repository, then add
Q&A blocks following
[`AI_TUTOR.md`](https://github.com/waseda-num-analysis-2026/materials/blob/main/AI_TUTOR.md).

---

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Then select the `.venv` interpreter in VS Code / Cursor.

---

## Render

```bash
quarto render linear-equations-handout.qmd
quarto render ex5-1.qmd
quarto render ex5-2.qmd
quarto render ex5-3.qmd
```

After rendering, open the generated `.html` files in your browser and check
that your answers, code output, figures, and Q&A blocks are visible.
Starting from Ex 5, the rendered HTML files and their supporting `*_files/`
folders are also part of the submission. This helps the instructor verify
exactly what you saw after rendering.

---

## Submission

```bash
git add .
git commit -m "Submit Ex 5"
git push
```

If a `*_files/` folder is not generated for a particular file, that is fine.
Commit all rendered HTML-related files that Quarto creates. The `.gitignore`
file is set up so that virtual environments, cache files, and Quarto
intermediate files are not submitted.

You may push as many times as you like before the deadline; the **last
commit before the deadline** will be graded.

**Deadline (JST):** May 21 (Thu), 23:59.

---

## Need help?

- Mattermost: <https://class.s-top.dev/numerical-analysis-2026/channels/question>
- Materials repo: <https://github.com/waseda-num-analysis-2026/materials>
- Lecture 5 slides: <https://waseda-num-analysis-2026.github.io/materials/050/5th.html>
- Shared handout: <https://waseda-num-analysis-2026.github.io/materials/050/linear-equations-handout.html>
