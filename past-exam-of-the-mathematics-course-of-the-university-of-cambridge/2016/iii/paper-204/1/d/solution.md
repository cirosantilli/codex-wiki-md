<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [union bound](../../../../../../boole-s-inequality.md) gives $g_k\leq\sum_{x\in\partial\Lambda_k}\mathbb P_p(0\leftrightarrow x)$. Hence some boundary [graph vertex](../../../../../../vertex-graph-theory.md) has [percolation two-point connection probability](../../../../../../percolation-two-point-connection-probability.md) at least $g_k/(8k)$. The rotations and reflections of the [square lattice](../../../../../../square-lattice.md) let us choose such a [graph vertex](../../../../../../vertex-graph-theory.md) as $x=(k,j)$, $-k\leq j\leq k$. Reflection in the vertical line through $x$ sends $0$ to $e_{2k}=(2k,0)$ and fixes $x$. Therefore

$$
\mathbb P_p(x\leftrightarrow e_{2k})=\mathbb P_p(0\leftrightarrow x).
$$

The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) applied to these two [increasing events](../../../../../../increasing-event.md) proves the [reflection lower bound for two-point percolation](../../../../../../reflection-lower-bound-for-two-point-percolation.md):

$$
h_{2k}\geq\mathbb P_p(0\leftrightarrow x,\ x\leftrightarrow e_{2k})\geq\left(\frac{g_k}{8k}\right)^2.
$$

Every [graph path](../../../../../../path-in-a-graph.md) from $0$ to $e_{2k}$ reaches $\partial\Lambda_{2k}$, so $h_{2k}\leq g_{2k}$. Taking roots gives

$$
\left(\frac{g_k}{8k}\right)^{1/k}\leq h_{2k}^{1/(2k)}\leq g_{2k}^{1/(2k)}.
$$

Both outside expressions have [limit of a sequence](../../../../../../limit-of-a-sequence.md) $\gamma$, proving the even case. For $p>0$, the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) with the last horizontal [edge](../../../../../../edge-of-a-graph.md) gives $h_{2k+1}\geq p h_{2k}$, and also $h_{2k+1}\leq g_{2k+1}$. The lower bound has root

$$
(p h_{2k})^{1/(2k+1)}=p^{1/(2k+1)}\left(h_{2k}^{1/(2k)}\right)^{2k/(2k+1)}\longrightarrow\gamma.
$$

The upper bound has the same [limit of a sequence](../../../../../../limit-of-a-sequence.md). At $p=0$ all positive-distance connection [probabilities](../../../../../../probability.md) vanish. **Thus $\lim_{n\to\infty}h_n^{1/n}=\gamma$ for every $p\in[0,1]$.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
