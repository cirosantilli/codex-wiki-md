<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a [spanning tree](../../../../../../spanning-tree.md) $T$ of $G$, rooted at $a$. A [depth-first traversal of a tree](../../../../../../depth-first-traversal-of-a-tree.md) gives a deterministic closed walk

$$
v_0=a,v_1,\ldots,v_{2(n-1)}=a
$$

that traverses each edge of $T$ once in each direction and visits every vertex. Define [stopping times](../../../../../../stopping-time.md) $S_0=0$ and

$$
S_{j+1}=\inf\{t\geq S_j:X_t=v_{j+1}\}.
$$

The [simple random walk](../../../../../../simple-random-walk.md) is at $v_j$ at time $S_j$. All these [hitting times](../../../../../../first-passage-time.md) have finite mean on the finite connected [graph](../../../../../../graph-split.md). By the [Strong Markov property](../../../../../../strong-markov-property.md),

$$
\mathbb E_a S_{2(n-1)}=\sum_{j=0}^{2(n-1)-1}\mathbb E_{v_j}\tau_{v_{j+1}}.
$$

The [cover time](../../../../../../cover-time.md) is no larger than $S_{2(n-1)}$. Grouping the summands by the two traversals of each tree edge and applying the [commute time identity](../../../../../../commute-time-identity.md) gives

$$
\mathbb E_a\tau_{\mathrm{cov}}\leq\sum_{\{u,v\}\in T}\bigl(\mathbb E_u\tau_v+\mathbb E_v\tau_u\bigr)=2|E|\sum_{\{u,v\}\in T}R_{\mathrm{eff}}^G(u,v).
$$

The [effective resistances](../../../../../../effective-resistance.md) are measured in the original [graph](../../../../../../graph-split.md), where each tree-edge pair is adjacent. Part (a) therefore bounds every summand by one, so

$$
\boxed{\mathbb E_a\tau_{\mathrm{cov}}\leq2(n-1)|E|.}
$$

For the one-vertex [graph](../../../../../../graph-split.md), the [cover time](../../../../../../cover-time.md) is zero and the same bound is immediate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
