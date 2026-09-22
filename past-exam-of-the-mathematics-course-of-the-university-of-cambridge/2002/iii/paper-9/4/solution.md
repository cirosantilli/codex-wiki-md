<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We use the following precise form of the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md). For every $0<\eta<1/2$ and positive [integer](../../../../../integer.md) $m_0$, there are [integers](../../../../../integer.md) $M,n_0$ such that every [graph](../../../../../graph-split.md) on $n\ge n_0$ [vertices](../../../../../vertex-graph-theory.md) has a partition

$$
V(G)=V_0\sqcup V_1\sqcup\cdots\sqcup V_k,
\qquad m_0\le k\le M,\quad |V_0|\le\eta n,\quad |V_1|=\cdots=|V_k|,
$$

with at most $\eta k^2$ irregular unordered pairs among the nonexceptional classes. Here $d(A,B)=e(A,B)/(|A||B|)$ for disjoint nonempty [sets](../../../../../set-split.md), and $(A,B)$ is an $\eta$-[regular pair](../../../../../regular-pair-of-vertex-sets.md) if

$$
|d(X,Y)-d(A,B)|\le\eta
$$

whenever $X\subseteq A$, $Y\subseteq B$, $|X|\ge\eta|A|$, $|Y|\ge\eta|B|$.

For the proof, let $f(x,y)$ be the adjacency indicator, including $f(x,x)=0$, and define $d(A,B)$ by averaging $f$ on $A\times B$ even for diagonal cells. The [regularity energy](../../../../../equitable-regularity-energy.md) of a partition $\mathcal P$ is

$$
q(\mathcal P)=\sum_{A,B\in\mathcal P}\frac{|A||B|}{n^2}d(A,B)^2,\qquad 0\le q\le1.
$$

Every exceptional [vertex](../../../../../vertex-graph-theory.md) is represented by its own singleton cell in this energy. If a rectangle $A\times B$ is refined into smaller rectangles with densities $d_{ij}$ and weights $w_{ij}=|A_i||B_j|$, expanding the square gives the [refinement variance identity for regularity energy](../../../../../refinement-variance-identity-for-regularity-energy.md)

$$
\sum_{i,j}w_{ij}d_{ij}^2-|A||B|d(A,B)^2
=\sum_{i,j}w_{ij}(d_{ij}-d(A,B))^2\ge0.
$$

Thus refinement never decreases energy.

Suppose an equitable partition with $k$ classes of size $L$ fails the desired conclusion. For every [irregular pair](../../../../../irregular-pair-of-vertex-sets.md) choose witness subsets $X\subseteq V_i$, $Y\subseteq V_j$, each of size at least $\eta L$, whose density differs from $d(V_i,V_j)$ by more than $\eta$. Split each class by all witness subsets involving it. Each class has at most $2^{k-1}$ atoms. On a witness rectangle, the weighted mean of $d_{ab}-d(V_i,V_j)$ is $d(X,Y)-d(V_i,V_j)$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) therefore bounds the energy increment on this rectangle below by

$$
\frac{|X||Y|}{n^2}\bigl(d(X,Y)-d(V_i,V_j)\bigr)^2
>\eta^4\frac{L^2}{n^2}.
$$

The different original cell pairs have disjoint rectangles. More than $\eta k^2$ irregular unordered pairs, with both orientations counted in the energy, thus increase it by more than $2\eta^5k^2L^2/n^2$. As long as $|V_0|\le\eta n<n/2$, this is greater than $\eta^5/2$, and in particular greater than $\eta^5/4$.

Restore equitability by dividing each atom into pieces of common size $\ell=\lfloor L/4^k\rfloor$, moving each leftover [vertex](../../../../../vertex-graph-theory.md) into the exceptional [set](../../../../../set-split.md) as a singleton energy cell. This remains a refinement, so the energy gain persists. There are at most $k2^k$ atoms, so the additional exceptional [vertices](../../../../../vertex-graph-theory.md) number at most

$$
k2^k\ell\le kL/2^k\le n/2^k.
$$

If $L\ge2\cdot4^k$, then $\ell\ge L/(2\cdot4^k)$, and the new number $k'$ of equal cells satisfies $k\le k'\le4k4^k$. For the lower bound, within each old class the leftover count is at most $2^k\ell<L$, so at least one full new cell survives. For the upper bound, $n/\ell\le2(n/L)4^k\le4k4^k$, using $kL\ge n/2$. This proves [equalization with a controlled exceptional set](../../../../../equalization-with-a-controlled-exceptional-set.md) without any energy loss.

