<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Oligarchic growth](../../../../../oligarchic-growth.md) is the stage in which a relatively small number of [planetary embryos](../../../../../planetary-embryo.md) dominate the dynamics of many smaller [planetesimals](../../../../../planetesimal.md). It follows [runaway planetesimal growth](../../../../../runaway-planetesimal-growth.md). The embryos remain separated, grow to broadly comparable masses within similar local disk conditions, and regulate their accretion by stirring the population that supplies their material. The primary numerical study describes this embryo–planetesimal structure and typical separations of about ten individual [Hill radii](../../../../../hill-radius.md).[1998, abstract: three-dimensional simulations, self-regulated comparable-mass protoplanets and typical orbital separation](../../../../../oligarchic-growth-of-protoplanets-by-eiichiro-kokubo-and-shigeru-ida.md)

The key feedback is [gravitational focusing](../../../../../gravitational-focusing.md). In a dispersion-dominated encounter with approach speed $v$ and a small impactor, [conservation of energy](../../../../../conservation-of-energy.md) and [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) give the collision cross-section

$$
\sigma_{\rm coll}\simeq\pi R^2\left(1+\frac{v_{\rm esc}^2}{v^2}\right),
\qquad v_{\rm esc}^2\simeq\frac{2GM}{R}.
$$

At fixed internal [mass density](../../../../../density.md), $R\propto M^{1/3}$ and $v_{\rm esc}^2\propto M^{2/3}$. If the background random speed initially is controlled by small planetesimals and varies little with embryo [mass](../../../../../mass.md), strong focusing gives $\sigma_{\rm coll}\propto M^{4/3}$. For a disk with planetesimal thickness of order $v_z/\Omega_K$ and a fixed ratio $v/v_z$, the associated estimate is

$$
\dot M\sim\Sigma_s\Omega_KR^2
\left(1+\frac{v_{\rm esc}^2}{v^2}\right),
$$

up to geometric factors. With nearly fixed $v$, this gives $\dot M\propto M^{4/3}$ and $\dot M/M\propto M^{1/3}$: the largest bodies have the shortest fractional growth times, the essence of runaway growth.

As embryos grow, their gravitational encounters increasingly excite the random eccentricities and inclinations of nearby [planetesimals](../../../../../planetesimal.md). This is [viscous stirring of planetesimals](../../../../../viscous-stirring-of-planetesimals.md), not molecular fluid viscosity. Higher encounter speeds lower the focusing factor. The largest local embryo heats its feeding population most strongly and thereby suppresses its own relative growth advantage. Gas [drag](../../../../../drag-physics.md) and dissipative collisions oppose stirring; [dynamical friction](../../../../../dynamical-friction.md) tends to keep the more massive embryos' random motions relatively small while transferring random energy to lighter bodies. The balance between these processes controls the accretion rate.

For an illustrative self-regulated scaling $v\propto M^{1/3}$, the ratio $v_{\rm esc}/v$ is approximately fixed. The previous growth estimate becomes

$$
\dot M\propto M^{2/3},\qquad
\boxed{\frac{\dot M}{M}\propto M^{-1/3},\quad
 t_{\rm grow}=\frac M{\dot M}\propto M^{1/3}.}
$$

Larger embryos now grow more slowly in fractional terms, allowing neighboring embryos in comparable environments to approach similar masses. This scaling illustrates the feedback; it is not a universal exact exponent for every planetesimal size distribution, damping law or disk surface-density profile. In particular, a two-body focusing cross-section must be modified in the shear-dominated regime, where encounters are governed by the stellar tidal field.

The relevant gravitational interaction scale is the [Hill radius](../../../../../hill-radius.md),

$$
R_H=a\left(\frac{M}{3M_\star}\right)^{1/3},\qquad v_H=\Omega_KR_H.
$$

Close embryo encounters and orbital repulsion keep adjacent embryos separated by several Hill-scale lengths. The [mutual Hill radius](../../../../../mutual-hill-radius.md) uses their combined [mass](../../../../../mass.md); for equal neighboring masses it is $2^{1/3}R_H$. Stating which definition is used matters when quoting a spacing coefficient. The spacing is a dynamical scale, not an exact universal integer.

<a id="3/c/image-neighboring-feeding-zones-and-the-change-from-runaway-to-self-regulated-fractional-growth"></a>
![](../../../../../past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2016/paper-1-oligarchic-growth.png)

**[Figure 4](#3/c/image-neighboring-feeding-zones-and-the-change-from-runaway-to-self-regulated-fractional-growth). Neighboring feeding zones and the change from runaway to self-regulated fractional growth**.

Each [feeding zone of a planetary embryo](../../../../../feeding-zone-of-a-planetary-embryo.md) contains a finite solid reservoir. To estimate its [isolation mass](../../../../../isolation-mass.md), let the full annular width be $\Delta a=B R_H$, where the dimensionless coefficient $B$ includes the stated choice of width and Hill-radius convention. For local solid [surface density](../../../../../surface-density-of-a-disk.md) $\Sigma_s$,

$$
M_{\rm iso}\simeq2\pi a\Delta a\Sigma_s
=2\pi B a^2\Sigma_s
\left(\frac{M_{\rm iso}}{3M_\star}\right)^{1/3}.
$$

Solving gives

$$
\boxed{M_{\rm iso}=\frac{(2\pi B a^2\Sigma_s)^{3/2}}
{(3M_\star)^{1/2}}.}
$$

Thus denser solid disks and wider feeding annuli allow larger embryos. If $\Sigma_s\propto a^{-p}$, the estimate scales as $M_{\rm iso}\propto a^{3-3p/2}$ at fixed host mass and $B$. This is a local exhaustion estimate, not an absolute maximum planet mass: radial delivery of solids, [pebble accretion](../../../../../pebble-accretion.md), migration and embryo mergers can replenish or enlarge a feeding zone. No solid surface-density normalization is given, so a numerical isolation mass would require an invented disk model.

As the local supply is depleted, growth slows further. After gas damping weakens, embryo orbits may cross and giant collisions can assemble larger [terrestrial planets](../../../../../terrestrial-planet.md). Farther out, sufficiently massive cores may instead acquire gas before [protoplanetary disk dispersal](../../../../../protoplanetary-disk-dispersal.md). **Oligarchic growth explains why a few comparable embryos share a disk while many smaller planetesimals remain: gravitational stirring weakens focusing and makes accretion self-regulating.**

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the exoplanets and Planetary Systems course of the University of Cambridge](../../../../split.md)
6. [Exoplanets and Planetary Systems course of the University of Cambridge](../../../../../exoplanets-and-planetary-systems-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
