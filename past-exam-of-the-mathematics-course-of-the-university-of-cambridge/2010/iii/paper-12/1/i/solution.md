<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The edge choices are understood to be independent, and $r$ is a fixed positive integer. We prove the [hypergraph extension property](../../../../../../hypergraph-extension-property.md) and then show directly that it determines a unique countable [hypergraph isomorphism](../../../../../../hypergraph-isomorphism.md) type.

For a finite $S\subseteq\mathbb N$, prescribe a family $\mathcal A\subseteq\binom S{r-1}$. We want a new [vertex](../../../../../../vertex-graph-theory.md) $v$ such that

$$
F\cup\{v\}\text{ is a hyperedge}\quad\Longleftrightarrow\quad F\in\mathcal A,
\qquad F\in\binom S{r-1}.
$$

For any $v\notin S$, the [probability](../../../../../../probability.md) of precisely this pattern in the [countable random uniform hypergraph](../../../../../../countable-random-uniform-hypergraph.md) is

$$
q=p^{|\mathcal A|}(1-p)^{\binom{|S|}{r-1}-|\mathcal A|}>0.
$$

Two different candidate vertices use disjoint [hyperedge](../../../../../../hyperedge.md) decisions: all the other vertices in each tested edge lie in $S$. The successes are therefore [independent random variables](../../../../../../independent-random-variables.md) with the same positive [probability](../../../../../../probability.md) $q$. The [probability](../../../../../../probability.md) that the first $N$ candidates all fail is $(1-q)^N\to0$. The same argument after discarding any finite initial set of candidates shows that infinitely many witnesses exist [almost surely](../../../../../../almost-sure-convergence.md).

There are only countably many finite subsets of $\mathbb N$, and finitely many prescriptions for each. A countable union of null events is null. Consequently the random [uniform hypergraph](../../../../../../uniform-hypergraph.md) satisfies every such extension prescription simultaneously [almost surely](../../../../../../almost-sure-convergence.md).

Now let $H$ and $K$ be two countably infinite $r$-[uniform hypergraphs](../../../../../../uniform-hypergraph.md) with the [hypergraph extension property](../../../../../../hypergraph-extension-property.md). Enumerate their [vertex sets](../../../../../../vertex-set.md) and construct increasing finite partial [hypergraph isomorphisms](../../../../../../hypergraph-isomorphism.md) by the [back-and-forth method](../../../../../../back-and-forth-method.md). At a forward step, take the least unused vertex $u$ of $H$. Its incident [hyperedges](../../../../../../hyperedge.md) with each $(r-1)$-subset of the current domain specify a pattern on the matched vertices of $K$. The [hypergraph extension property](../../../../../../hypergraph-extension-property.md) supplies an unused vertex $v$ of $K$ with exactly this pattern. Adding $u\mapsto v$ preserves and reflects every [hyperedge](../../../../../../hyperedge.md) in the enlarged domain. At the next step, take the least unused vertex of $K$ and perform the identical construction with $H$ and $K$ interchanged.

The union of the finite maps is defined on every vertex and has every vertex in its range. It is a [bijection](../../../../../../bijection.md), and each finite $r$-set appears at some finite stage, so all [hyperedges](../../../../../../hyperedge.md) and nonedges are preserved. Thus it is a [hypergraph isomorphism](../../../../../../hypergraph-isomorphism.md). Existence of at least one structure with the property follows from the probability-one construction already proved; fix one representative and call it $G^{(r)}_{\mathrm{univ}}$. Therefore

$$
\boxed{G^{(r)}_{\mathbb N,p}\cong G^{(r)}_{\mathrm{univ}}\quad\text{almost surely},\qquad0<p<1.}
$$

The [hypergraph isomorphism](../../../../../../hypergraph-isomorphism.md) type does not depend on $p$. In the case $r=2$ it is the [Rado graph](../../../../../../rado-graph.md). For $r=1$, the argument says that the infinitely many selected and unselected singleton vertices determine the same one-uniform structure for every $p\in(0,1)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
