<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p$ denote the [fluid pressure](../../../../../../fluid-pressure.md) perturbation divided by the reference [mass density](../../../../../../density.md), and let $b=-g\rho'/\rho_0$ be the [buoyancy perturbation](../../../../../../buoyancy-perturbation.md). The [buoyancy frequency](../../../../../../buoyancy-frequency.md) satisfies $N^2=-g\hat\rho_z/\rho_0$. [Linearization](../../../../../../linearization.md) requires small boundary slope $k|\eta_0|\ll1$, small displacements compared with the vertical scales of the disturbance and background, and [advection](../../../../../../advection.md) small compared with the oscillatory acceleration. For a propagating [internal gravity wave](../../../../../../internal-wave.md) this includes $|m\eta_0|\ll1$; boundary slope alone is insufficient when $|m|\gg k$. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) also requires small relative [mass density](../../../../../../density.md) differences over the region of interest. These conditions must hold for the resulting disturbance, including any amplification by [resonance](../../../../../../resonance.md).

The inviscid [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md) and linear [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) are

$$
u_t=-p_x,\qquad w_t=-p_z+b,\qquad b_t+N^2w=0,\qquad u_x+w_z=0,\qquad W(0)=-i\omega\eta_0.
$$

Write the [velocity field](../../../../../../velocity-field.md) as $(u,w)=\operatorname{Re}\{(U(z),W(z))e^{i(kx-\omega t)}\}$. [Incompressibility](../../../../../../incompressible-flow.md) and horizontal [momentum](../../../../../../momentum.md) balance give

$$
U=\frac{i}{k}W',\qquad P=\frac{i\omega}{k^2}W',\qquad B=-\frac{iN^2}{\omega}W.
$$

The vertical [momentum](../../../../../../momentum.md) balance therefore yields

$$
W''+k^2\left(\frac{N^2}{\omega^2}-1\right)W=0.
$$

For a real vertical [wavenumber](../../../../../../wavenumber.md) $m$, this gives the [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{\omega^2=\frac{N^2k^2}{k^2+m^2}}.
$$

When $0<\omega<N$, define $\ell=k\sqrt{N^2/\omega^2-1}$. The [radiation condition](../../../../../../radiation-condition.md) selects $m=-\ell$, because energy must leave the boundary upward. The [boundary-forced internal gravity wave](../../../../../../boundary-forced-internal-gravity-wave.md) is

$$
\boxed{W=-i\omega\eta_0e^{-i\ell z},\qquad U=\frac{\ell}{k}W}.
$$

Its [wavevector](../../../../../../wavevector.md) is $\mathbf K=(k,m)$, its [phase velocity](../../../../../../phase-velocity.md) is $\mathbf c_p=\omega\mathbf K/(k^2+m^2)$, and its [group velocity](../../../../../../group-velocity.md) is

$$
\mathbf c_g=\left(\frac{Nm^2}{(k^2+m^2)^{3/2}},-\frac{Nkm}{(k^2+m^2)^{3/2}}\right).
$$

Thus the [phase velocity](../../../../../../phase-velocity.md) points down and right, while the [group velocity](../../../../../../group-velocity.md) points up and right. They are perpendicular. [Internal-wave polarization](../../../../../../internal-wave-polarization.md) makes the particle motion an oscillation along the [group velocity](../../../../../../group-velocity.md) direction, with zero first-order mean transport. The [constant-phase lines of an internal gravity wave](../../../../../../constant-phase-line-of-an-internal-gravity-wave.md) are also parallel to the [group velocity](../../../../../../group-velocity.md). Their inclination $\vartheta$ above the horizontal satisfies $\sin\vartheta=\omega/N$.

When $\omega>N$, set $\kappa=k\sqrt{1-N^2/\omega^2}$. Boundedness at infinity selects the [evanescent wave](../../../../../../evanescent-wave.md)

$$
\boxed{W=-i\omega\eta_0e^{-\kappa z},\qquad U=-\frac{i\kappa}{k}W}.
$$

The horizontal and vertical [velocity](../../../../../../velocity.md) components are in quadrature: fluid particles describe small [ellipses](../../../../../../ellipse.md), and the response decays over $\kappa^{-1}$. There is no upward time-averaged [energy flux](../../../../../../energy-flux.md), because $P$ and $W$ are in quadrature. A real vertical [group velocity](../../../../../../group-velocity.md) is not defined for this [evanescent wave](../../../../../../evanescent-wave.md). The pattern travels horizontally with [phase velocity](../../../../../../phase-velocity.md) $\omega/k$.

For $N=0$ the response is the [evanescent wave](../../../../../../evanescent-wave.md) with $\kappa=k$; the ratios $\omega/N$ should not be used. At the cutoff $\omega=N>0$, the bounded harmonic solution has $W=-i\omega\eta_0$, $U=0$: it neither decays nor has nonzero upward [group velocity](../../../../../../group-velocity.md). It is the limiting cutoff response, rather than a localized radiating disturbance. A uniform nonzero [buoyancy frequency](../../../../../../buoyancy-frequency.md) in an infinitely deep [Boussinesq approximation](../../../../../../boussinesq-approximation.md) is itself a local idealization of the background [mass density](../../../../../../density.md).

<a id="1/a/image-propagating-and-evanescent-responses"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345-wave-regimes.png)

**[Figure 1](#1/a/image-propagating-and-evanescent-responses). Propagating and evanescent responses**.

The arrows distinguish the [phase velocity](../../../../../../phase-velocity.md), [group velocity](../../../../../../group-velocity.md), and oscillatory particle motion of the [internal gravity wave](../../../../../../internal-wave.md). The right panel shows the decay envelope and particle [ellipses](../../../../../../ellipse.md) of the [evanescent wave](../../../../../../evanescent-wave.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
