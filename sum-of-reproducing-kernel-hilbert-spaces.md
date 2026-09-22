# Sum of reproducing-kernel Hilbert spaces

↑ **Parent:** [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)

For [positive-semidefinite kernels](positive-semidefinite-kernel.md) $k_j$ with [Reproducing kernel Hilbert spaces](reproducing-kernel-hilbert-space.md) $\mathcal H_j$, the [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md) of $k=\sum_jk_j$ consists of sums $f=\sum_jf_j$, with

$$
\|f\|_{\mathcal H_k}^2=\min_{\sum_jf_j=f}\sum_j\|f_j\|_{\mathcal H_j}^2.
$$

The minimum is attained uniquely. Indeed, in the [Hilbert space](hilbert-space-split.md) direct sum $E=\bigoplus_j\mathcal H_j$, the tuples summing to zero form a closed subspace $N$: they are the intersection, over inputs $x$, of the kernels of the continuous maps $(f_j)\mapsto\sum_jf_j(x)$. Every affine fibre has a unique representative in $N^\perp$ by [orthogonal decomposition by a closed subspace](orthogonal-decomposition-by-a-closed-subspace.md). The [vector](vector.md) $(k_j(\cdot,x))_j$ lies in $N^\perp$ and represents evaluation in the quotient; its evaluation at $y$ is $\sum_jk_j(y,x)$, identifying the [positive-semidefinite kernel](positive-semidefinite-kernel.md) with $k$.

**Table of contents**

- [Common representer coefficients for a sum of kernels](common-representer-coefficients-for-a-sum-of-kernels.md)

## ↑ Ancestors (6)

1. [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)
2. [Positive-semidefinite kernel](positive-semidefinite-kernel.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Common representer coefficients for a sum of kernels](common-representer-coefficients-for-a-sum-of-kernels.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/1/solution.md)
