<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The zero means and orthogonality give the exact second moment

$$
\mathbb E A_N^2=\frac1{N^2}\sum_{n,m\leq N}\mathbb E(X_nX_m)=\frac1N.
$$

Thus $A_N\to0$ in $L^2$. [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) gives the requested [weak law of large numbers](../../../../../weak-law-of-large-numbers.md):

$$
\boxed{\mathbb P(|A_N|\geq\epsilon)\leq\frac1{N\epsilon^2}\longrightarrow0.}
$$

Independence is unnecessary; the stated second-moment orthogonality is sufficient.

For an explicit almost surely convergent subsequence take $N_j=2^j$. For each positive integer $m$,

$$
\sum_j\mathbb P(|A_{2^j}|\geq1/m)\leq m^2\sum_j2^{-j}<\infty.
$$

The [First Borel-Cantelli lemma](../../../../../borel-cantelli-first-lemma.md) makes only finitely many such exceedances occur. Intersecting the resulting probability-one events over $m$ gives **$A_{2^j}\to0$ almost surely**.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
