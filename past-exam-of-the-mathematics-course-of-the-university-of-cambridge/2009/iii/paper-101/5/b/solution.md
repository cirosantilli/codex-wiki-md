<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditional on $Z=k$, the summands are [independent](../../../../../../independent-random-variables.md) with the common [Laplace transform of a nonnegative random variable](../../../../../../laplace-transform-of-a-nonnegative-random-variable.md) $\phi(q)$. The empty sum for $k=0$ is zero. Therefore the [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) has

$$
\mathbb E[e^{-qY}\mid Z=k]=\phi(q)^k,
$$

and applying the [probability generating function](../../../../../../probability-generating-function.md) from part (a) gives

$$
\boxed{L_Y(q)=\mathbb Ee^{-qY}=\exp\{\lambda[\phi(q)-1]\}\qquad(q\geq0).}
$$

If $m=\mathbb EX_1<\infty$, differentiating at zero from the right gives $\phi'(0+)=-m$ and $L_Y'(0+)=-\lambda m$. Hence

$$
\boxed{\mathbb EY=\lambda\mathbb EX_1.}
$$

The differentiation is justified by $(1-e^{-qX_1})/q\leq X_1$ and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). No finite moment was assumed in the question, so the formula must also be interpreted when $m=\infty$. For any nonnegative [random variable](../../../../../../random-variable-split.md) $V$, the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) gives

$$
\mathbb EV=\lim_{q\downarrow0}\frac{1-\mathbb Ee^{-qV}}q\in[0,\infty].
$$

Apply this to $X_1$ and $Y$, and use $1-e^{-\lambda h}\sim\lambda h$ as $h\downarrow0$, with $h=1-\phi(q)$; it yields the same formula with value $+\infty$ when $m=\infty$. If $m=0$, nonnegativity makes all marks zero [almost surely](../../../../../../almost-sure-convergence.md) and the result is immediate.

For the second method, condition on the count rather than differentiating a transform. For finite $m$, the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives $\mathbb E[Y\mid Z]=Zm$, and $\mathbb EZ=\lambda$ gives $\mathbb EY=\lambda m$. More generally, [Tonelli's theorem](../../../../../../tonelli-theorem.md) and [independence](../../../../../../independent-random-variables.md) give

$$
\mathbb EY=\sum_{j=1}^\infty\mathbb E[X_j\mathbf1_{\{Z\geq j\}}]
=m\sum_{j=1}^\infty\mathbb P(Z\geq j)=m\mathbb EZ.
$$

For $m=\infty$, already the term $j=1$ is infinite since $\mathbb P(Z\geq1)>0$. Thus the two methods agree, including in the extended-valued case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
