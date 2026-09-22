<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the standard labelled encoding of a pointed [planar quadrangulation](../../../../../../../planar-quadrangulation.md), incidences at the distinguished vertex are represented by visits counted by the record variables $G_m$. Consequently its [degree of a vertex](../../../../../../../degree-graph-theory.md) is bounded by the largest such count encountered before the coding walk first reaches $-1$.

Before time $2n+1$ there are at most $2n+1$ possible record levels. The [union bound](../../../../../../../boole-s-inequality.md) and part i therefore imply

$$
\mathbb P\left(\max_mG_m\geq r,\ \sigma=2n+1\right)
\leq(2n+1)\left(\frac56\right)^{r-1}.
$$

Conditioning on $\sigma=2n+1$ and using the supplied lower bound gives

$$
\mathbb P\left(\deg(v^*)\geq r\mid\sigma=2n+1\right)
\leq C_0n^{5/2}\left(\frac56\right)^{r-1}.
$$

Set $r=C\log n$. If $C>5/(2\log(6/5))$, the right-hand side tends to zero. Hence for some constant $C>0$,

$$
\boxed{\mathbb P(\deg(v^*)\leq C\log n)\longrightarrow1}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 220](../../../../paper-220-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
