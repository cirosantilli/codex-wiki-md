<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S_N(x)=\sum_{n=1}^N|f_n(x)|$. These are nonnegative [measurable functions](../../../../measurable-function.md) increasing to the extended-valued [function](../../../../function-split.md) $S(x)=\sum_{n=1}^{\infty}|f_n(x)|$. The [monotone convergence theorem](../../../../monotone-convergence-theorem.md) gives

$$
\int_ES(x)\,dx=\lim_{N\to\infty}\sum_{n=1}^N\int_E|f_n(x)|\,dx
=\sum_{n=1}^{\infty}\|f_n\|_1<\infty.
$$

Therefore $S$ is finite [almost everywhere](../../../../almost-everywhere.md): if $S=\infty$ on a [measurable set](../../../../measurable-set.md) of positive [Lebesgue measure](../../../../lebesgue-measure.md), its [integral](../../../../integral-split.md) would exceed every finite bound. Hence the [series](../../../../series-mathematics.md) $\sum_nf_n(x)$ converges absolutely outside the [null set](../../../../null-set.md) $N=\{S=\infty\}$. This is [summable L1 norms imply almost-everywhere absolute convergence](../../../../summable-l1-norms-imply-almost-everywhere-absolute-convergence.md).

Define $s(x)=\sum_nf_n(x)$ off $N$ and set $s=0$ on $N$. The [function](../../../../function-split.md) is [Lebesgue measurable](../../../../lebesgue-measurable-set.md), being the pointwise [limit](../../../../limit-of-a-function.md) of measurable partial sums off a measurable [null set](../../../../null-set.md). Since $|s|\leq S$ [almost everywhere](../../../../almost-everywhere.md),

$$
\|s\|_1\leq\int_ES<\infty,
$$

so **the sum is [Lebesgue integrable](../../../../lebesgue-integrable-function.md)**.

For $s_N=\sum_{n=1}^Nf_n$, the absolute tail satisfies

$$
|s-s_N|\leq\sum_{n=N+1}^{\infty}|f_n|\qquad\text{almost everywhere}.
$$

Apply the [monotone convergence theorem](../../../../monotone-convergence-theorem.md) to the nonnegative tail partial sums. We obtain

$$
\|s-s_N\|_1\leq\sum_{n=N+1}^{\infty}\|f_n\|_1\longrightarrow0.
$$

Thus the partial sums converge in [L1 norm](../../../../l1-norm.md). The [triangle inequality for an integral](../../../../integral-triangle-inequality.md) yields

$$
\left|\int_Es-\sum_{n=1}^N\int_Ef_n\right|\leq\|s-s_N\|_1\longrightarrow0.
$$

Consequently

$$
\boxed{\int_E\sum_{n=1}^{\infty}f_n(x)\,dx=\sum_{n=1}^{\infty}\int_Ef_n(x)\,dx.}
$$

The scalar [series](../../../../series-mathematics.md) on the right also converges absolutely, since $\sum_n|\int_Ef_n|\leq\sum_n\|f_n\|_1<\infty$. This proves [integration of a series with summable L1 norms](../../../../integration-of-a-series-with-summable-l1-norms.md) without needing pointwise convergence on the exceptional [null set](../../../../null-set.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
