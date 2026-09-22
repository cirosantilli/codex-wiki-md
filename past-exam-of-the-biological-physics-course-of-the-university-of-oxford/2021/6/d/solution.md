<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A small swimming member of the [bacteria](../../../../bacteria.md) samples too little spatial separation across its own body to compare weak chemical gradients accurately. [Temporal sensing in bacterial chemotaxis](../../../../temporal-sensing-in-bacterial-chemotaxis.md) instead compares recent receptor activity with an adapted memory. Straight runs carry it between locations; tumbles reorient it. When conditions improve, tumbling becomes less frequent and favorable runs last longer. An unfavorable direction is abandoned sooner. Repetition creates a biased [random walk](../../../../random-walk-split.md) without requiring the cell to identify the best direction at each tumble. [Rotational diffusion](../../../../rotational-diffusion.md) and environmental obstacles eventually destroy the benefit of maintaining a direction indefinitely.

An order-of-magnitude transport estimate compares the time $\ell/v$ to swim a distance $\ell$ with the time $\ell^2/D$ for an attractant to diffuse that distance. Their crossover is a [Péclet number](../../../../peclet-number.md) of order one:

$$
\frac{\ell}{v}\sim\frac{\ell^2}{D},\qquad
\boxed{\ell\sim\frac Dv=\frac{1000}{30}\,\mathrm{\mu m}\simeq33\,\mathrm{\mu m},\qquad
\tau\sim\frac{D}{v^2}\simeq1.1\,\mathrm s.}
$$

This estimates a useful run scale: over much shorter distances, nutrient [diffusion](../../../../diffusion.md) rapidly replenishes the local environment compared with the organism's displacement. Runs of order a second also permit comparison along a substantial path before reorientation. The given $D$ and $v$ determine this scale, not an exact biological mean run length or a complete sensory optimization. If a one-coordinate root-mean-square diffusion length $\sqrt{2D\tau}$ is equated with $v\tau$, the resulting prefactor is two; a three-dimensional root-mean-square convention gives six. Such constants cannot be fixed by a scaling argument alone.

For a cilium of length $d$, compare its advective time $d/u$ with the local [diffusion](../../../../diffusion.md) time $d^2/D$. Significant stirring relative to [diffusion](../../../../diffusion.md) requires $\mathrm{Pe}_d=ud/D\gtrsim1$, so

$$
\boxed{u\gtrsim\frac Dd=10^3\,\mathrm{\mu m\,s^{-1}}=1\,\mathrm{mm\,s^{-1}}\qquad(d=1\,\mathrm{\mu m}).}
$$

This is about $33$ times the stated swimming speed. If the tip travelled on a circular path of radius $d$, that speed would correspond to an illustrative frequency $u/(2\pi d)\simeq160\,\mathrm{Hz}$. That geometric conversion is not a specified beat pattern. At microscopic scales the flow has small [Reynolds number](../../../../reynolds-number.md); useful transport depends on the actual nonreciprocal motion and resulting flow, and rapid motion alone does not guarantee increased uptake. The scaling explains why simply stirring with a very short appendage is demanding when molecular [diffusion](../../../../diffusion.md) is already fast.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
