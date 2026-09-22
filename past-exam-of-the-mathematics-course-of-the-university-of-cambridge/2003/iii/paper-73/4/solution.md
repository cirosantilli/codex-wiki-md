<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $\tau=m/\zeta$. The causal [Green function](../../../../../green-s-function.md) of the displacement equation is $G(t)=\zeta^{-1}(1-e^{-t/\tau})$ for $t>0$ and zero for $t<0$. Its derivative has the jump needed to give $mG''+\zeta G'=\delta(t)$. For the specified zero position and velocity,

$$
\boxed{x(t)=\frac1\zeta\int_0^t[1-e^{-(t-s)/\tau}]f(s)\,ds,\qquad
\dot x(t)=\frac1m\int_0^te^{-(t-s)/\tau}f(s)\,ds.}
$$

For [Gaussian white noise](../../../../../gaussian-white-noise.md) these are stochastic convolutions; their first two moments follow from the stated covariance even without assuming Gaussian higher moments. In particular $\langle x\rangle=\langle\dot x\rangle=0$, and

$$
\langle\dot x(t)^2\rangle=\frac F{m^2}\int_0^te^{-2(t-s)/\tau}\,ds
=\frac F{2m\zeta}(1-e^{-2t/\tau}).
$$

The required [equipartition theorem](../../../../../equipartition-theorem.md) limit therefore fixes the [fluctuation-dissipation relation for a Langevin particle](../../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md):

$$
\boxed{F=2\zeta k_BT.}
$$

Here $k_B$ denotes the printed Boltzmann constant $k$. Set $D=k_BT/\zeta$, the [Stokes–Einstein relation](../../../../../stokes-einstein-relation.md). Squaring the displacement kernel gives

$$
\boxed{\langle x(t)^2\rangle=2D\left[t-2\tau(1-e^{-t/\tau})+\frac\tau2(1-e^{-2t/\tau})\right].}
$$

Consequently **$\lim_{t\to\infty}\langle x\rangle=0$ and $\lim_{t\to\infty}\langle x^2\rangle=+\infty$**, with $\langle x^2\rangle=2Dt-3D\tau+o(1)$ for positive temperature. There is no finite equilibrium variance of position in an unconfined fluid. The [inertial Brownian displacement with zero initial velocity](../../../../../inertial-brownian-displacement-with-zero-initial-velocity.md) has short-time variance $2Dt^3/(3\tau^2)+O(t^4)$, rather than the ballistic law associated with an initially thermalized velocity.

For constant $D$, the [diffusion equation](../../../../../diffusion-equation-split.md) has fundamental density $P(x,t)=(4\pi Dt)^{-1/2}e^{-x^2/(4Dt)}$, whose mean is zero and variance is $2Dt$. It describes the large-time, overdamped limit of the [Langevin dynamics](../../../../../langevin-dynamics.md). Under the usual Gaussian-force assumption, the finite-time position density is Gaussian with the variance above and obeys a time-dependent diffusion equation with coefficient $D(1-e^{-t/\tau})^2$. It does not obey the constant-$D$ equation through the initial inertial transient. The given covariance alone determines the moments, not a Gaussian law; the density statement uses the standard Gaussian thermal-noise model.

Now write $\zeta(x)=\zeta_0+\varepsilon\zeta'_0x$ and $x=x_0+\varepsilon x_1+O(\varepsilon^2)$, with $\tau_0=m/\zeta_0$ and $D_0=k_BT/\zeta_0$. For a fixed realization of the additive force, the first-order equation is

$$
m\ddot x_1+\zeta_0\dot x_1=-\zeta'_0x_0\dot x_0.
$$

If the force amplitude is instead adjusted to local thermal equilibrium, its first-order noise term has zero mean in the inertial Itô formulation and does not change the following first-order mean calculation. The mixed unperturbed moment is

$$
\langle x_0\dot x_0\rangle=\tfrac12\frac{d}{dt}\langle x_0^2\rangle
=D_0(1-e^{-t/\tau_0})^2.
$$

Let $M(t)=\langle x_1(t)\rangle$. Averaging and solving the scalar forced relaxation equation, with $M(0)=M'(0)=0$, gives

$$
\begin{aligned}
M'(t)&=-\frac{\zeta'_0D_0}{\zeta_0}\left[1-e^{-2t/\tau_0}-\frac{2t}{\tau_0}e^{-t/\tau_0}\right],\\
M(t)&=-\frac{\zeta'_0D_0}{\zeta_0}\left[t-\frac{\tau_0}{2}(1-e^{-2t/\tau_0})
-2\tau_0\{1-(1+t/\tau_0)e^{-t/\tau_0}\}\right].
\end{aligned}
$$

Thus the long-time first-order coefficient and local mean drift are

$$
\boxed{M(t)\sim-\frac{k_BT\zeta'_0}{\zeta_0^2}t,\qquad
V_{\rm drift}=-\varepsilon\frac{k_BT\zeta'_0}{\zeta_0^2}.}
$$

Literally $\lim M=-\infty$ for $\zeta'_0>0$, $+\infty$ for $\zeta'_0<0$, and zero for $\zeta'_0=0$; the useful finite quantity is $\lim M'$. Because the viscosity gradient is only a local expansion, the physical drift result applies in the intermediate window $\tau_0\ll t\ll L_\zeta^2/D_0$, where $L_\zeta=\zeta_0/(\varepsilon|\zeta'_0|)$. Extrapolating the linear drag law to arbitrarily large displacements could make the drag negative and would invalidate the model.

The [isothermal diffusion with position-dependent drag](../../../../../isothermal-diffusion-with-position-dependent-drag.md) interpretation uses locally matched thermal noise and $D(x)=k_BT/\zeta(x)$. Integrating the printed Fickian [diffusion equation](../../../../../diffusion-equation-split.md) against $x$, with vanishing boundary fluxes, gives

$$
\frac{d}{dt}\langle x\rangle=-\int D P_x\,dx=\int D'(x)P\,dx.
$$

Since $D'(x)=-\varepsilon k_BT\zeta'_0/\zeta_0^2+O(\varepsilon^2)$, this reproduces the same drift after the inertial transient. Equivalently the overdamped [Itô diffusion](../../../../../ito-diffusion.md) has drift $D'$ and noise amplitude $\sqrt{2D}$. Omitting that drift would give $P_t=(DP)_{xx}$, which is a different [Fokker-Planck equation](../../../../../fokker-planck-equation.md) and not the stated Fickian equation.

Noise conventions cannot be mixed silently. If the force covariance is held at the spatially constant value $F_0=2\zeta_0k_BT$ while drag varies, the local overdamped diffusion coefficient is instead $\widetilde D=F_0/(2\zeta^2)$ and its Itô drift is $\widetilde D'/2$. Its density equation is $P_t=\partial_x[\widetilde D P_x+(\widetilde D'/2)P]$, not the isothermal Fickian equation. This still gives the same displayed first-order mean drift at $x=0$, but has different spatial diffusion and equilibrium properties. The stated Fickian interpretation therefore requires local thermal-noise matching.

Physically, thermally driven excursions travel farther on the lower-drag side. Their displacement is correlated with velocity, so averaging the position-dependent friction leaves a net drift toward greater [diffusivity](../../../../../diffusion-coefficient.md), without an applied [force](../../../../../force.md). This is not a violation of equilibrium: in the isothermal Fickian model the drift and spatially varying noise cancel in the probability flux for a uniform density. It is a local diffusion-induced shift of the centroid of an initially localized particle distribution.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
