<h1 id="14f/solution">Solution</h1>

↑ **Parent:** [14F](../14f.md)

A [basis of a topology](../../../../../basis-of-a-topology.md) is a family $\mathcal B$ of open sets such that every open set is a union of members of $\mathcal B$. Equivalently, whenever $x\in U$ and $U$ is open, there is $B\in\mathcal B$ with $x\in B\subseteq U$. For a [metric space](../../../../../metric-space.md), all open balls form a basis. For the [product topology](../../../../../product-topology.md) on $X\times Y$, the rectangles $U\times V$ with $U,V$ open in their respective factors form a basis; rectangles made from factor bases also suffice.

If $C\subseteq X$ and $D\subseteq Y$ are countable [dense subsets](../../../../../dense-set.md), then $C\times D$ is countable. Every nonempty basic rectangle meets it, since $U\cap C$ and $V\cap D$ are nonempty. Every nonempty open set contains such a rectangle, proving that **a product of two separable spaces is separable**.

Suppose a [metric space](../../../../../metric-space.md) has a countable dense set $C$. The balls $B(c,r)$ with $c\in C$ and positive rational $r$ form a countable basis. Indeed, given $x\in U$ open, choose $\epsilon>0$ with $B(x,\epsilon)\subseteq U$, then choose $c\in C$ with $d(c,x)<\epsilon/3$ and rational $r$ satisfying

$$
d(c,x)<r<\epsilon-d(c,x).
$$

The triangle inequality gives $x\in B(c,r)\subseteq B(x,\epsilon)\subseteq U$. Conversely, from any countable basis select one point of each nonempty member. These points form a countable [dense subset](../../../../../dense-set.md), because every nonempty open set contains a basis member. This direction holds for arbitrary topological spaces. Thus a [metric space](../../../../../metric-space.md) is separable exactly when it is a [second-countable space](../../../../../second-countable-space.md). Intersecting a countable basis with a subspace gives a countable basis for its [subspace topology](../../../../../subspace-topology.md); selecting points as above shows that **every subspace of a separable metric space is separable**.

For the [Sorgenfrey line](../../../../../lower-limit-topology.md), $\mathbb Q$ meets every nonempty interval $[a,b)$, so it is a countable [dense subset](../../../../../dense-set.md). In the [Sorgenfrey plane](../../../../../sorgenfrey-plane.md), however, for any $x\in\mathbb R$ and $\epsilon>0$,

$$
\bigl([x,x+\epsilon)\times[-x,-x+\epsilon)\bigr)\cap Y=\{(x,-x)\}.
$$

Indeed, $(t,-t)$ in that rectangle requires both $t\geq x$ and $t\leq x$. Every singleton is therefore open in the [subspace topology](../../../../../subspace-topology.md) on $Y$, which is the [discrete topology](../../../../../discrete-space.md). A dense subset of a discrete space must contain every point. Since $Y$ is in bijection with the uncountable set $\mathbb R$, it has no countable dense subset. Hence **$X$ is separable and $Y$ is not separable**, illustrating why the metric assumption in the inheritance statement matters.

## ↑ Ancestors (10)

1. [14F](../14f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
