<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The periodic centered-difference kinetic matrix $T_h$ is real symmetric, and the sampled real potential $V_h$ is a real diagonal matrix. Therefore $-iT_h$ and $-iV_h$ are skew-Hermitian, so each matrix exponential in the [Strang splitting](../../../../../../strang-splitting.md) is a [unitary matrix](../../../../../../unitary-matrix.md). Their product is unitary as well. Hence

$$
\boxed{\lVert u^{n+1}\rVert_2^2
=\lVert u^n\rVert_2^2,
\qquad
\sum_m|u_m^n|^2=\text{constant}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
