<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using the printed measurement-vector convention, the [unitary operator](../../../../../../unitary-operator.md) is

$$
U(\theta)=\frac1{\sqrt2}\begin{pmatrix}1&e^{-i\theta}\\1&-e^{-i\theta}\end{pmatrix}
=H\operatorname{diag}(1,e^{-i\theta})=J(-\theta).
$$

Thus it is a [phase gate](../../../../../../phase-gate.md) followed by a [Hadamard gate](../../../../../../hadamard-gate.md), with angle sign opposite to the parameter in the catalogued [J gate](../../../../../../j-gate-in-measurement-based-quantum-computation.md). Its rows are the conjugate transposes of the orthonormal measurement vectors, so it is unitary. Right multiplication by the [Pauli Z gate](../../../../../../pauli-z-gate.md) changes the sign of the second column, which is exactly the effect of left multiplication by the [Pauli X gate](../../../../../../pauli-x-gate.md), exchanging the two rows. Explicitly,

$$
U(\theta)Z=\frac1{\sqrt2}\begin{pmatrix}1&-e^{-i\theta}\\1&e^{-i\theta}\end{pmatrix}=XU(\theta).
$$

Similarly, right multiplication by the [Pauli X gate](../../../../../../pauli-x-gate.md) exchanges columns, giving

$$
U(\theta)X=\frac1{\sqrt2}\begin{pmatrix}e^{-i\theta}&1\\-e^{-i\theta}&1\end{pmatrix}
=e^{-i\theta}Z\frac1{\sqrt2}\begin{pmatrix}1&e^{i\theta}\\1&-e^{i\theta}\end{pmatrix}.
$$

Therefore the exact identities, retaining the [global phase](../../../../../../global-phase.md) in the second one, are

$$
\boxed{U(\theta)Z=XU(\theta),\qquad U(\theta)X=e^{-i\theta}ZU(-\theta).}
$$

These supply [Pauli-frame propagation along a measurement wire](../../../../../../pauli-frame-propagation-along-a-measurement-wire.md).

## ↑ Ancestors (11)

1. [A](../a.md)
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
