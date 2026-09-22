<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Multiplying the reciprocal [improper prior](../../../../../../improper-prior.md) by the [likelihood function](../../../../../../likelihood-function.md) gives

$$
p(N\mid y)=\frac{N^{-2}}{S_y},\qquad N\geq y,
\qquad S_y=\sum_{k=y}^{\infty}k^{-2}<\infty.
$$

Thus this [discrete uniform endpoint posterior](../../../../../../discrete-uniform-endpoint-posterior.md) is proper. Its exact cumulative probability is $S_y^{-1}\sum_{k=y}^n k^{-2}$. Integral approximation gives $S_y\approx\int_y^\infty t^{-2}\,dt=1/y$ and $\sum_{k=y}^n k^{-2}\approx\int_y^n t^{-2}\,dt=1/y-1/n$, so

$$
\boxed{\Pr(N\leq n\mid y)\approx1-\frac yn,\qquad
\operatorname{median}(N\mid y)\approx2y=200.}
$$

These approximations are useful when $y$ is moderately large and are not exact discrete identities. For example the exact untruncated median at $y=100$ is $199$. Although its [quantiles](../../../../../../quantile-function.md) are finite, its [posterior mean](../../../../../../posterior-mean.md) is infinite, since its expectation numerator is the divergent sum $\sum_{N=y}^\infty1/N$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
