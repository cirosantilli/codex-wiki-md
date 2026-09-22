<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Assume $\mathbb E|g(X)|<\infty$, or use nonnegative $g$ with extended expectations. Let $p_{ij}=\mathbb P(X=x_i,Y=y_j)$ and $p_j=\mathbb P(Y=y_j)$. For $p_j>0$, the discrete [conditional expectation](../../../../../conditional-expectation.md) is $\mathbb E[g(X)\mid Y=y_j]=\sum_i g(x_i)p_{ij}/p_j$. Therefore [Fubini's theorem](../../../../../fubini-s-theorem.md), or [Tonelli theorem](../../../../../tonelli-theorem.md) in the nonnegative case, gives the [tower property of conditional expectation](../../../../../law-of-total-expectation.md):

$$
\boxed{\mathbb E[\mathbb E[g(X)\mid Y]]=\sum_{j:p_j>0}\sum_i g(x_i)p_{ij}=\sum_i g(x_i)\mathbb P(X=x_i)=\mathbb E[g(X)].}
$$

Values of a [conditional expectation](../../../../../conditional-expectation.md) on zero-probability conditioning events do not affect the sum. An unrestricted signed $g$ whose expectation is undefined is outside this assertion.

Write $M(x)=\mathbb E[N(x)]$. The waiting time for two increments larger than $1/2$ dominates $N(x)$ for $0\leq x\leq1$ and has mean $4$, so $M$ is finite. Conditioning on the first increment, one step is always consumed; if that increment is below $x$, the remaining independent sequence has the original law. Thus [first-step analysis](../../../../../first-step-analysis.md) and the [tower property of conditional expectation](../../../../../law-of-total-expectation.md) give

$$
M(x)=1+\int_0^xM(x-u)\,du=1+\int_0^xM(s)\,ds.
$$

This first makes $M$ continuous and then gives $M'=M$, with $M(0)=1$. Hence the [uniform-sum crossing time below one](../../../../../uniform-sum-crossing-time-below-one.md) has

$$
\boxed{\mathbb E[N(x)]=e^x,\qquad 0\leq x\leq1.}
$$

An independent explanation uses the [tail-sum formula](../../../../../tail-sum-formula.md): $\mathbb P(N(x)>n)=\mathbb P(U_1+\cdots+U_n\leq x)=x^n/n!$ for $x\leq1$, since this region is an $n$-dimensional simplex inside the unit cube. Summing from $n=0$ gives $e^x$. In particular the strict-crossing convention gives $N(0)=1$ almost surely and $\mathbb E N(1)=e$.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
