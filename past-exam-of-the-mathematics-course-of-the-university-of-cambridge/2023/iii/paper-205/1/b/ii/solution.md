<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $V_1,\ldots,V_d$ be independent standard [Cauchy random variables](../../../../../../../cauchy-random-variable.md). Their [characteristic functions](../../../../../../../characteristic-function.md) and independence give

$$
\mathbb E e^{i\lambda V^T(x-y)}
=\prod_{j=1}^d e^{-\lambda|x_j-y_j|}
=e^{-\lambda\|x-y\|_1}.
$$

Taking real parts yields

$$
e^{-\lambda\|x-y\|_1}
=\mathbb E\!\left[
\cos(\lambda V^Tx)\cos(\lambda V^Ty)
+\sin(\lambda V^Tx)\sin(\lambda V^Ty)
\right].
$$

For each realization of $V$, both products are rank-one [positive-semidefinite kernels](../../../../../../../positive-semidefinite-kernel.md). Their sum and then their expectation remain positive semidefinite by the [closure property of positive-semidefinite kernels](../../../../../../../closure-property-of-positive-semidefinite-kernels.md). This is a [Random Fourier feature](../../../../../../../random-fourier-features.md) representation of the [Laplace kernel](../../../../../../../laplace-kernel.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 205](../../../../paper-205-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
