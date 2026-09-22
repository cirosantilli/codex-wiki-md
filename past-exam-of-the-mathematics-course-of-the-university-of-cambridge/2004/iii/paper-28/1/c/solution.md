<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $V=\mathbb EX_n^2$. For $c\geq0$, the process $(X_m+c)^2$ is a nonnegative [submartingale](../../../../../../submartingale.md), by the [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md). A crossing of $x$ by $X$ implies a crossing of $(x+c)^2$ by this squared process. Since $\mathbb EX_n=\mathbb EX_0=0$, the [Doob maximal inequality](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) gives

$$
\mathbb P\left(\max_{m\leq n}X_m\geq x\right)
\leq\frac{\mathbb E(X_n+c)^2}{(x+c)^2}
=\frac{V+c^2}{(x+c)^2}.
$$

For $V>0$, [differentiation](../../../../../../differentiation.md) of the last expression gives $2(cx-V)/(x+c)^3$, so its minimum over $c\geq0$ occurs at $c=V/x$. Substitution proves the [one-sided martingale maximal inequality](../../../../../../one-sided-martingale-maximal-inequality.md)

$$
\boxed{\mathbb P\left(\max_{0\leq m\leq n}X_m\geq x\right)
\leq\frac{V}{V+x^2}.}
$$

If $V=0$, then $X_n=0$ [almost surely](../../../../../../almost-sure-convergence.md) and $X_m=\mathbb E[X_n\mid\mathcal F_m]=0$ for every $m\leq n$, so the same conclusion holds. The constant is sharp: at one step take $X_1=x$ with probability $V/(V+x^2)$ and $X_1=-V/x$ otherwise. This has [mean](../../../../../../expected-value.md) zero, [variance](../../../../../../variance-split.md) $V$, and achieves equality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
