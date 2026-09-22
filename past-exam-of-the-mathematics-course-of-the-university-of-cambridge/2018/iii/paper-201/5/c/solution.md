<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $T_y=\inf\{s\geq0:B_s=y\}$. Reflect at this [stopping time](../../../../../../stopping-time.md), using the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) from (a). Path [continuity](../../../../../../continuous-function.md) gives $\{S_t\geq y\}=\{T_y\leq t\}$, and on this [event](../../../../../../event.md) the reflected endpoint is $\widehat B_t=2y-B_t$. Consequently

$$
\{S_t\geq y,\ B_t\leq x\}
=\{T_y\leq t,\ \widehat B_t\geq2y-x\}.
$$

Since $x\leq y$, an endpoint $\widehat B_t\geq2y-x\geq y$ forces the reflected path to have hit $y$ by time $t$. Reflection preserves the first hit of $y$, so the condition $T_y\leq t$ is redundant on the right. As $\widehat B$ has the same [probability distribution](../../../../../../probability-distribution.md) as $B$, the [joint distribution of Brownian motion and its running maximum](../../../../../../joint-distribution-of-brownian-motion-and-its-running-maximum.md) satisfies

$$
\boxed{\mathbb P(S_t\geq y,\ B_t\leq x)=\mathbb P(B_t\geq2y-x).}
$$

This argument includes $x=y$; at positive $t$ the boundary endpoint has zero probability under the [normal distribution](../../../../../../normal-distribution.md). At $t=0$ both sides vanish because $y>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
