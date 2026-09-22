<h1 id="section-b/b4/solution">Solution</h1>

↑ **Parent:** [B4](../b4.md)

**Ideal and self-avoiding walks.** An [ideal chain](../../../../ideal-chain.md) has independent isotropic coarse-grained steps and permits self-intersections in its mathematical model. For $N$ steps of length $b$, the cross terms average to zero, so its root-mean-square [end-to-end distance of a polymer chain](../../../../end-to-end-distance-of-a-polymer-chain.md) obeys

$$
\boxed{\langle R^2\rangle=Nb^2,\qquad R_{\mathrm{rms}}\propto N^{1/2}}.
$$

A [self-avoiding walk](../../../../self-avoiding-walk.md) excludes repeated occupancy or intersection at the segment scale. This represents positive [excluded volume](../../../../excluded-volume.md) in a dilute [good solvent](../../../../good-solvent.md). The nonlocal constraint correlates otherwise distant portions of the chain and swells it:

$$
\boxed{R_{\mathrm{rms}}\propto bN^\nu,\qquad \nu\simeq0.588\quad\text{in three dimensions}}.
$$

The [Flory approximation](../../../../flory-approximation.md) replaces this exponent by $3/5$, by balancing stretching free energy $R^2/(Nb^2)$ with an interaction contribution $vN^2/R^3$. The result is a more extended and less internally dense coil than the ideal walk; self-avoidance changes the statistics, not merely the local step length.

**Two ideal-chain regimes.** At the [theta temperature](../../../../theta-temperature.md) for a dilute polymer–solvent pair, leading effective segment attractions and repulsions cancel. Large-scale chain statistics are approximately ideal, even though microscopic atoms still have finite size. In a homogeneous [polymer melt](../../../../polymer-melt.md), surrounding chains screen long-range [excluded volume](../../../../excluded-volume.md) interactions of a chosen chain, again making its equilibrium large-scale size approximately ideal. Local bond-angle correlations must be included in an effective statistical length such as the [Kuhn length](../../../../kuhn-length.md). [Polymer entanglements](../../../../polymer-entanglement.md) can slow the dynamics without invalidating this leading equilibrium size law.

**Semiflexible DNA.** The [nucleic acid double helix](../../../../nucleic-acid-double-helix.md) gives double-stranded [DNA](../../../../deoxyribonucleic-acid.md) a bending stiffness and substantial local orientational persistence. Independent step orientations are therefore a poor description on short scales, while self-avoidance alone does not specify the energy cost of bending. The [worm-like chain](../../../../worm-like-chain.md) describes the molecule as a continuously bendable, locally inextensible curve $\mathbf r(s)$ parameterized by [arc length](../../../../arc-length.md) $s$, with unit tangent $\mathbf t(s)=d\mathbf r/ds$. Its bending energy is

$$
E_b=\frac A2\int_0^L\left|\frac{d\mathbf t}{ds}\right|^2ds,\qquad |\mathbf t|=1,
$$

where $A$ is [bending stiffness](../../../../bending-stiffness.md). In the free three-dimensional model, the [persistence length](../../../../persistence-length.md) is $\ell_p=A/(k_BT)$ and

$$
\boxed{\langle\mathbf t(s)\cdot\mathbf t(s+u)\rangle=e^{-u/\ell_p}}.
$$

Thus $\ell_p$ is the contour separation over which tangent alignment falls by the factor $e^{-1}$; it quantifies stiffness relative to thermal bending. The model bridges locally rod-like and globally coil-like conformations. It omits long-range self-avoidance in its simplest form, so sufficiently long dilute DNA can require excluded-volume corrections.

**Flexible and rigid limits.** Integrating the tangent correlation over the two contour positions gives the [end-to-end distance of a worm-like chain](../../../../end-to-end-distance-of-a-worm-like-chain.md):

$$
\langle R^2\rangle=2\int_0^L(L-u)e^{-u/\ell_p}du
=2\ell_pL-2\ell_p^2(1-e^{-L/\ell_p}).
$$

