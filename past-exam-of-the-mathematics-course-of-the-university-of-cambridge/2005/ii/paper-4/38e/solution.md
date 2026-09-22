<h1 id="38e/solution">Solution</h1>

↑ **Parent:** [38E](../38e.md)

For inviscid barotropic flow, conservation gives $\rho_t+\nabla\cdot(\rho u)=0$ and $\rho(u_t+u\cdot\nabla u)=-\nabla p$. Linearizing about uniform rest $\rho_0,p_0$ gives

$$
\rho'_t+\rho_0\nabla\cdot u=0,\qquad
\rho_0u_t=-\nabla p',\qquad
p'=c_0^2\rho',\qquad
\boxed{c_0^2=(dp/d\rho)_{\rho_0}},
$$

with the [derivative](../../../../../derivative.md) adiabatic for ordinary sound.

Taking curl gives $\partial_t(\nabla\times u)=0$. Therefore the acoustic velocity is irrotational if the initial [vorticity](../../../../../vorticity.md) is zero. Uniform rest as the background does not alone forbid a superposed stationary vortical perturbation: for example $u=\varepsilon(\sin y,0,0)$, $\rho'=p'=0$ solves the linearized equations but has nonzero curl. Thus the printed irrotational conclusion requires the usual restriction to the longitudinal acoustic mode. In that mode set $u=\nabla\phi$ and absorb a time-only gauge into $\phi$, so $p'=-\rho_0\phi_t$. [Continuity](../../../../../continuous-function.md) gives

$$
\boxed{\phi_{tt}-c_0^2\Delta\phi=0}.
$$

This separates the sound wave from the [stationary vorticity mode in linear acoustics](../../../../../stationary-vorticity-mode-in-linear-acoustics.md).

Define the quadratic [acoustic energy density](../../../../../acoustic-energy-density.md) and [acoustic energy flux](../../../../../acoustic-energy-flux.md) by

$$
e=\frac{\rho_0}2|u|^2+\frac{(p')^2}{2\rho_0c_0^2},\qquad
j=p'u.
$$

Multiplying momentum by $u$ and the pressure form of [continuity](../../../../../continuous-function.md) by $p'/(\rho_0c_0^2)$ gives

$$
\boxed{\partial_t e+\nabla\cdot j=0}.
$$

For any progressive [plane wave](../../../../../plane-wave.md), not necessarily sinusoidal, let $\phi=F(\xi)$ with $\xi=\widehat k\cdot x-c_0t$. Then $u=F'(\xi)\widehat k$ and $p'=\rho_0c_0F'(\xi)$. Its kinetic and compressional [energy](../../../../../energy.md) densities both equal $\rho_0(F')^2/2$, so

$$
\boxed{j=c_0\widehat k\,e}.
$$

The [energy](../../../../../energy.md) is transported at the [sound speed](../../../../../speed-of-sound.md) in the propagation direction. A superposition of oppositely traveling waves can form a standing wave and need not have this pointwise equality; the statement concerns a single progressive wave.

For a spherical outgoing wave, $\phi=F(r-c_0t)/r$. Its radial velocity and pressure are

$$
u_r=\frac{F'}r-\frac F{r^2},\qquad p'=\rho_0c_0\frac{F'}r.
$$

Therefore

$$
\boxed{e_K=\frac{\rho_0}2\left(\frac{F'}r-\frac F{r^2}\right)^2,\qquad
e_P=\frac{\rho_0}2\left(\frac{F'}r\right)^2}.
$$

They are generally unequal because of the additional near-field velocity term; their difference is $\rho_0[F^2/r^4-2FF'/r^3]/2$. They agree only to leading far-field order, or for special profile values. This is the [near-field energy imbalance in a spherical acoustic wave](../../../../../near-field-energy-imbalance-in-a-spherical-acoustic-wave.md).

## ↑ Ancestors (10)

1. [38E](../38e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
