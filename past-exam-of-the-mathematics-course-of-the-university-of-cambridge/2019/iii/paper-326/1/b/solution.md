<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u^\dagger=A^\dagger f$. Linearity and the [triangle inequality](../../../../../../triangle-inequality.md) give the [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md)

$$
\|R_{\alpha(\delta)}f_\delta-u^\dagger\|
\leq\|R_{\alpha(\delta)}(f_\delta-f)\|
+\|R_{\alpha(\delta)}f-u^\dagger\|
\leq\delta\|R_{\alpha(\delta)}\|
+\|R_{\alpha(\delta)}f-A^\dagger f\|.
$$

The first term tends to zero by the assumed noise-amplification bound. The second tends to zero because $\alpha(\delta)\to0$ and $R_\alpha$ is a [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md). The right side is independent of the particular noisy datum within its allowed ball. Its convergence therefore proves the uniform noisy-data convergence required of a [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
