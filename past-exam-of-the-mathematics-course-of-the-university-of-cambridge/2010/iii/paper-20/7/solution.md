<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The exponent-two [Erdős-Rado theorem for pairs](../../../../../erdos-rado-theorem-for-pairs.md) says that for every infinite [cardinal](../../../../../cardinal-number.md) $\lambda$,

$$
\boxed{(2^\lambda)^+\longrightarrow(\lambda^+)^2_\lambda.}
$$

In particular, a finite or countable coloring of pairs from $(2^{\aleph_0})^+$ has an uncountable [monochromatic](../../../../../monochromatic-set.md) subset. We prove the general statement by an end-homogeneous tree construction.

Let $c:[\mu]^2\to\nu$ be any coloring on an [ordinal](../../../../../ordinal.md) $\mu$. Route a vertex $\beta$ through an increasing sequence of preceding vertices as follows. Start with the least vertex. After ancestors $a_\eta$, $\eta<\xi$, have been selected, choose the least remaining candidate $\gamma\leq\beta$, above those ancestors, satisfying

$$
c(\{a_\eta,\gamma\})=c(\{a_\eta,\beta\})\qquad(\eta<\xi).
$$

The terminal candidate $\beta$ always qualifies, so the procedure eventually reaches it. Candidate sets shrink and their least elements increase. If an intermediate candidate is $\gamma$, its route is precisely the earlier part of the route to $\beta$, because all earlier color tests agree. Consequently the routes define a [set-theoretic tree](../../../../../set-theoretic-tree.md) on the vertices.

Along a branch, the color from an ancestor to every later branch vertex is constant. Also a node of height $\alpha$ is determined by its sequence of $\alpha$ colors to its ancestors: reconstruct the ancestors as successive least candidates with those prescribed colors, then reconstruct the node as the least final candidate. Thus its level has at most $\nu^{|\alpha|}$ nodes.

Apply this with $\mu=(2^\lambda)^+$ and $\nu=\lambda$. If every node had height less than $\lambda^+$, each level would have size at most $\lambda^\lambda\leq2^\lambda$, and there would be at most $\lambda^+$ such levels. Their total size would be at most $2^\lambda$, contradicting $|\mu|=(2^\lambda)^+$. Hence some route has at least $\lambda^+$ ancestors. For each ancestor mark its constant color to all later route points. Since there are only $\lambda$ colors, one occurs on $\lambda^+$ ancestors. Those ancestors form the required [monochromatic](../../../../../monochromatic-set.md) set. This proves the theorem.

To make the [ordinal](../../../../../ordinal.md) function precise, one useful [ordinal partition-bound function](../../../../../ordinal-partition-bound-function.md) is

$$
f(\alpha)=\min\{\beta\geq\alpha:\text{for every nonzero cardinal }\nu<\alpha,\ \beta\longrightarrow(\alpha)^2_\nu\}.
$$

The target here is [ordinal](../../../../../ordinal.md) order type. For infinite $\alpha$, the proved theorem with $\lambda=|\alpha|$ supplies a bound $(2^\lambda)^+$: its homogeneous set has order type at least $\lambda^+>\alpha$, and it handles all the required color counts. Finite targets are handled by finite [Ramsey theorem](../../../../../ramsey-theorem.md) bounds. Thus $f$ is total, nondecreasing and $f(\alpha)\geq\alpha$.

Suppose a sequence of transfinite iterates $\alpha_{\xi+1}=f(\alpha_\xi)$, with suprema at limit stages, has supremum an uncountable [cardinal](../../../../../cardinal-number.md) $\kappa$ at a limit stage, with every earlier iterate below $\kappa$. Then

$$
\theta<\kappa\quad\Longrightarrow\quad f(\theta)<\kappa:
$$

choose an earlier iterate at least $\theta$ and use the next one as a bound. If the iteration has already stabilized, it has already found a fixed point instead.

This closure forces $\kappa$ to be a [strong limit cardinal](../../../../../strong-limit-cardinal.md). For any infinite $\lambda<\kappa$, color pairs of distinct binary strings of length $\lambda$ by their first differing coordinate. This uses $\lambda$ colors and has no [monochromatic](../../../../../monochromatic-set.md) triangle: three binary digits at one coordinate cannot be pairwise different. It gives a coloring on $2^\lambda$ with no homogeneous target of type $\lambda+1$. Since $\lambda$ colors are allowed when the target is the [ordinal](../../../../../ordinal.md) $\lambda+1$, we have

$$
2^\lambda<f(\lambda+1)<\kappa.
$$

Finite exponents satisfy the strong-limit requirement automatically for uncountable $\kappa$.

The needed additional condition is the [tree property](../../../../../tree-property.md): every tree of height $\kappa$, with nonempty levels of size less than $\kappa$, has a cofinal branch. In the present convention it forces $\kappa$ to be a [regular cardinal](../../../../../regular-cardinal.md). If $\kappa$ were singular, take a cofinal sequence of smaller [cardinals](../../../../../cardinal-number.md) of length $\operatorname{cf}(\kappa)$ and form the disjoint union of chains of those lengths. This tree has height and total size $\kappa$, levels of size at most $\operatorname{cf}(\kappa)<\kappa$, but no branch of length $\kappa$, a contradiction.

For any $\nu<\kappa$, apply the preceding color-routing tree to a coloring $[\kappa]^2\to\nu$. If a route already has length $\kappa$, use it. Otherwise its levels are indexed below $\kappa$ and each has size

$$
\nu^{|\alpha|}\leq2^{\nu\cdot|\alpha|}<\kappa
$$

for infinite exponents, by the strong-limit property; finite cases satisfy the same needed bound directly. The tree has $\kappa$ nodes, so regularity forces its height to be $\kappa$. The [tree property](../../../../../tree-property.md) supplies a cofinal branch. The ancestor-color partition of that branch has one class of size $\kappa$, since $\nu<\kappa$ and $\kappa$ is regular. Thus $\kappa\to(\kappa)^2_\nu$ for every $\nu<\kappa$, and

$$
\boxed{f(\kappa)=\kappa.}
$$

We have proved that an uncountable function-closed [cardinal](../../../../../cardinal-number.md) with the [tree property](../../../../../tree-property.md) is regular and strong limit, hence **strongly inaccessible**, and that it is the requested fixed point.

The paper's final sentence, read as a claim about the [tree property](../../../../../tree-property.md) alone, is false. Already $\aleph_0$ has it by the [König infinity lemma](../../../../../konig-s-lemma.md) but is not uncountable; even with uncountability stipulated, there are relative-consistency models with the [tree property](../../../../../tree-property.md) at $\aleph_2$. The latter counterexample is documented in [the research account of Mitchell forcing](https://scholar.harvard.edu/files/apoveda/files/210520.pdf). The rigorous conclusion in the iterated-function context is the one just proved: function closure supplies strong limit, and the [tree property](../../../../../tree-property.md) supplies regularity and a branch. Strong limit and regularity follow from distinct hypotheses in this context.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
