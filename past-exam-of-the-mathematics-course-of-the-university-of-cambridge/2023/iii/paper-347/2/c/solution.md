<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Steady [mass conservation](../../../../../../mass-conservation.md) gives $\dot M=-2\pi R\Sigma u_R$. Substituting this into the angular-momentum equation and integrating from the [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md) with zero torque gives

$$
\nu\Sigma R^3\frac{d\Omega}{dR}
=-\frac{\dot M}{2\pi}(l-l_{\rm ISCO})
=R\Sigma u_R(l-l_{\rm ISCO}).
$$

Therefore

$$
u_R=\frac{\nu R^2\,d\Omega/dR}{l-l_{\rm ISCO}}.
$$

Using $\nu=\alpha c_sH$, $c_s\simeq H\Omega$, $l=Ru_\phi$, and $R\,d\Omega/dR$ of order $-\Omega$ gives

$$
\boxed{|u_R|\simeq
\alpha\frac{H^2}{R^2}
\frac{u_\phi l}{l-l_{\rm ISCO}},}
$$

up to the order-unity Keplerian factor $3/2$.

At the sonic transition, $|u_R|\simeq c_s\simeq(H/R)u_\phi$. Hence

$$
\frac{l-l_{\rm ISCO}}l\simeq\alpha\frac HR\ll1
$$

for a geometrically thin disk with $\alpha\ll1$. The [specific angular momentum](../../../../../../specific-angular-momentum.md) therefore differs only fractionally from $l_{\rm ISCO}$ before the gas enters the [plunging region of a black-hole accretion disk](../../../../../../plunging-region-of-a-black-hole-accretion-disk.md). Its much shorter inflow time then prevents appreciable viscous transport, justifying angular-momentum conservation across the ISCO and the zero-torque boundary condition.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
