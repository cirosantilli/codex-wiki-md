<h1 id="26k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take independent random variables $U_1,\ldots,U_d$, each uniform on $[0,1/2]$, and independent [Rademacher random variables](../../../../../../rademacher-distribution.md) $\varepsilon_1,\ldots,\varepsilon_{d-1}$. Define

$$
X_i=\varepsilon_iU_i\quad(1\leq i<d),
\qquad
X_d=\left(\prod_{i=1}^{d-1}\varepsilon_i\right)U_d,
$$

and let $\eta$ be the joint law of $(X_1,\ldots,X_d)$.

Each $X_i$ is uniform on $[-1/2,1/2]$. If the $d$th coordinate is omitted, the remaining signs are the independent $\varepsilon_i$. If coordinate $j<d$ is omitted, the remaining signs are

$$
(\varepsilon_i)_{i\ne j},
\qquad
\prod_{i=1}^{d-1}\varepsilon_i,
$$

which are again uniformly distributed over all $2^{d-1}$ sign vectors because this map from $(\varepsilon_1,\ldots,\varepsilon_{d-1})$ is a bijection. The independent magnitudes then show that every $(d-1)$-coordinate marginal is Lebesgue measure.

The full law is not $d$-dimensional Lebesgue measure, because

$$
\prod_{i=1}^d\operatorname{sgn}(X_i)=1
$$

almost surely, whereas this product is equally likely to have either sign under independent Lebesgue coordinates.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [26K](../../26k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
