<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $k_z=v_z=0$, define the complex vertical [vorticity](../../../../../../vorticity.md) [amplitude](../../../../../../wave-amplitude.md)

$$
Z=i(k_xv_y-k_yv_x).
$$

Take the curl of the [amplitude](../../../../../../wave-amplitude.md) equations, including $\dot k_x=2Ak_y$. Incompressibility cancels the [pressure](../../../../../../pressure.md) and rotation terms, giving

$$
\dot Z=-\nu k^2Z.
$$

Equivalently, the uniform basic absolute [vorticity](../../../../../../vorticity.md) has no gradient for the perturbation to advect. The general [two-dimensional viscous shearing wave](../../../../../../two-dimensional-viscous-shearing-wave.md) solution is

$$
\boxed{Z(t)=Z_0\exp\!\left[-\nu\int_{t_0}^t(k_x(s)^2+k_y^2)\,ds\right],\qquad v_x=\frac{ik_yZ}{k^2},\qquad v_y=-\frac{ik_xZ}{k^2},}
$$

where $Z_0$ is an arbitrary complex constant and $k_x(t_0)$ is an arbitrary real initial radial [wavenumber](../../../../../../wavenumber.md). The perturbation [pressure](../../../../../../pressure.md) follows from part (ii), or explicitly $\Pi=(4Ak_y^2-2\Omega k^2)Z/k^4$.

For $A\ne0$, shift the time origin to the swing $k_x=0$ and put $T=k_x/k_y=2At$, $T_0=2At_0$ and $\mathrm{Re}=A/(\nu k_y^2)$. Then

$$
k^2=k_y^2(1+T^2),\qquad Z(T)=Z_0\exp\!\left[-\frac{g(T)-g(T_0)}{2\mathrm{Re}}\right],\qquad g(T)=T+\frac{T^3}{3}.
$$

The spatially averaged perturbation kinetic-energy [mass density](../../../../../../density.md) is $E=\rho\langle|\mathbf u'|^2\rangle/2=\rho|\mathbf v|^2/4$, and $|\mathbf v|^2=|Z|^2/k^2$. Consequently

$$
\boxed{\frac{E(T)}{E(T_0)}=\frac{1+T_0^2}{1+T^2}\exp\!\left[-\frac{g(T)-g(T_0)}{\mathrm{Re}}\right],\qquad E(T)\propto\frac{e^{-(T+T^3/3)/\mathrm{Re}}}{1+T^2}.}
$$

The proportionality constant depends on the initial data; the exponential profile is not a claim of infinite physical growth from the remote past. For $A>0$, leading waves with $T<0$ can gain velocity [amplitude](../../../../../../wave-amplitude.md) as their [wavevector](../../../../../../wavevector.md) magnitude decreases, before [viscosity](../../../../../../dynamic-viscosity.md) and later winding damp them. This is the [Orr mechanism](../../../../../../orr-mechanism.md), and it is independent of uniform rotation for these two-dimensional disturbances.

If $A=0$, the [wavevector](../../../../../../wavevector.md) is constant and $\mathbf v(t)=\mathbf v(t_0)e^{-\nu k^2(t-t_0)}$, so there is no shear amplification. The formulas with the physical-time integral remain valid, although $T=2At$ is no longer a useful coordinate. The high-positive-Reynolds-number case in the next part takes $A>0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
