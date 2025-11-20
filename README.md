# semanticbold.sty — Semantic Boldness for Numeric Tables (40–40–20)

`semanticbold` is a lightweight LaTeX package that automatically applies
semantic boldness to numeric tables based on the **numeric value range**.
It performs a **two-pass scan** of your table to determine where each value lies
within the data distribution and highlights it accordingly:

- **Lowest 40% of numeric range** → *regular*
- **Middle 40%** → **bold**
- **Top 20%** → **extra-bold** (double overprint)

The package requires **no manual configuration** and works on standard LaTeX
installations (including Overleaf).

---

## Features

- Fully automatic: no thresholds needed.
- Works with any numeric table.
- Two-pass system: first collects values, second styles them.
- Highlights based strictly on **numeric range**, not rank.
- Safe for Overleaf (no advanced expl3 functions).
- Simple interface with two commands:
  - `\begin{semanticbold} ... \end{semanticbold}`
  - `\SBnum{<number>}`

---

## Installation

Copy `semanticbold.sty` into your project folder.  
Load it in your preamble:

```latex
\usepackage{semanticbold}
