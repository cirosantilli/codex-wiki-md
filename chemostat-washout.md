# Chemostat washout

↑ **Parent:** [Chemostat](chemostat.md)

[Chemostat washout](chemostat-washout.md) means the culture's [biomass concentration](biomass-concentration.md) tends to zero because growth cannot sustain replacement of the cells leaving the vessel. In the ideal [Monod equation](monod-equation.md) [chemostat](chemostat.md) with $D>0$, its [equilibrium](equilibrium-point-of-a-dynamical-system.md) is $(s,x)=(s_{\mathrm{in}},0)$. Its [Jacobian matrix](jacobian-matrix.md) has [eigenvalues](eigenvalue.md) $-D$ and $\mu(s_{\mathrm{in}})-D$: a small inoculum grows when $D<\mu(s_{\mathrm{in}})$, whereas [chemostat washout](chemostat-washout.md) is [locally asymptotically stable](asymptotic-stability.md) when $D>\mu(s_{\mathrm{in}})$. For nonnegative initial [concentrations](concentration.md), [chemostat washout](chemostat-washout.md) occurs for $D\ge\mu(s_{\mathrm{in}})$; the boundary case also loses biomass asymptotically.

At $D=D_c$ the positive [chemostat steady state](chemostat-steady-state.md) meets the [chemostat washout](chemostat-washout.md) [equilibrium](equilibrium-point-of-a-dynamical-system.md), and one [eigenvalue](eigenvalue.md) is zero, so linearization alone does not decide the boundary case. On the invariant nutrient-equivalent balance $s+x/Y=s_{\mathrm{in}}$, small positive $x$ obeys $\dot x=-[\mu'(s_{\mathrm{in}})/Y]x^2+O(x^3)$: nutrient consumption lowers the [specific growth rate](specific-growth-rate.md) below $D_c$, leading to slow decay rather than a positive [biomass concentration](biomass-concentration.md). The continued mathematical branches exchange stability in a [transcritical bifurcation](transcritical-bifurcation.md); the positive-biomass branch becomes physically inadmissible beyond $D_c$.

## ↑ Ancestors (5)

1. [Chemostat](chemostat.md)
2. [Mathematical biology](mathematical-biology-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Chemostat](chemostat.md)
- [Chemostat steady state](chemostat-steady-state.md)
- [Chemostat washout](chemostat-washout.md)
- [Dilution rate](dilution-rate.md)
