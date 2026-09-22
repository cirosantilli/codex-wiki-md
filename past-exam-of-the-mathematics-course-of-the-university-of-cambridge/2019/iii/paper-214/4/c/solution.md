<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Exhaust $\mathbb Z^2$ by finite boxes $G_n$ and let $T_n$ be a [uniform spanning tree](../../../../../../uniform-spanning-tree.md) of $G_n$. Every finite tree satisfies the [handshaking lemma](../../../../../../degree-sum-formula.md), so

$$
\frac1{|V(G_n)|}\sum_{v\in V(G_n)}\deg_{T_n}(v)
=\frac{2(|V(G_n)|-1)}{|V(G_n)|}\longrightarrow2.
$$

Choose the root uniformly from $V(G_n)$. The proportion of roots within any fixed distance of the boundary tends to zero, and the rooted trees converge locally to the uniform spanning tree $T$ of $\mathbb Z^2$. Since every degree is at most four, expectations also converge. Translation invariance therefore gives

$$
\mathbb E[\deg_T(0)]=2.
$$

The four edges incident to $0$ have equal inclusion probability by the rotations and reflections of the square lattice. If that common probability is $r$, then $4r=\mathbb E\deg_T(0)=2$. Consequently

$$
\boxed{\mathbb P(e\in T)=\frac12}
$$

for every edge $e$ by translation invariance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
