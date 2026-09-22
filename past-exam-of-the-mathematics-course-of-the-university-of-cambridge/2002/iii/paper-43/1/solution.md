<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [density](../../../../../density.md) deficit in a [flux tube](../../../../../flux-tube.md) is not by itself an [instability](../../../../../instability.md) calculation. For example, a straight magnetized tube in otherwise field-free gas at the same [temperature](../../../../../temperature.md) has lateral balance $p_i+B_i^2/(2\mu_0)=p_e$. The [perfect gas](../../../../../ideal-gas.md) law then gives $\rho_i<\rho_e$, so the tube rises unless some other force balances its weight deficit. This configuration simply lacks [magnetostatic equilibrium](../../../../../magnetostatic-equilibrium.md). A [magnetic buoyancy instability](../../../../../magnetic-buoyancy-instability.md), in contrast, starts from a force-balanced atmosphere and asks whether a small allowed displacement grows. A balanced horizontal magnetic layer can be stable or unstable; the presence of [magnetic pressure](../../../../../magnetic-pressure.md) alone does not decide this.

Assume a smooth equilibrium, with downward gravitational [acceleration](../../../../../acceleration.md) $g>0$, and write $\mathcal R$ for the gas constant per unit mass. The ambient total [pressure](../../../../../pressure.md) and force balance are

$$
P(z)=p(z)+\frac{B_0(z)^2}{2\mu_0},\qquad
P'(z)=-\rho(z)g,\qquad p=\mathcal R\rho T.
$$

We use ideal [magnetic flux freezing](../../../../../magnetic-flux-freezing.md) on the displacement time scale and rapid lateral [pressure](../../../../../pressure.md) equilibration. A bodily displacement perpendicular to a straight horizontal tube does not change its length or bend its field. If its area is $\mathcal A$, conservation of [magnetic flux](../../../../../magnetic-flux.md) and mass per unit length gives $B\mathcal A=\mathrm{constant}$ and $\rho\mathcal A=\mathrm{constant}$. Thus the tube preserves

$$
f=\frac{B}{\rho}.
$$

Efficient heat exchange fixes its [temperature](../../../../../temperature.md) to the ambient [temperature](../../../../../temperature.md) at its new height, not to its original [temperature](../../../../../temperature.md). This is the thermal assumption that distinguishes the requested criterion from the adiabatic one.

Take a tube initially at $z_0$ and let $f_0=B_0(z_0)/\rho(z_0)$. After a small upward displacement $\xi$, let $\rho_i(z)$ be the [density](../../../../../density.md) it would have in lateral balance at $z=z_0+\xi$. Its preserved $f_0$ and imposed local [temperature](../../../../../temperature.md) give

$$
\mathcal R T(z)\rho_i(z)+\frac{f_0^2\rho_i(z)^2}{2\mu_0}=P(z).
$$

At the initial position $\rho_i=\rho$. Differentiate this relation at $z_0$:

$$
\left(c_T^2+v_A^2\right)\rho_i'+\mathcal R\rho T'=-\rho g,
\qquad c_T^2=\frac p\rho=\mathcal RT,\quad
v_A^2=\frac{B_0^2}{\mu_0\rho}.
$$

For the ambient atmosphere the same differentiation must also differentiate $f(z)=B_0(z)/\rho(z)$. It gives

$$
\left(c_T^2+v_A^2\right)\rho'+\mathcal R\rho T'
+\frac{\rho B_0}{\mu_0}f'=-\rho g.
$$

Subtracting isolates the actual displaced [density](../../../../../density.md) contrast:

$$
\rho_i(z_0+\xi)-\rho(z_0+\xi)
=\frac{\rho B_0}{\mu_0(c_T^2+v_A^2)}f'\xi+O(\xi^2).
$$

The pressure-gradient force on the tube balances the weight of the displaced ambient gas, so its leading vertical [buoyancy](../../../../../buoyancy.md) [acceleration](../../../../../acceleration.md) is

$$
\ddot\xi=-\frac{gB_0}{\mu_0(c_T^2+v_A^2)}
\frac{d}{dz}\left(\frac{B_0}{\rho}\right)\xi.
$$

The coefficient multiplying $\xi$ is positive precisely when the tube becomes lighter on upward displacement. Thus the [isothermal interchange criterion for magnetic buoyancy](../../../../../isothermal-interchange-criterion-for-magnetic-buoyancy.md) is

$$
\boxed{B_0\frac{d}{dz}\left(\frac{B_0}{\rho}\right)<0,
\quad\text{equivalently}\quad
\frac{d}{dz}\left(\frac{B_0^2}{\rho^2}\right)<0.}
$$

Where $B_0>0$, this is simply $d(B_0/\rho)/dz<0$, or $d\log B_0/dz<d\log\rho/dz$. The squared form is independent of the field's choice of direction. Equality is neutral at this order, and the reversed inequality is restoring for these displacements. A layer with an interval satisfying the strict inequality admits local growing interchange disturbances under the assumed [pressure](../../../../../pressure.md)/thermal equilibration. The calculation does not address field-bending undular modes, finite heat-transfer times or magnetic [diffusion](../../../../../diffusion.md); those can change the criterion. In particular, the [localized interchange criterion for a magnetized atmosphere](../../../../../localized-interchange-criterion-for-a-magnetized-atmosphere.md) with an adiabatic gas response is not interchangeable with this fast-thermal-exchange result.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
