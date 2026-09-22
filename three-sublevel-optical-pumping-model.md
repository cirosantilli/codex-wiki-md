# Three-sublevel optical pumping model

↑ **Parent:** [Optical pumping](optical-pumping.md)

Consider an original hypothetical atom with a lower [angular momentum](angular-momentum.md) multiplet $F=1$, $m=-1,0,+1$, and one opposite-[parity](parity.md) excited level $F'=0,m'=0$. Stipulate that all [spontaneous emission](spontaneous-emission.md) returns to these three lower [quantum states](quantum-state.md), with no other decay channel. This is an isolated four-state model, not the actual [sodium](sodium.md) or [rubidium](rubidium.md) D-line structure. In particular, the physical [rubidium](rubidium.md) cell above contains multiple [hyperfine structure](hyperfine-structure.md) levels.

The [electric-dipole selection rule](electric-dipole-selection-rule.md) permits $\Delta F=-1$ here; $\sigma^+$ absorption with $\Delta m=+1$ excites only $m=-1$. Decay from $F'=0$ has three equal integrated branching probabilities $b_-=b_0=b_+=1/3$: rotational symmetry gives equal squared [Clebsch-Gordan coefficients](clebsch-gordan-coefficients.md). The emitted [photons](photon.md) carry the three permitted [angular momentum](angular-momentum.md) projections; equal integrated branching does not imply equal intensity in every observation direction. Thus $m=0$ and $m=+1$ are both dark. The chosen beam cannot prepare a unique pure $m=+1$ state.

Let $R\ge0$ be the absorption rate of an atom in $m=-1$, and let $\Gamma$ be the excited-state [spontaneous emission](spontaneous-emission.md) rate, both in inverse seconds. Assume $R,\gamma\ll\Gamma$, negligible [stimulated emission](stimulated-emission.md), and no maintained [quantum coherence](quantum-coherence-in-a-specified-basis.md) between sublevels. Eliminating the short-lived excited population gives normalized lower populations $p_-+p_0+p_+=1$ to this approximation. At each scattering event the atom leaves $m=-1$ with probability $2/3$; the remaining $1/3$ simply returns it there.

Model depolarizing collisions and other population relaxation by resets to the unpolarized distribution at rate $\gamma\ge0$. The [rate equations](rate-equation.md) are

$$
\dot p_-=-\frac{2R}{3}p_-+\gamma\left(\frac13-p_-\right),\qquad
\dot p_0=\frac R3p_-+\gamma\left(\frac13-p_0\right),\qquad
\dot p_+=\frac R3p_-+\gamma\left(\frac13-p_+\right).
$$

This relaxation prescription assumes that [Zeeman splitting](zeeman-splitting.md) is small compared with thermal [energy](energy-split.md), so the unpolarized distribution approximates [thermal equilibrium](thermal-equilibrium-split.md). It is not an energy-independent relaxation law at arbitrarily low [temperature](temperature-split.md).

Every transfer has a nonnegative rate: optical transfers $-\to0$ and $-\to+$ each have rate $R/3$, and relaxation transfers between each distinct pair have rate $\gamma/3$. These define a [continuous-time Markov chain](continuous-time-markov-chain-split.md). The three derivatives sum to zero, and at $p_i=0$ the corresponding derivative cannot be negative. Hence the model conserves population and preserves nonnegative populations. Optical cycles that return to $m=-1$ contribute to scattering even though they cause no net population transfer.

<a id="image-three-sublevel-pumping-spontaneous-branching-and-dark-state-dynamics"></a>
![](optical-pumping-three-sublevel-rate-dynamics.png)

**[Figure 12](#image-three-sublevel-pumping-spontaneous-branching-and-dark-state-dynamics). Three-sublevel pumping, spontaneous branching and dark-state dynamics**. Original hypothetical $F=1\to F'=0$ model. Solid blue shows selective absorption; dashed purple arrows show equal spontaneous branching. Two lower states are dark to the selected beam. Curves start unpolarized and compare pure pumping with chosen $R/\gamma=6$. Rates and curves are stipulated examples, not historical data or a model of the full rubidium spectrum.

## ↑ Ancestors (5)

1. [Optical pumping](optical-pumping.md)
2. [Atomic measurement methods](atomic-measurement-methods.md)
3. [Atomic physics](atomic-physics-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
