<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [Monge representation](../../../../monge-representation.md) $\mathbf r(x,y)=(x,y,h(x,y))$ for a single-valued surface without overhangs. Its [area](../../../../surface-area.md) element is $dA=\sqrt{1+|\nabla h|^2}\,dx\,dy$; at small slopes, $dA\simeq[1+|\nabla h|^2/2]dx\,dy$ and twice the [mean curvature](../../../../mean-curvature.md) is $2\mathcal H\simeq\nabla^2h$, up to orientation sign. For zero spontaneous curvature, the quadratic excess [Helfrich energy](../../../../helfrich-energy.md) is

$$
\boxed{F=\frac12\int dx\,dy\,[\kappa(\nabla^2h)^2+\sigma|\nabla h|^2].}
$$

The [fluid membrane shear response](../../../../fluid-membrane-shear-response.md) has no equilibrium static in-plane [shear modulus](../../../../shear-modulus.md): constituents can rearrange to relax shear. Bending and isotropic tension still cost [energy](../../../../energy-split.md); viscous [shear stresses](../../../../shear-stress.md) can matter during motion. A [Gaussian curvature](../../../../gaussian-curvature.md) term is omitted under the stated approximation; for fixed closed-surface [topology](../../../../topology-split.md) its integral is constant, but boundaries and [topology](../../../../topology-split.md) changes require care. The small-slope Monge expression describes weak deformations, not an entire fully wrapped sphere.[section II.C, equation (12), p. 695: curvature-elastic energy; only the generic continuum mechanics is used here](../../../../elastic-properties-of-lipid-bilayers-theory-and-possible-experiments-by-wolfgang-helfrich.md)

For [spherical-particle wrapping by a fluid membrane](../../../../spherical-particle-wrapping-by-a-fluid-membrane.md), integrate the spherical [area](../../../../surface-area.md) element from polar angle $0$ to $\alpha$:

$$
A=\int_0^{2\pi}d\varphi\int_0^\alpha r_0^2\sin\theta\,d\theta
=2\pi r_0^2(1-\cos\alpha)=2\pi r_0^2\xi.
$$

Its footprint [radius](../../../../radius.md) is $r_\parallel=r_0\sin\alpha$, so

$$
A_\parallel=\pi r_0^2(2\xi-\xi^2),\qquad
\boxed{\Delta A=\pi r_0^2\xi^2.}
$$

For a spherical surface $2\mathcal H=2/r_0$, making the bending cost $\kappa(2/r_0)^2A/2=4\pi\kappa\xi$. [adhesion](../../../../adhesion.md) contributes $-2\pi wr_0^2\xi$, and tension contributes $\sigma\Delta A$. Therefore

$$
\boxed{\frac{E}{\pi\kappa}=(4-2\bar w)\xi+\bar\sigma\xi^2,\qquad
\bar w=\frac{wr_0^2}{\kappa},\quad\bar\sigma=\frac{\sigma r_0^2}{\kappa}.}
$$

All three contributions are energies; $\bar w$ and $\bar\sigma$ are dimensionless. This is the specified bound-patch model: deformation of the free membrane and the neck is omitted.

The allowed interval $0\leq\xi\leq2$ corresponds to no [adhesion](../../../../adhesion.md), partial wrapping and full wrapping. At $\xi=2$, the cap covers a whole sphere and its footprint shrinks to zero. This is a closed neck in the geometric limit. It does not by itself prove membrane scission: creating a detached enclosure changes [topology](../../../../topology-split.md) and involves neck physics absent from this [energy](../../../../energy-split.md).

For positive [membrane tension](../../../../membrane-tension.md), $E''/(\pi\kappa)=2\bar\sigma>0$. Projecting the unconstrained [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) $(\bar w-2)/\bar\sigma$ onto the allowed interval gives

$$
\boxed{\xi_{\min}=\begin{cases}
0,&\bar w\leq2,\\
(\bar w-2)/\bar\sigma,&2<\bar w<2+2\bar\sigma,\\
2,&\bar w\geq2+2\bar\sigma.
\end{cases}}
$$

The [tension-dependent wrapping phase diagram](../../../../tension-dependent-wrapping-phase-diagram.md) boundaries are $\bar w=2$ and $\bar w=2+2\bar\sigma$. At zero [membrane tension](../../../../membrane-tension.md), the [energy](../../../../energy-split.md) is linear: the [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) jumps from $0$ to $2$ as $\bar w$ crosses $2$, while all indentation values are degenerate at $\bar w=2$. Negative [membrane tension](../../../../membrane-tension.md) is outside the stable-flat-membrane interpretation used here. Increasing [membrane tension](../../../../membrane-tension.md) makes the excess [area](../../../../surface-area.md) required for wrapping more expensive, broadening the partially wrapped region.

<a id="4/image-original-phase-diagram-of-the-stipulated-bound-patch-energy-with-finite-tension-partial-wrapping"></a>
![](../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2013/paper-1-wrapping-phases.png)

**[Figure 4](#4/image-original-phase-diagram-of-the-stipulated-bound-patch-energy-with-finite-tension-partial-wrapping). Original phase diagram of the stipulated bound-patch energy, with finite-tension partial wrapping**.

TODO: **user-deferred biological application**. The final request for biological relevance is intentionally left unsolved; all preceding generic geometry and membrane mechanics are included.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
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
