<h1 id="15f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [character of a representation](../../../../../../character-of-a-representation.md) is its trace. The [exterior power](../../../../../../exterior-power.md) character is the elementary symmetric [polynomial](../../../../../../polynomial-split.md) of degree $n$ in the [eigenvalues](../../../../../../eigenvalue.md), so the specified sign convention $Q(g,X)=\det(g-XI)$ gives

$$
\boxed{Q(g,X)=\sum_{n=0}^d(-1)^{d-n}\chi_{\Lambda^nV}(g)X^{d-n}.}
$$

To obtain the [character generating series of symmetric powers](../../../../../../character-generating-series-of-symmetric-powers.md), sum the monomial [eigenvalues](../../../../../../eigenvalue.md) over all degrees. As an identity of [formal power series](../../../../../../formal-power-series.md),

$$
\boxed{\sum_{n\geq0}\chi_{S^nV}(g)t^n=\prod_{j=1}^d(1-\lambda_jt)^{-1}=\frac1{(-t)^dQ(g,t^{-1})}.}
$$

The apparent negative powers cancel in the denominator, which has constant term $1$. Equivalently, this series is the reciprocal of $\sum_{j=0}^d(-1)^j\chi_{\Lambda^jV}(g)t^j$. Comparing coefficients gives $\sum_{j=0}^{\min(d,n)}(-1)^j\chi_{\Lambda^jV}(g)\chi_{S^{n-j}V}(g)=0$ for $n>0$, an explicit recurrence computing the symmetric-power characters from $Q$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15F](../../15f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
