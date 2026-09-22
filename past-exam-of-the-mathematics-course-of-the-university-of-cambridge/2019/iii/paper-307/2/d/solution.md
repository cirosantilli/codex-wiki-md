<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Diagonalize $T$ with eigenvalues $\lambda_a$ and use the periodic [Fourier series](../../../../../../fourier-series-split.md)

$$
\eta^a(t)=\sum_{k\in\mathbb Z}\eta_k^ae^{2\pi ikt},
\qquad
\bar\eta^a(t)=\sum_{k\in\mathbb Z}\bar\eta_k^ae^{-2\pi ikt}.
$$

Each [Berezin integral](../../../../../../berezin-integral.md) contributes its quadratic coefficient, so

$$
Z=\prod_{a=1}^n\prod_{k\in\mathbb Z}(2\pi ik+\lambda_a).
$$

Pairing $k$ with $-k$ and using the infinite product for the hyperbolic sine gives, up to the local regularization factor,

$$
\prod_{k\in\mathbb Z}(2\pi ik+\lambda)
=2\sinh\frac\lambda2
=e^{\lambda/2}(1-e^{-\lambda}).
$$

The product of the prefactors is $e^{\operatorname{tr}T/2}=1$ because $T$ is traceless. Thus

$$
\boxed{Z=\prod_a(1-e^{-\lambda_a})=\det(1-e^{-T})}.
$$

This agrees with the direct identity that the [supertrace](../../../../../../supertrace.md) of an induced linear map on an exterior algebra is its characteristic determinant.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 307](../../../paper-307-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
