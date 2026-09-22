# Gibbs free energy of an ideal-gas mixture

↑ **Parent:** [Gibbs free energy](gibbs-free-energy.md)

For a single-phase [ideal gas](ideal-gas.md) mixture with molar amounts $N_i$, common [temperature](temperature.md) $T$, and [pressure](pressure.md) $P$, extensivity and ideal mixing give

$$
G=\sum_iN_i\mu_i=N\sum_i x_i\left[\mu_i^\circ(T)+\mathcal RT\log\left(\frac{x_iP}{P^\circ}\right)\right].
$$

Here $N=\sum_iN_i$, $x_i$ is the [mole fraction](mole-fraction.md), $\mathcal R$ is the molar gas constant, and $P^\circ$ is the standard [pressure](pressure.md). Integrating $\partial\mu_i/\partial P=\mathcal RT/P$ and including the ideal mixing [entropy](entropy.md) proves $\mu_i=\mu_i^\circ+\mathcal RT\log(x_iP/P^\circ)$. Reactions can change $N$, so fractions alone do not set the extensive [Gibbs free energy](gibbs-free-energy.md). Its composition Hessian is $\mathcal RT(\delta_{ij}/N_i-1/N)$; it is positive semidefinite by the weighted [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md).

## ↑ Ancestors (6)

1. [Gibbs free energy](gibbs-free-energy.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/2/b/ii/solution.md)
