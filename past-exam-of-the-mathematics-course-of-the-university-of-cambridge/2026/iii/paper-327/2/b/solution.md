<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each one-dimensional factor $P_j(D_j)$, choose its [retarded fundamental solution](../../../../../../retarded-fundamental-solution.md) $E_j=H(x_j)g_j(x_j)$. Partial-fraction decomposition of the reciprocal polynomial gives

$$
g_j(x_j)=\sum_{r=1}^{N_j}\alpha_{rj}(x_j)e^{\beta_{rj}x_j},
$$

where each $\alpha_{rj}$ is a polynomial whose degree is one less than the multiplicity of the associated root. Constants, including powers of $i$ from $D=-i\partial$, can be absorbed into the polynomials and exponents.

Take the tensor product

$$
E(x_1,\ldots,x_n)=\prod_{j=1}^nE_j(x_j).
$$

It vanishes unless every $x_j>0$, has the required polynomial-exponential form there, and satisfies

$$
\boxed{P(D)E=\prod_{j=1}^nP_j(D_j)E_j=\delta_0(x_1)\otimes\cdots\otimes\delta_0(x_n)=\delta_0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
