<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Order configurations coordinatewise: $\omega\leq\eta$ means that every open [edge](../../../../../edge-of-a-graph.md) of $\omega$ is open in $\eta$. An [increasing event](../../../../../increasing-event.md) $A$ satisfies $\omega\in A,\ \omega\leq\eta\Rightarrow\eta\in A$. For $K\subseteq E$, let $\mathbf1_K$ be the configuration with exactly the [edges](../../../../../edge-of-a-graph.md) of $K$ open. For [increasing events](../../../../../increasing-event.md),

$$
A\circ B=\{\omega:\exists K,L\subseteq\{e:\omega(e)=1\},\
K\cap L=\varnothing,\ \mathbf1_K\in A,\ \mathbf1_L\in B\}.
$$

The disjoint sets $K,L$ are open witnesses: fixing those [edges](../../../../../edge-of-a-graph.md) open forces the respective events whatever happens elsewhere. This is [disjoint occurrence of increasing events](../../../../../disjoint-occurrence-of-increasing-events.md). The [BK inequality](../../../../../van-den-berg-kesten-inequality.md) states that under the independent density-$p$ [product measure](../../../../../product-measure.md),

$$
\boxed{\mathbb P_p(A\circ B)\leq\mathbb P_p(A)\mathbb P_p(B)}.
$$

Disjoint occurrence means disjoint witnesses, not disjoint events.

Now take the lattice rectangle with width $2n$ and height $2n-1$. Make the dual bonds open exactly when the primal bonds they cross are closed. A primal open left-right crossing and a dual open top-bottom crossing cannot coexist: the two curves must intersect, requiring a bond and its crossing dual bond both to be open. Conversely, if no primal left-right crossing exists, the boundary separating vertices reachable from the left side from the right side contains a closed-bond dual top-bottom path. One obtains it by tracing the interface of the left-reachable set; it cannot terminate in the interior, and it separates the two vertical boundary sides. Thus exactly one of the two crossing events occurs.

For the precise dual dimensions, its vertices have coordinates

$$
x=\tfrac12,\tfrac32,\ldots,2n-\tfrac12,\qquad
y=-\tfrac12,\tfrac12,\ldots,2n-\tfrac12.
$$

The top and bottom rows are the terminals of dual [edges](../../../../../edge-of-a-graph.md) crossing the primal boundary horizontal bonds. Initially no horizontal bonds along these two terminal rows are needed. Adding independent density-$(1-p)$ horizontal bonds there does not change a top-bottom crossing event: an initial run along the top row can be removed by starting at its last vertex, and a final run along the bottom row can be removed similarly. The completed dual rectangle has width $2n-1$ and height $2n$. Rotate it through a right angle and translate it: its top-bottom crossing has exactly the law of the original left-right event at density $1-p$. Therefore

$$
\boxed{\mathbb P_p(A)+\mathbb P_{1-p}(A)=1},\qquad
\mathbb P_{1/2}(A)=\frac12.
$$

Write $R_n(v)=\{v\leftrightarrow\partial(v+[-n,n]^2)\}$ and $r_n=\mathbb P_{1/2}(R_n(0))$. This event is determined by finitely many bonds, since a path can be stopped on first hitting that boundary. On $A$, erase loops from a crossing path and choose a vertex $v=(n,y)$ where it meets the middle column. Its two portions run to the left and right boundary respectively, each reaching distance at least $n$ from $v$. Stop each portion at its first radius-$n$ boundary hit. The two portions have no common [edges](../../../../../edge-of-a-graph.md), giving disjoint witnesses for $R_n(v)$ twice. Hence

$$
A\subseteq\bigcup_{y=0}^{2n-1}\bigl(R_n((n,y))\circ R_n((n,y))\bigr).
$$

There are exactly $2n$ relevant middle-column vertices. The additional hinted vertex at $y=2n$ is outside this rectangle and need not be included. [Translation invariance](../../../../../translation-invariance.md), the [union bound](../../../../../boole-s-inequality.md) and the [BK inequality](../../../../../van-den-berg-kesten-inequality.md) yield

$$
\frac12\leq\sum_{y=0}^{2n-1}\mathbb P_{1/2}\bigl(R_n((n,y))\circ R_n((n,y))\bigr)
\leq2n\,r_n^2.
$$

The cluster radius is its maximum distance in the $\ell_\infty$ norm, taking value $\infty$ for an unbounded cluster; thus $R_n(0)=\{\operatorname{rad}(C)\geq n\}$. Taking square roots proves the [square-lattice one-arm lower bound from disjoint occurrence](../../../../../square-lattice-one-arm-lower-bound-from-disjoint-occurrence.md)

$$
\boxed{\mathbb P_{1/2}(\operatorname{rad}(C)\geq n)\geq\frac1{2\sqrt n}}\qquad(n\geq1).
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
