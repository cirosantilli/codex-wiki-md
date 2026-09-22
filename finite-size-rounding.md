# Finite-size rounding

↑ **Parent:** [Thermodynamic limit](thermodynamic-limit.md)

[Finite-size rounding](finite-size-rounding.md) replaces a limiting discontinuity or divergence by a finite crossover or peak. For a spatial system near a [continuous phase transition](continuous-phase-transition.md), the bulk description ceases to apply unchanged when the [correlation length](correlation-length.md) becomes comparable with the sample size. How the crossover width and location depend on size also depends on the model, geometry and [boundary conditions](boundary-condition.md); there is no universal $1/N$ rule for every [phase transition](phase-transition.md).

An exact finite example is the [Curie–Weiss model](curie-weiss-model.md) with $s_i=\pm1$, $J>0$, and a conjugate field $h$ in [energy](energy.md) units. Set $K=J/(k_BT)$ and $u=h/(k_BT)$. Its [statistical Hamiltonian](statistical-hamiltonian.md) and finite [partition function](canonical-partition-function.md) are

$$
H_N=-\frac{J}{2N}\left(\sum_i s_i\right)^2-h\sum_i s_i,\qquad
Z_N(K,u)=\sum_{k=0}^N\binom Nk\exp\left[\frac{K}{2N}(2k-N)^2+u(2k-N)\right].
$$

The [binomial coefficient](binomial-coefficient.md) counts the [microstates](microstate.md) with $k$ positive [Ising spins](ising-spin-variable.md). The diagonal terms in the square add a configuration-independent constant to the [energy](energy.md); retaining them fixes the normalization used here. Divide each summand by $Z_N$ to obtain the [probability mass function](probability-mass-function.md) of $m_k=(2k-N)/N$. In particular,

$$
\langle m\rangle=\frac1N\partial_u\log Z_N,\qquad
\partial_u\langle m\rangle=N\operatorname{Var}(m).
$$

The [variance](variance-split.md) expression makes the finite response nonnegative, while [spin inversion symmetry](spin-inversion-symmetry.md) gives $\langle m\rangle=0$ exactly at $u=0$ for every plotted $N$.

<a id="image-exact-finite-curie-weiss-rounding-in-field-and-temperature"></a>
![](curie-weiss-finite-size-rounding.png)

**[Figure 9](#image-exact-finite-curie-weiss-rounding-in-field-and-temperature). Exact finite Curie–Weiss rounding in field and temperature**.

Every curve is computed from the finite [partition function](canonical-partition-function.md), without selecting one minimum of the [Bragg-Williams free energy of the Ising model](bragg-williams-free-energy-of-the-ising-model.md). The field panel holds $K=1.5$ fixed and shows increasingly rapid switching between opposite [spin magnetizations](spin-magnetization.md). The [temperature](temperature.md) panel uses $u=0$: its nonzero $\langle|m|\rangle$ measures the typical magnitude, while the mean [spin magnetization](spin-magnetization.md) stays zero. The reference $k_BT/J=1$ marks the limiting [critical temperature](critical-temperature.md), not a singular point of any finite curve.

A short limiting argument explains the field panel. Combining the [binomial coefficient](binomial-coefficient.md) with its leading [entropy](entropy.md) gives a [Helmholtz free energy](helmholtz-free-energy.md) per spin whose stationarity equation is $m=\tanh(Km+u)$. For $K>1$ and $u=0$ the two ordered minima have $m=\pm m_*$, where $m_*=\tanh(Km_*)$. For large $N$ well below the [critical temperature](critical-temperature.md), their relative [Boltzmann weight](boltzmann-factor.md) is approximately $e^{2Num_*}$, giving $\langle m\rangle\approx m_*\tanh(Num_*)$. Thus this two-peak approximation has a field width of order $1/(Nm_*)$ in $u$. It is not valid at the [critical temperature](critical-temperature.md), where the peaks merge; the figure uses the exact finite sum throughout.

## ↑ Ancestors (5)

1. [Thermodynamic limit](thermodynamic-limit.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite-size rounding](finite-size-rounding.md)
- [Surface correction to thermodynamic free energy](surface-correction-to-thermodynamic-free-energy.md)
- [Thermodynamic limit](thermodynamic-limit.md)
