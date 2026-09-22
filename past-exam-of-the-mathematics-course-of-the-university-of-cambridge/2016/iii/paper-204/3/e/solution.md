<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the following general result, including its site version: independent [site percolation](../../../../../../site-percolation-split.md) on $\mathbb Z^d$ has [almost surely](../../../../../../almost-sure-convergence.md) at most one [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) at each fixed parameter; for every fixed $r>p_c$ it has exactly one [almost surely](../../../../../../almost-sure-convergence.md). This is the [uniqueness of the infinite percolation cluster](../../../../../../uniqueness-of-the-infinite-percolation-cluster.md), also called the [Burton-Keane theorem](../../../../../../uniqueness-of-the-infinite-percolation-cluster.md). For $d\geq2$, the additional general fact $p_c<1$ ensures a choice of a parameter strictly between $p_c$ and $1$. In dimension one, $p_c=1$ and the asserted interval is empty.

Fix $p\in(p_c,1]$ and choose $q\in(p_c,p)$. Let $\mathcal C_q$ be the unique infinite open [connected component of a graph](../../../../../../component-graph-theory.md) at $q$. Under the [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md), it is contained in the unique infinite open [connected component of a graph](../../../../../../component-graph-theory.md) at $p$. On $I_p$, the origin and $\mathcal C_q$ therefore lie in that same [connected component of a graph](../../../../../../component-graph-theory.md), and a finite $p$-open [graph path](../../../../../../path-in-a-graph.md) connects $0$ to some [graph vertex](../../../../../../vertex-graph-theory.md) of $\mathcal C_q$.

For this fixed deterministic $p$, the countable [set](../../../../../../set-split.md) of uniforms satisfies $U_v\ne p$ at every [graph vertex](../../../../../../vertex-graph-theory.md) [almost surely](../../../../../../almost-sure-convergence.md). Thus all uniforms on that finite [graph path](../../../../../../path-in-a-graph.md) are strictly less than $p$, including its endpoints. If $t$ is their maximum, choose $r$ with $\max(q,t)<r<p$. The [graph path](../../../../../../path-in-a-graph.md) is then $r$-open, and its endpoint remains connected to infinity through $\mathcal C_q$. Consequently $I_r$ occurs and $M<p$. We have proved

$$
\mathbb P(I_p\cap\{M=p\})=0.
$$

Part (d) gives left continuity at this $p$; part (b) supplies right continuity when $p<1$. The same finite-path proof gives left continuity at $p=1$, since all uniforms are strictly less than $1$ [almost surely](../../../../../../almost-sure-convergence.md). **Thus $\theta$ is continuous on $(p_c,1]$**, without asserting continuity at $p_c$. This is [supercritical continuity of percolation probability](../../../../../../supercritical-continuity-of-percolation-probability.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
