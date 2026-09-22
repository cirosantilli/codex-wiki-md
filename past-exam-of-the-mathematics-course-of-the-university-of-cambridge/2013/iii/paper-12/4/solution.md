<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In this enumeration problem, monotone means [subgraph-closed graph property](../../../../../subgraph-closed-graph-property.md): both deleting [vertices](../../../../../vertex-graph-theory.md) and deleting [edges](../../../../../edge-of-a-graph.md) preserve membership. This is a decreasing convention, rather than the increasing-edge convention often used for random-graph thresholds. Assume first that the property is proper and has [graphs](../../../../../graph-split.md) of arbitrarily large orders. These are the usual nondegenerate hypotheses for the formula.

Put $r+1=\min\{\chi(F):F\notin\mathcal Q\}$. Every [graph](../../../../../graph-split.md) of [chromatic number](../../../../../chromatic-number.md) at most $r$ belongs to $\mathcal Q$. In particular, all subgraphs of a fixed balanced [Turán graph](../../../../../turan-graph.md) $T_r(n)$ belong. Choosing each of its [edges](../../../../../edge-of-a-graph.md) independently as present or absent gives

$$
|\mathcal Q_n|\ge2^{t_r(n)}=2^{(1-1/r)\binom n2+O(n)}.
$$

For the upper bound, fix $F\notin\mathcal Q$ with $\chi(F)=r+1$. Every member of $\mathcal Q$ is $F$-free, by closure under subgraphs.

We use the following standard regularity consequences. For every sufficiently small regularity error $\eta$, large minimum cluster count $q_0$, and fixed positive density cutoff $d$, the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) gives an equitable partition into $q_0\le q\le M$ clusters and an exceptional set of at most $\eta n$ [vertices](../../../../../vertex-graph-theory.md), with at most $\eta q^2$ irregular pairs. The [graph embedding lemma for regular pairs](../../../../../graph-embedding-lemma-for-regular-pairs.md) says that a fixed [graph](../../../../../graph-split.md) with a prescribed proper colouring embeds into the corresponding clusters if all its required cross pairs are regular with density at least $d$, provided $\eta$ is sufficiently small relative to $d$ and the [graph](../../../../../graph-split.md). Hence the [reduced graph of a regularity partition](../../../../../reduced-graph-of-a-regularity-partition.md), joining regular pairs of density at least $d$, is $K_{r+1}$-free: such a [clique](../../../../../clique-graph-theory.md) would embed $F$.

By the [Turan theorem](../../../../../turan-s-theorem.md), this reduced [graph](../../../../../graph-split.md) has at most $(1-1/r)q^2/2$ [edges](../../../../../edge-of-a-graph.md). On its dense pairs allow arbitrary choices of original [edges](../../../../../edge-of-a-graph.md), giving at most $(1-1/r)n^2/2+O(n)$ free binary choices. All [edges](../../../../../edge-of-a-graph.md) within clusters, touching the exceptional set, or lying in irregular pairs contribute $O((\eta+1/q_0)n^2)$ further choices. On each remaining pair there are at most $d$ times its number of possible [edges](../../../../../edge-of-a-graph.md). The elementary [binary entropy](../../../../../binary-entropy.md) estimate

$$
\sum_{j\le dL}\binom Lj\le2^{H_2(d)L},\qquad H_2(d)=-d\log_2d-(1-d)\log_2(1-d),\quad 0<d<1/2,
$$

bounds the total sparse-pair contribution by $H_2(d)n^2/2$. The partition and pair classifications have at most $(M+1)^n2^{O(M^2)}$ descriptions, whose logarithm is $O(n)$ since $M$ is fixed. Choose $q_0$ large, then $d$ small, then $\eta$ sufficiently small; their total error can be made arbitrarily small. This proves

$$
\boxed{\log_2|\mathcal Q_n|=(1-1/r+o(1))\binom n2.}
$$

It is the [enumeration of subgraph-closed graph properties](../../../../../enumeration-of-subgraph-closed-graph-properties.md).

For the hereditary extension, a [hereditary graph property](../../../../../hereditary-graph-property.md) is closed under induced subgraphs. Define the [clique-independent partition class](../../../../../clique-independent-partition-class.md) $\mathcal C(a,b)$, for $0\le b\le a$, to consist of [graphs](../../../../../graph-split.md) partitionable into $a$ possibly empty classes, exactly $b$ designated as [cliques](../../../../../clique-graph-theory.md) and the other $a-b$ designated as independent sets; cross [edges](../../../../../edge-of-a-graph.md) are unrestricted. Thus $a$ is the total number of classes. The [colouring number of a hereditary graph property](../../../../../colouring-number-of-a-hereditary-graph-property.md) is

$$
r(\mathcal P)=\max\{a:\mathcal C(a,b)\subseteq\mathcal P\text{ for some }0\le b\le a\}.
$$

Use value zero if this set is empty, and infinity for the class of all [graphs](../../../../../graph-split.md).

