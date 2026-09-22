<h1 id="26k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The independent standard [Gaussian random variables](../../../../../../gaussian-random-variable.md) have mean zero and variance one. For $m>n$, the mixed products have expectation zero, giving

$$
\|Y_m-Y_n\|_2^2=\mathbb E\left(\sum_{j=n+1}^m\alpha_jX_j\right)^2=\sum_{j=n+1}^m\alpha_j^2\longrightarrow0
$$

uniformly over $m>n$ as $n\to\infty$. Thus $(Y_n)$ is Cauchy in the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). Its completeness, proved in (i), supplies

$$
\boxed{\exists Y\in L^2:\quad\|Y_n-Y\|_2\longrightarrow0.}
$$

Moreover $L^2$ convergence implies convergence of the means and second moments: $\mathbb EY=0$ and $\mathbb EY^2=\lim_n\sum_{j\leq n}\alpha_j^2=\sigma^2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [26K](../../26k.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
