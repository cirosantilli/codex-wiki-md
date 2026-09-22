<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $P_n:\ell^2(\mathbb N)\to\mathbb C^n$ be coordinate projection and set

$$
T_n=P_nAP_n^*.
$$

This finite matrix is computable from the matrix entries of $A$. Compute its [singular value decomposition](../../../../../../singular-value-decomposition.md)

$$
T_n=V_n\Sigma_nW_n^*
$$

and define the [unitary polar factor of a finite compression](../../../../../../unitary-polar-factor-of-a-finite-compression.md)

$$
\boxed{A_n=V_nW_n^*.}
$$

This is a unitary operator on $\mathbb C^n$, including when $T_n$ is singular.

Put $Q_n=P_n^*P_n$. Since $Q_n\to I$ strongly and $A$ is unitary,

$$
P_n^*T_n^*T_nP_nv
=Q_nA^*Q_nAQ_nv\longrightarrow v.
$$

The continuous functional calculus for positive matrices therefore gives

$$
P_n^*|T_n|P_nv\longrightarrow v.
$$

The polar identity $T_n=A_n|T_n|$ now yields

$$
\|P_n^*(A_n-T_n)P_nv\|
=\|(I-|T_n|)P_nv\|\longrightarrow0.
$$

Also $P_n^*T_nP_n=Q_nAQ_n\to A$ strongly, and hence

$$
\boxed{P_n^*A_nP_n\longrightarrow A\quad\text{strongly}.}
$$

In particular the weak convergence required in part (c) holds. The construction uses only a finite block of the given matrix and a finite [singular value decomposition](../../../../../../singular-value-decomposition.md), so it is an algorithm realizing all the assumptions of part (c).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
