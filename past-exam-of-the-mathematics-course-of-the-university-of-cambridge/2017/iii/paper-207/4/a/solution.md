<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative continuous event time, the [survivor function](../../../../../../survival-function.md) is $F(t)=\mathbb P(T>t)$; here the printed $F$ denotes survival, not the usual [cumulative distribution function](../../../../../../cumulative-distribution-function.md). A lower [median](../../../../../../median.md) is

$$
\boxed{m=\inf\{t\geq0:F(t)\leq1/2\}.}
$$

For a continuous strictly decreasing [survivor function](../../../../../../survival-function.md) this is the unique solution of $F(m)=1/2$. If the curve has a flat stretch at $1/2$, the distribution has a nonunique median and the infimum specifies the lower endpoint.

The [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md) follows from $T=\int_0^\infty\mathbf1\{T>t\}\,dt$ and [Tonelli theorem](../../../../../../tonelli-theorem.md). Therefore, when survival vanishes beyond $t^*$,

$$
\boxed{\mathbb ET=\int_0^{t^*}F(t)\,dt.}
$$

If $F(t)>0$ at every finite time, the mean is finite precisely when $\int_0^\infty F(t)\,dt<\infty$. For a concrete sufficient condition, require $F(t)\leq Ct^{-1-\varepsilon}$ for all $t\geq M>0$, with $C<\infty$ and $\varepsilon>0$. The integral over $[0,M]$ is at most $M$, and the tail integral is at most $CM^{-\varepsilon}/\varepsilon$. An exponential tail bound also suffices. Merely having $F(t)\to0$, or even $tF(t)\to0$, does not suffice: a properly completed decreasing tail proportional to $1/(t\log t)$ for $t\geq e$ has infinite mean.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
