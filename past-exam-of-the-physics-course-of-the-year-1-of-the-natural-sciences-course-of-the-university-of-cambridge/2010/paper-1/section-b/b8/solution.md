<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Integrating coaxial cylindrical shells gives

$$
I=\int_0^a r^2\frac{2m r}{a^2}\,dr=\frac12ma^2.
$$

[Rolling without slipping](../../../../../rolling-without-slipping.md) has spin [speed](../../../../../speed.md) $u/a$, so **$K=mu^2/2+Iu^2/(2a^2)=3mu^2/4$**.

For the [rolling-cylinder loop contact threshold](../../../../../rolling-cylinder-loop-contact-threshold.md), set $\ell=R-a$, the [radius](../../../../../radius.md) of the centre's circular path, and let $\theta$ run from the loop bottom. The centre starts $h$ above its lowest centre position. Its height gain from the bottom is $\ell(1-\cos\theta)$. [Energy](../../../../../energy-split.md) conservation gives

$$
u^2=\frac43g[h-\ell(1-\cos\theta)].
$$

At the top, contact requires $N=m(u_t^2/\ell-g)\ge0$, hence $u_t^2\ge g\ell$. Inserting the [energy](../../../../../energy-split.md) relation proves the limiting condition

$$
\boxed{h\ge\frac{11}{4}\ell=\frac{11(R-a)}4.}
$$

The same condition keeps $N\ge0$ elsewhere on the circle, since

$$
\frac{N}{mg}=\frac43(h/\ell-1)+\frac73\cos\theta
$$

is smallest at the top.

For the centre's [acceleration](../../../../../acceleration.md), the inward normal component is $u^2/\ell$ and the tangential component is $-(2g/3)\sin\theta$. If $A=h/\ell-1\ge7/4$ and $x=\cos\theta$,

$$
|\mathbf a_C|^2=\frac{4g^2}{9}[4A^2+8Ax+3x^2+1].
$$

This convex quadratic has its largest endpoint value at $x=1$. **The maximum on the circular loop is at the bottom, directed vertically upward.** For the limiting release height,

$$
\boxed{a_{C,\max}=u_b^2/\ell=\frac{11g}{3}\approx36.0\,\mathrm{m\,s^{-2}}.}
$$

The approach track's curvature is unspecified, so a global bound for an arbitrary approach shape cannot be proved from the sketch alone; the result above concerns the specified circular part and the usual smooth approach interpretation.

The [finite-friction qualification of a marginal rolling loop](../../../../../finite-friction-qualification-of-a-marginal-rolling-loop.md) also matters: the contact threshold presumes the stated no-slip idealization. At equality, near the top, required tangential [friction](../../../../../friction.md) vanishes linearly with angular distance from the top but $N$ vanishes quadratically. Thus any finite coefficient of [static friction](../../../../../static-friction.md) requires a release height above this limiting bound to maintain rolling everywhere; no coefficient is provided. This does not change the requested ideal contact criterion.

## ↑ Ancestors (13)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
