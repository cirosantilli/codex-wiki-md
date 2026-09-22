<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $u^2$ denote one-component [velocity](../../../../../../velocity.md) [variance](../../../../../../variance-split.md), $F=u^2f$ the [longitudinal velocity correlation](../../../../../../longitudinal-velocity-correlation.md), and $S_p=\langle(\Delta v)^p\rangle$ the signed [longitudinal structure functions](../../../../../../longitudinal-velocity-structure-function.md). Homogeneity gives $F=u^2-S_2/2$, while the third-order convention here is $u^3K=S_3/6$. Thus the [Kármán-Howarth equation](../../../../../../karman-howarth-equation.md) becomes

$$
\partial_tF=\frac1{r^4}\partial_r\left[r^4\left(\frac{S_3}{6}-\nu S_2'\right)\right].
$$

The mean [kinetic energy](../../../../../../kinetic-energy.md) per unit mass is $3u^2/2$, so its decay gives $\partial_tu^2=-2\epsilon/3$. In the [universal equilibrium range](../../../../../../equilibrium-range.md), the small-scale variation $\partial_tS_2$ is negligible at leading order, hence $\partial_tF\simeq-2\epsilon/3$. Integrating from zero and using regularity gives

$$
r^4\left(\frac{S_3}{6}-\nu S_2'\right)
=-\frac{2\epsilon}{3}\frac{r^5}{5}.
$$

The [Kolmogorov equation for structure functions](../../../../../../kolmogorov-equation-for-structure-functions.md) is therefore

$$
\boxed{S_3(r)-6\nu S_2'(r)=-\frac45\epsilon r}.
$$

For finite local unsteadiness the right side has the additional term $-3r^{-4}\int_0^r s^4\partial_tS_2(s,t)\,ds$; dropping it is the local-equilibrium approximation used here.

In the [inertial range](../../../../../../inertial-range.md) the viscous term is also negligible, leaving the [Kolmogorov four-fifths law](../../../../../../kolmogorov-four-fifths-law.md), **$S_3(r)=-4\epsilon r/5$**. Its coefficient and sign follow from the exact energy balance and [Kármán-Howarth equation](../../../../../../karman-howarth-equation.md), rather than from dimensional similarity. It supplies a firm third-order constraint on [Kolmogorov 1941 theory](../../../../../../kolmogorov-1941-theory.md) and measures the forward [energy cascade](../../../../../../energy-cascade.md), while leaving the second- and higher-order exponents open to [internal intermittency](../../../../../../internal-intermittency.md) corrections.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
