<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

By [diagonalizability](../../../../../../diagonalizable-matrix.md), $V$ has an [eigenbasis](../../../../../../eigenbasis.md) $e_1,\ldots,e_m$ with $Te_j=\lambda_je_j$. Arrange the [basis](../../../../../../basis.md) so that $\lambda_1=\cdots=\lambda_r=0$ and the remaining [eigenvalues](../../../../../../eigenvalue.md) are nonzero. If there are no zero or no nonzero [eigenvalues](../../../../../../eigenvalue.md), the corresponding [linear span](../../../../../../linear-span.md) below is simply the zero [vector subspace](../../../../../../vector-subspace.md).

For $v=\sum_j a_je_j$, the equation $Tv=0$ holds precisely when $a_j=0$ for every $j>r$. Thus

$$
\ker T=\operatorname{span}\{e_1,\ldots,e_r\}.
$$

Every output is in $\operatorname{span}\{e_{r+1},\ldots,e_m\}$, and conversely $e_j=T(\lambda_j^{-1}e_j)$ for each $j>r$. Therefore

$$
\operatorname{im}T=\operatorname{span}\{e_{r+1},\ldots,e_m\}.
$$

These two disjoint parts of a [basis](../../../../../../basis.md) span $V$ and their [linear spans](../../../../../../linear-span.md) intersect only at zero. This is exactly the [direct sum of vector spaces](../../../../../../direct-sum.md) assertion

$$
\boxed{V=\ker T\oplus\operatorname{im}T.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
