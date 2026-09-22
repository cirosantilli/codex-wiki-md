<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since the binary trait $Y$ has marginal [Bernoulli distribution](../../../../../../bernoulli-distribution.md) with probability $K=p\alpha^2$, its total [variance](../../../../../../variance-split.md) is

$$
\boxed{\operatorname{Var}(Y)=p\alpha^2(1-p\alpha^2).}
$$

Within a specified [genotype](../../../../../../genotype.md) $G=g$, the [conditional variance](../../../../../../conditional-variance.md) is $q_g(1-q_g)$. The within-genotype contribution to total variance is its average over the population:

$$
V_W=\mathbb E[q_G(1-q_G)]
=\mathbb E(q_G)-\mathbb E(q_G^2).
$$

Another [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md) average gives

$$
\mathbb E(q_G^2)
=p^2[(1-\phi)+\phi\theta^2]^2=p^2\beta^2,
\qquad\beta=1+\phi(\theta^2-1).
$$

Hence

$$
\boxed{V_W=p\alpha^2-p^2\beta^2.}
$$

By the [law of total variance](../../../../../../law-of-total-variance.md), the remaining between-genotype component is the [genetic variance of penetrance](../../../../../../genetic-variance-of-penetrance.md), namely

$$
\boxed{V_G=\operatorname{Var}(q_G)
=\operatorname{Var}(Y)-V_W=p^2(\beta^2-\alpha^4).}
$$

It is nonnegative, as a [variance](../../../../../../variance-split.md) must be. It also follows from $\beta-\alpha^2=\phi(1-\phi)(\theta-1)^2\geq0$. The single-genotype variance and its population average are different quantities; both have been specified.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
