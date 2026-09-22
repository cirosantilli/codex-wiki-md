# Mayer f-function

↑ **Parent:** [Pair potential](pair-potential.md)

The [Mayer f-function](mayer-f-function.md) measures how a [pair potential](pair-potential.md) changes a pair's [Boltzmann factor](boltzmann-factor.md) relative to the noninteracting value one:

$$
f(r)=e^{-\beta u(r)}-1,\qquad \beta=\frac{1}{k_BT}.
$$

It vanishes where $u=0$, lies between $-1$ and $0$ for repulsion, and is positive for attraction. Even an infinite hard-core [potential energy](potential-energy.md) produces the finite value $f=-1$. This is why expanding in [Mayer f-functions](mayer-f-function.md) handles a [hard-sphere gas](hard-sphere-gas.md) more naturally than a [Taylor series](taylor-series.md) in $u$. [Tong, section 2.5.1, equation 2.72](https://davidtong.org/teaching/statistical-physics/statmechhtml/S2#S2.S5.SS1)

For pairwise-additive [potential energy](potential-energy.md) $U=\sum_{i<j}u(r_{ij})$, the exact identity

$$
e^{-\beta U}=\prod_{i<j}\bigl[1+f(r_{ij})\bigr]
$$

turns the configurational part of the [canonical partition function](canonical-partition-function.md) into a sum of products associated with pairs. Drawing one edge for each chosen factor $f(r_{ij})$ gives the [graphs](graph-split.md) used in the [cluster expansion](cluster-expansion.md). The [second virial coefficient](second-virial-coefficient.md) uses just one pair's relative-position [integral](integral.md), $B_2=-\frac12\int f\,d^3\mathbf r$.

For the square-well toy [pair potential](pair-potential.md) in [second virial coefficient](second-virial-coefficient.md), $f=-1$ in the core, $f=e^{1/T^*}-1$ in the attractive shell, and $f=0$ beyond it. Its positive plateau need not be small: low [number density](number-density.md), rather than small $f$ at every separation, controls the dilute-gas approximation. The [integral](integral.md) weights each plateau by spherical-shell [volume](volume.md); equal-looking unweighted areas on a plot of $f$ versus $r$ need not cancel in $B_2$.

## ↑ Ancestors (5)

1. [Pair potential](pair-potential.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Cluster expansion](cluster-expansion.md)
- [Hard-sphere gas](hard-sphere-gas.md)
- [Mayer f-function](mayer-f-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/35a/ii/solution.md)
- [Second virial coefficient](second-virial-coefficient.md)