Put $T=\lceil4\eta^{-5}\rceil+1$. Choose $k_0\ge m_0$ with $T2^{-k_0}\le\eta/2$. Start with $k_0$ equal classes and fewer than $k_0$ exceptional [vertices](../../../../../vertex-graph-theory.md). Iterate the bounded recurrence $k\mapsto4k4^k$ $T$ times to obtain a bound $M$. Choose $n_0$ so large that the initial remainder is at most $\eta n/2$ and, for every $k\le M$, $(1-\eta)n/k\ge2\cdot4^k$. The total exceptional [set](../../../../../set-split.md) remains at most $\eta n$, since at most $T$ rounds each add at most $n2^{-k_0}$. Each failing round raises an energy in $[0,1]$ by more than $\eta^5/4$, so fewer than $T$ rounds can fail. This proves the lemma with all constants independent of the input [graph](../../../../../graph-split.md).

For the application, write $h=|V(F)|$ and $\chi(F)=r+1$. We may replace the given tolerance by a smaller one, so assume $0<\varepsilon<1$. [Set](../../../../../set-split.md) $d=\varepsilon/4$, take $m_0\ge8/\varepsilon$, and choose

$$
0<\eta<\min\left\{\frac\varepsilon8,\frac d2,\frac{(d/2)^h}{4h}\right\}.
$$

Apply the lemma and delete all [edges](../../../../../edge-of-a-graph.md) incident with $V_0$, all [edges](../../../../../edge-of-a-graph.md) inside a class, all [edges](../../../../../edge-of-a-graph.md) across [irregular pairs](../../../../../irregular-pair-of-vertex-sets.md), and all [edges](../../../../../edge-of-a-graph.md) across [regular pairs](../../../../../regular-pair-of-vertex-sets.md) of density below $d$. The resulting spanning subgraph $H$ loses at most

$$
\eta n^2+\frac{n^2}{2k}+\eta k^2L^2+\frac d2 k^2L^2
\le\left(2\eta+\frac1{2m_0}+\frac d2\right)n^2
<\varepsilon n^2.
$$

Let $R$ be the [reduced graph of a regularity partition](../../../../../reduced-graph-of-a-regularity-partition.md), whose [edges](../../../../../edge-of-a-graph.md) represent the surviving [regular pairs](../../../../../regular-pair-of-vertex-sets.md) of density at least $d$. We show that a copy of $K_{r+1}$ in $R$ forces a copy of $F$ in $G$.

Choose a proper $(r+1)$-coloring of $F$ and assign its color classes to the corresponding clusters. Embed its [vertices](../../../../../vertex-graph-theory.md) one at a time. For each unembedded [vertex](../../../../../vertex-graph-theory.md) maintain the candidate [set](../../../../../set-split.md) in its cluster consisting of unused [vertices](../../../../../vertex-graph-theory.md) adjacent to all already embedded [neighbours](../../../../../neighbour-of-a-vertex.md). After at most $h$ restrictions its size is at least $(d-\eta)^hL-h\ge(d/2)^hL-h$. This last quantity is at least $2h\eta L$ when $L$ is large, so every such candidate [set](../../../../../set-split.md) is large enough for regularity. In an $\eta$-regular pair of density $p\ge d$, fewer than $\eta L$ [vertices](../../../../../vertex-graph-theory.md) on one side have fewer than $(p-\eta)|Y|$ [neighbours](../../../../../neighbour-of-a-vertex.md) in any fixed [set](../../../../../set-split.md) $Y$ on the other side of size at least $\eta L$: otherwise these [vertices](../../../../../vertex-graph-theory.md) and $Y$ violate regularity. For the [vertex](../../../../../vertex-graph-theory.md) currently being embedded, there are at most $h$ relevant future candidate [sets](../../../../../set-split.md). At most $h\eta L$ [vertices](../../../../../vertex-graph-theory.md) are bad for one of them. Its own candidate [set](../../../../../set-split.md) has at least $2h\eta L$ [vertices](../../../../../vertex-graph-theory.md), so an unused good [vertex](../../../../../vertex-graph-theory.md) can be chosen. All future candidate [sets](../../../../../set-split.md) shrink by at most the factor $d-\eta$, apart from the removal of a used [vertex](../../../../../vertex-graph-theory.md); the stated size bound follows inductively, since the accumulated removals are at most $h$. This completes the [graph embedding lemma for regular pairs](../../../../../graph-embedding-lemma-for-regular-pairs.md) in the form needed here.

Since $G$ is $F$-free, $R$ is $K_{r+1}$-free. Any $K_{r+1}$ in $H$ would use distinct clusters, because intraclass [edges](../../../../../edge-of-a-graph.md) were deleted, and project to a $K_{r+1}$ in $R$. Therefore

$$
\boxed{K_{r+1}\not\subseteq H,\qquad e(G)-e(H)<\varepsilon n^2.}
$$

The required threshold on $n$ depends only on $F$ and $\varepsilon$, since $k\le M$ makes every nonexceptional cluster sufficiently large.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
