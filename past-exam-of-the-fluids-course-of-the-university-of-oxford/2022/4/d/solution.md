<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Retain the clean-bubble approximation $\eta_a\ll\eta_w$ used in parts (b) and (c), with constant [mass densities](../../../../density.md) and [diffusion coefficient](../../../../diffusion-coefficient.md). For a spherical bubble,

$$
M=\frac{4\pi}{3}\rho_a a^3,\qquad
4\pi\rho_a a^2\dot a=-4\pi aD_a\rho_a.
$$

Consequently

$$
\boxed{\dot a=-\frac{D_a}{a},\qquad a^2(t)=a_0^2-2D_at,\qquad
t_{\mathrm{diss}}=\frac{a_0^2}{2D_a}.}
$$

The [buoyancy](../../../../buoyancy.md) minus bubble weight is $4\pi(\rho_w-\rho_a)ga^3/3$. Balancing it against the [clean-bubble Stokes drag](../../../../clean-bubble-stokes-drag.md) gives the instantaneous [terminal velocity](../../../../terminal-velocity.md)

$$
\dot z=U(a)=\frac{(\rho_w-\rho_a)g}{3\eta_w}a^2\equiv Ka^2.
$$

Set $z=0$ at the initial position. Combining this with the dissolution equation gives $da/dz=-D_a/(Ka^3)$ and hence the [dissolution-limited bubble rise](../../../../dissolution-limited-bubble-rise.md) law

$$
\boxed{a(z)=\left[a_0^4-\frac{12\eta_wD_a}{(\rho_w-\rho_a)g}z\right]^{1/4},\qquad
z_{\mathrm{diss}}=\frac{(\rho_w-\rho_a)ga_0^4}{12\eta_wD_a}.}
$$

The expression applies until the bracket vanishes. The rise speed decreases continuously as the bubble shrinks. Equivalently, $z(t)=K(a_0^2t-D_at^2)$, providing a direct check on the elimination of time.

The phrase “constant terminal velocity” must here mean rapid adjustment to a force balance at each radius. A literally time-independent speed is incompatible with that balance because $U\propto a^2$. If instead an external mechanism maintained a fixed $U_*$, the distinct result would be $a^2(z)=a_0^2-2D_az/U_*$ and $z_{\mathrm{diss}}=U_*a_0^2/(2D_a)$. In particular, holding the initial terminal speed fixed doubles the predicted rise distance; it is not the freely rising shrinking-bubble model.

Using the supplied values and $g=9.81\,\mathrm{m\,s^{-2}}$ gives

$$
t_{\mathrm{diss}}\simeq50\,\mathrm s,\qquad
\boxed{d\gtrsim z_{\mathrm{diss}}\simeq0.82\,\mathrm m.}
$$

Equality means dissolution exactly on arrival at the surface; dissolution strictly before arrival needs a greater initial depth. This is a **formal low-[Reynolds number](../../../../reynolds-number.md) estimate**. The same values predict $U(a_0)\simeq0.033\,\mathrm{m\,s^{-1}}$ and a radius-based [Reynolds number](../../../../reynolds-number.md) $\rho_wU(a_0)a_0/\eta_w\simeq3.3$; the diameter-based value is about $6.5$. Neither is $\ll1$. Thus the numerical input does not consistently satisfy the [Stokes flow](../../../../stokes-flow-split.md) assumption initially, and the $0.82\,\mathrm m$ result should not be presented as an accurate oceanic prediction. Within the stated ideal model, bubble compression, contaminants and changes in dissolved-gas concentration are also excluded.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
