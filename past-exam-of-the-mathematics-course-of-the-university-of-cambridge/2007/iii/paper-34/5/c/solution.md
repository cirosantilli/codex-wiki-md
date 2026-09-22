<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [orthogonal projection](../../../../../../orthogonal-projection.md) onto the $+1$ eigenspace of the [Pauli matrix](../../../../../../pauli-matrices.md) $\sigma_z$ is $P_+=(I+\sigma_z)/2$. By the [Born rule](../../../../../../born-rule.md) and the [Bloch vector](../../../../../../bloch-vector.md) representation,

$$
\mathbb P(+1)=\operatorname{Tr}(\rho P_+)=\frac12\left(1+\operatorname{Tr}(\rho\sigma_z)\right)=\frac{1+s_z}{2}.
$$

Since $s_z=1/5$,

$$
\boxed{\mathbb P(+1)=\frac35.}
$$

The given vector has length $19/30<1$, so it lies inside the [Bloch ball](../../../../../../bloch-ball.md) and indeed defines a valid mixed qubit state. For the physical spin operator $S_z=(\hbar/2)\sigma_z$, the corresponding outcome is $+\hbar/2$ with the same probability.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
