# Computational tradeoffs of the kernel trick

↑ **Parent:** [Kernel trick](kernel-trick.md)

For $d$ input coordinates, the homogeneous quadratic [polynomial kernel](polynomial-kernel.md) has a weighted [quadratic feature map](quadratic-feature-map.md) with $D=d(d+1)/2$ distinct [monomials](monomial.md). Computing an [inner product](inner-product-split.md) of already stored mapped [vectors](vector.md) costs $O(D)$ arithmetic operations, whereas $(x^Tz)^2$ costs $O(d)$ using the input [vectors](vector.md). Here $O$ denotes [big O notation](big-o-notation.md). Higher fixed degrees can make the dimension gap much larger.

Sample count still matters. With $n$ training examples, materializing a dense [kernel matrix](kernel-matrix.md) stores $n^2$ numbers and requires $n(n+1)/2$ distinct evaluations using symmetry. A dense direct solve for [kernel ridge regression](kernel-ridge-regression.md) typically takes $O(n^3)$ operations after constructing the [kernel matrix](kernel-matrix.md), while a dual prediction with $m$ nonzero coefficients uses $m$ kernel evaluations. Explicit finite [feature maps](feature-map.md) can be preferable when $D$ is small relative to $n$, and a stored primal weight [vector](vector.md) can make prediction depend on $D$ rather than on $n$. [The kernel trick by Ryan Giordano](the-kernel-trick-by-ryan-giordano.md) (sections Ridge regression and The polynomial kernel) explains the change from feature-coordinate equations to training-example equations; neither representation is universally faster.

The [kernel trick](kernel-trick.md) saves explicit feature construction when the [positive-semidefinite kernel](positive-semidefinite-kernel-split.md) is economical to evaluate; it does not remove the cost of optimization, choose a useful [positive-semidefinite kernel](positive-semidefinite-kernel-split.md), or establish [generalization](generalization-in-statistical-learning.md). [Random Fourier features](random-fourier-features.md) illustrate a different tradeoff: replacing the exact [Gaussian kernel](gaussian-kernel.md) with a finite approximate [feature map](feature-map.md) can reduce dependence on the sample count while introducing approximation error.

## ↑ Ancestors (7)

1. [Kernel trick](kernel-trick.md)
2. [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)
3. [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
