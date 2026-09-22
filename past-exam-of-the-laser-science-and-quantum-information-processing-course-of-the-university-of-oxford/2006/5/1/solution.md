<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For one input [bit](../../../../bit.md), a [Boolean function](../../../../boolean-function.md) is specified by the pair $(f(0),f(1))$, and $k=f(0)+f(1)$ counts its [satisfying assignments](../../../../satisfying-assignment.md). In the ordered [computational basis](../../../../computational-basis.md) $(|0\rangle,|1\rangle)$, the supplied [phase oracle](../../../../phase-oracle.md) convention gives

$$
U_f|x\rangle=(-1)^{f(x)\oplus1}|x\rangle,\qquad
U_f=\operatorname{diag}\bigl(2f(0)-1,2f(1)-1\bigr).
$$

Here $\oplus$ is [exclusive or](../../../../exclusive-or.md): **the oracle changes the sign of the inputs with $f(x)=0$**. With $I$ the [identity matrix](../../../../identity-matrix.md) and $Z$ the [Pauli Z gate](../../../../pauli-z-gate.md), all four cases are

$$
\begin{array}{c|c|c|c}
f(x)&(f(0),f(1))&k&U_f\\\hline
0&(0,0)&0&\begin{pmatrix}-1&0\\0&-1\end{pmatrix}=-I\\[3pt]
x&(0,1)&1&\begin{pmatrix}-1&0\\0&1\end{pmatrix}=-Z\\[3pt]
1-x&(1,0)&1&\begin{pmatrix}1&0\\0&-1\end{pmatrix}=Z\\[3pt]
1&(1,1)&2&\begin{pmatrix}1&0\\0&1\end{pmatrix}=I
\end{array}
$$

The two middle cases are [balanced Boolean functions](../../../../balanced-boolean-function.md); the others are [constant functions](../../../../constant-function.md). The specified zero-state sign change and the [Hadamard gate](../../../../hadamard-gate.md) are

$$
\boxed{U_0=\begin{pmatrix}-1&0\\0&1\end{pmatrix}=-Z,\qquad
H=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix}.}
$$

Use the top [qubit](../../../../qubit.md) as the first [tensor product](../../../../tensor-product.md) factor. Write the [controlled unitary gate](../../../../controlled-unitary-gate.md) as $C(V)=|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes V$. Reading the bracketed [quantum circuit](../../../../quantum-circuit-split.md) from left to right, its four operations are $C(U_f)$, $C(H)$, $C(U_0)$, $C(H)$. Thus the target operation in its control-one branch is

$$
G=H U_0 H U_f,
\qquad C(G)=C(H)C(U_0)C(H)C(U_f),
$$

where the rightmost [matrix](../../../../matrix.md) acts first. The control-zero branch is the [identity operator](../../../../identity-operator.md). The [Hadamard conjugation of a controlled gate](../../../../hadamard-conjugation-of-a-controlled-gate.md) identity gives

$$
\boxed{C(H)C(U_0)C(H)=(I\otimes H)C(U_0)(I\otimes H).}
$$

Indeed, on control zero the replacement applies $H I H=I$ to the target, while on control one both sides apply $H U_0 H$. By [linearity](../../../../linearity.md), the identity holds on every [quantum superposition](../../../../quantum-superposition.md) and therefore in every repetition of the bracket. This replaces the two internal controlled [Hadamard gates](../../../../hadamard-gate.md) as a pair.

The [global phase of a controlled quantum gate](../../../../global-phase-of-a-controlled-quantum-gate.md) must be preserved: $C(-I)=Z\otimes I$, whereas $C(I)=I\otimes I$. Consequently the minus signs in $U_0=-Z$ and the special [phase oracles](../../../../phase-oracle.md) $U_f=-I,-Z$ cannot be discarded as an unobservable [global phase](../../../../global-phase.md) of the complete [quantum circuit](../../../../quantum-circuit-split.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [5](../../5-split.md)
3. [2006](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
