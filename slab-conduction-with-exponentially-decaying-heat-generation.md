# Slab conduction with exponentially decaying heat generation

↑ **Parent:** [Thermal conduction](thermal-conduction.md)

A one-dimensional [thermal conduction](thermal-conduction.md) model with constant [thermal conductivity](thermal-conductivity.md), source $q'''(x)=q_0e^{-\mu x}$ and prescribed face [temperatures](temperature-split.md) $T(0)=T(a)=T_0$. Its [steady state](steady-state.md) solution is

$$
T-T_0=\frac{q_0}{k\mu^2}\left[1-e^{-\mu x}-(1-e^{-\mu a})\frac{x}{a}\right].
$$

Positive internal heating makes the profile concave. Its maximum lies toward the more strongly heated face, at $x_m=\mu^{-1}\ln[\mu a/(1-e^{-\mu a})]$. The uniform-source limit is $T-T_0=q_0x(a-x)/(2k)$.

## ↑ Ancestors (7)

1. [Thermal conduction](thermal-conduction.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
