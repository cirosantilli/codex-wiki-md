<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose the inverse norms did not tend to infinity. Some subsequence would satisfy $\|a_n^{-1}\|\leq C$. Since $a_n\to a$, for its large indices $\|a_n^{-1}(a-a_n)\|<1$. Then

$$
a=a_n\bigl(1+a_n^{-1}(a-a_n)\bigr)
$$

is invertible in $A$ by the [Neumann series](../../../../../../neumann-series.md), contradicting the hypothesis. Hence **$\boxed{\|a_n^{-1}\|\to\infty}$**, the [inverse norm divergence at noninvertible boundary points](../../../../../../inverse-norm-divergence-at-noninvertible-boundary-points.md) property.

If $a$ were invertible in $B$, then [continuity of inversion in a Banach algebra](../../../../../../continuity-of-inversion-in-a-banach-algebra.md) would give $a_n^{-1}\to a^{-1}$ in $B$. Explicitly, the same factorization around $a$ gives a [Neumann series](../../../../../../neumann-series.md) and the bound $\|a_n^{-1}-a^{-1}\|\leq\|a_n^{-1}\|\|a-a_n\|\|a^{-1}\|$, with the inverse norms locally bounded in $B$. Since every $a_n^{-1}$ belongs to the closed subalgebra $A$, so would $a^{-1}$. That would make $a\in G(A)$, again a contradiction. Therefore **$a\notin G_B(A)$**.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
