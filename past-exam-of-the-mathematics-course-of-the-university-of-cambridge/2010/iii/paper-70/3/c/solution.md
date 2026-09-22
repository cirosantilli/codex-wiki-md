<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Translation invariance in $y$, together with a $y$-independent incident field, permits a $y$-independent solution. In homogeneous space Maxwell's equations then separate into two scalar sectors.

For a [TE wave](../../../../../../transverse-electric-polarization.md), set $\mathbf E=\widehat{\mathbf y}E_y(x,z)$. Its component satisfies $(\partial_x^2+\partial_z^2+k^2)E_y=0$. The $y$ direction is tangent to the conducting surface, so vanishing tangential [electric field](../../../../../../electric-field.md) imposes $E_y(x,h(x))=0$. Therefore **TE scattering is exactly the two-dimensional Dirichlet scalar problem**, with $E_y$ replacing the acoustic scalar. Its first-order boundary expansion and angular-spectrum formula are those above.

For a [TM wave](../../../../../../transverse-magnetic-polarization.md), set $\mathbf H=\widehat{\mathbf y}H_y(x,z)$. Maxwell's equation $\nabla\times\mathbf H=-i\omega\epsilon\mathbf E$ gives

$$
\mathbf E=\frac{i}{\omega\epsilon}(-\partial_zH_y,0,\partial_xH_y).
$$

A surface tangent is $(1,0,h')$, so vanishing tangential [electric field](../../../../../../electric-field.md) gives

$$
\boxed{(\partial_z-h'\partial_x)H_y(x,h(x))=0,\quad\text{equivalently }\partial_nH_y=0.}
$$

Thus **TM also reduces to two dimensions, but to a Neumann problem, not the [Dirichlet problem](../../../../../../dirichlet-problem.md) in part (a)**. This is [scalar polarization reduction at a conducting corrugation](../../../../../../scalar-polarization-reduction-at-a-conducting-corrugation.md).

For example the flat TM reflection has positive sign, $H^{[0]}=A_i e^{ip_ix}(e^{-iq_iz}+e^{iq_iz})$. Its linearized rough forcing is

$$
\partial_zH_s^{[1]}(x,0)=2A_i e^{ip_ix}\bigl(q_i^2h+ip_i h'\bigr).
$$

In the transform domain this becomes $2A_i(k^2-p_i\xi)\widehat h(\xi-p_i)$, and propagation divides by $i\beta(\xi)$ rather than prescribing the electric Dirichlet trace. The explicit slope term and different reflection sign show why simply reusing the TE boundary formula for TM would be incorrect.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
