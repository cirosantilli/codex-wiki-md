<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a function smooth on finitely many closed pieces with finite one-sided derivatives, integration by parts gives its [Fourier series](../../../../../../fourier-series-split.md) coefficients, for $n\ne0$,

$$
c_n=\frac1{2\pi in}\sum_rJ_re^{-2\pi inx_r}+O(n^{-2}),
$$

where $J_r=f(x_r+)-f(x_r-)$ includes the jump of the periodic extension at the endpoint when necessary. In particular $|c_n|\le C/|n|$. Keeping frequencies $|n|\le K$, with $N\asymp K$, gives squared error $O(\sum_{n>K}n^{-2})=O(N^{-1})$.

A [best N-term approximation](../../../../../../best-n-term-approximation.md) cannot improve this worst-case rate. For example, $f=\chi_{[0,1/2)}$ has $|c_n|=1/(\pi|n|)$ on odd nonzero $n$ and zero on even nonzero $n$. Even the optimal selection therefore leaves a squared tail comparable to $N^{-1}$. Thus for the class with jumps,

$$
\boxed{\text{linear and nonlinear squared errors have sharp worst-case rate }N^{-1},}
$$

or $N^{-1/2}$ in the $L^2$ [norm](../../../../../../norm.md). Individual functions with no jumps, or additional cancellation, can converge faster. “Smooth except at finitely many points” must include controlled one-sided smoothness; smoothness merely on open pieces permits pathological behavior near their endpoints.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
