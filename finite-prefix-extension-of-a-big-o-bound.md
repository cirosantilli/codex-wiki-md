# Finite-prefix extension of a big O bound

↑ **Parent:** [Big O notation](big-o-notation.md)

Let $f,g:\mathbb N\to\mathbb R$, with $g(n)\ne0$ everywhere. An eventual bound $|f(n)|\leq C|g(n)|$ can be made valid for all natural numbers by enlarging $C$ to the maximum of itself and the finitely many ratios $|f(n)|/|g(n)|$ before its cutoff. Conversely, a global bound is an eventual bound. Nonvanishing on the finite prefix is essential: $g(0)=0$, $f(0)=1$, and $f(n)=g(n)=1$ for $n\geq1$ give an eventual bound but no global one. The useful principle is that finitely many finite ratios cannot destroy a [big O notation](big-o-notation.md).

## ↑ Ancestors (6)

1. [Big O notation](big-o-notation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/2/b/solution.md)
