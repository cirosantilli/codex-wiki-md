<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) with outcomes $m$ is specified, in the single-operator-per-outcome description, by [linear operators](../../../../../linear-operator.md) $M_m$ satisfying $\sum_mM_m^\dagger M_m=I$. Its effects $F_m=M_m^\dagger M_m$ form a [positive operator-valued measure](../../../../../positive-operator-valued-measure.md). The two measurement postulates are the [Born rule](../../../../../born-rule.md) for outcomes and the conditional state update:

$$
\boxed{p_m=\langle\psi|M_m^\dagger M_m|\psi\rangle,\qquad
|\psi\rangle\longmapsto\frac{M_m|\psi\rangle}{\sqrt{p_m}}\quad(p_m>0).}
$$

For a [density operator](../../../../../density-matrix.md) the corresponding formulas are $p_m=\operatorname{Tr}(M_m\rho M_m^\dagger)$ and $\rho_m=M_m\rho M_m^\dagger/p_m$. More general [quantum instruments](../../../../../quantum-instrument.md) have multiple operators for each outcome and sum these terms. For a [projective measurement](../../../../../projective-measurement.md) of an [observable](../../../../../observable.md) $A=\sum_m a_mP_m$, take $M_m=P_m$; the outcome value is $a_m$ and the postmeasurement state lies in its eigenspace. A POVM alone specifies probabilities, whereas the measurement operators or instrument also specify the backaction.

For [quantum teleportation](../../../../../quantum-teleportation.md), Alice and Bob initially share the [Bell pair](../../../../../bell-pair.md) $|\Phi^+\rangle_{AB}=(|00\rangle+|11\rangle)/\sqrt2$. Alice also holds the input $|\psi\rangle_C=\alpha|0\rangle+\beta|1\rangle$, with $|\alpha|^2+|\beta|^2=1$. The shared entanglement is a resource; the two transmitted [classical bits](../../../../../bit.md) alone could not transfer an arbitrary unknown quantum state.

Alice applies a [controlled-NOT gate](../../../../../controlled-not-gate.md) with $C$ as control and $A$ as target, then a [Hadamard gate](../../../../../hadamard-gate.md) to $C$. Starting from $|\psi\rangle_C|\Phi^+\rangle_{AB}$, direct expansion gives

$$
\frac12\left(
|00\rangle_{CA}|\psi\rangle_B+
|01\rangle_{CA}X|\psi\rangle_B+
|10\rangle_{CA}Z|\psi\rangle_B+
|11\rangle_{CA}XZ|\psi\rangle_B
\right).
$$

For example, the four receiver vectors are $\alpha|0\rangle+\beta|1\rangle$, $\beta|0\rangle+\alpha|1\rangle$, $\alpha|0\rangle-\beta|1\rangle$, and $-\beta|0\rangle+\alpha|1\rangle$. Thus the gate calculation fixes the ordering of the Pauli corrections, including the last branch's sign.

Alice measures $C,A$ in the [computational basis](../../../../../computational-basis.md), obtaining $(a,b)$. The [Born rule](../../../../../born-rule.md) gives each outcome probability $1/4$, independent of the input amplitudes. Bob's normalized conditional state is $X^bZ^a|\psi\rangle$. Alice sends the two outcome bits. Bob applies the inverse, $Z^aX^b$, and hence

$$
\boxed{Z^aX^bX^bZ^a|\psi\rangle=|\psi\rangle.}
$$

The same circuit is a [Bell-basis measurement](../../../../../bell-basis-measurement.md) on Alice's two qubits, expressed using ordinary gates followed by computational-basis measurements. It restores the state without Alice or Bob knowing $\alpha,\beta$.

By [linearity](../../../../../linearity.md), the calculation also holds when the input is entangled with a reference: each outcome has branch map $|\psi\rangle\mapsto X^bZ^a|\psi\rangle/2$, and after correction every branch is one-half of the identity map. Summing the four corrected density operators gives exactly the original input density operator, with all reference correlations preserved. This is [teleportation as an identity channel on a reference](../../../../../teleportation-as-an-identity-channel-on-a-reference.md). Without the two classical bits Bob must average the four uncorrected states, giving $\tfrac14\sum_{a,b}X^bZ^a\rho Z^aX^b=I/2$, so the process cannot signal before the message arrives. The Bell pair is consumed and Alice retains no copy of the unknown state, in accordance with the [no-cloning theorem](../../../../../no-cloning-theorem.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
