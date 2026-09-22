<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Regard each centered random variable $g(x)$ as a vector $h_x$ in the Hilbert space $L^2(\mathbb P)$. Then

$$
\operatorname{Var}(g(x)-g(x'))=\lVert h_x-h_{x'}\rVert_2^2,
$$

so $k$ is the [Gaussian kernel](../../../../../../gaussian-kernel.md) on the finite subset $\{h_x:x\in\mathcal X\}$ of that Hilbert space. More explicitly,

$$
k(x,x')=e^{-\lVert h_x\rVert^2/(2\eta^2)}e^{-\lVert h_{x'}\rVert^2/(2\eta^2)}
\sum_{m=0}^\infty\frac{\langle h_x,h_{x'}\rangle^m}{m!\eta^{2m}}.
$$

Every power of the inner-product kernel is [positive semidefinite](../../../../../../positive-semidefinite-kernel.md), and the [closure property of positive-semidefinite kernels](../../../../../../closure-property-of-positive-semidefinite-kernels.md) under nonnegative sums, pointwise limits, and multiplication by one-variable factors proves that $k$ is positive definite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
