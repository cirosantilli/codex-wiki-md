<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a fixed perfectly absorbing spherical target, steady [diffusion](../../../../diffusion.md) outside radius $r_0$ obeys $\nabla^2c=0$, $c(r_0)=0$, and $c(\infty)=c_\infty$. Spherical symmetry gives $c=A+B/r$, hence $c(r)=c_\infty(1-r_0/r)$. The inward [diffusion](../../../../diffusion.md) flux integrated over the target is $4\pi r_0^2D_A c'(r_0)=4\pi r_0D_Ac_\infty$. Consequently the number-density rate constant is

$$
\boxed{k_a=4\pi r_0D_A.}
$$

This [Smoluchowski association rate](../../../../smoluchowski-association-rate.md) has units $\mathrm{m^3\,s^{-1}}$, as required by the given number-density rate law. If both partners moved independently, their relative [diffusion coefficient](../../../../diffusion-coefficient.md) would be the sum; the chromosomal target is treated as fixed here.

For a spherical [RNA polymerase](../../../../rna-polymerase.md) of radius $a=10\,\mathrm{nm}$, the [Stokes–Einstein relation](../../../../stokes-einstein-relation.md) gives

$$
D_A=\frac{k_BT}{6\pi\eta a}\simeq2.18\times10^{-12}\,\mathrm{m^2\,s^{-1}}\quad(T=298.15\,\mathrm K).
$$

For $N=6000$ free independent, approximately well-mixed searchers in a [volume](../../../../volume.md) $V$, the small-target encounter hazard is approximately $Nk_a/V$. Thus

$$
\boxed{\tau_3\simeq\frac{V}{6000\,4\pi r_0D_A}
=0.304\,\mathrm{ms}\left(\frac{V}{1\,\mu\mathrm m^3}\right)
\left(\frac{20\,\mathrm{nm}}{r_0}\right)
\left(\frac{298.15\,\mathrm K}{T}\right).}
$$

The numerical coefficient explicitly uses a typical illustrative cell [volume](../../../../volume.md) and an illustrative effective capture radius, **not dimensions supplied by the source**. A 60-base-pair B-form [DNA](../../../../deoxyribonucleic-acid.md) segment has a contour length of about $20\,\mathrm{nm}$, motivating an encounter size of this order, but its contour length does not uniquely determine an absorbing sphere's radius. Taking $r_0=10\,\mathrm{nm}$ instead doubles the estimate. A unique numerical answer requires $V$, $T$, and a capture-geometry convention, none specified in this block.

The estimate also treats all 6000 molecules as freely available and every encounter as productive. Crowding, nonspecific binding, orientation constraints, imperfect reaction, and finite-domain initial transients can alter it. In particular, an arbitrary first-passage distribution's mean does not divide by $N$ exactly; the division follows from the approximate exponential-hazard description.[Small-target well-mixed limit and its assumptions](../../../../earliest-diffusive-target-encounter-among-independent-searchers.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
