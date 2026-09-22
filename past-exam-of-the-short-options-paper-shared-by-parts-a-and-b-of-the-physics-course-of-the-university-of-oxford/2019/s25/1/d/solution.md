<h1 id="s25/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a convective layer $T(z)=T_s-\Gamma z$ capped at an isothermal minimum $T_t$ at height $z_t$. Let the initial [optical depth](../../../../../optical-depth.md) be $\tau(z)=\tau_se^{-z/H_\tau}$ and $\tau_t=\tau_se^{-z_t/H_\tau}$. Within the lapse-rate layer, $dB_\lambda/d\tau=B'\Gamma H_\tau/\tau$; above it the derivative vanishes. The supplied [Schwarzschild equation](../../../../../schwarzschild-equation.md) therefore gives

$$
I_0=\pi B_\lambda(T_t)+\pi B'\Gamma H_\tau G(\tau_t,\tau_s).
$$

Assume the additional [carbon dioxide](../../../../../carbon-dioxide.md) multiplies the relevant opacity by $a=1.1$, leaving temperatures, the lapse rate and $H_\tau$ initially fixed. All material surfaces then acquire $a$ times their previous [optical depth](../../../../../optical-depth.md). Hence

$$
\boxed{\Delta I_0=\pi B'\Gamma H_\tau\big[G(1.1\tau_t,1.1\tau_s)-G(\tau_t,\tau_s)\big].}
$$

For $\tau_t\ll1$ and $\tau_s\gg10$, the specified approximation gives

$$
\boxed{\Delta T_{\rm BT}=\frac{\Delta I_0}{\pi B'}=-\Gamma H_\tau\ln1.1\simeq-0.09531\Gamma H_\tau.}
$$

For illustration, $\Gamma=6.5\,\mathrm{K\,km^{-1}}$ and $H_\tau=7\,\mathrm{km}$ give $-4.34\,\mathrm K$; these are illustrative, not supplied data. The inequalities put the effective emitting level $\tau\sim1$ inside the decreasing-temperature layer, well above an opaque surface and below the thin isothermal cap. Increasing opacity raises that emitting level by $H_\tau\ln1.1$, so it is colder. In a spectral window or above a temperature inversion the approximation and possibly the sign change. Opacity proportional to mixing ratio is also an assumption, not exact for every absorption mechanism.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [S25](../../../s25.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
