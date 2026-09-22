<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Tychonoff theorem](../../../../../../tychonoff-s-theorem.md) states that an arbitrary product of [compact spaces](../../../../../../compact-space.md), with the [product topology](../../../../../../product-topology.md), is compact; no [Hausdorff](../../../../../../hausdorff-space.md) hypothesis is necessary. We prove it using [Zorn's lemma](../../../../../../zorn-s-lemma.md) and the [axiom of choice](../../../../../../axiom-of-choice.md).

First, every proper [filter on a set](../../../../../../filter-set-theory.md) extends to an [ultrafilter](../../../../../../ultrafilter.md). Order its proper extensions by inclusion. The union of a chain is again a proper filter: any finite collection of its members occurs in one member of the chain, and the empty set occurs in none. [Zorn's lemma](../../../../../../zorn-s-lemma.md) gives a maximal proper filter $\mathcal U$. If $A\notin\mathcal U$, adjoining $A$ must destroy properness, so some $F\in\mathcal U$ has $F\cap A=\varnothing$, and hence $X\setminus A\in\mathcal U$. This proves the decision property of an [ultrafilter](../../../../../../ultrafilter.md).

Next prove the [ultrafilter characterization of compactness](../../../../../../ultrafilter-characterization-of-compactness.md). In a [compact space](../../../../../../compact-space.md) the [closed sets](../../../../../../closed-set.md) $\overline F$, for $F\in\mathcal U$, have the [finite intersection property](../../../../../../finite-intersection-property.md), so their intersection contains a point $x$. Every open neighbourhood $O$ of $x$ belongs to $\mathcal U$: otherwise its closed complement belongs to $\mathcal U$ and contains $x$, a contradiction. Thus the ultrafilter converges to $x$. Conversely, if an open cover has no finite subcover, the closed complements have the [finite intersection property](../../../../../../finite-intersection-property.md) and generate a proper filter. Extend it to an ultrafilter. A limit point lies in some member $O$ of the cover, so both $O$ and its complement would belong to the ultrafilter. This is impossible. These arguments also prove the closed-set form of [compactness](../../../../../../compact-space.md) directly by taking complements.

Now let $X=\prod_{j\in J}X_j$. If a factor is empty, the product is empty and compact. Otherwise the [axiom of choice](../../../../../../axiom-of-choice.md) makes $X$ nonempty. For an [ultrafilter](../../../../../../ultrafilter.md) $\mathcal U$ on $X$, its coordinate image

$$
\mathcal U_j=\{A\subseteq X_j:\pi_j^{-1}(A)\in\mathcal U\}
$$

is an ultrafilter. [Compactness](../../../../../../compact-space.md) of $X_j$ supplies at least one limit $x_j$; use the [axiom of choice](../../../../../../axiom-of-choice.md) to choose one for every $j$. A basic open neighbourhood of $x=(x_j)_j$ restricts finitely many coordinates. Each corresponding inverse image belongs to $\mathcal U$, so their finite intersection also does. Hence $\mathcal U$ converges to $x$ in the [product topology](../../../../../../product-topology.md). The ultrafilter criterion proves the theorem. The explicit choices and the maximal-filter argument are exactly the places where choice enters.

The [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) states that the closed [unit ball](../../../../../../unit-ball.md) of the [continuous dual space](../../../../../../continuous-dual-space-split.md) $V^*$ of a real or complex [normed vector space](../../../../../../normed-vector-space.md) $V$ is compact in the [weak-star topology](../../../../../../weak-star-topology.md) $\sigma(V^*,V)$. Completeness of $V$ is not required.

For each $v\in V$, let $D_v=\{z\in\mathbb K:|z|\leq\|v\|\}$, a compact scalar disk or interval. By the [Tychonoff theorem](../../../../../../tychonoff-s-theorem.md), $P=\prod_{v\in V}D_v$ is compact. Inside $P$, impose the equations

$$
z_{u+v}=z_u+z_v,\qquad z_{\alpha v}=\alpha z_v
\quad(u,v\in V,\ \alpha\in\mathbb K).
$$

Each equation defines a closed subset, since it concerns continuous coordinate projections into a [Hausdorff](../../../../../../hausdorff-space.md) scalar [field](../../../../../../field.md). Their intersection $K$ is therefore compact. A point in $K$ defines a [linear functional](../../../../../../linear-functional.md) $\ell(v)=z_v$, and the coordinate bounds give $|\ell(v)|\leq\|v\|$. Conversely, every $\ell\in V^*$ with $\|\ell\|\leq1$ gives such a point. Thus $K$ is exactly the image of the dual [unit ball](../../../../../../unit-ball.md) under $\ell\mapsto(\ell(v))_{v\in V}$. The induced [product topology](../../../../../../product-topology.md) is precisely pointwise convergence on $V$, which is the [weak-star topology](../../../../../../weak-star-topology.md). This proves

$$
\boxed{\{\ell\in V^*:\|\ell\|\leq1\}\text{ is weak-star compact}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
