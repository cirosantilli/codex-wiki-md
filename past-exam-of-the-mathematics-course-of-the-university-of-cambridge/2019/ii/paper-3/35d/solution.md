<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

The [chemical potential](../../../../../chemical-potential.md) is the change in [internal energy](../../../../../internal-energy.md) when one particle is added at fixed [entropy](../../../../../entropy.md) and [volume](../../../../../volume.md):

$$
\mu=\left(\frac{\partial E}{\partial N}\right)_{S,V}.
$$

Equivalently, $\mu=(\partial F/\partial N)_{T,V}$ for the [Helmholtz free energy](../../../../../helmholtz-free-energy.md).

Let a microstate $s$ have [energy](../../../../../energy.md) $E_s$ and particle number $N_s$. Maximizing the [Gibbs entropy](../../../../../gibbs-entropy.md) subject to normalization and fixed mean values of $E$ and $N$ is the [maximum-entropy derivation of equilibrium ensembles](../../../../../maximum-entropy-derivation-of-equilibrium-ensembles.md). With [Lagrange multipliers](../../../../../lagrange-multiplier.md) $\alpha$, $\beta$, and $-\beta\mu$, vary

$$
-\sum_s p_s\log p_s
-\alpha\left(\sum_s p_s-1\right)
-\beta\sum_s p_s(E_s-\mu N_s).
$$

The stationarity equation is $-\log p_s-1-\alpha-\beta(E_s-\mu N_s)=0$. Normalization therefore gives the [grand canonical ensemble](../../../../../grand-canonical-ensemble.md)

$$
\boxed{
p_s=\frac{e^{-\beta(E_s-\mu N_s)}}{\mathcal Z},
\qquad
\mathcal Z=\sum_s e^{-\beta(E_s-\mu N_s)},
\qquad
\beta=\frac1{k_BT}.}
$$

Here $\mathcal Z$ is the [grand canonical partition function](../../../../../grand-canonical-partition-function.md) and $k_B$ is the [Boltzmann constant](../../../../../boltzmann-constant.md).

For one fermionic [quantum state](../../../../../quantum-state.md) of energy $\varepsilon$, the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md) permits occupation numbers only $n=0,1$. Its two grand-canonical weights are $1$ and $e^{-\beta(\varepsilon-\mu)}$, so its mean occupation is the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md)

$$
\boxed{
n_F(\varepsilon)
=\frac{e^{-\beta(\varepsilon-\mu)}}{1+e^{-\beta(\varepsilon-\mu)}}
=\frac1{e^{\beta(\varepsilon-\mu)}+1}.}
$$

For a free nonrelativistic particle, $\varepsilon=\hbar^2k^2/(2m)$. In a region of area $A$, the number of wave-vector states in the annulus from $k$ to $k+dk$, including the two [spin angular momentum](../../../../../spin.md) states, is

$$
2\frac{A}{(2\pi)^2}2\pi k\,dk.
$$

Since $k\,dk=(m/\hbar^2)d\varepsilon$, the [two-dimensional free-electron density of states](../../../../../two-dimensional-free-electron-density-of-states.md) is constant:

$$
\boxed{g(\varepsilon)=\frac{Am}{\pi\hbar^2}.}
$$

We now use units in which $k_B=1$, as in the question. At zero [temperature](../../../../../temperature.md), the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) is a [step function](../../../../../step-function.md), and hence

$$
N=g\int_0^{\varepsilon_F}d\varepsilon=g\varepsilon_F.
$$

At positive temperature the same fixed particle number satisfies the exact relation

$$
N=g\int_0^\infty\frac{d\varepsilon}{e^{(\varepsilon-\mu)/T}+1}
=gT\log(1+e^{\mu/T}).
$$

Thus

$$
\mu=T\log(e^{\varepsilon_F/T}-1)
=\varepsilon_F+T\log(1-e^{-\varepsilon_F/T})
=\varepsilon_F+O(Te^{-\varepsilon_F/T}).
$$

This is the [low-temperature particle-number cancellation for constant density of states](../../../../../low-temperature-particle-number-cancellation-for-constant-density-of-states.md). Therefore, for $T\ll\varepsilon_F$, the mean number of particles in the energy interval $[\varepsilon,\varepsilon+d\varepsilon]$ is

$$
\boxed{
g(\varepsilon)n_F(\varepsilon)d\varepsilon
\simeq
\frac{N}{\varepsilon_F}
\frac{d\varepsilon}{e^{(\varepsilon-\varepsilon_F)/T}+1}.}
$$

Finally, compare the [internal energy](../../../../../internal-energy.md) with its zero-temperature value. The thermally excited particles above $\varepsilon_F$ and holes below $\varepsilon_F$ have equal leading particle numbers, so their terms proportional to $\varepsilon_F$ cancel. With $x=|\varepsilon-\varepsilon_F|/T$,

$$
U(T)-U(0)
=2gT^2\int_0^\infty\frac{x\,dx}{e^x+1}
=\frac{\pi^2}{6}gT^2,
$$

where the integral follows from the [fermion-to-boson thermal integral ratio](../../../../../fermion-to-boson-thermal-integral-ratio.md). Differentiation gives the [linear low-temperature heat capacity of a two-dimensional Fermi gas](../../../../../linear-low-temperature-heat-capacity-of-a-two-dimensional-fermi-gas.md):

$$
\boxed{
C_A=\left(\frac{\partial U}{\partial T}\right)_{N,A}
=\frac{\pi^2}{3}gT
=\frac{\pi^2N}{3\varepsilon_F}T.}
$$

The requested [power law](../../../../../power-law.md) is therefore **linear in $T$**, with exponent one.

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
