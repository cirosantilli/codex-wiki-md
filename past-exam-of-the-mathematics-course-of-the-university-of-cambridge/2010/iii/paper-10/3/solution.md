<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An $r$-[uniform hypergraph](../../../../../uniform-hypergraph.md) is [strongly saturated with respect to a complete uniform hypergraph](../../../../../strong-saturation-of-a-uniform-hypergraph.md) of order $r+t$ if adding any missing [edge](../../../../../edge-of-a-graph.md) creates a new [complete uniform hypergraph](../../../../../complete-uniform-hypergraph.md) on $r+t$ [vertices](../../../../../vertex-graph-theory.md) containing that [edge](../../../../../edge-of-a-graph.md). Equivalently, for every missing $r$-set $e$, there is an $(r+t)$-set $T\supseteq e$ for which all other $r$-subsets are [edges](../../../../../edge-of-a-graph.md). Existing complete subhypergraphs are allowed in this strong-saturation definition.

We prove the bound by an [exterior-power quotient bound for strong hypergraph saturation](../../../../../exterior-power-quotient-bound-for-strong-hypergraph-saturation.md). Assume $r,t\geq1$ and $n\geq r+t$. Let $V=\mathbb R^n$ with [basis](../../../../../basis.md) $e_1,\ldots,e_n$. Choose distinct real numbers $a_1,\ldots,a_n$ and let $U$ be the kernel of the $t\times n$ matrix whose column $i$ is

$$
(1,a_i,\ldots,a_i^{t-1})^\mathsf T.
$$

Every $t$ columns are [linearly independent](../../../../../linear-independence.md) by the [Vandermonde determinant](../../../../../vandermonde-determinant.md), so $\dim U=n-t$. Form the [quotient vector space](../../../../../quotient-vector-space.md)

$$
W=\bigwedge^rV\big/\bigwedge^rU,\qquad
\dim W=\binom nr-\binom{n-t}{r}.
$$

For each $r$-set $e=\{i_1<\cdots<i_r\}$, let $v_e$ be the image in $W$ of the [exterior product](../../../../../exterior-product.md) $e_{i_1}\wedge\cdots\wedge e_{i_r}$. These images [span](../../../../../linear-span.md) $W$.

For an $(r+t)$-set $T$, let $V_T$ be its coordinate subspace. The matrix restricted to $T$ has rank $t$, so $U\cap V_T$ has [dimension](../../../../../dimension-vector-space.md) $r$. The wedge of a [basis](../../../../../basis.md) of this intersection is a nonzero vector

$$
\alpha_T=\sum_{e\in T^{(r)}}c_e\,e_{i_1}\wedge\cdots\wedge e_{i_r}
\quad\text{in }\bigwedge^rU.
$$

Every coefficient $c_e$ is nonzero. Indeed, projection from $U\cap V_T$ onto the $r$ coordinates in $e$ is an isomorphism: a vector in its kernel would be supported on $T\setminus e$, where the $t$ columns are independent, and hence would be zero. That projection's determinant is precisely the corresponding wedge coefficient. Thus, in the [quotient vector space](../../../../../quotient-vector-space.md),

$$
\sum_{e\in T^{(r)}}c_e v_e=0\qquad(c_e\ne0).
$$

For a missing [edge](../../../../../edge-of-a-graph.md), choose its strong-saturation witness $T$. All other vectors in this relation come from present [edges](../../../../../edge-of-a-graph.md), so the missing [edge](../../../../../edge-of-a-graph.md)'s vector is in their [span](../../../../../linear-span.md). Consequently the present-edge vectors already [span](../../../../../linear-span.md) all of $W$. Their number is at least its [dimension](../../../../../dimension-vector-space.md):

$$
\boxed{|E(H)|\geq\binom nr-\binom{n-t}{r}.}
$$

This is sharp. Take all $r$-sets that meet a fixed $t$-set $D$. A missing [edge](../../../../../edge-of-a-graph.md) $e$ is disjoint from $D$, and on $e\cup D$ every other $r$-set meets $D$; adding $e$ completes the required [clique](../../../../../clique-graph-theory.md). The number of [edges](../../../../../edge-of-a-graph.md) is exactly the boxed difference. If $r\leq n<r+t$, no missing [edge](../../../../../edge-of-a-graph.md) could have a witness, so a strongly saturated [hypergraph](../../../../../hypergraph-split.md) must be complete; the substantive construction above is for the usual range $n\geq r+t$.

For the set-pair problem, write $m=|I|$ and choose $x_i\in R_i\cap S_i$. If $i\ne j$, the cross-disjointness implies that $x_i$ is in neither $R_j$ nor $S_j$. In particular, the witnesses are distinct. Let $D=\{x_i:i\in I\}$; each $R_i$ and $S_i$ contains exactly its own witness from $D$.

Choose two different indices $i,j$. The [sets](../../../../../set-split.md) $R_i\setminus\{x_i\}$ and $S_j\setminus\{x_j\}$ are disjoint, lie outside $D$, and have sizes $r-1$ and $s-1$. Hence

$$
n-m\geq(r-1)+(s-1),\qquad
\boxed{|I|\leq n-r-s+2.}
$$

For equality, partition the ground [set](../../../../../set-split.md) into disjoint [sets](../../../../../set-split.md) $P,Q,D$ with sizes $r-1,s-1,n-r-s+2$, respectively, and enumerate $D$ as $x_1,\ldots,x_m$. [Set](../../../../../set-split.md)

$$
\boxed{R_i=P\cup\{x_i\},\qquad S_i=Q\cup\{x_i\}.}
$$

Then $R_i\cap S_j$ is $\{x_i\}$ for $i=j$ and empty otherwise. This realizes equality whenever the bound permits $m\geq2$. The argument is a [diagonal-intersection set-pair bound](../../../../../diagonal-intersection-set-pair-bound.md), with no additional assumptions on intersections among the $R_i$ or among the $S_i$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