**$r(\mathcal C(a,b))=a$ for $a\ge1$.** The lower bound follows from the definition. For the upper bound, fix any $s\in\{0,\ldots,a+1\}$ and a balanced partition of a large $N$-vertex set into $a+1$ classes with $s$ [clique](../../../../../clique-graph-theory.md) classes. Independent choices of cross [edges](../../../../../edge-of-a-graph.md) give $2^{(1-1/(a+1))N^2/2-O(1)}$ distinct [graphs](../../../../../graph-split.md) in $\mathcal C(a+1,s)$. On the other hand, all [graphs](../../../../../graph-split.md) in $\mathcal C(a,b)$ can be described by at most $a^N$ partitions, each with at most $(1-1/a)N^2/2$ unrestricted cross pairs. The former count is strictly larger for large $N$, so $\mathcal C(a+1,s)$ is not contained in $\mathcal C(a,b)$ for any $s$. A contained class with even more parts would contain one of these $(a+1)$-part classes by making unused parts empty, so it is also impossible.

The main changes for the [hereditary graph enumeration theorem](../../../../../hereditary-graph-enumeration-theorem.md) are as follows. The lower bound now uses a contained class $\mathcal C(r,b)$: within-class [edges](../../../../../edge-of-a-graph.md) are fixed as complete or empty, and the balanced cross pairs still give $(1-1/r)n^2/2-O(1)$ free [edge](../../../../../edge-of-a-graph.md) choices. For the upper bound, since no $\mathcal C(r+1,b)$ is wholly contained in $\mathcal P$, choose one forbidden induced [graph](../../../../../graph-split.md) $F_b\in\mathcal C(r+1,b)\setminus\mathcal P$ for each $b=0,\ldots,r+1$.

Use the standard [induced regularity template lemma](../../../../../induced-regularity-template-lemma.md): for a fixed finite forbidden induced family and any error tolerance, a regularity refinement gives bounded-size templates with internal [clique](../../../../../clique-graph-theory.md)/independent types and cross pairs classified as sparse, almost complete, or intermediate. A [clique](../../../../../clique-graph-theory.md) of intermediate pairs on $a$ classes realizes every fixed induced pattern consistent with the internal types of those classes. This induced embedding conclusion uses a Ramsey refinement within clusters and regularity for both [edges](../../../../../edge-of-a-graph.md) and nonedges; the total exceptional-pair cost can be made arbitrarily small. Applied to the $F_b$, a [clique](../../../../../clique-graph-theory.md) on $r+1$ intermediate classes would realize the forbidden $F_b$ whose number of [clique](../../../../../clique-graph-theory.md) types is $b$. Thus the [graph](../../../../../graph-split.md) of intermediate pairs is $K_{r+1}$-free. Only intermediate pairs contribute unrestricted binary choices; sparse pairs and the missing [edges](../../../../../edge-of-a-graph.md) in almost-complete pairs each have the same entropy bound as before. The [Turan theorem](../../../../../turan-s-theorem.md) and the earlier counting argument now give

$$
\boxed{|\mathcal P_n|=2^{(1-1/r+o(1))\binom n2},\qquad r=r(\mathcal P).}
$$

This formula assumes $1\le r<\infty$. For the universal property the count is exactly $2^{\binom n2}$; a hereditary property of bounded order has $r=0$ and has no [graphs](../../../../../graph-split.md) on sufficiently large [vertex](../../../../../vertex-graph-theory.md) sets, so the displayed expression with $1/r$ is not applicable.

For a proper [subgraph-closed graph property](../../../../../subgraph-closed-graph-property.md), any contained $\mathcal C(a,b)$ must have $b=0$: if $b\ge1$, it contains arbitrarily large complete [graphs](../../../../../graph-split.md), and closure under subgraphs would force every [graph](../../../../../graph-split.md) into the property. Consequently its colouring number is exactly one less than the least chromatic number of an excluded [graph](../../../../../graph-split.md). The excluded family of an intersection is the union of the two excluded families, whose minimum chromatic number is the smaller of their minima. Therefore **$r(\mathcal P\cap\mathcal Q)=\min(r(\mathcal P),r(\mathcal Q))$ for subgraph-closed properties**, with the universal case treated by $r=\infty$.

For hereditary properties take $\mathcal P=\mathcal C(2,0)$ and $\mathcal Q=\mathcal C(2,2)$, both of colouring number two. A [graph](../../../../../graph-split.md) in their intersection is both bipartite and a union of two [cliques](../../../../../clique-graph-theory.md). A [clique](../../../../../clique-graph-theory.md) in a bipartite [graph](../../../../../graph-split.md) has at most two [vertices](../../../../../vertex-graph-theory.md); hence every such [graph](../../../../../graph-split.md) has at most four [vertices](../../../../../vertex-graph-theory.md). The intersection contains no complete clique-independent class on arbitrarily large orders, so **$r(\mathcal P\cap\mathcal Q)=0<2$**. This also demonstrates why the bounded-order exception to the enumeration formula is necessary.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
