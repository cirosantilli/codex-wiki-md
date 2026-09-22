# Ising ring bond correlation

↑ **Parent:** [Four-spin Ising ring](four-spin-ising-ring.md)

The [Ising ring bond correlation](ising-ring-bond-correlation.md) is the neighboring [two-point correlation function](two-point-correlation-function.md) $c_1=\langle\sigma_i\sigma_{i+1}\rangle$ in the [four-spin Ising ring](four-spin-ising-ring.md). All four [edges](edge-of-a-graph.md) are equivalent. At zero field each mean [Ising spin](ising-spin-variable.md) is zero by [spin inversion symmetry](spin-inversion-symmetry.md), so $c_1$ also equals the [connected correlation function](connected-correlation-function.md). Agreement gives bond product $+1$ and disagreement $-1$; thus $P(\sigma_i=\sigma_{i+1})=(1+c_1)/2$.

Differentiating the finite [partition function](canonical-partition-function.md) with respect to $K=\beta J$ inserts the sum of four bond products. Therefore

$$
c_1=\frac14\frac{d\log Z}{dK}
=\frac{\sinh(4K)}{\cosh(4K)+3},\qquad
U=\langle H\rangle=-4Jc_1.
$$

Here $U$ is [internal energy](internal-energy-split.md). At $K=(\ln2)/4$, the class-weight calculation gives $c_1=(4-1)/17=3/17$ and $U=-12J/17$. The agreement [probability](probability.md) for a selected bond is $10/17$, despite the exactly zero mean [spin magnetization](spin-magnetization.md).

A second [derivative](derivative.md) gives the [energy](energy-split.md) [variance](variance-split.md), and hence the [heat capacity](heat-capacity.md) $C_H=dU/dT$ at fixed $J$ and $h=0$:

$$
\frac{\operatorname{Var}(H)}{J^2}
=\frac{d^2\log Z}{dK^2}
=\frac{16[1+3\cosh(4K)]}{[\cosh(4K)+3]^2},\qquad
\frac{C_H}{k_B}=K^2\frac{\operatorname{Var}(H)}{J^2}.
$$

To see the [variance](variance-split.md) identity directly, a [derivative](derivative.md) of an [expected value](expected-value-split.md) under weights $e^{KS}$ inserts $S-\langle S\rangle$, where $S=\sum_i\sigma_i\sigma_{i+1}=-H/J$. The factor $K^2$ follows from $dK/dT=-K/T$. At the same exact example, $\operatorname{Var}(H)/J^2=1216/289$. The [heat capacity](heat-capacity.md) vanishes both as $K\to0$ and as $K\to\infty$: at high [temperature](temperature-split.md) its dimensionless factor $K^2$ vanishes, while at low [temperature](temperature-split.md) excited [microstates](microstate.md) become exponentially rare.

## ↑ Ancestors (7)

1. [Four-spin Ising ring](four-spin-ising-ring.md)
2. [Ising model](ising-model.md)
3. [Spin model](spin-model-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ising ring bond correlation](ising-ring-bond-correlation.md)
- [Ising ring magnetization fluctuations](ising-ring-magnetization-fluctuations.md)
