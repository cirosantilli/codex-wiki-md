<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Kernel principal component analysis](../../../../../../../kernel-principal-component-analysis.md) diagonalizes the centered $n$ by $n$ [kernel matrix](../../../../../../../kernel-matrix.md) instead of an explicit covariance operator in a possibly infinite-dimensional feature space. A new point has coordinate

$$
\langle\widehat u_j,\phi(x)\rangle_{\mathcal H}
=\sum_i\widehat\alpha_{ji}k(X_i,x),
$$

so the leading coordinates require only evaluations of the [positive-semidefinite kernel](../../../../../../../positive-semidefinite-kernel.md).

Running the [K-nearest neighbors algorithm](../../../../../../../k-nearest-neighbors-algorithm.md) in a truncated collection of these coordinates can remove low-variance noise, reduce effective dimension, and allow a nonlinear boundary in the original covariates. This is the [kernel trick](../../../../../../../kernel-trick.md): every feature-space inner product needed for fitting and projection is replaced by $k(x,z)=\langle\phi(x),\phi(z)\rangle_{\mathcal H}$ without constructing $\phi(x)$ explicitly.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 218](../../../../paper-218-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
