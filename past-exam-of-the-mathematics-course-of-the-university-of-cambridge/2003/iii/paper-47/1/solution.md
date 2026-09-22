<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the [Hadamard gate](../../../../../hadamard-gate.md) to be $H=2^{-1/2}\begin{pmatrix}1&1\\1&-1\end{pmatrix}$ and the [phase gate](../../../../../phase-gate.md) to be $P(\phi)=\operatorname{diag}(1,e^{i\phi})$. This fixes the sign convention for the interference phase.

For the coherent [quantum circuit](../../../../../quantum-circuit-split.md), the successive [quantum states](../../../../../quantum-state.md) are

$$
|0\rangle\longmapsto\frac{|0\rangle+|1\rangle}{\sqrt2}
\longmapsto\frac{|0\rangle+e^{i\phi}|1\rangle}{\sqrt2}
\longmapsto\frac{(1+e^{i\phi})|0\rangle+(1-e^{i\phi})|1\rangle}{2}.
$$

The [Born rule](../../../../../born-rule.md) therefore gives the concise answer

$$
\boxed{P_0(\phi)=\frac{|1+e^{i\phi}|^2}{4}=\frac{1+\cos\phi}{2}=\cos^2(\phi/2).}
$$

With the stated [quantum decoherence](../../../../../quantum-decoherence.md) after the [phase gate](../../../../../phase-gate.md), the joint [pure state](../../../../../pure-state.md) before the last [Hadamard gate](../../../../../hadamard-gate.md) is

$$
\frac{|0\rangle|e_0\rangle+e^{i\phi}|1\rangle|e_1\rangle}{\sqrt2}.
$$

After that [Hadamard gate](../../../../../hadamard-gate.md), its environment coefficient at output zero is $(|e_0\rangle+e^{i\phi}|e_1\rangle)/2$. Squaring its [norm](../../../../../norm.md) sums over every unobserved environment outcome, so

$$
P_0=\frac14\left(2+e^{i\phi}\langle e_0|e_1\rangle+e^{-i\phi}\langle e_1|e_0\rangle\right),\qquad
\boxed{P_0(\phi,v,\alpha)=\frac{1+v\cos(\phi+\alpha)}2.}
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $0\le v\le1$. In this [single-qubit interference with conditional environment states](../../../../../single-qubit-interference-with-conditional-environment-states.md), $v$ is the [interference visibility](../../../../../interferometric-visibility.md): orthogonal environment states erase the fringe, while a unit-modulus overlap shifts its phase without reducing visibility. The plus sign in $\phi+\alpha$ follows from the specified overlap $\langle e_0|e_1\rangle$, rather than its complex conjugate.

If the same [quantum decoherence](../../../../../quantum-decoherence.md) occurs before the [phase gate](../../../../../phase-gate.md), the joint [pure state](../../../../../pure-state.md) is first $(|0\rangle|e_0\rangle+|1\rangle|e_1\rangle)/\sqrt2$. The [phase gate](../../../../../phase-gate.md) then produces exactly the same state used above. Equivalently, the controlled environment interaction commutes with the diagonal [phase gate](../../../../../phase-gate.md). **The probability is unchanged.**

For the [Deutsch algorithm](../../../../../deutsch-algorithm.md), use the reversible [Boolean quantum oracle](../../../../../boolean-quantum-oracle.md)

$$
U_f|x\rangle|y\rangle=|x\rangle|y\oplus f(x)\rangle.
$$

The algebraic oracle map printed in the source has its arguments misplaced: taken literally, it sends two distinct answer inputs to the same output for constant $f$, so it cannot be a [unitary operator](../../../../../unitary-operator.md). The corrected map above agrees with the diagram's input-control, answer-target arrangement. Put the answer [qubit](../../../../../qubit.md) in $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$. Since the [Pauli X gate](../../../../../pauli-x-gate.md) satisfies $X|-\rangle=-|-\rangle$, [quantum phase kickback](../../../../../phase-kickback.md) gives

$$
U_f|x\rangle|-\rangle=(-1)^{f(x)}|x\rangle|-\rangle.
$$

Write $b=f(0)\oplus f(1)$. Up to the irrelevant [global phase](../../../../../global-phase.md) $(-1)^{f(0)}$, the input [qubit](../../../../../qubit.md) acquires relative phase $(-1)^b$, so its ideal final [computational-basis measurement](../../../../../quantum-measurement-in-the-computational-basis.md) returns $b$: zero for a constant function and one for a balanced function.

Let the specified [quantum decoherence](../../../../../quantum-decoherence.md) occur in the interference portion between the two [Hadamard gates](../../../../../hadamard-gate.md). It commutes with the oracle's effective diagonal phase on the input, so the same analysis applies whether it occurs just before or just after the query. The two likelihoods are

$$
\Pr(0\mid b)=\frac{1+(-1)^b v\cos\alpha}{2},\qquad
\Pr(1\mid b)=\frac{1-(-1)^b v\cos\alpha}{2}.
$$

Thus the diagram's usual zero-for-constant decision rule has

$$
\boxed{P_{\mathrm{correct}}=\frac{1+v\cos\alpha}{2}.}
$$

This is the reliability for either promised class separately, with no prior needed. For equally likely classes, if $v\cos\alpha$ is known to be negative, reversing the interpretation gives $(1+|v\cos\alpha|)/2$. A known environment phase can instead be compensated by the [phase gate](../../../../../phase-gate.md) $P(-\alpha)$ before the final [Hadamard gate](../../../../../hadamard-gate.md), giving **success probability $(1+v)/2$**. In particular, $v=0$ gives no information and $v=1$ permits certainty after phase compensation. These refinements distinguish a shifted fringe from lost [quantum coherence](../../../../../quantum-coherence-in-a-specified-basis.md); with the unmodified diagram a phase shift alone can reverse the apparent answer. [Quantum decoherence](../../../../../quantum-decoherence.md) after the final [Hadamard gate](../../../../../hadamard-gate.md) leaves its computational populations unchanged, so that different placement would not spoil the measured answer.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
