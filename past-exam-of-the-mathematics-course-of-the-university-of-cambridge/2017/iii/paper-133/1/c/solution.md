<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Retain the [metric geodesic](../../../../../../metric-geodesic.md) subdivision and orbit-density parts of the usual [Milnor–Švarc lemma](../../../../../../milnor-svarc-lemma.md) proof. Drop the step using proper discontinuity and compactness to prove that the displacement-bounded generating set is finite.

More explicitly, let $L=d_X(x,gx)$ and $m=\max\{1,\lceil L\rceil\}$. Subdivide a [metric geodesic](../../../../../../metric-geodesic.md) from $x$ to $gx$ into $m$ segments of length at most one. Choose orbit points $g_i x$ within distance $R$ of the subdivision points, choosing the endpoints exactly: $g_0=1$, $g_m=g$. Then

$$
d_X(g_{i-1}x,g_i x)\leq2R+1,
$$

so every nonidentity increment $g_{i-1}^{-1}g_i$ lies in $S$. Their telescoping product is $g$, and hence

$$
|g|_S\leq m\leq L+1.
$$

This also covers $L=0$, when the one increment may be a nontrivial stabilizer element. Conversely, for any word $g=s_1\cdots s_k$ in $S$, the [triangle inequality](../../../../../../triangle-inequality.md) and invariance under the isometric action give

$$
d_X(x,gx)\leq\sum_{i=1}^k d_X(x,s_i x)\leq(2R+1)k.
$$

Taking the shortest word gives the other inequality. Thus **the proof works unchanged except that the resulting generating set may be infinite**. Neither local compactness nor a finite stabilizer is used in this weaker argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