For a very flexible chain on the scale of its total length, $L/\ell_p\gg1$, the exponential is negligible and

$$
\boxed{\langle R^2\rangle\simeq2\ell_pL,\qquad R_{\mathrm{rms}}\simeq\sqrt{2\ell_pL}\ll L}.
$$

This is the [ideal chain](../../../../ideal-chain.md) result with [Kuhn length](../../../../kuhn-length.md) $b_K=2\ell_p$ and effective step count $N_K=L/(2\ell_p)$. Many persistent sections have decorrelated orientations. The flexible limit means a large ratio $L/\ell_p$ within the continuum model's range, not an extrapolation of the persistence length below all molecular length scales.

For a nearly rigid chain, $L/\ell_p\ll1$, the constant and linear terms in the exponential cancel those outside it. The [Taylor series](../../../../taylor-series.md) gives

$$
\langle R^2\rangle=L^2-\frac{L^3}{3\ell_p}+\frac{L^4}{12\ell_p^2}+\cdots,
$$

so

$$
\boxed{R_{\mathrm{rms}}\simeq L\left(1-\frac{L}{6\ell_p}+\cdots\right)\longrightarrow L}.
$$

This is the expected rod limit: all tangents are nearly aligned, and the end-to-end distance approaches the [arc length](../../../../arc-length.md).

**Helix–coil curves.** A [helix-coil transition model](../../../../helix-coil-transition-model.md) allows ordered helical runs and disordered coil regions. Use $s$ and $\sigma$ with exactly the free-energy conventions defined in the paper. A negative $\Delta F_{\mathrm{hc}}$ gives $s>1$ and favors the helical state; a positive junction cost gives $0<\sigma<1$ and penalizes starting new domains. The supplied helical fraction is the long-chain form associated with the [Zimm-Bragg model](../../../../zimm-bragg-model.md).

Its main features follow directly without assuming a sharp transition. Put $Q=(s-1)^2+4s\sigma$. For every $\sigma>0$,

$$
\boxed{\lim_{s\downarrow0}f_h(s)=0,\qquad f_h(1)=\frac12,\qquad\lim_{s\to\infty}f_h(s)=1},
$$

and differentiating gives

$$
\boxed{\frac{df_h}{ds}=\frac{\sigma(s+1)}{Q^{3/2}}>0,\qquad
\left.\frac{df_h}{ds}\right|_{s=1}=\frac1{4\sqrt\sigma}}.
$$

Thus all curves rise monotonically and cross at $(1,1/2)$. Increasing the boundary free-energy cost reduces $\sigma$, suppresses frequent coil–helix boundaries and makes longer runs favorable. The transition region becomes narrower and steeper: balancing $(s-1)^2$ against $4s\sigma$ gives a width of order $\sqrt\sigma$ near $s=1$.

<a id="section-b/b4/image-helical-fraction-and-the-sharpening-of-a-helix-coil-crossover"></a>
![](../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018-scm-helix-coil.png)

**[Figure 3](#section-b/b4/image-helical-fraction-and-the-sharpening-of-a-helix-coil-crossover). Helical fraction and the sharpening of a helix-coil crossover**. Original plots of the supplied fraction for several positive initiation parameters, with a magnified view near the common midpoint.

For $\sigma=1$, the fraction simplifies to $\boxed{f_h=s/(1+s)}$, the noncooperative two-state result. For $0<\sigma\ll1$, the steep curve describes cooperative helix formation. In the singular limit $\sigma\downarrow0$, it approaches zero for $s<1$ and one for $s>1$; its midpoint remains $1/2$ when approached through positive $\sigma$. Setting $\sigma=0$ directly makes the formula indeterminate at $s=1$. For any fixed positive $\sigma$, the given long-chain curve is smooth: it is a cooperative crossover, not a true discontinuity. The plot varies $s$ at fixed $\sigma$; in an actual temperature scan both parameters may change, and a finite chain can further round the crossover.

## ↑ Ancestors (13)

1. [B4](../b4.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
