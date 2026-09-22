# Trapped-ion sideband pulse model

↑ **Parent:** [Motional sideband](motional-sideband.md)

Consider an original ideal calculation with no heating, [decoherence](quantum-decoherence.md), detuning or spectator modes. In the ordered basis $(|g,n\rangle,|e,n-1\rangle)$ for $n\ge1$, the red [motional sideband](motional-sideband.md) has $H_r=\hbar\eta\Omega\sqrt n\,\sigma_x/2$. Here $\sigma_x$ is the [Pauli matrix](pauli-matrices.md) exchanging the two basis states. Since $\sigma_x^2=I$, its [unitary time evolution](unitary-time-evolution.md) is

$$
U_n(t)=\cos\frac{\theta\sqrt n}{2}\,I-i\sin\frac{\theta\sqrt n}{2}\,\sigma_x,\qquad
\theta=\eta\Omega t.
$$

Thus $U_n^\dagger U_n=I$, and excitation from $|g,n\rangle$ has [probability](probability.md) $P_r(n,t)=\sin^2(\theta\sqrt n/2)$. For $n=0$ it vanishes. The blue [motional sideband](motional-sideband.md) similarly gives $P_b(n,t)=\sin^2(\theta\sqrt{n+1}/2)$. A red [Rabi pi pulse](rabi-pi-pulse.md) calibrated for $n=1$ has $\theta=\pi$; it is not a [Rabi pi pulse](rabi-pi-pulse.md) for every occupied $n$.

Choose $\eta=0.08$, $\Omega/(2\pi)=100\ \mathrm{kHz}$ and $\nu/(2\pi)=2\ \mathrm{MHz}$. The $n=1$ red [Rabi pi pulse](rabi-pi-pulse.md) lasts $t_\pi=\pi/(\eta\Omega)=62.5\ \mathrm{\mu s}$. Let motion have the [Boltzmann distribution](boltzmann-distribution.md) of a [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md), with chosen mean occupation $\bar n=0.25$:

$$
p_n=(1-r)r^n,\qquad r=\frac{\bar n}{1+\bar n}=0.2,\qquad
P_r(t)=\sum_{n=0}^{\infty}p_n\sin^2\frac{\theta\sqrt n}{2},\qquad
P_b(t)=\sum_{n=0}^{\infty}p_n\sin^2\frac{\theta\sqrt{n+1}}{2}.
$$

Here $\sum p_n=1$, $\sum np_n=\bar n$ and $p_0=0.8$. Reindex the red sum using $n=m+1$ and $p_{m+1}=rp_m$: $P_r(t)=rP_b(t)$ for equal resonant pulse parameters, even outside the short-pulse limit. At times with $P_b>0$, the ratio $R=P_r/P_b$ therefore gives $\bar n=R/(1-R)$. A nonthermal distribution, unequal drive strengths, detuning or state-detection bias can invalidate that thermometer. Ground-state population cannot generally be deduced from the mean alone without specifying the distribution.

<a id="image-chosen-thermal-motion-and-ideal-red-blue-sideband-pulse-responses"></a>
![](trapped-ion-thermal-sideband-pulse.png)

**[Figure 7](#image-chosen-thermal-motion-and-ideal-red-blue-sideband-pulse-responses). Chosen thermal motion and ideal red/blue sideband pulse responses**. Original calculation with stipulated parameters, not experimental data. Both responses average the same initial thermal number-state distribution. The vertical line marks a red pi pulse for the $n=1$ component; a thermal mixture has no single common pi-pulse time.

The chosen pulse gives $P_r\simeq0.181393$ and $P_b\simeq0.906967$. These are internal excitation [probabilities](probability.md), not [quantum gate](quantum-logic-gate.md) fidelities or cooling-cycle efficiencies. An independent [matrix](matrix.md) exponentiation of each two-state block agrees with the sine formula and preserves normalization. Summing $n=0,\ldots,79$ omits [probability](probability.md) $r^{80}<1.21\times10^{-56}$; because every sine squared lies between zero and one, this also bounds each omitted response. The thermal relation supplies a separate dimensional check:

$$
\bar n=\frac{1}{e^{\hbar\nu/(k_BT)}-1},\qquad
T=\frac{\hbar\nu}{k_B\log(1+1/\bar n)}\simeq59.6\ \mathrm{\mu K}.
$$

Here $k_B$ is the [Boltzmann constant](boltzmann-constant.md). Substitution recovers $\bar n=0.25$; the thermal root-mean-square expansion parameter is $\eta\sqrt{2\bar n+1}\simeq0.098$. This checks the populated part of the [Lamb-Dicke regime](lamb-dicke-regime.md), while exponentially rare large $n$ still exceed any fixed small-parameter criterion. The pulse is a leading-order model; it does not bound corrections from the full coupling or experimental noise.

## ↑ Ancestors (8)

1. [Motional sideband](motional-sideband.md)
2. [Trapped-ion internal and motional states](trapped-ion-internal-and-motional-states.md)
3. [Trapped-ion quantum control](trapped-ion-quantum-control.md)
4. [Ion trap](ion-trap.md)
5. [Atomic measurement methods](atomic-measurement-methods.md)
6. [Atomic physics](atomic-physics-split.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
