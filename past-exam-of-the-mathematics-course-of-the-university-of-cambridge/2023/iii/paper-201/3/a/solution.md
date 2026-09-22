<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The probability generating function of each $X_i$ is $\exp(z-1)$. Independence makes the generating function of $S_n$ equal to $\exp(n(z-1))$, so the [addition of independent Poisson random variables](../../../../../../addition-of-independent-poisson-random-variables.md) gives $S_n\sim\operatorname{Pois}(n)$.

The [Poisson distribution](../../../../../../poisson-distribution.md) has mean and variance $n$, hence $\mathbb E Y_n=0$ and $\mathbb E[Y_n^2]=1$. Since $Y_n^-\leq|Y_n|$, [Chebyshev inequality](../../../../../../chebyshev-inequality.md) gives

$$
\boxed{\mathbb P(Y_n^-\geq a)
\leq\mathbb P(|Y_n|\geq a)
\leq\frac1{a^2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
