<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

In [tight coupling](../../../../../../tight-coupling-approximation.md), the scattering time $|\dot\tau|^{-1}$ is short compared with an acoustic period and an expansion time: $k/|\dot\tau|\ll1$ and $\mathcal H/|\dot\tau|\ll1$. Photons and baryons have nearly the same velocity; higher photon multipoles and the [photon-baryon velocity slip](../../../../../../photon-baryon-velocity-slip.md) are suppressed by powers of this small ratio. Here retain the collision operator as printed, which ignores [CMB polarization](../../../../../../cosmic-microwave-background-polarization.md). Its diffusion coefficient differs from the polarized result.

Neglect gravity and expansion, so $R$ is constant on the timescale under consideration. The quadrupole equation of the [photon Boltzmann hierarchy](../../../../../../photon-boltzmann-hierarchy.md) is

$$
\dot\Theta_2+k\left(\frac37\Theta_3-\frac23\Theta_1\right)=\frac9{10}\dot\tau\Theta_2.
$$

To first order in $k/|\dot\tau|$, $\dot\Theta_2$ and $k\Theta_3$ are subleading relative to the dipole source. Hence

$$
\Theta_2\simeq-\frac{20}{27}\frac k{\dot\tau}\Theta_1,
\qquad \boxed{\Pi_\gamma\simeq-\frac49\frac k{\dot\tau}v_\gamma.}
$$

This is the [temperature-only tight-coupling quadrupole](../../../../../../temperature-only-tight-coupling-quadrupole.md). The negative collision rate is essential to its sign.

Put $\Delta=v_\gamma-v_b$. Subtracting the [baryon Euler equation with Thomson drag](../../../../../../baryon-euler-equation-with-thomson-drag.md) from the [photon Euler equation](../../../../../../photon-euler-equation.md) gives

$$
\dot\Delta=-\frac k4\delta_\gamma-\frac23k\Pi_\gamma
+\dot\tau\frac{1+R}{R}\Delta.
$$

The zeroth-order common velocity obeys $(1+R)\dot v=-k\delta_\gamma/4$. Solving the slip equation to its first nonzero order therefore gives

$$
\Delta\simeq\frac{R}{1+R}\frac{k\delta_\gamma}{4\dot\tau},\qquad
\dot\Delta\simeq\frac{R}{1+R}\frac{k\dot\delta_\gamma}{4\dot\tau}.
$$

The second expression assumes that $R$ and $\dot\tau$ vary only on the neglected background timescale. Terms from their variation would need retaining if cosmic expansion were restored. Multiplying the [baryon Euler equation with Thomson drag](../../../../../../baryon-euler-equation-with-thomson-drag.md) by $R$ and adding it to the photon equation eliminates drag. Since $v_b=v_\gamma-\Delta$,

$$
(1+R)\dot v_\gamma=-\frac k4\delta_\gamma-\frac23k\Pi_\gamma+R\dot\Delta.
$$

Using $v_\gamma=3\dot\delta_\gamma/(4k)$ from the [photon continuity equation](../../../../../../photon-continuity-equation.md), the quadrupole term contributes $(2/9)k\dot\delta_\gamma/\dot\tau$, and the slip term contributes $R^2k\dot\delta_\gamma/[4(1+R)\dot\tau]$. Hence

$$
\boxed{(1+R)\dot v_\gamma=-\frac k4\delta_\gamma
-\frac k4|\dot\tau|^{-1}\left(\frac{R^2}{1+R}+\frac89\right)\dot\delta_\gamma.}
$$

Differentiating the [photon continuity equation](../../../../../../photon-continuity-equation.md) gives the [photon-baryon diffusion damping equation](../../../../../../photon-baryon-diffusion-damping-equation.md)

$$
\boxed{\ddot\delta_\gamma+D\dot\delta_\gamma+c_s^2k^2\delta_\gamma=0,\quad
c_s^2=\frac1{3(1+R)},\quad
D=\frac{k^2|\dot\tau|^{-1}}{3(1+R)}\left(\frac{R^2}{1+R}+\frac89\right).}
$$

The sound speed reflects baryon inertia; the $R^2$ term is heat conduction through velocity slip, and the $8/9$ term is photon shear viscosity for the unpolarized hierarchy.

For constant coefficients the characteristic roots are $-D/2\pm\sqrt{D^2/4-c_s^2k^2}$. On the acoustic branch where $D<2c_sk$,

$$
\delta_\gamma(\eta)=e^{-D\eta/2}\left[A\cos(\omega\eta)+B\sin(\omega\eta)\right],\qquad
\omega=\sqrt{c_s^2k^2-D^2/4}.
$$

Thus the solutions are **damped acoustic oscillations**, with positive diffusion damping growing as $k^2$. This is [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md). Slowly varying coefficients give an approximate envelope $\exp[-\frac12\int D\,d\eta]$ and acoustic phase $k\int c_s\,d\eta$. The mathematical critically damped and overdamped cases follow from the roots, but extrapolation beyond the tight-coupling range is not reliable. For very large $R$, the acoustic and damping scales must be compared explicitly rather than inferring underdamping from $k/|\dot\tau|\ll1$ alone.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
