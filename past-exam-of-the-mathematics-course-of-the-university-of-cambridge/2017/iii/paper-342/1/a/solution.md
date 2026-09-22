<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $h$ positive downwards and write $B$ for the [filament bending modulus](../../../../../../filament-bending-modulus.md). Under the material-modulus interpretation of the printed $A$ as [Young's modulus](../../../../../../young-s-modulus.md), the circular cross-section gives the [second moment of area](../../../../../../second-moment-of-area.md) and bending modulus

$$
I=\int_{\rm section}y^2\,dS=\frac{\pi a^4}{4},\qquad B=AI=\frac{A\pi a^4}{4}.
$$

Indeed a small [curvature](../../../../../../curvature.md) $\kappa$ gives axial [strain](../../../../../../strain.md) $-y\kappa$, so integrating $A y^2\kappa^2/2$ over the section gives bending [energy](../../../../../../energy.md) $B\kappa^2/2$ per unit length. Keeping this distinction is essential to the powers of radius in the answer.

After allowing for [buoyancy](../../../../../../buoyancy.md), the effective downward [force](../../../../../../force.md) per unit length is

$$
w=(\rho_f-\rho)\pi a^2g>0.
$$

The filament loses [potential energy](../../../../../../potential-energy.md) as it moves down; the displaced fluid's hydrostatic contribution is included through the density difference. For an [inextensible filament](../../../../../../inextensible-filament.md) with arc-length coordinate $s$, the geometric bending and gravitational [energy](../../../../../../energy.md) is $\int_0^L[B\kappa(s)^2/2-wh(s)]ds$, up to a constant. For the small-slope [Monge representation](../../../../../../monge-representation.md) this reduces to

$$
\boxed{E[h]=\int_0^L\left[\frac{B}{2}(h_{xx})^2-wh\right]dx,
\qquad B=\frac{A\pi a^4}{4},\quad w=(\rho_f-\rho)\pi a^2g.}
$$

The upward-positive convention reverses the sign of $h$ and the gravitational term together. There is no stretching contribution at this order when bending a slender filament without imposed axial tension. The wording does not explicitly distinguish a material elastic modulus from a flexural modulus: if $A$ instead denotes the [filament bending modulus](../../../../../../filament-bending-modulus.md) in the intended convention, set $B=A$ throughout; then the $\pi a^4/4$ factor is already included in $A$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
