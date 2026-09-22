<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The required identity is [CNOT control reversal in the Hadamard basis](../../../../cnot-control-reversal-in-the-hadamard-basis.md). To derive it using standard [quantum circuit](../../../../quantum-circuit-split.md) identities, let $\mathrm{CZ}$ be the [Controlled-Z gate](../../../../controlled-z-gate.md), which multiplies $|11\rangle$ by $-1$ and fixes the other [computational-basis states](../../../../computational-basis-state.md). Since $HXH=Z$,

$$
C_{1\to2}=(I\otimes H)\,\mathrm{CZ}\,(I\otimes H).
$$

The [Controlled-Z gate](../../../../controlled-z-gate.md) is symmetric in its two wires. Combining this symmetry with $H^2=I$ gives

$$
\begin{aligned}
(H\otimes H)C_{1\to2}(H\otimes H)
&=(H\otimes I)\,\mathrm{CZ}\,(H\otimes I)\\
&=\boxed{C_{2\to1}}.
\end{aligned}
$$

This is an **exact operator identity**, including its [global phase](../../../../global-phase.md), and applies to arbitrary inputs. One can also check it directly from the [orthogonal projectors](../../../../orthogonal-projection.md) $P_b=|b\rangle\langle b|$: conjugating $C_{1\to2}=P_0\otimes I+P_1\otimes X$ by $H\otimes H$ gives

$$
\frac{I+X}{2}\otimes I+\frac{I-X}{2}\otimes Z
=I\otimes P_0+X\otimes P_1=C_{2\to1}.
$$

For the three-wire [quantum circuit](../../../../quantum-circuit-split.md), put $W=H^{\otimes3}$. Conjugation distributes over products because $W^2=I$: $WABW=(WAW)(WBW)$. Each [CNOT gate](../../../../controlled-not-gate.md) in $U_a$ therefore reverses direction, while the [Hadamard gates](../../../../hadamard-gate.md) on untouched wires cancel. The [Hadamard-conjugated linear oracle](../../../../hadamard-conjugated-linear-oracle.md) is

$$
\boxed{WU_aW=C_{y\to2}^{\,a_2}C_{y\to1}^{\,a_1}.}
$$

These are the simplified [quantum circuits](../../../../quantum-circuit-split.md) in the figure: for $a=00$ there are no gates; for $a=01$ there is $C_{y\to2}$; for $a=10$ there is $C_{y\to1}$; and for $a=11$ there are both. The [ancilla qubit](../../../../ancilla-qubit.md) becomes their common control. On every [computational-basis state](../../../../computational-basis-state.md), the entire simplified circuit acts as

$$
|x_1x_2\rangle|b\rangle
\longmapsto
|x_1\oplus ba_1,\ x_2\oplus ba_2\rangle|b\rangle.
$$

Starting the data [qubits](../../../../qubit.md) at $|00\rangle$, the prescribed [computational basis](../../../../computational-basis.md) preparation of the [ancilla qubit](../../../../ancilla-qubit.md) must therefore be **$|1\rangle$**: it activates the required flips and gives $|a\rangle|1\rangle$. Starting it at $|0\rangle$ instead gives $|00\rangle|0\rangle$ for every $a$, so no information is obtained.

More generally, an initial [ancilla qubit](../../../../ancilla-qubit.md) state $\alpha|0\rangle+\beta|1\rangle$ in this same fixed [quantum circuit](../../../../quantum-circuit-split.md) gives

$$
\alpha|00\rangle|0\rangle+\beta|a\rangle|1\rangle.
$$

For nonzero $a$, the desired data output has [probability](../../../../probability.md) $|\beta|^2$, and exact identification for every $a$ requires $\alpha=0$. This condition refers to the displayed [ancilla preparation for the Bernstein-Vazirani algorithm](../../../../ancilla-preparation-for-the-bernstein-vazirani-algorithm.md): the state entering the [function oracle](../../../../function-oracle.md) must be $|-\rangle$, up to [global phase](../../../../global-phase.md). Other [quantum state preparation](../../../../quantum-state-preparation.md) procedures that deliver this same state are equivalent; $|1\rangle$ is the prescribed input before the first [Hadamard gate](../../../../hadamard-gate.md).

For arbitrary $n$, [linearity](../../../../linearity.md) of the [linear Boolean function](../../../../linear-boolean-function.md) supplies

$$
U_a=\prod_{j=1}^{n}C_{j\to y}^{\,a_j},
\qquad
H^{\otimes(n+1)}U_aH^{\otimes(n+1)}
=\prod_{j=1}^{n}C_{y\to j}^{\,a_j}.
$$

This decomposition is for analysis: the [Bernstein-Vazirani algorithm](../../../../bernstein-vazirani-algorithm.md) calls the unknown [function oracle](../../../../function-oracle.md) as one supplied operation. The common control starts at $1$, so the simplified [quantum circuit](../../../../quantum-circuit-split.md) takes $|0\rangle^{\otimes n}|1\rangle$ to $|a\rangle|1\rangle$. Equivalently, [phase kickback](../../../../phase-kickback.md) gives a product state

$$
\frac1{\sqrt{2^n}}\sum_{x\in\{0,1\}^n}(-1)^{a\cdot x}|x\rangle
=\bigotimes_{j=1}^{n}\frac{|0\rangle+(-1)^{a_j}|1\rangle}{\sqrt2},
$$

which the final [Hadamard transform](../../../../hadamard-transform.md) decodes to $|a\rangle$. Thus **one quantum oracle call suffices for every $n\ge1$**, compared with $n$ classical calls. This counts [function oracle](../../../../function-oracle.md) uses; the surrounding [Hadamard gates](../../../../hadamard-gate.md) and final [computational-basis measurement](../../../../quantum-measurement-in-the-computational-basis.md) still act on $n+1$ and $n$ [qubits](../../../../qubit.md), respectively.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [6](../../6-split.md)
3. [2010](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
