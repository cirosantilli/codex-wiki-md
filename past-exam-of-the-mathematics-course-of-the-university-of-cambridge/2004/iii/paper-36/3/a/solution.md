<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $v\in Z$, write $M(v)=\max_i v_i$. Maximizing a linear functional on the price [simplex](../../../../../../simplex.md) gives

$$
g(v)=\operatorname{co}\{e_i:v_i=M(v)\}.
$$

Thus $g(v)$ is a nonempty closed [convex](../../../../../../convex-function.md) face of the [compact](../../../../../../compact-space.md) price [simplex](../../../../../../simplex.md). Its [graph of a set-valued mapping](../../../../../../graph-of-a-set-valued-mapping.md) is closed: if $v_n\to v$, $p_n\to p$ and $p_n\in g(v_n)$, then, for every fixed $q\in P$, the inequalities $p_n\cdot v_n\geq q\cdot v_n$ pass to $p\cdot v\geq q\cdot v$.

Each value $z(p)$ is closed in $Z$ by the closed-graph hypothesis, hence [compact](../../../../../../compact-space.md); it is nonempty and [convex](../../../../../../convex-function.md) by assumption. Therefore $F(p,v)=g(v)\times z(p)$ has nonempty closed [convex](../../../../../../convex-function.md) values in the nonempty [compact convex set](../../../../../../compact-convex-set.md) $K=P\times Z$.

Its [graph of a set-valued mapping](../../../../../../graph-of-a-set-valued-mapping.md) is also closed. If $(p_n,v_n)\to(p,v)$ and $(q_n,w_n)\to(q,w)$ with $q_n\in g(v_n)$ and $w_n\in z(p_n)$, the two closed-graph properties give $q\in g(v)$ and $w\in z(p)$. Finally, this closed graph implies [upper hemicontinuity](../../../../../../upper-hemicontinuity.md) because the whole output space $K$ is [compact](../../../../../../compact-space.md). If an open set containing $F(p,v)$ failed to contain the nearby values, select outputs outside it along a convergent input sequence. A subsequence of those outputs converges in $K$; closedness puts its limit in $F(p,v)$, whereas closedness of the open set's complement puts it outside. This contradiction proves [upper hemicontinuity](../../../../../../upper-hemicontinuity.md).

Consequently **all the hypotheses of the Kakutani fixed-point theorem hold**: the domain is nonempty, compact and convex, and the [set-valued mapping](../../../../../../set-valued-mapping.md) maps it into itself with nonempty closed convex values and upper hemicontinuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
