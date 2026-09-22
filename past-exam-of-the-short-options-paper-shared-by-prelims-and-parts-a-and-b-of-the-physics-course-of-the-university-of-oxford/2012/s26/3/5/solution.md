<h1 id="s26/3/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a spherical [mass distribution](../../../../../mass-distribution.md) with constant circular [speed](../../../../../speed.md) $v_c$,

$$
M(<r)=\frac{v_c^2r}{G},\qquad
\boxed{\rho(r)=\frac{1}{4\pi r^2}\frac{dM}{dr}=\frac{v_c^2}{4\pi Gr^2}.}
$$

For $v_c=220\,\mathrm{km\,s^{-1}}$, this is about $0.0140(r/8\,\mathrm{kpc})^{-2}M_\odot\,\mathrm{pc^{-3}}$. It is the spherical model's total density; it is singular if extrapolated to the very centre and is intended only over the flat-rotation region.

For a sharp outer truncation at $r_*$, the exterior mass is fixed at $M_*=v_c^2r_*/G$. Integrating the gravitational work from $r$ to the boundary and then to infinity gives

$$
\frac12v_{\rm esc}^2=\int_r^{r_*}\frac{v_c^2}{s}\,ds+\int_{r_*}^\infty\frac{GM_*}{s^2}\,ds
=v_c^2\left[\log\frac{r_*}{r}+1\right].
$$

Thus

$$
\boxed{v_{\rm esc}(r)=\sqrt{2}v_c\sqrt{1+\log(r_*/r)}.}
$$

The exterior contribution cannot be dropped: at $r=r_*$ it correctly gives the point-mass escape speed $\sqrt2v_c$.

If the fastest measured radial speed is assumed to approximate both the total speed and the local escape speed of a bound star, then at $r=8\,\mathrm{kpc}$,

$$
\boxed{r_*\simeq r\exp\left(\frac{430^2}{2(220)^2}-1\right)\simeq19.9\,\mathrm{kpc}.}
$$

Without those extra assumptions, the measurement gives only a bound: a bound star's total speed is at least its radial component, and the sample maximum need not reach escape, so $r_*\gtrsim19.9\,\mathrm{kpc}$ within this model. An unbound interloper would invalidate even that bound. This is not a determination of the real Milky Way halo edge.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [3](../../3.md)
3. [S26](../../../s26.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
