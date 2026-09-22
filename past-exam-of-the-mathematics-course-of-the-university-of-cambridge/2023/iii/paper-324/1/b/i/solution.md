<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $P_1=\sigma_1\otimes\sigma_2$ and $|\psi\rangle=|A\rangle^{\otimes2}$. After the first [Hadamard gate](../../../../../../../hadamard-gate.md) and the two controlled Pauli gates, the joint state is

$$
\frac{|0\rangle|\psi\rangle+|1\rangle P_1|\psi\rangle}{\sqrt2}.
$$

The final Hadamard gate changes this to

$$
\frac12\left[
|0\rangle(I+P_1)|\psi\rangle
+|1\rangle(I-P_1)|\psi\rangle
\right].
$$

Conditioned on ancilla outcome $s\in\{0,1\}$, the normalized data state is therefore

$$
\boxed{
|\Psi_a\rangle=
\frac{[I+(-1)^sP_1]|A\rangle^{\otimes2}}
{\sqrt{2[1+(-1)^s\langle A|^{\otimes2}P_1|A\rangle^{\otimes2}]}}}.
$$

Write the input in the two [eigenspaces](../../../../../../../eigenspace.md) of $P_1$ as

$$
|A\rangle^{\otimes2}=\alpha|p_+\rangle+\beta|p_-\rangle,
\qquad
P_1|p_\pm\rangle=\pm|p_\pm\rangle,
$$

where the displayed eigenstates are normalized. A direct PBC measurement gives

$$
|\Psi_b\rangle=
\begin{cases}
|p_+\rangle,&\text{outcome }+1,\\
|p_-\rangle,&\text{outcome }-1,
\end{cases}
$$

with probabilities $|\alpha|^2$ and $|\beta|^2$. Hence the ancilla circuit and the [Pauli measurement](../../../../../../../measurement-of-a-pauli-observable.md) have identical outcome distributions and conditional data states after identifying the Pauli outcome with $(-1)^s$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
