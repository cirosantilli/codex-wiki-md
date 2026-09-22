<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite sample, the Gram matrix of $k_1k_2$ is the entrywise product of the two positive-semidefinite Gram matrices. The [Schur product theorem](../../../../../../schur-product-theorem.md) makes it positive semidefinite, proving the product closure.

The [Gaussian kernel](../../../../../../gaussian-kernel.md) with bandwidth $\sigma^2$ is

$$
\boxed{k_\sigma(x,x')=
\exp\left(-\frac{\|x-x'\|_2^2}{2\sigma^2}\right).}
$$

Factor it as

$$
e^{-\|x\|^2/(2\sigma^2)}e^{-\|x'\|^2/(2\sigma^2)}
\sum_{m=0}^\infty\frac{(x^Tx')^m}{m!\sigma^{2m}}.
$$

The linear kernel $x^Tx'$ is positive semidefinite; products and nonnegative scalar multiples preserve positivity, as does multiplication by $a(x)a(x')$. The partial sums are therefore kernels, and pointwise-limit closure proves that the Gaussian kernel is positive semidefinite.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
