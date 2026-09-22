<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Pauli Z gate](../../../../../../pauli-z-gate.md) exchanges the two [Hadamard basis](../../../../../../hadamard-basis.md) states: $Z|+\rangle=|-\rangle$ and $Z|-\rangle=|+\rangle$. Multiplying the displayed gate by the [Pauli X gate](../../../../../../pauli-x-gate.md) gives

$$
U(\theta)X=|+\rangle\langle1|+e^{-i\theta}|-\rangle\langle0|.
$$

On the other hand,

$$
e^{-i\theta}ZU(-\theta)
=e^{-i\theta}Z\left(|+\rangle\langle0|+e^{i\theta}|-\rangle\langle1|\right)
=e^{-i\theta}|-\rangle\langle0|+|+\rangle\langle1|.
$$

The two operators agree, proving

$$
\boxed{U(\theta)X=e^{-i\theta}ZU(-\theta).}
$$

Also $U(\theta)=H\operatorname{diag}(1,e^{-i\theta})=J(-\theta)$ in the [J gate](../../../../../../j-gate-in-measurement-based-quantum-computation.md) convention. Keeping this angle sign explicit avoids confusing the two conventions for [equatorial qubit measurements](../../../../../../equatorial-qubit-measurement.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
