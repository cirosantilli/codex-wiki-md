<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\theta\to(\eta)^r_\lambda$ when every $\lambda$-coloring of the $r$-element subsets of $\theta$ has a homogeneous subset of order type $\eta$. The [Erdős-Rado theorem for pairs](../../../../../../erdos-rado-theorem-for-pairs.md) states, for infinite $\lambda$,

$$
\boxed{(2^\lambda)^+\longrightarrow(\lambda^+)^2_\lambda.}
$$

In particular a countable-color partition of pairs from $(2^{\aleph_0})^+$ has an uncountable [homogeneous set](../../../../../../homogeneous-set-for-a-colouring.md). The standard [Erdős-Rado theorem for finite arities](../../../../../../erdos-rado-theorem-for-finite-arities.md) is

$$
\beth_r(\lambda)^+\longrightarrow(\lambda^+)^{r+1}_\lambda,
\qquad \beth_0(\lambda)=\lambda,\quad\beth_{r+1}(\lambda)=2^{\beth_r(\lambda)}.
$$

We prove it, including the pair case, by constructing an [end-homogeneous routing tree](../../../../../../end-homogeneous-routing-tree.md).

For a coloring $c:[\theta]^{r+1}\to\lambda$, $r\ge1$, route each vertex $\beta<\theta$ as follows. Given its previously selected increasing ancestors, choose the least $\gamma\leq\beta$ greater than all those ancestors such that

$$
c(s\cup\{\gamma\})=c(s\cup\{\beta\})
\quad\text{for every }r\text{-subset }s\text{ of those ancestors}.
$$

The candidate $\beta$ always qualifies. Select it and stop if it is the minimum; otherwise add the selected $\gamma$ to the ancestors and continue, including at limit stages. The ancestors are strictly increasing below $\beta$, so the process must stop. If a selected ancestor $\gamma$ is routed separately, its earlier path is the same: its color constraints agree with those of $\beta$ and the same least choices are forced. Thus the paths define a tree order on the vertices.

A node at depth $\alpha$ is determined by the table of its colors on the $r$-subsets of its ancestors. Given the table on $[\alpha]^r$, recursively take the least compatible candidate at each depth; at a limit depth use all preceding constraints. This recovers both the path and its final node. Therefore

$$
|T_\alpha|\leq\lambda^{|[\alpha]^r|}.
$$

Along any branch, once an $r$-tuple $s$ of ancestors is fixed, the color $c(s\cup\{\beta\})$ is independent of all subsequent choices of $\beta$ on that branch. This is exactly end-homogeneity.

For the pair case take $r=1$ and $\theta=(2^\lambda)^+$. If all node depths were below $\lambda^+$, then each level would have size at most $\lambda^\lambda\leq2^\lambda$, and the union of $\lambda^+$ levels would have size at most $2^\lambda$. This contradicts the number of vertices. Hence some node has at least $\lambda^+$ ancestors. On that branch assign to each ancestor its constant color to all later ancestors. Regularity of $\lambda^+$ implies that one of the $\lambda$ colors occurs $\lambda^+$ times, giving the desired [homogeneous set](../../../../../../homogeneous-set-for-a-colouring.md). Its increasing enumeration has a subsequence of order type $\lambda^+$.

For the higher-arity induction let $\mu=\beth_{r-1}(\lambda)$, so $\theta=(2^\mu)^+$. At depths below $\mu^+$ the same bound is at most $\lambda^\mu\leq2^\mu$, forcing a branch of length $\mu^+$. End-homogeneity defines a coloring $d$ of its $r$-tuples by the common color of adjoining a later branch vertex. The previous-arity theorem gives a subset of order type $\lambda^+$ homogeneous for $d$, and every $(r+1)$-tuple from it then has the same color under $c$. The base case $r=0$ is the infinite pigeonhole principle at $\lambda^+$. This proves the full finite-arity statement.

One suitable [ordinal partition-bound function](../../../../../../ordinal-partition-bound-function.md) is

$$
f(\alpha)=\min\{\beta\geq\alpha:\ \forall\text{ nonzero cardinals }\nu<\alpha,
\ \beta\to(\alpha)^2_\nu\}.
$$

