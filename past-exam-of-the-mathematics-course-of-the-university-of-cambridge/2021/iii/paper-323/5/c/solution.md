<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Discarding the outcome of the complete projective measurement gives

$$
\boxed{\sigma=\sum_iP_i\rho P_i}.
$$

For $m$ projectors, let $\omega=e^{2\pi i/m}$ and $U=\sum_j\omega^jP_j$. Then the pinching identity is

$$
\sigma=\frac1m\sum_{k=0}^{m-1}U^k\rho U^{-k}.
$$

The [Concavity of Von Neumann entropy](../../../../../../concavity-of-von-neumann-entropy.md) and its invariance under [unitary operators](../../../../../../unitary-operator.md) imply

$$
\boxed{S(\sigma)\geq\frac1m\sum_kS(U^k\rho U^{-k})
=S(\rho)}.
$$

Equality holds exactly when every conjugate in the average is the same, equivalently

$$
\boxed{[\rho,P_i]=0\quad\hbox{for every }i}.
$$

**Thus equality holds when the input already has no coherence between distinct measurement subspaces.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
