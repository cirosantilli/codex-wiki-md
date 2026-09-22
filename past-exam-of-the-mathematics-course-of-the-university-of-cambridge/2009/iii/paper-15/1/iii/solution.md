<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**No.** The [parallel-bond ray with different site and bond thresholds](../../../../../../parallel-bond-ray-with-different-site-and-bond-thresholds.md) supplies a [locally finite graph](../../../../../../locally-finite-graph.md) counterexample. Take vertices $v_0,v_1,\ldots$ and $n+1$ parallel [directed edges](../../../../../../directed-edge.md) from $v_n$ to $v_{n+1}$. Its underlying [multigraph](../../../../../../multigraph.md) is connected and every individual degree is finite, but there is no uniform incoming-degree bound.

For [bond percolation](../../../../../../bond-percolation-split.md) rooted at $v_0$, survival means that every successive group of parallel bonds contains at least one open bond. Independence gives

$$
\theta_b(p)=\prod_{n=0}^{\infty}\bigl(1-(1-p)^{n+1}\bigr).
$$

For $p>0$, the sum of the failure [probabilities](../../../../../../probability.md) is $\sum_{n\ge0}(1-p)^{n+1}=(1-p)/p<\infty$. Eventually these terms are at most $1/2$, and $\log(1-t)\ge-2t$ for $0\le t\le1/2$. The tail of the [infinite product](../../../../../../infinite-product.md) is therefore bounded below by a positive exponential; its finitely many initial factors are positive as well. Thus $\theta_b(p)>0$ for every $p>0$.

For [site percolation](../../../../../../site-percolation-split.md), however, every vertex of the unique underlying ray must be open. For $p<1$, the [probability](../../../../../../probability.md) that its first $N$ vertices are all open is $p^N\to0$. At $p=1$ the ray is open. Consequently

$$
\boxed{p_H^b=0<1/10,\qquad p_H^s=1.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