It is nondecreasing and $f(\alpha)\geq\alpha$. It is total: choose an infinite [cardinal](../../../../../../cardinal-number.md) $\lambda\geq|\alpha|$; the pair theorem supplies a homogeneous subset of size $\lambda^+$ for every allowed color number, and its order type contains a copy of $\alpha$. Thus $(2^\lambda)^+$ is a bound in the displayed minimum.

Let an uncountable [cardinal](../../../../../../cardinal-number.md) $\kappa$ be the supremum of a cofinal increasing sequence of iterates of $f$, with each iterate and its successor still below $\kappa$. For every $\xi<\kappa$, monotonicity and some later iterate give $f(\xi)<\kappa$. Thus the relevant consequence of being such a supremum is

$$
f``\kappa\subseteq\kappa.
$$

If the iteration already reaches a fixed point, its constant continuation of course has that fixed point as supremum as well. A strictly increasing countable iteration instead has a countable-cofinality supremum and cannot satisfy the uncountable regular tree-property condition below; one must not assume existence of the extra condition from iteration alone.

Here closure under $f$ forces a strong-limit bound. For infinite $\lambda<\kappa$, color distinct binary strings in $2^\lambda$ by their first differing coordinate. Three strings cannot have all three first-difference coordinates equal, because there are only two bit values at that coordinate. Hence this $\lambda$-coloring has no homogeneous triangle, and in particular no homogeneous subset of order type $\lambda+1$. Therefore

$$
f(\lambda+1)>2^\lambda.
$$

Since $\lambda+1<\kappa$ and $f(\lambda+1)<\kappa$, it follows that **$2^\lambda<\kappa$ for every $\lambda<\kappa$**.

Now impose the [tree property](../../../../../../tree-property.md): every tree of height $\kappa$, with nonempty levels of size below $\kappa$, has a cofinal branch. If this definition is extended to singular [cardinals](../../../../../../cardinal-number.md), it also forces regularity. For a singular $\kappa$, take disjoint chains of lengths cofinal in $\kappa$, one for each index below $\operatorname{cf}\kappa$. Every level has at most $\operatorname{cf}\kappa<\kappa$ nodes and the height is $\kappa$, but each branch remains in one shorter chain. A common new root may be added if [rooted trees](../../../../../../rooted-tree.md) are required. Under the more usual convention the [tree property](../../../../../../tree-property.md) is only defined at regular uncountable [cardinals](../../../../../../cardinal-number.md), so regularity is part of the convention instead.

For a coloring $c:[\kappa]^2\to\nu$ with $\nu<\kappa$, the routing tree has levels of size at most $\nu^{|\alpha|}<\kappa$ by the strong-limit property. If some node has height at least $\kappa$, there is already an end-homogeneous branch of that length. Otherwise the tree has height exactly $\kappa$: a smaller number of levels of size below $\kappa$ could not contain its $\kappa$ nodes, by regularity. The [tree property](../../../../../../tree-property.md) then supplies a cofinal branch. Along it, one of the fewer than $\kappa$ ancestor colors occurs $\kappa$ times, again by regularity. Thus $\kappa\to(\kappa)^2_\nu$ for every $\nu<\kappa$, giving

$$
\boxed{f(\kappa)=\kappa.}
$$

Moreover the closure argument gives strong limit and the tree argument gives regularity. Thus **an uncountable $f$-closed [cardinal](../../../../../../cardinal-number.md) with the [tree property](../../../../../../tree-property.md) is strongly inaccessible**.

The final printed assertion requires that qualification. The ordinary [tree property](../../../../../../tree-property.md) alone does not imply strong inaccessibility. At $\omega$ it is König's infinity lemma and $\omega$ is not uncountable. Even when the convention excludes $\omega$, there are relative-consistency models in which $\aleph_2$ has the [tree property](../../../../../../tree-property.md), although a [successor cardinal](../../../../../../successor-cardinal.md) is never strongly inaccessible; this result is recalled in [the introduction of Friedman, Honzik and Stejskalová](https://www.logic.univie.ac.at/~dsyfriedman/papers/joint.radek.sarka.aleph-omega.pdf). No proof of the bare implication is possible under that standard definition. The preceding paragraphs prove the corrected implication in the actual $f$-closure setting and the requested fixed-point conclusion, without silently replacing [tree property](../../../../../../tree-property.md) by weak [compactness](../../../../../../compact-space.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
