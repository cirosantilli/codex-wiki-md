<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [force](../../../../../../force.md) scale is $F\sim\rho ga^3$. At the distant [free surface](../../../../../../free-surface.md), the Stokeslet's [pressure](../../../../../../pressure.md) and viscous normal-stress scales are $F/d^2$. Gravity restores a displaced surface by a [pressure](../../../../../../pressure.md) change $\rho gh$, so

$$
\boxed{h\sim\frac F{\rho gd^2}=O\!\left(\frac{a^3}{d^2}\right).}
$$

Thus $h/d=O((a/d)^3)\ll1$, consistent with treating the boundary as approximately flat and impermeable at leading order. This uses the stipulated gravity-dominated restoring balance.

The liquid-air interface has negligible tangential traction. The [stress-free image of a normal Stokeslet](../../../../../../stress-free-image-of-a-normal-stokeslet.md) places an opposite point [force](../../../../../../force.md) at the reflection point, a distance $2d$ above the bubble centre. Across the flat surface the combined normal [velocity](../../../../../../velocity.md) is odd and the tangential [velocity](../../../../../../velocity.md) is even, so the normal [velocity](../../../../../../velocity.md) and tangential stress vanish there. A same-radius inviscid drop of density $2\rho$ has downward excess weight $4\pi\rho ga^3/3$, exactly opposite the bubble's upward [buoyancy](../../../../../../buoyancy.md). Its exterior Stokeslet therefore supplies this image, giving the asserted full-space comparison to leading order in $a/d$.

The image's incident axial [velocity](../../../../../../velocity.md) at the bubble is

$$
u_{\rm image}=-\frac{F}{4\pi\mu(2d)}=-\frac{F}{8\pi\mu d}.
$$

To first reflection, the bubble translates with this locally uniform incident [velocity](../../../../../../velocity.md) plus its isolated rise speed $F/(4\pi\mu a)$. Hence the [bubble rise near a distant stress-free free surface](../../../../../../bubble-rise-near-a-distant-stress-free-free-surface.md) is

$$
\boxed{U_b=\frac{F}{4\pi\mu a}-\frac{F}{8\pi\mu d}
=U\left(1-\frac a{2d}+o(a/d)\right).}
$$

Only the first relative correction is retained; the image's spatial variation and additional reflections affect higher terms.

The customary capillary-controlled small-deformation condition is a small [capillary number](../../../../../../capillary-number.md),

$$
\boxed{\mathrm{Ca}=\frac{\mu U}{\gamma}=\frac{\rho ga^2}{3\gamma}\ll1,}
$$

equivalently a small [Bond number](../../../../../../bond-number.md) $\mathrm{Bo}=\rho ga^2/\gamma$. This is a sufficient condition, not a necessary condition for the special isolated spherical solution in part (b). More precisely, the image's strain is $O(F/(\mu d^2))$, so its deformation-producing normal stress compared with $\gamma/a$ is $O(\mathrm{Bo}(a/d)^2)$. When exploiting the exact isolated solution, that smaller combination controls the leading boundary-induced distortion. If capillarity at the distant free surface is also retained, the gravity-dominated deflection scaling requires $\gamma/(\rho gd^2)\ll1$; $a\ll\sqrt{\gamma/(\rho g)}\ll d$ allows both the usual spherical-bubble criterion and gravity-dominated surface restoration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
