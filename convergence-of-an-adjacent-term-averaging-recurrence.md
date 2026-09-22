# Convergence of an adjacent-term averaging recurrence

↑ **Parent:** [Recurrence relation](recurrence-relation.md)

For $0<\alpha<1$, the successive differences satisfy $d_{n+1}=-(1-\alpha)d_n$. Summing the resulting [geometric series](geometric-series.md) gives

$$
x_n=x_0+\frac{x_1-x_0}{2-\alpha}\bigl[1-(\alpha-1)^n\bigr],\qquad
\lim_{n\to\infty}x_n=\frac{(1-\alpha)x_0+x_1}{2-\alpha}.
$$

Equivalently, the two-dimensional update [matrix](matrix.md) has [eigenvalues](eigenvalue.md) $1$ and $\alpha-1$, with only the second mode decaying. At $\alpha=0$, generic initial values instead alternate and do not converge.

## ↑ Ancestors (8)

1. [Recurrence relation](recurrence-relation.md)
2. [Sequence](sequence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematical-methods-i-course-of-the-university-of-oxford/2021/9/c/solution.md)
