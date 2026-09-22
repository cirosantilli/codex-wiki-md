<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With equal type probabilities, $F$ and $S$ have the same marginal [probability generating function](../../../../../../probability-generating-function.md), namely $G_N((1+s)/2)$. Their assumed [independence](../../../../../../independent-random-variables.md), together with $N=F+S$, gives

$$
\boxed{G_N(s)=G_F(s)G_S(s)=G_N\left(\frac{1+s}{2}\right)^2.}
$$

Set $H(t)=G_N(1-t)$ for $0\le t\le1$. The identity becomes $H(t)=H(t/2)^2$ and, after $k$ iterations,

$$
H(t)=H(t/2^k)^{2^k}.
$$

The finite [expected value](../../../../../../expected-value.md) gives $G_N(1-h)=1-\mu h+o(h)$ as $h\downarrow0$. To justify this without any analyticity assumption at the endpoint, note that $(1-(1-h)^N)/h\to N$ and is bounded above by $N$; [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives the derivative $G_N'(1-)=\mu$. Substituting the expansion into the iterated identity yields

$$
H(t)=\left(1-\frac{\mu t}{2^k}+o(2^{-k})\right)^{2^k}\longrightarrow e^{-\mu t}.
$$

The left side is independent of $k$, so it equals the limit. Thus $G_N(s)=e^{\mu(s-1)}$ on $[0,1]$ and uniqueness of the power-series coefficients proves **$N\sim\operatorname{Poisson}(\mu)$**. Only finite [expected value](../../../../../../expected-value.md) was needed; the given finite [variance](../../../../../../variance-split.md) is stronger. This proves the [Poisson characterization by independent binomial splitting](../../../../../../poisson-characterization-by-independent-binomial-splitting.md) rather than assuming the original count distribution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
