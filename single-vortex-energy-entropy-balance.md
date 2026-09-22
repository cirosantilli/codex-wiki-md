# Single-vortex energy-entropy balance

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](berezinskii-kosterlitz-thouless-transition.md)

Consider an original counting example: a square two-dimensional [XY model](xy-model.md) of side $L$, a microscopic core radius $a$, and a fixed [phase stiffness](phase-stiffness.md) $\rho_s$. This deliberately neglects screening by other [vortices](phase-vortex.md). Away from a unit [phase vortex](phase-vortex.md), $\theta=\arg(x+iy)$ and $|\nabla\theta|=1/r$. Integrating the [Goldstone-mode effective free energy](goldstone-mode-effective-free-energy.md) over an annulus gives

$$
E_{\rm v}=E_c+\frac{\rho_s}{2}\int_a^L\frac{2\pi r\,dr}{r^2}
=E_c+\pi\rho_s\log(L/a).
$$

Boundary shape changes finite terms. There are order $(L/a)^2$ core positions, so the positional [entropy](entropy-split.md) is $S_{\rm v}=2k_B\log(L/a)+O(k_B)$, where $k_B$ is the [Boltzmann constant](boltzmann-constant.md). With $K=\rho_s/(k_BT)$, subtracting $TS_{\rm v}$ gives the displayed [free energy](thermodynamic-free-energy.md).

For $L/a=1000$ and $E_c/(k_BT)=2$, the dimensionless [free energy](thermodynamic-free-energy.md) cost is about $5.546$ at $K=0.8$ and $-0.965$ at $K=0.5$. The same logarithm appears in the cost and the positional reward: increasing the system size strengthens whichever has the larger coefficient. The corresponding one-defect [Boltzmann factors](boltzmann-factor.md), about $0.00390$ and $2.62$, are relative statistical weights, not normalized probabilities. The latter signals failure of a dilute single-defect estimate.

A single net [phase vortex](phase-vortex.md) requires compatible boundaries: on a periodic sample use neutral pairs, as required by [vortex charge neutrality](vortex-charge-neutrality.md). This argument identifies a possible threshold, but predicting the [universal stiffness jump](universal-stiffness-jump.md) requires the renormalized [phase stiffness](phase-stiffness.md), after smaller pairs have responded. It does not justify setting the transition [temperature](temperature-split.md) equal to a bare lattice coupling divided by a universal constant.

## ↑ Ancestors (7)

1. [Berezinskii–Kosterlitz–Thouless transition](berezinskii-kosterlitz-thouless-transition.md)
2. [Lower critical dimension](lower-critical-dimension.md)
3. [Critical phenomenon](critical-phenomenon-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
