<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

The [integral test for convergence](../../../../../integral-test-for-convergence.md) applies when $a_n=h(n)$ for all sufficiently large $n$, where $h$ is nonnegative, continuous and nonincreasing on $[N,\infty)$. It states that $\sum_{n=N}^\infty a_n$ converges if and only if the [improper integral](../../../../../improper-integral.md) $\int_N^\infty h(x)\,dx$ is finite. Its comparison bounds are

$$
\int_N^{M+1}h(x)\,dx\le\sum_{n=N}^M h(n)\le h(N)+\int_N^M h(x)\,dx.
$$

No conclusion about an arbitrary nonnegative sequence follows without such a monotone comparison function; finite initial terms do not affect convergence.

For $h(x)=x^{-\alpha}$ with $\alpha>0$, all the hypotheses hold. If $\alpha\ne1$,

$$
\int_1^R x^{-\alpha}\,dx=\frac{R^{1-\alpha}-1}{1-\alpha},
$$

whereas for $\alpha=1$ the integral is $\log R$. The first expression has a finite limit exactly when $\alpha>1$. Thus the [p-series](../../../../../p-series.md) satisfies

$$
\boxed{\sum_{n=1}^\infty n^{-\alpha}\text{ converges iff }\alpha>1;\quad\text{it diverges for }0<\alpha\le1.}
$$

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
