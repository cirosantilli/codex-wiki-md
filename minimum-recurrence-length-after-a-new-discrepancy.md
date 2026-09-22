# Minimum recurrence length after a new discrepancy

↑ **Parent:** [Berlekamp-Massey algorithm](berlekamp-massey-algorithm.md)

Suppose a connection polynomial $C$ of degree at most $L$, with recurrence span $L$ gives zero recurrence discrepancies through index $r-1$ but a nonzero discrepancy at $r$. If a polynomial $D$ of span $L'$ successfully explains the prefix through $r$ and $L+L'\leq r$, evaluate the coefficient at $r$ in the convolution $(CD)x$. Applying $D$ first makes it zero. Applying $C$ first leaves its nonzero discrepancy at $r$, because the earlier discrepancies vanish and $D$ has constant coefficient one. This contradiction gives the displayed lower bound. It is the minimality step used by the [Berlekamp-Massey algorithm](berlekamp-massey-algorithm.md); the algorithm cancels the new discrepancy with a shifted earlier failed polynomial.

## ↑ Ancestors (7)

1. [Berlekamp-Massey algorithm](berlekamp-massey-algorithm.md)
2. [Linear-feedback shift register](linear-feedback-shift-register.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/12j/solution.md)
