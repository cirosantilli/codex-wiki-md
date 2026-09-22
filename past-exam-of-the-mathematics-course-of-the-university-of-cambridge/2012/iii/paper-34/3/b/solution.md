<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\tau=S_r\wedge T_R$. The stopped logarithm lies between $\log r$ and $\log R$, so the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes it a true bounded [martingale](../../../../../../martingale-split.md). Also $\tau$ is finite almost surely. Indeed $|B_t|^2-2t$ is a [martingale](../../../../../../martingale-split.md), and applying its stopped identity through $t\wedge T_R$ gives

$$
2\mathbb E(t\wedge T_R)=\mathbb E|B_{t\wedge T_R}|^2-1\leq R^2-1.
$$

[monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) implies $\mathbb E T_R\leq(R^2-1)/2<\infty$, hence $\tau\leq T_R<\infty$ almost surely. Boundedness permits [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) in the stopped logarithm as $t\to\infty$. Consequently

$$
\boxed{\mathbb E\log|B_{S_r\wedge T_R}|=0.}
$$

The standard results used are Itô's formula, the bounded-local-martingale criterion, the stopped [martingale](../../../../../../martingale-split.md) identity at bounded [stopping times](../../../../../../stopping-time.md), and dominated/[monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). At exit the radius is either $r$ or $R$ by continuity. Solving $p\log r+(1-p)\log R=0$ also gives the [planar Brownian annulus hitting probability](../../../../../../planar-brownian-annulus-hitting-probability.md)

$$
\mathbb P(S_r\leq T_R)=\frac{\log R}{\log R-\log r}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
