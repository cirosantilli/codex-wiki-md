# Kernel trick

↑ **Parent:** [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_trick)

The kernel trick evaluates [inner products](inner-product.md) of [feature map](feature-map.md) outputs through $k(x,z)=\langle\phi(x),\phi(z)\rangle$ without explicitly constructing those [vectors](vector.md). An algorithm expressed entirely through these [inner products](inner-product.md) can therefore operate on nonlinear derived coordinates using only evaluations of a [positive-semidefinite kernel](positive-semidefinite-kernel.md) on the original inputs. A [classifier](classifier.md) linear in the derived coordinates can have a nonlinear boundary in the original coordinates.

The [polynomial kernel](polynomial-kernel.md) gives a finite, fully visible example: $k(x,z)=(x^Tz)^2$ corresponds to $\phi(x)=(x_1^2,\sqrt2 x_1x_2,x_2^2)^T$. The [XOR separation by a product feature](xor-separation-by-a-product-feature.md) below makes the interaction coordinate $x_1x_2$ useful, while [dual prediction with a kernel](dual-prediction-with-a-kernel.md) shows how to predict without calculating it explicitly.

An arbitrary score called a similarity need not be a [positive-semidefinite kernel](positive-semidefinite-kernel.md). Symmetry alone, even with nonnegative entries, is insufficient: the symmetric [matrix](matrix.md)

$$
S=\begin{pmatrix}1&2\\2&1\end{pmatrix}
$$

has $a^TSa=-2$ for $a=(1,-1)^T$, so it cannot be a [Gram matrix](gram-matrix.md) of real [inner products](inner-product.md). A [positive-semidefinite kernel](positive-semidefinite-kernel.md) requires a [positive semidefinite matrix](positive-semidefinite-matrix.md) for every finite choice of inputs, not just the observed [training data](training-data.md).[Section 4.1, p. 80: Gram matrices, quadratic-form definition of positive semidefiniteness, and nonnegative eigenvalues](gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams.md) The existing [Moore-Aronszajn theorem](moore-aronszajn-theorem.md) connects this requirement to a [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md); this example needs only finite [linear algebra](linear-algebra-split.md).

**Table of contents**

- [XOR separation by a product feature](xor-separation-by-a-product-feature.md)
- [Dual prediction with a kernel](dual-prediction-with-a-kernel.md)
- [Computational tradeoffs of the kernel trick](computational-tradeoffs-of-the-kernel-trick.md)
- [Kernel principal component analysis](kernel-principal-component-analysis.md)

## ↑ Ancestors (6)

1. [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)
2. [Positive-semidefinite kernel](positive-semidefinite-kernel.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Computational tradeoffs of the kernel trick](computational-tradeoffs-of-the-kernel-trick.md)
- [Kernel support vector machine](kernel-support-vector-machine.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-218/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/6/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-218/4/f/solution.md)
- [Polynomial kernel](polynomial-kernel.md)
