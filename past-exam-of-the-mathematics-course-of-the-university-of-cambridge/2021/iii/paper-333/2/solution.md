<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Represent a horizontal vector $(u,v)$ by the [complex number](../../../../../complex-number.md) $W=u+iv$, let $s=\operatorname{sgn}f$, and define the two [Ekman layer](../../../../../ekman-layer.md) depths and drag coefficients by

$$
\delta_j=\sqrt{\frac{2\nu_j}{|f|}},
\qquad
r_j=\frac{\rho_j\nu_j}{\delta_j}
=\rho_j\sqrt{\frac{\nu_j|f|}{2}},
\qquad j\in\{a,o\}.
$$

The atmospheric and oceanic departures from their respective [geostrophic flow](../../../../../geostrophic-flow.md) satisfy

$$
\nu_jW_{j,zz}=ifW_j.
$$

The solutions that decay away from the ice are

$$
W_a-W_a^\infty=(W_i-W_a^\infty)
\exp\left[-\frac{(1+is)z}{\delta_a}\right],
\qquad z>0,
$$

and

$$
W_o-W_o^\infty=(W_i-W_o^\infty)
\exp\left[\frac{(1+is)z}{\delta_o}\right],
\qquad z<0.
$$

Here $W_a^\infty$ and $W_o^\infty$ denote the atmospheric and oceanic geostrophic velocities.

The [viscous stress](../../../../../viscous-stress-tensor.md) exerted on the ice by the atmosphere and ocean is, respectively,

$$
\tau_a=(1+is)r_a(W_a^\infty-W_i),
\qquad
\tau_o=(1+is)r_o(W_o^\infty-W_i).
$$

Because the ice is an infinitesimally thin, freely moving sheet, its horizontal force balance is $\tau_a+\tau_o=0$. The common Ekman turning factor cancels, leaving

$$
\boxed{
W_i=\frac{r_aW_a^\infty+r_oW_o^\infty}{r_a+r_o}
}.
$$

Thus the ice moves along the weighted mean of the two geostrophic currents. In particular, as $\nu_a\to0$ one has $r_a\to0$ and $W_i\to W_o^\infty$: an atmosphere with vanishing viscosity transmits no finite stress to the ice.

The atmospheric [Ekman transport](../../../../../ekman-transport.md) relative to its geostrophic current is

$$
\mathcal M_a
=\int_0^\infty(W_a-W_a^\infty)\,dz
=\frac{\delta_a}{1+is}(W_i-W_a^\infty)
=-\frac{\delta_a r_o}{2(r_a+r_o)}
(1-is)(W_a^\infty-W_o^\infty).
$$

The atmospheric stress is

$$
\tau_a=\frac{(1+is)r_ar_o}{r_a+r_o}
(W_a^\infty-W_o^\infty).
$$

If the two geostrophic currents are parallel but unequal, both directions are obtained by rotating their velocity difference: in the Northern Hemisphere the stress lies $45^\circ$ anticlockwise from $W_a^\infty-W_o^\infty$, while the atmospheric transport lies $45^\circ$ clockwise from its negative. Both rotations reverse in the Southern Hemisphere. If the two currents are identical, the shear, stress, and relative Ekman transport all vanish.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
