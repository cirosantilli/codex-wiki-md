<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Define the [Hadamard basis](../../../../hadamard-basis.md) states $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. The initial two [Hadamard gates](../../../../hadamard-gate.md) prepare $|+\rangle|+\rangle$. For one bracket, the two control branches give

$$
|+\rangle|+\rangle\ \longmapsto
\frac{|0\rangle|+\rangle+|1\rangle G|+\rangle}{\sqrt2}.
$$

Using the [Pauli X gate](../../../../pauli-x-gate.md) $X=\begin{pmatrix}0&1\\1&0\end{pmatrix}$, [unitary conjugation](../../../../unitary-conjugation.md) by the [Hadamard gate](../../../../hadamard-gate.md) gives $H U_0 H=-X$, so $G=-XU_f$. Keeping every sign, the target states along the control-one branch, in the exact gate order, are

$$
\begin{array}{c|c|c|c|c|c}
f&U_f|+\rangle&H U_f|+\rangle&U_0 H U_f|+\rangle&G|+\rangle&H G|+\rangle\\\hline
0&-|+\rangle&-|0\rangle&|0\rangle&|+\rangle&|0\rangle\\
x&-| -\rangle&-|1\rangle&-|1\rangle&-| -\rangle&-|1\rangle\\
1-x&| -\rangle&|1\rangle&|1\rangle&| -\rangle&|1\rangle\\
1&|+\rangle&|0\rangle&-|0\rangle&-|+\rangle&-|0\rangle
\end{array}
$$

The last column also includes the final target [Hadamard gate](../../../../hadamard-gate.md), which lies outside the bracket. Writing $|\chi_f\rangle=HG|+\rangle$, applying the final top [Hadamard gate](../../../../hadamard-gate.md) gives the exact normalized two-[qubit](../../../../qubit.md) [quantum state](../../../../quantum-state.md)

$$
|\Psi_f\rangle=\frac12\left[|0\rangle\bigl(|0\rangle+|\chi_f\rangle\bigr)+|1\rangle\bigl(|0\rangle-|\chi_f\rangle\bigr)\right].
$$

Thus the complete outputs, in top-then-bottom [computational basis](../../../../computational-basis.md) order, are

$$
\boxed{\begin{array}{c|c|c}
f&|\Psi_f\rangle&\langle Z\otimes I\rangle\\\hline
0&|00\rangle&+1\\[2pt]
x&\tfrac12\bigl(|00\rangle-|01\rangle+|10\rangle+|11\rangle\bigr)&0\\[2pt]
1-x&\tfrac12\bigl(|00\rangle+|01\rangle+|10\rangle-|11\rangle\bigr)&0\\[2pt]
1&|10\rangle&-1
\end{array}}
$$

For the first [qubit](../../../../qubit.md), the [Pauli matrix](../../../../pauli-matrices.md) $\sigma_z=Z$ has [expectation value](../../../../expectation-value.md) $P(0)-P(1)$ by the [Born rule](../../../../born-rule.md). The two $k=1$ cases each have $P(0)=P(1)=1/2$, while the $k=0$ and $k=2$ cases are deterministic. Equivalently, this [Hadamard test](../../../../hadamard-test.md) measures

$$
\langle Z\otimes I\rangle=\operatorname{Re}\langle+|G|+\rangle=1-k
\qquad(r=1,\ n=1).
$$

This explains the [approximate quantum counting](../../../../approximate-quantum-counting.md) interpretation: repeated preparations estimate the [expectation value](../../../../expectation-value.md), and hence $k$. A single top-[qubit](../../../../qubit.md) [computational-basis measurement](../../../../quantum-measurement-in-the-computational-basis.md) need not identify $k$.

## ↑ Ancestors (12)

1. [2](../2.md)
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
