<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Model the target as a perfectly absorbing sphere of reaction radius $r_0$, with a fixed target and a dilute far-field polymerase density $c_\infty$. Steady radial [diffusion](../../../../diffusion.md) satisfies $\nabla^2c=0$, $c(r_0)=0$, $c(\infty)=c_\infty$, hence

$$
c(r)=c_\infty(1-r_0/r),\qquad
J=4\pi r_0^2D_A\left.\frac{dc}{dr}\right|_{r_0}=4\pi D_Ar_0c_\infty.
$$

Therefore, for a rate law multiplying [number densities](../../../../number-density.md),

$$
\boxed{k_a=4\pi D_Ar_0,\qquad [k_a]=\mathrm{m^3\,s^{-1}}.}
$$

For the [earliest diffusive target encounter among independent searchers](../../../../earliest-diffusive-target-encounter-among-independent-searchers.md), with $N_p$ independent well-mixed searchers in [volume](../../../../volume.md) $V$, the approximate first-arrival rate is $N_pk_a/V$, giving $\tau_3\simeq V/(N_pk_a)$. The target's effective reaction radius includes encounter geometry and is not uniquely determined by its [contour length](../../../../polymer-contour-length.md).

A numerical estimate needs [temperature](../../../../temperature-split.md), cell [volume](../../../../volume.md) and a capture-geometry convention, none of which is fixed numerically in the source. State representative estimates $T=300\,\mathrm K$ and $V=1\,\mathrm{\mu m^3}$. The [Stokes–Einstein](../../../../stokes-einstein-relation.md) estimate for a sphere of radius $15\,\mathrm{nm}$ in the stipulated [viscosity](../../../../dynamic-viscosity-split.md) is

$$
D_A=\frac{k_BT}{6\pi\eta(15\,\mathrm{nm})}
\simeq1.46\times10^{-12}\,\mathrm{m^2\,s^{-1}}.
$$

Using the target contour scale $40\times0.34\,\mathrm{nm}=13.6\,\mathrm{nm}$ as an order-of-magnitude $r_0$ gives $k_a\simeq2.50\times10^{-19}\,\mathrm{m^3\,s^{-1}}$ and

$$
\boxed{\tau_3\simeq1.33\times10^{-2}\,\mathrm s\,
\frac{V}{1\,\mathrm{\mu m^3}}\frac{300}{N_p}
\frac{13.6\,\mathrm{nm}}{r_0}\frac{300\,\mathrm K}{T}.}
$$

This is an idealized $10^{-2}$-second-scale estimate, not a unique geometric prediction. Finite cell shape, crowded motion, accessibility and orientational restrictions can reduce the ideal capture rate.

If nonspecific binding merely sequesters searchers and their free fraction is $0.2$, the three-dimensional capture hazard is reduced fivefold: $\tau\simeq\tau_3/0.2\simeq0.067\,\mathrm s$ for those estimates. If bound molecules instead search productively by [sliding](../../../../facilitated-target-search.md), a free-time fraction alone cannot determine the total arrival time or its sign of change. That is the distinct [facilitated-search](../../../../facilitated-target-search.md) mechanism treated in [c](../c.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
