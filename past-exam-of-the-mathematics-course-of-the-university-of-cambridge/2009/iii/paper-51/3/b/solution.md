<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the normalized input [quantum state](../../../../../../quantum-state.md) as $|\psi\rangle=a|0\rangle+b|1\rangle$. The fresh [quantum ancilla](../../../../../../quantum-ancilla.md) is $|+\rangle$, so the [Controlled-Z gate](../../../../../../controlled-z-gate.md) creates

$$
a|0\rangle|+\rangle+b|1\rangle|-\rangle.
$$

Applying the measurement bra $\langle v_k(\theta)|$ to the first [qubit](../../../../../../qubit.md) leaves the unnormalized second-[qubit](../../../../../../qubit.md) vector

$$
|\widetilde\psi_k\rangle=\frac1{\sqrt2}\left(a|+\rangle+(-1)^k e^{-i\theta}b|-\rangle\right).
$$

Since $|+\rangle,|-\rangle$ form an [orthonormal basis](../../../../../../orthonormal-basis.md),

$$
\Pr(k)=\langle\widetilde\psi_k|\widetilde\psi_k\rangle
=\frac{|a|^2+|b|^2}{2}=\frac12.
$$

Also $U(\theta)|\psi\rangle=a|+\rangle+e^{-i\theta}b|-\rangle$, while the [Pauli X gate](../../../../../../pauli-x-gate.md) fixes $|+\rangle$ and changes the sign of $|-\rangle$. Dividing by the branch norm therefore gives

$$
\boxed{|\psi'_k\rangle=X^kU(\theta)|\psi\rangle,\qquad\Pr(k=0)=\Pr(k=1)=\frac12.}
$$

This is [one-bit teleportation](../../../../../../one-bit-teleportation.md) with the present positive-exponent measurement vectors; the transferred logical gate is $U(\theta)=J(-\theta)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
