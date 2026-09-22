<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md) states that the [polynomials](../../../../../../polynomial-split.md) are a [dense subspace](../../../../../../dense-subspace.md) of $C[0,1]$ in the [supremum norm](../../../../../../supremum-norm.md). By [linearity](../../../../../../linearity.md) and (c), $B_np\to p$ uniformly for every [polynomial](../../../../../../polynomial-split.md) $p$. Given $f\in C[0,1]$ and $\varepsilon>0$, choose a [polynomial](../../../../../../polynomial-split.md) $p$ with $\|f-p\|_\infty<\varepsilon$. The [operator norm](../../../../../../operator-norm.md) estimate in (a) gives

$$
\|B_nf-f\|_\infty\le\|B_n(f-p)\|_\infty+\|B_np-p\|_\infty+\|p-f\|_\infty\le2\varepsilon+\|B_np-p\|_\infty.
$$

First let $n\to\infty$, then $\varepsilon\downarrow0$. Hence **$\|B_nf-f\|_\infty\to0$ for every continuous $f$**. This is an instance of [extension of approximation operators from a dense subspace](../../../../../../extension-of-approximation-operators-from-a-dense-subspace.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
