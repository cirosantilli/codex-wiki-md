<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**There is a genuine error in the printed threshold.** With $\ell=3$, its only nontrivial requirement is that some two consecutive classes contain at least one vertex of the triple. Every triple meets some class, so every triple qualifies. For example, when $r=4$, the printed construction is the complete 3-uniform [hypergraph](../../../../../hypergraph-split.md), of edge density $1$, whereas the claimed density is $(2/4)^2=1/4$. Thus the stated edge-count assertion is false even in a nondegenerate parameter range.

The intended [cyclic Turán covering construction](../../../../../cyclic-turan-covering-construction.md), which gives the claimed density and the stated lower bound, uses threshold $k+1$, in the natural range $2\le\ell\le r+1$. We solve this repaired version explicitly. Denote it by $G^+$ to keep it separate from the literal printed construction.

**A cyclic prefix argument gives the covering property.** We first prove the relevant [cycle lemma](../../../../../cycle-lemma.md). If integers $b_1,\ldots,b_m$ satisfy $\sum_i b_i=1$, exactly one cyclic starting position has every nonempty partial sum strictly positive. Existence follows by starting after the last minimum among the proper partial sums $0,b_1,\ldots,b_1+\cdots+b_{m-1}$. Subsequent nonwrapped sums are strictly above that minimum, and wrapped sums add the total $1$. For uniqueness, if two starts split the cycle into arcs with sums $x$ and $1-x$, both positive, their integrality would require $x\ge1$ and $1-x\ge1$, a contradiction.

Take any $r+1$ vertices and let $a_i$ count them in class $V_i$. The increments $b_i=a_i-1$ sum to one. The [cycle lemma](../../../../../cycle-lemma.md) gives a start for which the first $k$ classes contain at least $k+1$ vertices, for every $1\le k\le r$. Take the first $\ell$ vertices encountered from that start in class order. The first $\ell-1$ classes already contain at least $\ell$ vertices; the chosen vertices therefore satisfy all the repaired prefix inequalities. Hence

$$
\boxed{\text{Every }(r+1)\text{-set contains an edge of }G^+.}
$$

Every repaired edge also satisfies the weaker printed inequalities. Thus this argument proves the covering assertion for the printed construction too, although it cannot repair its false edge count.

**Count the repaired edges by labelled class assignments.** Put $m=\ell-1$. For a fixed cyclic start, an edge satisfying the repaired inequalities has all $\ell$ vertices in its first $m$ classes. Assign $\ell$ labelled vertices to these $m$ positions. There are $m^\ell$ assignments in total. Their occupancy counts $a_1,\ldots,a_m$ satisfy $\sum_i(a_i-1)=1$; the [cycle lemma](../../../../../cycle-lemma.md) says exactly one of their $m$ cyclic starts has the required prefixes. Rotational symmetry therefore gives exactly $m^{\ell-1}$ good assignments for a specified start.

We must check that summing over the $r$ starts does not count an edge twice. Suppose two starts cut the circle into arcs of lengths $h$ and $r-h$. If an arc has length at most $m$, goodness of its starting point forces that arc to contain at least its length plus one vertices. If its length is greater than $m$, it contains all $\ell$ vertices, while the other good start demands vertices in the disjoint complementary arc, impossible. If both lengths are at most $m$, their combined demand is at least $r+2>\ell$ vertices, again impossible. Thus a repaired edge has a unique good start.

There are consequently $r m^{\ell-1}$ good assignments of class labels to $\ell$ labelled vertices. For any such assignment, balanced class sizes give

$$
\prod_i(|V_i|)_{a_i}=(n/r)^\ell+O(n^{\ell-1}),
$$

where $(x)_a$ is the [falling factorial](../../../../../falling-factorial.md). Divide the total count of ordered distinct vertices by $\ell!$. For fixed $\ell,r$,

$$
\boxed{e(G^+)=\left(\frac{\ell-1}{r}\right)^{\ell-1}\binom n\ell+O(n^{\ell-1})
=(1+o(1))\left(\frac{\ell-1}{r}\right)^{\ell-1}\binom n\ell.}
$$

This is precisely the edge density requested, but for the corrected construction.

**Pass from covering to a forbidden-[hypergraph clique](../../../../../complete-uniform-hypergraph.md) construction.** Use $r-1$ balanced classes in $G^+$ and take its [hypergraph complement](../../../../../hypergraph-complement.md). Every $r$-set contains an edge of $G^+$, so the complement contains no complete $\ell$-uniform [hypergraph](../../../../../hypergraph-split.md) $K_r^\ell$. The preceding count gives

$$
\boxed{\pi(K_r^\ell)\ge1-\left(\frac{\ell-1}{r-1}\right)^{\ell-1},\qquad r\ge\ell.}
$$

Here [Turán density](../../../../../turan-density.md) means $\pi(F)=\lim_{n\to\infty}\operatorname{ex}(n,F)/\binom n\ell$ for a fixed $\ell$-uniform forbidden [hypergraph](../../../../../hypergraph-split.md); the limit exists because these normalized extremal densities are nonincreasing under averaging over smaller vertex subsets.

A corresponding classical upper bound is the [de Caen bound for hypergraph Turán density](../../../../../de-caen-bound-for-hypergraph-turan-density.md):

$$
\boxed{\pi(K_r^\ell)\le1-\frac1{\binom{r-1}{\ell-1}}.}
$$

Equivalently, an $\ell$-uniform covering [hypergraph](../../../../../hypergraph-split.md) in which every $r$-set contains an edge has asymptotic edge density at least $1/\binom{r-1}{\ell-1}$. Its proof recursively counts complete subhypergraphs by their one-vertex extensions. [Double counting](../../../../../double-counting-proof-technique.md) the extensions and applying the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to common extension neighbourhoods gives a lower bound for the ratio of successive [hypergraph clique](../../../../../complete-uniform-hypergraph.md) counts. If the missing-edge density were smaller than $1/\binom{r-1}{\ell-1}$, those bounds would force a positive number of $r$-vertex [hypergraph cliques](../../../../../complete-uniform-hypergraph.md), a contradiction. Applying the resulting covering bound to the complement of a $K_r^\ell$-free [hypergraph](../../../../../hypergraph-split.md) gives the displayed upper bound. This incidence argument supplies the extra factor beyond the simpler direct count of one covering edge in each $r$-set, which alone yields only $1-1/\binom r\ell$.

The lower bound is therefore valid via $G^+$, while **the printed enumeration cannot be proved with threshold $k-1$**. Both the counterexample and the necessary repair are part of the solution, rather than a silent change of the definition.

The general upper bound is recorded, for example, in [Turán densities of some hypergraphs related to complete uniform hypergraphs](https://math.gsu.edu/yzhao6/TuranBBBZ.pdf).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
