<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The claimed universality is false for the particular gate specified in part (d). Every allowed single-[qubit](../../../../../../qubit.md) gate is local, and $C_{\mathrm{phase}}=-Z\otimes Z$ is local too. Products of these gates remain of the form $e^{i\chi}A\otimes B$. They preserve all [product states](../../../../../../product-state.md) and cannot, for example, implement the [CNOT gate](../../../../../../controlled-not-gate.md) that sends $|+\rangle\otimes|0\rangle$ to $(|00\rangle+|11\rangle)/\sqrt2$. Equivalently, its [diagonal two-qubit phase entanglement criterion](../../../../../../diagonal-two-qubit-phase-entanglement-criterion.md) gives the alternating phase $\pi-0-0+\pi=0$ modulo $2\pi$. **No construction with only the printed phase gate and local rotations implements arbitrary two-qubit gates**.

The intended universality argument works after replacing that local gate by an entangling controlled phase. The same tunable [Ising coupling](../../../../../../ising-coupling-of-two-qubits.md) supplies

$$
V=e^{-i\pi Z\otimes Z/4},\qquad
\mathrm{CZ}=e^{-i\pi/4}\{R_z(-\pi/2)\otimes R_z(-\pi/2)\}V=\operatorname{diag}(1,1,1,-1).
$$

Thus this quarter-area Ising pulse, with local corrections, realizes the [Controlled-Z gate](../../../../../../controlled-z-gate.md). Conjugating it by the [Hadamard gate](../../../../../../hadamard-gate.md) on the second qubit gives $\mathrm{CNOT}=(I\otimes H)\mathrm{CZ}(I\otimes H)$, with harmless scalar phases if the Hadamards are implemented using traceless control Hamiltonians.

The [Cartan decomposition of a two-qubit gate](../../../../../../cartan-decomposition-of-a-two-qubit-gate.md) writes a target as

$$
U=e^{i\chi}(A_1\otimes A_2)e^{-i(c_xX\otimes X+c_yY\otimes Y+c_zZ\otimes Z)}(B_1\otimes B_2),
$$

with local $SU(2)$ factors. The three central Pauli-product operators commute, so their exponential is a product of three variable interaction gates. From two fixed [CNOT gates](../../../../../../controlled-not-gate.md) and a variable local [rotation about the z-axis](../../../../../../rotation-about-the-z-axis.md),

$$
\mathrm{CNOT}\{I\otimes R_z(2c)\}\mathrm{CNOT}=e^{-icZ\otimes Z},
$$

because $\mathrm{CNOT}(I\otimes Z)\mathrm{CNOT}=Z\otimes Z$. Conjugating this interaction by $R_y(\pi/2)$ on both qubits yields $e^{-icX\otimes X}$; conjugating by $R_x(-\pi/2)$ on both yields $e^{-icY\otimes Y}$. Part (c) implements all outer local factors. This gives the full requested Cartan construction with an entangling phase gate, and pinpoints the defect in the printed version. Exact arbitrary scalar phase requires an identity Hamiltonian term; the physical gate construction is up to [global phase](../../../../../../global-phase.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
