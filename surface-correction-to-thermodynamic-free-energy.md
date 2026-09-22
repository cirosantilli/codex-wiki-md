# Surface correction to thermodynamic free energy

↑ **Parent:** [Thermodynamic limit](thermodynamic-limit.md)

For finite-range interactions and bounded wall couplings, only sites within an interaction range of the wall have altered local environments. In a regular container of linear size $L$ and dimension $d$, the [surface area](surface-area.md) scales as $A\sim L^{d-1}$ while [volume](volume-thermodynamics.md) scales as $V\sim L^d$. A boundary contribution of order $A$ therefore gives an order-$1/L$ correction to [free-energy density](free-energy-density.md). Away from a [critical phenomenon](critical-phenomenon-split.md), a regular surface contribution often has the form $F=Vf+A\gamma+\cdots$, with $\gamma$ a wall [Helmholtz free energy](helmholtz-free-energy.md) per area. Critical [finite-size rounding](finite-size-rounding.md), edges and long-range interactions require separate care; vanishing relative boundary size does not guarantee a simple surface expansion in every regime.

An exact check uses the zero-field nearest-neighbour [Ising model](ising-model.md) on a chain of $N\ge3$ sites with fixed coupling $J>0$ and $K=J/(k_BT)$. The open chain has $N-1$ bonds, while the periodic ring has $N$. Their finite [partition functions](canonical-partition-function.md) and dimensionless [Helmholtz free energies](helmholtz-free-energy.md) per spin $g_N=F_N/(Nk_BT)$ are

$$
Z_N^{\rm open}=2(2\cosh K)^{N-1},\qquad
Z_N^{\rm ring}=(2\cosh K)^N+(2\sinh K)^N,
$$



$$
g_\infty=-\log(2\cosh K),\qquad
g_N^{\rm open}-g_\infty=\frac{\log\cosh K}{N},\qquad
g_N^{\rm ring}-g_\infty=-\frac{\log[1+(\tanh K)^N]}{N}.
$$

For the open chain, sum the last [Ising spin](ising-spin-variable.md) successively: each removed bond contributes $2\cosh K$, leaving a factor of two. For the ring, the [transfer matrix for the one-dimensional Ising model](transfer-matrix-for-the-one-dimensional-ising-model.md) has [eigenvalues](eigenvalue.md) $2\cosh K$ and $2\sinh K$, and its $N$th power's [trace](matrix-trace.md) gives the displayed sum. The two ends are a constant-size boundary in one dimension, so the open-chain total correction is $k_BT\log\cosh K$, and its per-spin correction is exactly proportional to $1/N$.

<a id="image-exact-boundary-corrections-for-a-finite-ising-chain-and-ring"></a>
![](ising-chain-finite-boundary-free-energy.png)

**[Figure 10](#image-exact-boundary-corrections-for-a-finite-ising-chain-and-ring). Exact boundary corrections for a finite Ising chain and ring**.

Both sets of finite results approach the same $g_\infty$ at the fixed plotted $K=0.8$. Multiplying the correction by $N$ exposes the open-chain boundary term, while the ring correction vanishes exponentially at fixed finite $K$. This model's [thermodynamic limit](thermodynamic-limit.md) remains a [real analytic function](real-analytic-function.md) at every positive [temperature](temperature.md): having a [thermodynamic limit](thermodynamic-limit.md) does not require a [phase transition](phase-transition.md).

## ↑ Ancestors (5)

1. [Thermodynamic limit](thermodynamic-limit.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Thermodynamic limit](thermodynamic-limit.md)
