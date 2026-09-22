<h1 id="18c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Independence gives $\mathbb E[X_1(1-X_2)]=\theta(1-\theta)=\phi$, proving unbiasedness. Conditional on $K=k$, all binary sample strings with $k$ ones are equally likely. Therefore

$$
\mathbb E[X_1(1-X_2)\mid K=k]
=\frac kn\frac{n-k}{n-1}=\frac{k(n-k)}{n(n-1)}.
$$

The [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md), or the tower property and total [variance](../../../../../../variance-split.md) decomposition directly, yields the improved estimator

$$
\boxed{\widetilde\phi=\frac{K(n-K)}{n(n-1)}=\frac n{n-1}\widehat\phi.}
$$

It is unbiased by [conditional expectation](../../../../../../conditional-expectation.md) and is a function of the requested MLE. Its [variance](../../../../../../variance-split.md) is strictly smaller, since

$$
\operatorname{Var}(X_1(1-X_2))
=\operatorname{Var}(\widetilde\phi)+\mathbb E[\operatorname{Var}(X_1(1-X_2)\mid K)].
$$

For $0<\theta<1$, the event $K=1$ has positive probability. On it, $X_1(1-X_2)$ has probability $1/n$ of being one, strictly between zero and one for $n\geq2$. Thus the final expectation is strictly positive. This proves **strict [variance](../../../../../../variance-split.md) reduction**, not merely a weak inequality.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
