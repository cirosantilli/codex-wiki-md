<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
P(\tau)=q\prod_{n\geq1}(1-q^n)^{24},
\qquad q=e^{2\pi i\tau}.
$$

The [infinite product](../../../../../../infinite-product.md) converges locally uniformly and never vanishes on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). With $D=q\,d/dq=(2\pi i)^{-1}d/d\tau$, logarithmic differentiation gives

$$
D\log P
=1-24\sum_{n\geq1}\sum_{r\geq1}nq^{nr}
=1-24\sum_{m\geq1}\sigma_1(m)q^m
=E_2.
$$

The product is unchanged by $T:\tau\mapsto\tau+1$. To study $S:\tau\mapsto-1/\tau$, define

$$
R(\tau)=\frac{P(-1/\tau)}{\tau^{12}P(\tau)}.
$$

Using the transformation law for the [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md),

$$
\frac{d}{d\tau}\log R
=\frac{2\pi i}{\tau^2}E_2(-1/\tau)-\frac{12}{\tau}-2\pi iE_2(\tau)=0.
$$

Thus $R$ is constant. At the fixed point $\tau=i$, one has $i^{12}=1$, so $R(i)=1$. Hence

$$
P(-1/\tau)=\tau^{12}P(\tau).
$$

The transformations under $S$ and $T$, which generate the [modular group](../../../../../../modular-group.md), show that $P$ is a weight-twelve [modular form](../../../../../../modular-form.md). Its Fourier expansion begins $q+O(q^2)$, so it is a [cusp form](../../../../../../cusp-form.md). The normalized element of $S_{12}(\Gamma(1))$ is unique by part (a), and therefore

$$
\boxed{\Delta(\tau)=q\prod_{n\geq1}(1-q^n)^{24}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
