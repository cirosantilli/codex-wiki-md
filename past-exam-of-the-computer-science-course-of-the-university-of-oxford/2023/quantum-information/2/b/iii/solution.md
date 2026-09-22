<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Initialize two [qubits](../../../../../../qubit.md) in $|00\rangle$. A [Hadamard gate](../../../../../../hadamard-gate.md) on the first followed by a [controlled-NOT gate](../../../../../../controlled-not-gate.md) $1\to2$ prepares the [Bell state](../../../../../../bell-state-split.md) $|\phi_+\rangle$. The permitted [T gates](../../../../../../t-gate.md) and [Hadamard gates](../../../../../../hadamard-gate.md) implement the needed [Pauli gates](../../../../../../pauli-gate.md) exactly:

$$
Z=T^4,\qquad X=HT^4H.
$$

Apply $T_1^4$, followed by $H_2,T_2,T_2,T_2,T_2,H_2$. These are a [Pauli Z gate](../../../../../../pauli-z-gate.md) on the first [qubit](../../../../../../qubit.md) and a [Pauli X gate](../../../../../../pauli-x-gate.md) on the second, giving

$$
\frac{|00\rangle+|11\rangle}{\sqrt2}
\xrightarrow{Z_1}\frac{|00\rangle-|11\rangle}{\sqrt2}
\xrightarrow{X_2}\boxed{\frac{|01\rangle-|10\rangle}{\sqrt2}.}
$$

Every operation is in the allowed gate set; no [quantum measurement](../../../../../../quantum-measurement-split.md) or probabilistic branch is needed.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
