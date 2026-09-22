<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $m=F^{-1}(1/2)$. Since $F$ has an everywhere positive density, it is continuous and strictly increasing, so $F(m)=1/2$. Membership in the [Kolmogorov neighborhood of a distribution](../../../../../../kolmogorov-neighborhood-of-a-distribution.md) gives

$$
\Phi(m)-\varepsilon\leq\frac12\leq\Phi(m)+\varepsilon.
$$

By the symmetry of the [standard normal distribution](../../../../../../standard-normal-distribution.md),

$$
-\Phi^{-1}\left(\frac12+\varepsilon\right)
\leq m\leq
\Phi^{-1}\left(\frac12+\varepsilon\right).
$$

The stated asymptotic-bias formula for the [sample median](../../../../../../sample-median.md) therefore yields

$$
\boxed{\sup_{F\in\mathcal P_\varepsilon^K(\Phi)\cap\mathcal M}
b(\{T_n\},F)\leq b_1},
\qquad
b_1=\Phi^{-1}\left(\frac12+\varepsilon\right).
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
