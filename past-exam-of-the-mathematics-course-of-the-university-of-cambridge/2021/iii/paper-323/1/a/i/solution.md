<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Schmidt decomposition](../../../../../../../schmidt-decomposition.md) states that every finite-dimensional bipartite pure state has

$$
\boxed{|\phi\rangle_{AB}
=\sum_{j=1}^r s_j|a_j\rangle_A|b_j\rangle_B},
$$

where $s_j>0$, $\sum_js_j^2=1$, and the two displayed families are orthonormal. The integer $r$ is the [Schmidt rank](../../../../../../../schmidt-rank.md).

To prove it, choose product bases and write

$$
|\phi\rangle=\sum_{m,n}C_{mn}|m\rangle_A|n\rangle_B.
$$

Apply the [singular value decomposition](../../../../../../../singular-value-decomposition.md) $C=USV^\dagger$. Absorbing the columns of $U$ and the complex conjugates of the columns of $V$ into new orthonormal bases gives the stated sum, with the nonzero singular values as the [Schmidt coefficients](../../../../../../../schmidt-coefficient.md). Equivalently, $s_j^2$ are the common nonzero eigenvalues of the two [reduced density matrices](../../../../../../../reduced-density-matrix.md), so $r=\operatorname{rank}\rho_A=\operatorname{rank}\rho_B$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
