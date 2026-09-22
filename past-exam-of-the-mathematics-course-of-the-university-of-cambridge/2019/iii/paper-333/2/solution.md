<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $f_0>0$ for definiteness and define $K=(k^2+l^2)^{1/2}>0$. [Thermal-wind balance](../../../../../thermal-wind.md) gives $U_z=-b_y/f_0=\Lambda$, and the lower boundary condition fixes $U=\Lambda z$. The basic interior [quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) has no gradient, so a boundary-supported [normal mode](../../../../../normal-mode.md) $\psi'=\operatorname{Re}[\phi(z)e^{i(kx+ly-\omega t)}]$ has zero interior potential-vorticity perturbation. Its vertical equation is

$$
\phi''-\mu_0^2\phi=0,\qquad \mu_0=\frac{N_0K}{f_0}.
$$

Decay upward selects $\phi=Ae^{-\mu_0z}$.

The [buoyancy perturbation](../../../../../buoyancy-perturbation.md) is $b'=f_0\psi'_z$. At a rigid boundary $w'=0$, linearized material conservation of buoyancy gives

$$
(\partial_t+U\partial_x)\psi'_z-\Lambda\psi'_x=0.
$$

At $z=0$, this is $c\phi'(0)+\Lambda\phi(0)=0$, where $c=\omega/k$ for $k\ne0$. The [Eady edge wave](../../../../../eady-edge-wave.md) therefore has

$$
\boxed{c=\frac\Lambda{\mu_0}=\frac{\Lambda f_0}{N_0K},\qquad \omega=\frac{\Lambda f_0k}{N_0\sqrt{k^2+l^2}}.}
$$

It is an exponentially trapped boundary-buoyancy wave, not a vertically propagating interior mode. The formula for $\omega$ extends to $k=0$, where the perturbation is stationary.

For the two-region problem, absence of a density jump at the common material interface requires continuity of buoyancy:

$$
(N_1^2-N_2^2)h(y)=f_0(\Lambda_1-\Lambda_2)y.
$$

Thus its basic slope is $a=h_y=f_0(\Lambda_1-\Lambda_2)/(N_1^2-N_2^2)$. For a nondegenerate stratification contrast, its variation over horizontal scale $L$ is $aL/D=O(\operatorname{Ro}/\operatorname{Bu})$, which is small in the usual [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md) with [Burgers number](../../../../../burgers-number.md) of order one. The matching conditions can therefore be applied at the constant reference level $z=0$ to leading order. An exceptionally small stratification contrast would require checking this flat-interface ordering separately.

Pressure and normal velocity must be continuous because there is no membrane or singular interfacial force. Since base buoyancy is continuous, expanding pressure continuity at the displaced interface gives simply $\phi_1(0)=\phi_2(0)$. The base horizontal velocity is also continuous there; call it $U_I$. Decay away from the interface then gives

$$
\phi_1=Ae^{\mu_1z}\quad(z<0),\qquad \phi_2=Ae^{-\mu_2z}\quad(z>0),\qquad \mu_j=\frac{N_jK}{f_0}.
$$

Linearized buoyancy conservation in each region gives

$$
w_j'=\frac{ikf_0}{N_j^2}\left[(c-U_I)\phi_j'+\Lambda_j\phi_j\right].
$$

Matching normal velocity gives $w_1'=w_2'$: the common slope correction to normal velocity cancels because pressure continuity also makes the horizontal velocity perturbation continuous. Hence

$$
(c-U_I)\left(\frac{\phi_1'}{N_1^2}-\frac{\phi_2'}{N_2^2}\right)+\left(\frac{\Lambda_1}{N_1^2}-\frac{\Lambda_2}{N_2^2}\right)A=0.
$$

The [quasi-geostrophic wave at a stratification interface](../../../../../quasi-geostrophic-wave-at-a-stratification-interface.md) has intrinsic [phase velocity](../../../../../phase-velocity.md)

$$
\boxed{c-U_I=\frac{\Lambda_2/N_2^2-\Lambda_1/N_1^2}{\mu_1/N_1^2+\mu_2/N_2^2}=\frac{f_0}{K}\frac{\Lambda_2N_1^2-\Lambda_1N_2^2}{N_1N_2(N_1+N_2)}.}
$$

As $N_1/N_2\to\infty$ with $N_2$ and the shears bounded, the lower region becomes effectively rigid and

$$
\boxed{c-U_I\longrightarrow\frac{\Lambda_2f_0}{N_2K},}
$$

recovering the upper-fluid [Eady edge wave](../../../../../eady-edge-wave.md). The matching calculation describes regular interface-supported modes; arbitrary interior potential-vorticity initial disturbances can additionally be advected by the shear.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
