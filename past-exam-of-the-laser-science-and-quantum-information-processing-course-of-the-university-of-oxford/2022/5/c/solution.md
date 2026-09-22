<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Read the source network as a [Hadamard test](../../../../hadamard-test.md): a [Hadamard gate](../../../../hadamard-gate.md) on the first [qubit](../../../../qubit.md), a [controlled unitary gate](../../../../controlled-unitary-gate.md) with the first [qubit](../../../../qubit.md) as control, and another [Hadamard gate](../../../../hadamard-gate.md) on that control. Starting from $|0\rangle|\phi\rangle$, the successive [quantum states](../../../../quantum-state.md) are

$$
\begin{aligned}
|\Psi_1\rangle&=\frac{|0\rangle+|1\rangle}{\sqrt2}|\phi\rangle,\\
|\Psi_2\rangle&=\frac{|0\rangle|\phi\rangle+|1\rangle U|\phi\rangle}{\sqrt2},\\
|\Psi_3\rangle&=\frac12\left[|0\rangle(I+U)|\phi\rangle+|1\rangle(I-U)|\phi\rangle\right].
\end{aligned}
$$

Apply [b](../b.md) to the last line. Since $U^\dagger U=I$ by [unitarity](../../../../unitary-operator.md),

$$
\begin{aligned}
P_0&=\tfrac14\langle\phi|(I+U^\dagger)(I+U)|\phi\rangle
=\tfrac12\left[1+\operatorname{Re}\langle\phi|U|\phi\rangle\right],\\
P_1&=\tfrac14\langle\phi|(I-U^\dagger)(I-U)|\phi\rangle
=\tfrac12\left[1-\operatorname{Re}\langle\phi|U|\phi\rangle\right].
\end{aligned}
$$

For the [Pauli Z gate](../../../../pauli-z-gate.md) observable on the first [qubit](../../../../qubit.md), the two [eigenvalues](../../../../eigenvalue.md) are $+1$ and $-1$. Thus

$$
\boxed{\langle Z\rangle=P_0-P_1=\operatorname{Re}\langle\phi|U|\phi\rangle.}
$$

As a check, $U=I$ returns outcome zero certainly, while $U=-I$ returns one certainly. The [controlled unitary gate](../../../../controlled-unitary-gate.md) makes this relative [phase](../../../../phase-waves.md) measurable even though multiplying an isolated system's [quantum state](../../../../quantum-state.md) by $-1$ is only a [global phase](../../../../global-phase.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
