<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $m_0=M_0/\rho_0$ and $f_0=F_0/\rho_0>0$ under the literal mass convention. Their dimensions are $[m_0]=L^4T^{-2}$ and $[f_0]=L^4T^{-3}$. [Dimensional analysis](../../../../../../dimensional-analysis.md) gives

$$
\boxed{L_J=\frac{m_0^{3/4}}{f_0^{1/2}}
=\frac{M_0^{3/4}}{\rho_0^{1/4}F_0^{1/2}}}.
$$

The [jet length](../../../../../../jet-length.md) compares source [momentum](../../../../../../momentum.md) with [buoyancy](../../../../../../buoyancy.md). The region near the source behaves as a [turbulent round jet](../../../../../../turbulent-round-jet.md); sufficiently far away, the [forced plume](../../../../../../forced-plume.md) behaves like a [pure plume](../../../../../../pure-plume.md). With the constant [entrainment coefficient](../../../../../../entrainment-coefficient.md) retained explicitly, substantial turning occurs over a length of order $\ell_J=L_J/\sqrt E$, where $E=2\alpha\sqrt\pi$. Statements involving $s\ll L_J$ or $s\gg L_J$ normally hold this dimensionless coefficient fixed.

Near the point source, $m\sim m_0$ and the [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) gives $q\sim E\sqrt{m_0}s$. Therefore

$$
m_z=m_0\sin\theta_0+\frac{Ef_0}{2\sqrt{m_0}}s^2+O(s^4),\qquad
\theta=\theta_0+\frac{Ef_0\cos\theta_0}{2m_0^{3/2}}s^2+O(s^4).
$$

Integrating the centreline tangent gives

$$
\begin{aligned}
x(s)&=s\cos\theta_0-\frac{Ef_0\sin\theta_0\cos\theta_0}{6m_0^{3/2}}s^3+O(s^5),\\
z(s)&=s\sin\theta_0+\frac{Ef_0\cos^2\theta_0}{6m_0^{3/2}}s^3+O(s^5).
\end{aligned}
$$

**To leading order the centreline is a straight [turbulent round jet](../../../../../../turbulent-round-jet.md) at its source inclination.** For the horizontal source, the first curvature is the [horizontal forced-plume trajectory](../../../../../../horizontal-forced-plume-trajectory.md)

$$
\boxed{z\sim\frac{Ef_0}{6m_0^{3/2}}x^3
=\frac{\alpha\sqrt\pi}{3L_J^2}x^3}.
$$

For a vertical source, $\cos\theta_0=0$, the trajectory stays vertical rather than developing this cubic transverse displacement. If $F_0=0$, there is no finite buoyancy-induced [jet length](../../../../../../jet-length.md) and the [turbulent round jet](../../../../../../turbulent-round-jet.md) remains straight.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
