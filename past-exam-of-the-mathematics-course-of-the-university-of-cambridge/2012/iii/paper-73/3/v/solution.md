<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Multiply the [Kármán-Howarth equation](../../../../../../karman-howarth-equation.md) for $C(r,t)$ by $4\pi r^2$ and integrate in $r$. [Integration by parts](../../../../../../integration-by-parts.md) gives the exact boundary-flux expression

$$
\boxed{\frac{dL}{dt}=4\pi\left[\frac1r\frac{d}{dr}(r^4u^3K)+2\nu r^2\frac{dC}{dr}\right]_{0}^{\infty}}.
$$

At the origin smooth isotropic correlations give $K=O(r)$ or smaller and $C'=O(r)$, so both boundary terms vanish. At infinity the usual regular power-law decay $K=O(r^{-4})$, with the corresponding derivative decay, makes the first term tend to zero. A sufficiently smooth integrable trace correlation makes $r^2C'\to0$ as well. Under these physical far-field conditions,

$$
\boxed{dL/dt=0}.
$$

The exact required conditions are the limits of these two boundary fluxes. A bare big-$O$ condition on $K$ without control of its derivatives is not by itself a rigorous sufficient condition: the smooth tail $K(r)=r^{-4}\sin(r^2)$ is $O(r^{-4})$, but $r^{-1}(r^4K)'=2\cos(r^2)$ has no zero limit. The intended power-law assumption excludes such increasingly rapid far-field oscillations; this qualification is needed in a literal proof.

Physically, $L$ is the large-volume [momentum](../../../../../../momentum.md) [variance](../../../../../../variance-split.md) divided by volume. Internal advective and [pressure](../../../../../../pressure.md) forces exchange [momentum](../../../../../../momentum.md) among eddies but do not provide a net [impulse](../../../../../../impulse.md) to the whole unforced field. For a large spherical region, the [variance](../../../../../../variance-split.md) balance is driven by its boundary [momentum](../../../../../../momentum.md) flux. The stated correlation decay makes that contribution negligible per unit volume as the region grows. Thus **the conservation law preserves [momentum](../../../../../../momentum.md)-fluctuation density, not [kinetic energy](../../../../../../kinetic-energy.md)**. [kinematic viscosity](../../../../../../kinematic-viscosity.md) can remove [kinetic energy](../../../../../../kinetic-energy.md) while leaving this integral invariant.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
