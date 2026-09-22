<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Split $X^\mu=x_0^\mu+X'^\mu$. Integrating the constant mode gives [momentum conservation](../../../../../../momentum-conservation.md),

$$
\int d^{26}x_0\,e^{ix_0\cdot\sum_i p_i}
\propto\delta^{26}\!\left(\sum_i p_i\right).
$$

For the nonzero modes, [Wick theorem](../../../../../../wick-s-theorem.md) and the propagator give

$$
\left\langle\prod_{i=1}^4{}:e^{ip_i\cdot X(z_i)}:\right\rangle
=\exp\!\left[-\sum_{j<k}p_j\cdot p_k
\left\langle X(z_j)X(z_k)\right\rangle\right]
=\prod_{j<k}|z_j-z_k|^{\alpha'p_j\cdot p_k}.
$$

Thus, up to source-independent numerical normalization, the four-point amplitude is

$$
\boxed{
\mathcal A^{(4)}\sim
\frac{g_s^2\delta^{26}(\sum_i p_i)}{\operatorname{Vol}(SL(2,\mathbb C))}
\int\prod_{i=1}^4d^2z_i
\prod_{j<k}|z_j-z_k|^{\alpha'p_j\cdot p_k}}.
$$

The product is the [Koba-Nielsen factor](../../../../../../koba-nielsen-factor.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
