<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

View a [set family](../../../../../set-family.md) as a set of vertices of the [Boolean lattice](../../../../../boolean-lattice.md). The operation $D_i$ acts independently on each pair $\{S,S\cup\{i\}\}$, where $i\notin S$: it keeps a full or empty pair and moves a sole upper member down. Thus [downward coordinate compression](../../../../../downward-coordinate-compression.md) preserves [cardinality](../../../../../cardinality.md).

Fix a tracing set $Y$. If $i\notin Y$, compression leaves the [trace of a set family](../../../../../trace-of-a-set-family.md) on $Y$ unchanged. If $i\in Y$, write $B_0,B_1\subseteq\mathcal P(Y\setminus\{i\})$ for the two sections of the old trace, according to absence or presence of $i$. The absent-$i$ section of the new trace is $B_0\cup B_1$. Its present-$i$ section is contained in $B_0\cap B_1$: an upper member survives only when its lower partner was also present in the original family. Consequently

$$
\boxed{|(D_i\mathcal F)_{|Y}|\leq|B_0\cup B_1|+|B_0\cap B_1|=|B_0|+|B_1|=|\mathcal F_{|Y}|.}
$$

In particular, [downward coordinate compression](../../../../../downward-coordinate-compression.md) cannot create new [set shattering](../../../../../set-shattering.md).

Repeatedly apply any changing [downward coordinate compression](../../../../../downward-coordinate-compression.md). Each change strictly decreases $\sum_{A\in\mathcal F}|A|$, so the process terminates at a [down-set](../../../../../down-set.md) $\mathcal D$ with the same [cardinality](../../../../../cardinality.md) and with no larger trace on any $Y$. The [Sauer-Shelah lemma](../../../../../sauer-shelah-lemma.md) says that a family shattering no $k$-element set satisfies

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^{k-1}\binom nj\qquad(1\leq k\leq n).}
$$

Indeed, the compressed [down-set](../../../../../down-set.md) also shatters no $k$-element set. If it contained any member of size at least $k$, all subsets of a $k$-subset of that member would belong to the [down-set](../../../../../down-set.md), contradicting this restriction. Every member therefore has size at most $k-1$, giving the bound. Equivalently, [VC dimension](../../../../../vc-dimension.md) at most $d$ gives size at most $\sum_{j=0}^d\binom nj$. The family of all sets of size at most $d$ attains this bound.

There is a different extremal example when $n\geq3$. Toggle a fixed coordinate in the family of sets of size at most two:

$$
\boxed{\mathcal F=\{B\mathbin\triangle\{1\}:B\subseteq[n],\ |B|\leq2\}.}
$$

The [symmetric difference](../../../../../symmetric-difference.md) is a bijection, so this family has $1+n+\binom n2$ members. On each tracing set $Y$, it simply toggles coordinate $1$ if $1\in Y$; thus it preserves trace [cardinality](../../../../../cardinality.md) and [set shattering](../../../../../set-shattering.md). A triple has seven trace patterns, not eight. The new family differs from the original one because it contains $\{1,2,3\}$. For $n\leq2$ the specified [cardinality](../../../../../cardinality.md) is $2^n$, so the entire [power set](../../../../../power-set.md) is the unique family of that size; the different example requires $n\geq3$.

For the final bound, let $e_i(\mathcal F)$ count pairs $S,S\cup\{i\}$ both in the family. Deleting coordinate $i$ identifies precisely these pairs, so

$$
|\mathcal F_{|[n]\setminus\{i\}}|=|\mathcal F|-e_i(\mathcal F).
$$

Suppose every deletion lost at least two members, so $e_i(\mathcal F)\geq2$ for every $i$. The trace inequality and preservation of [cardinality](../../../../../cardinality.md) show that $e_i(\mathcal D)\geq e_i(\mathcal F)$ after [downward coordinate compression](../../../../../downward-coordinate-compression.md). The [down-set](../../../../../down-set.md) $\mathcal D$ contains the empty set and every singleton. For each $i$, its second edge in direction $i$ has an upper endpoint of size at least two. Downward closure then supplies a pair $\{i,j\}\in\mathcal D$. The pairs in $\mathcal D$ therefore cover all $n$ coordinates, so at least $\lceil n/2\rceil$ pairs are needed. This proves [two cube edges in every direction force many vertices](../../../../../two-cube-edges-in-every-direction-force-many-vertices.md):

$$
|\mathcal F|=|\mathcal D|\geq1+n+\lceil n/2\rceil=\lceil3n/2\rceil+1.
$$

Taking the contrapositive gives the required answer:

$$
\boxed{|\mathcal F|\leq\lceil3n/2\rceil\ \Longrightarrow\ \exists i:\ |\mathcal F_{|[n]\setminus\{i\}}|\geq|\mathcal F|-1.}
$$

The threshold is sharp for every $n\geq2$. Take the empty set, all singletons and $\lceil n/2\rceil$ pairs covering every coordinate. For even $n$, use the disjoint pairs $12,34,\ldots,(n-1)n$; for odd $n$, pair the first $n-1$ coordinates and add $(n-1)n$. This [down-set](../../../../../down-set.md) has exactly $\lceil3n/2\rceil+1$ members and at least two edges in every direction, so every $(n-1)$-coordinate trace has size at most $|\mathcal F|-2$. Adding further members preserves those pairs and therefore preserves the failure whenever a larger [cardinality](../../../../../cardinality.md) is feasible. For $n=1$, the putative counterexample [cardinality](../../../../../cardinality.md) is three, exceeding the size of the [Boolean lattice](../../../../../boolean-lattice.md); the sharpness construction naturally starts at $n=2$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
