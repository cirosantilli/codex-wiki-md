# Vorticity-sheet eigenfunction of inviscid Couette flow

↑ **Parent:** [Inviscid Couette continuous spectrum](inviscid-couette-continuous-spectrum.md)

Let $G_a$ be the [Dirichlet Green function](dirichlet-green-function.md) of $D^2-a^2$ on $[-1,1]$, with $a=|\alpha|$:

$$
G_a(z,\xi)=-\frac{\sinh[a(z_<+1)]\sinh[a(1-z_>)]}{a\sinh(2a)}.
$$

It is continuous and has derivative jump one, so $(D^2-a^2)G_a=\delta(z-\xi)$. The [Dirac delta multiplication identity](dirac-delta-multiplication-identity.md) gives $(z-\xi)\delta(z-\xi)=0$, proving it is a [generalized eigenfunction](generalized-eigenfunction.md) of the [inviscid Couette continuous spectrum](inviscid-couette-continuous-spectrum.md). Integrating $G_a(z,\xi)q_0(\xi)e^{-i\alpha\xi t}$ reconstructs the evolving vertical [velocity](velocity.md) from its initial vorticity.

## ↑ Ancestors (7)

1. [Inviscid Couette continuous spectrum](inviscid-couette-continuous-spectrum.md)
2. [Rayleigh equation for inviscid shear flow](rayleigh-equation-for-inviscid-shear-flow.md)
3. [Hydrodynamic stability](hydrodynamic-stability-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
