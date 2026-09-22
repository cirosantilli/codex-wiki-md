<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Compute the honest one-qubit [density operators](../../../../../density-matrix.md) in the [computational basis](../../../../../computational-basis.md). Writing $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$ and $|u\rangle=(5|0\rangle+|1\rangle)/\sqrt{26}$, the two [quantum state ensembles](../../../../../quantum-state-ensemble.md) give

$$
\begin{aligned}
\rho_0&=\tfrac12|0\rangle\langle0|+\tfrac14|+\rangle\langle+|+\tfrac14|1\rangle\langle1|=\begin{pmatrix}5/8&1/8\\1/8&3/8\end{pmatrix},\\
\rho_1&=\tfrac{13}{20}|u\rangle\langle u|+\tfrac7{20}|1\rangle\langle1|=\begin{pmatrix}5/8&1/8\\1/8&3/8\end{pmatrix}.
\end{aligned}
$$

The equality includes the off-diagonal coherence; comparing only the basis outcome probabilities would not suffice.

**The protocol is perfectly hiding against Bob when Alice is honest.** Independence of the honest preparations makes his full received [density operator](../../../../../density-matrix.md) $\rho_0^{\otimes N}=\rho_1^{\otimes N}$. For any [POVM](../../../../../positive-operator-valued-measure.md) $\{E_z\}$, including collective measurements and measurements using ancillas, the [Born rule](../../../../../born-rule.md) gives the same outcome probabilities $\operatorname{Tr}(E_z\rho_0^{\otimes N})=\operatorname{Tr}(E_z\rho_1^{\otimes N})$. Thus no measurement supplies information about the committed bit.

**It is not binding against Alice.** Here is an explicit [ensemble-steering attack on quantum bit commitment](../../../../../ensemble-steering-attack-on-quantum-bit-commitment.md). For each position, Alice prepares the normalized two-qubit [pure state](../../../../../pure-state.md)

$$
|\Omega\rangle=\sqrt{\frac{13}{20}}|0\rangle_A|u\rangle_B+\sqrt{\frac7{20}}|1\rangle_A|1\rangle_B,
$$

retains $A$ and sends $B$. Its [partial trace](../../../../../partial-trace.md) on $A$ is the honest common [density operator](../../../../../density-matrix.md). She sends the $B$ halves of $N$ independent copies while retaining all the $A$ halves, and chooses her bit only at unveiling.

To open one, she makes a [projective measurement](../../../../../projective-measurement.md) of each retained [qubit](../../../../../qubit.md) in the [computational basis](../../../../../computational-basis.md). Outcome zero has [probability](../../../../../probability.md) $13/20$ and prepares Bob's state $|u\rangle$; outcome one has [probability](../../../../../probability.md) $7/20$ and prepares $|1\rangle$. She announces that list. It has exactly the honest bit-one distribution, and every declared-state test passes.

To open zero, she instead measures each retained [qubit](../../../../../qubit.md) using a three-outcome [POVM](../../../../../positive-operator-valued-measure.md) with effects $E_j=|v_j\rangle\langle v_j|$, where

$$
|v_0\rangle=\begin{pmatrix}2/\sqrt5\\-2/\sqrt{70}\end{pmatrix},\quad
|v_+\rangle=\begin{pmatrix}1/\sqrt5\\4/\sqrt{70}\end{pmatrix},\quad
|v_1\rangle=\begin{pmatrix}0\\\sqrt{5/7}\end{pmatrix}.
$$

All effects are positive. Their diagonal sums are $4/5+1/5=1$ and $4/70+16/70+5/7=1$, and the off-diagonal sum is zero, so $E_0+E_++E_1=I$. This establishes that the proposed [POVM](../../../../../positive-operator-valued-measure.md) is physically valid.

To verify the conditional states directly, the coefficient [matrix](../../../../../matrix.md) of $|\Omega\rangle$, with Bob's index as the row and Alice's as the column, is

$$
C=\begin{pmatrix}\sqrt{5/8}&0\\\sqrt{1/40}&\sqrt{7/20}\end{pmatrix}.
$$

A real rank-one effect $|v_j\rangle\langle v_j|$ on Alice's half gives the unnormalized Bob state vector $Cv_j$. For the three effects above,

$$
Cv_0=\sqrt{1/2}|0\rangle,\qquad Cv_+=\tfrac12|+\rangle,\qquad Cv_1=\tfrac12|1\rangle.
$$

Their squared norms are therefore $1/2,1/4,1/4$, exactly the honest bit-zero probabilities, and Bob's conditional [pure states](../../../../../pure-state.md) are the corresponding declared states. Independent measurements on the retained halves produce the honest distribution of the entire list, so even checks on the declared frequencies do not defeat the attack. Every declared-state projector test again succeeds.

Alice can consequently unveil either bit with acceptance [probability](../../../../../probability.md) one, without having chosen it when sending the [qubits](../../../../../qubit.md). This is the [Hughston–Jozsa–Wootters theorem](../../../../../hughston-jozsa-wootters-theorem.md) mechanism implemented by an explicit measurement, rather than merely an appeal to the general impossibility of perfectly hiding and binding quantum [bit commitment](../../../../../bit-commitment.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
