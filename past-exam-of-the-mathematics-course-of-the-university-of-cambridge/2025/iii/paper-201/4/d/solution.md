<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $p_n=\mathbb P(B_n\mid\mathcal F_{n-1})$, $S_n=\sum_{j\leq n}\mathbf1_{B_j}$, and $A_n=\sum_{j\leq n}p_j$. Then $M_n=S_n-A_n$ is a martingale with bounded increments and conditional variance at most $p_n$. On $\{A_\infty<\infty\}$, localization and the $L^2$ martingale convergence theorem make $M_n$ converge, so the integer-valued increasing sequence $S_n$ is finite. On $\{A_\infty=\infty\}$, applying martingale convergence to

$$
\sum_n\frac{\mathbf1_{B_n}-p_n}{1+A_n}
$$

and [Kronecker lemma](../../../../../../kronecker-lemma.md) gives $M_n/A_n\to0$. Hence $S_n/A_n\to1$ and $S_n\to\infty$. This is the [Conditional Borel-Cantelli lemma](../../../../../../conditional-borel-cantelli-lemma.md), and proves the two events equal almost surely.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
