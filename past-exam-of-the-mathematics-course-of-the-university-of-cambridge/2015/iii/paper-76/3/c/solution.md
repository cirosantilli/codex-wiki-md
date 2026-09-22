<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the convention required by the printed expansion:

$$
 Av_i=\sigma_i u_i,\qquad A^*u_i=\sigma_i v_i,\qquad \sigma_i>0,
$$

where $u_i\in Y$ and $v_i\in X$ form the positive-singular-value parts of the [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md). Consequently $A^*Av_i=\sigma_i^2v_i$. Apply part (b)'s polynomial to each such [eigenvector](../../../../../../eigenvector.md), using noisy data:

$$
 x_n^{(\delta)}=\sum_i\tau\sigma_i\sum_{j=0}^{n-1}(1-\tau\sigma_i^2)^j
 \langle y^{(\delta)},u_i\rangle v_i.
$$

The [geometric series](../../../../../../geometric-series.md) then gives the full inverse coefficient, or [Landweber full inverse filter](../../../../../../landweber-full-inverse-filter.md),

$$
\boxed{g_\alpha(\sigma)=\frac{1-(1-\tau\sigma^2)^{1/\alpha}}{\sigma},
\qquad \alpha=1/n,\quad n\in\mathbb N.}
$$

In particular, for the unrelaxed iteration $\tau=1$, $g_\alpha(\sigma)=[1-(1-\sigma^2)^{1/\alpha}]/\sigma$. The dimensionless [Landweber spectral filter](../../../../../../landweber-spectral-filter.md) is instead $\sigma g_\alpha(\sigma)$; the printed expression uses the full coefficient and therefore needs the denominator $\sigma$.

For each fixed finite $n$, the filter extends continuously at zero by $g_{1/n}(0)=0$, since $g_{1/n}(\sigma)=n\tau\sigma+O(\sigma^3)$ as $\sigma\to0$. Small [singular values](../../../../../../singular-value.md) are suppressed rather than immediately divided into noisy data. A component of $y^{(\delta)}$ in $\ker A^*$ contributes nothing. The parameter here is discrete: $1/\alpha$ is an integer. This matters when $1-\tau\sigma^2<0$; arbitrary real powers are not intended. A family for every $\alpha>0$ can use $n=\lfloor1/\alpha\rfloor$ instead.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
