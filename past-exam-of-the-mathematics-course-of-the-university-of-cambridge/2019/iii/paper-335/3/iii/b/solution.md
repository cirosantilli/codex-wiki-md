<h1 id="3/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Add and subtract the exact-data iterate. The [noise-bias decomposition for linear regularization](../../../../../../../noise-bias-decomposition-for-linear-regularization.md) gives

$$
x_n^{(\delta)}-x^\dagger=(x_n-x^\dagger)+(x_n^{(\delta)}-x_n),
$$

so the supplied [Landweber noise amplification bound](../../../../../../../landweber-noise-amplification-bound.md) yields

$$
\boxed{\|x_n^{(\delta)}-x^\dagger\|\leq\underbrace{\|x_n-x^\dagger\|}_{\text{regularization bias}}+\underbrace{\sqrt n\,\delta}_{\text{data-error bound}}.}
$$

With unit step and zero initial iterate, the exact-data error is $x^\dagger-x_n=(I-A^*A)^nx^\dagger$. Its squared norm is

$$
\sum_j(1-\sigma_j^2)^{2n}|\langle x^\dagger,v_j\rangle|^2\longrightarrow0
$$

by the [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md). Stopping with $n\to\infty$ but $n\delta^2\to0$ therefore makes both errors vanish.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [3](../../../3.md)
4. [Paper 335](../../../../paper-335-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
