# Finite trajectory entropy production

↑ **Parent:** [Fluctuation theorem](fluctuation-theorem.md)

Consider a finite-duration [Markov process](markov-process-split.md) with discrete, time-even states coupled to one [thermal reservoir](heat-bath.md) at positive [temperature](temperature.md) $T$. Let $P_F[\gamma]$ include the initial [probability](probability.md) $\rho_0(x_0)$ of the [sample trajectory](sample-path.md) $\gamma$. Define $P_R$ by reversing the control protocol and initializing it with the actual forward final [probability distribution](probability-distribution.md) $\rho_\tau$. Write $\Theta\gamma$ for the same states visited in reverse time order. Require normalized path laws with matching [probability support](support-of-a-probability-distribution.md): a path has positive forward weight exactly when its reverse has positive reverse weight. This excludes irreversible forbidden transitions and missing initial states.

Under [local detailed balance](local-detailed-balance.md), with positive [heat](heat.md) $Q_{\rm bath}$ delivered to the [thermal reservoir](heat-bath.md), the full path-weight [logarithm](logarithm.md) is

$$
\Sigma_F[\gamma]=\ln\frac{P_F[\gamma]}{P_R[\Theta\gamma]}
=\frac{Q_{\rm bath}[\gamma]}{k_BT}+\ln\frac{\rho_0(x_0)}{\rho_\tau(x_\tau)}
=\frac{\Delta S_{\rm tot}[\gamma]}{k_B}.
$$

The endpoint term is the change in stochastic system [entropy](entropy.md); the conditional path ratio alone accounts for the [thermal reservoir](heat-bath.md). Here $k_B$ is the [Boltzmann constant](boltzmann-constant.md). Both terms matter even for a short observation. [Seifert, 2005, Eqs. (14)–(18) and (30): conditional and full path weights, endpoint distributions, total entropy](entropy-production-along-a-stochastic-trajectory-and-an-integral-fluctuation-theorem-by-udo-seifert.md)

Define the conjugate reverse functional by $\Sigma_R[\eta]=\ln(P_R[\eta]/P_F[\Theta\eta])$, so $\Sigma_R[\Theta\gamma]=-\Sigma_F[\gamma]$. Summing the path identity over paths with a given value gives the exact finite [fluctuation theorem](fluctuation-theorem.md)

$$
\frac{p_F(s)}{p_R(-s)}=e^s,
$$

for nonzero denominator, using [probability masses](probability-mass.md) or corresponding [probability density functions](probability-density-function.md). This $\Sigma_R$ is defined by the paired laws: it need not be the total [entropy production](entropy-production.md) obtained by independently restarting the thermodynamic construction for the reverse experiment. A generic driven experiment therefore does not imply $p_F(s)/p_F(-s)=e^s$.

**Table of contents**

- [Integral fluctuation theorem](integral-fluctuation-theorem.md)

## ↑ Ancestors (8)

1. [Fluctuation theorem](fluctuation-theorem.md)
2. [Entropy production](entropy-production.md)
3. [Stochastic thermodynamics](stochastic-thermodynamics.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Crooks fluctuation theorem](crooks-fluctuation-theorem.md)
- [Dragged-bead fluctuation theorem experiment](dragged-bead-fluctuation-theorem-experiment.md)
