<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

There is a necessary distinction between a failure bound averaged over the unknown state, a worst-case bound, and a separate bound for each candidate state. The last interpretation is false: a forger can discard the inputs and always prepare $|\psi_0\rangle^{\otimes N}$. If the actual state is $|\psi_0\rangle$, every authenticity test passes with [probability](../../../../../probability.md) one. **The meaningful uniform statement concerns worst-case failure, or average failure under any fixed prior giving both states positive probability.** The PDF does not specify that prior; the argument below gives an explicit bound for either interpretation.

Put $c=|\langle\psi_0|\psi_1\rangle|\in(0,1)$. Any unconditional strategy producing $N$ output [qubits](../../../../../qubit.md), including ancillas, adaptive [measurement in quantum measurements](../../../../../quantum-measurement-split.md) and correlated outputs, is a [quantum channel](../../../../../quantum-channel.md) $\mathcal E$. Its inputs and ideal outputs are the [density operators](../../../../../density-matrix.md)

$$
\sigma_i=\big(|\psi_i\rangle\langle\psi_i|\big)^{\otimes M},\qquad P_i=\big(|\psi_i\rangle\langle\psi_i|\big)^{\otimes N},\qquad \rho_i=\mathcal E(\sigma_i).
$$

The [projective measurements](../../../../../projective-measurement.md) on the different banknotes commute, and their all-pass effect is exactly $P_i$. Therefore the [probability](../../../../../probability.md) of at least one rejection, conditional on input $i$, is

$$
e_i=1-\operatorname{Tr}(P_i\rho_i).
$$

This remains true for entangled outputs; no independence of their individual test outcomes is assumed.

Use [trace distance](../../../../../trace-distance.md) $D(\rho,\sigma)=\tfrac12\|\rho-\sigma\|_1$. The [pure-state trace distance and fidelity identity](../../../../../pure-state-trace-distance-and-fidelity-identity.md) gives

$$
D(\sigma_0,\sigma_1)=\sqrt{1-c^{2M}},\qquad D(P_0,P_1)=\sqrt{1-c^{2N}}.
$$

For completeness, two pure-state projectors differ by a [matrix](../../../../../matrix.md) with nonzero [eigenvalues](../../../../../eigenvalue.md) $\pm\sqrt{1-|\langle u|v\rangle|^2}$, which proves this identity. Also the [pure-target upper bound on trace distance](../../../../../pure-target-upper-bound-on-trace-distance.md) gives $D(\rho_i,P_i)\leq\sqrt{e_i}$. To see the mixed-state step, write $\rho_i=\sum_jq_j|u_j\rangle\langle u_j|$ and use [convexity](../../../../../convex-function.md) of the [trace norm](../../../../../trace-norm.md) followed by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md):

$$
D(\rho_i,P_i)\leq\sum_jq_j\sqrt{1-\langle u_j|P_i|u_j\rangle}\leq\sqrt{1-\operatorname{Tr}(P_i\rho_i)}.
$$

Finally, [trace-distance contraction under quantum channels](../../../../../trace-distance-contraction-under-quantum-channels.md) gives $D(\rho_0,\rho_1)\leq D(\sigma_0,\sigma_1)$. This follows from $D(\rho,\sigma)=\max_{0\leq E\leq I}\operatorname{Tr}[E(\rho-\sigma)]$: the adjoint channel is positive and unital, so its image of any effect $E$ is still an effect.

The [triangle inequality](../../../../../triangle-inequality.md) now yields

$$
\begin{aligned}
\sqrt{1-c^{2N}}&\leq D(P_0,\rho_0)+D(\rho_0,\rho_1)+D(\rho_1,P_1)\\
&\leq\sqrt{e_0}+\sqrt{1-c^{2M}}+\sqrt{e_1}.
\end{aligned}
$$

Thus the [cloning failure bound from trace-distance contraction](../../../../../cloning-failure-bound-from-trace-distance-contraction.md) is

$$
\sqrt{e_0}+\sqrt{e_1}\geq\Delta,\qquad \Delta=\sqrt{1-c^{2N}}-\sqrt{1-c^{2M}}>0,
$$

and in particular $\max(e_0,e_1)\geq\Delta^2/4$. For positive priors $\pi_0+\pi_1=1$, another [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
(\sqrt{e_0}+\sqrt{e_1})^2\leq(\pi_0e_0+\pi_1e_1)(\pi_0^{-1}+\pi_1^{-1}),
$$

so the average rejection [probability](../../../../../probability.md) satisfies

$$
\boxed{P_{\mathrm{fail}}=\pi_0e_0+\pi_1e_1\geq\pi_0\pi_1\Delta^2>p_0:=\tfrac12\pi_0\pi_1\Delta^2>0.}
$$

For equal priors, one may take $p_0=\Delta^2/8$; the same choice is a strict lower bound on worst-case rejection. This proves a quantitative version of the [no-cloning theorem](../../../../../no-cloning-theorem.md) for the bank's all-pass test. It concerns an unconditional attempt: heralded success cannot be postselected while omitting failed attempts from the accounting.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
