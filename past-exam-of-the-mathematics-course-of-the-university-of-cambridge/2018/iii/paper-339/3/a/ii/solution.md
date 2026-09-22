<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Consider $B_n$ on the [finite-dimensional vector space](../../../../../../../finite-dimensional-vector-space.md) $E=\mathbb R[x]_{\le d}$ and use the monomial basis. For $j\ge1$, a [binomial distribution](../../../../../../../binomial-distribution.md) and the [falling factorial](../../../../../../../falling-factorial.md) moment formula give

$$
B_n(x^j)=\frac1{n^j}\sum_{\ell=0}^j S(j,\ell)(n)_\ell x^\ell,
$$

where $S(j,\ell)$ is the [Stirling number of the second kind](../../../../../../../stirling-numbers-of-the-second-kind.md) and $(n)_\ell=n(n-1)\cdots(n-\ell+1)$. This follows by expanding $K^j=\sum_\ell S(j,\ell)(K)_\ell$ and using $\mathbb E(K)_\ell=(n)_\ell x^\ell$. Also $B_n(1)=1$.

Each monomial maps to a polynomial of no larger degree. The resulting matrix is triangular with diagonal entries $1$ and $(n)_j/n^j$, $1\le j\le d$. When $n\ge d$ and $n\ge1$, all entries are positive. Therefore

$$
\boxed{B_n(E)\subseteq E,\qquad B_n:E\to E\text{ is invertible for }n\ge\max(1,d).}
$$

For constant polynomials the conclusion is immediate. Taking positive indices avoids the undefined sample expression $k/n$ at $n=0$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
