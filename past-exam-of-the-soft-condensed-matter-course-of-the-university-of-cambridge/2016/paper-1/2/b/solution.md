<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Flory interaction parameter](../../../../../flory-interaction-parameter.md) $\chi$ measures the excess cost of unlike segment contacts. In a simple lattice with coordination number $z$, contact [energies](../../../../../energy-split.md) $\epsilon_{AA},\epsilon_{BB},\epsilon_{AB}$ and [temperature](../../../../../temperature-split.md) $T$,

$$
\chi=\frac{z}{k_BT}\left[\epsilon_{AB}-\frac{\epsilon_{AA}+\epsilon_{BB}}2\right].
$$

A positive [Flory interaction parameter](../../../../../flory-interaction-parameter.md) penalizes unlike contacts; a negative value favors them. Mixing still depends on the balance with [entropy of mixing](../../../../../entropy-of-mixing.md), rather than the sign of $\chi$ alone.

For two [polymers](../../../../../polymer-split.md) of degrees of polymerization $N_A,N_B$, let $\phi$ be the [volume fraction](../../../../../volume-fraction.md) of species $A$. The [binary Flory-Huggins polymer blend](../../../../../binary-flory-huggins-polymer-blend.md) has mixing [free energy](../../../../../thermodynamic-free-energy.md) per lattice site

$$
\frac{f(\phi)}{k_BT}=\frac\phi{N_A}\ln\phi+
\frac{1-\phi}{N_B}\ln(1-\phi)+\chi\phi(1-\phi).
$$

The logarithmic terms favor mixing. Their factors $1/N_A$ and $1/N_B$ arise because an entire chain translates as one object; connecting many segments greatly reduces the mixing [entropy](../../../../../entropy-split.md) per segment. Hence long [polymers](../../../../../polymer-split.md) can demix for a much smaller positive [Flory interaction parameter](../../../../../flory-interaction-parameter.md) than small [molecules](../../../../../molecule-split.md).

For composition-independent $\chi$, the local stability criterion is

$$
\frac{f''(\phi)}{k_BT}=
\frac1{N_A\phi}+\frac1{N_B(1-\phi)}-2\chi.
$$

Positive curvature means stability to small composition fluctuations, zero curvature locates the [spinodal](../../../../../spinodal.md), and negative curvature means spontaneous growth of fluctuations. Actual two-phase coexistence is determined by the [common-tangent construction](../../../../../common-tangent-construction.md), or equality of both species' [chemical potentials](../../../../../chemical-potential-split.md); its boundary is the [binodal](../../../../../binodal.md). A locally stable but globally unfavourable homogeneous [mixture](../../../../../mixture-split.md) can lie between the [binodal](../../../../../binodal.md) and [spinodal](../../../../../spinodal.md).

Setting the second and third [derivatives](../../../../../derivative.md) of $f$ to zero gives

$$
\phi_c=\frac{\sqrt{N_B}}{\sqrt{N_A}+\sqrt{N_B}},\qquad
\chi_c=\frac12\left(N_A^{-1/2}+N_B^{-1/2}\right)^2.
$$

For the [symmetric Flory-Huggins polymer blend](../../../../../symmetric-flory-huggins-polymer-blend.md), **$\phi_c=1/2$ and $\chi_c=2/N$**. For a [polymer solution](../../../../../polymer-solution.md) with $N_B=1$ and long chains of species $A$, $\chi_c\to1/2$, consistent with the [theta solvent](../../../../../theta-solvent.md) limit. An effective [Flory interaction parameter](../../../../../flory-interaction-parameter.md) can depend on [temperature](../../../../../temperature-split.md) and composition; in the simple energetic case $\chi\propto1/T$, heating encourages mixing, but that temperature trend is not universal.

<a id="2/b/image-increasing-the-flory-interaction-parameter-can-destroy-stability-of-a-symmetric-polymer-blend"></a>
![](../../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1-polymer-mixing.png)

**[Figure 1](#2/b/image-increasing-the-flory-interaction-parameter-can-destroy-stability-of-a-symmetric-polymer-blend). Increasing the Flory interaction parameter can destroy stability of a symmetric polymer blend**.

The original illustration uses stipulated $N_A=N_B=100$. At $\chi=0.01$ the mixing [free energy](../../../../../thermodynamic-free-energy.md) is convex, whereas at $\chi=0.03$ a central unstable region appears. The horizontal [common-tangent construction](../../../../../common-tangent-construction.md) in the latter case joins the symmetric coexisting compositions; its contacts differ from the [spinodal](../../../../../spinodal.md) boundaries. These are model curves, not supplied experimental data.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
