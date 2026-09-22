# Paper 10

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper10.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper10.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Identify the [discrete cube](../../../combinatorics.md#boolean-hypercube) $Q_n$ with the subsets of $[n]$, with [hypercube graph](../../../graph.md#hypercube-graph) adjacency given by changing one element. Write $N[A]$ for the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) and $\partial A=N[A]\setminus A$ for the [external vertex boundary](../../../graph-theory.md#external-vertex-boundary). The [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube) first orders by set size and then by [lexicographic order](../../../extremal-set-theory.md#lexicographic-order), with the smallest differing coordinate belonging to the earlier set.

[Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) states that, for every [set family](../../../extremal-set-theory.md#set-family) $A\subseteq Q_n$,

$$
|N[A]|\geq |N[C(|A|)]|,
\qquad\text{equivalently}\qquad
|\partial A|\geq|\partial C(|A|)|.
$$

Here is the [simplicial section compression](../../../combinatorics.md#simplicial-section-compression) proof. Induct on $n$, the one-dimensional case being immediate. Split $A$ by a coordinate into sections $A_0,A_1\subseteq Q_{n-1}$. Its neighbourhood sections are

$$
N[A]_0=N[A_0]\cup A_1,\qquad N[A]_1=N[A_1]\cup A_0.
$$

Replace $A_0,A_1$ by equally large simplicial [initial segments](../../../set.md#initial-segment) $I_0,I_1$. By induction $|N[I_j]|\leq|N[A_j]|$. Also the neighbourhood of a simplicial [initial segment](../../../set.md#initial-segment) is itself a simplicial [initial segment](../../../set.md#initial-segment): at its last occupied level the extra vertices form the [upper shadow](../../../extremal-set-theory.md#upper-shadow) of a lexicographic [initial segment](../../../set.md#initial-segment), again lexicographically initial. Consequently the compressed unions have sizes $\max\{|N[I_0]|,|I_1|\}$ and $\max\{|N[I_1]|,|I_0|\}$, no larger than the original unions. The compression preserves $|A|$ and cannot increase $|N[A]|$.

Repeat in every coordinate until all sections are initial. Every nontrivial compression strictly decreases the sum of the global simplicial positions, so the process terminates. To describe the [terminal families for simplicial section compression](../../../combinatorics.md#terminal-families-for-simplicial-section-compression), suppose an earlier absent vertex $S$ precedes a later present vertex $T$. They cannot share a coordinate value: otherwise they lie in the same compressed section, contradicting its initiality. Thus $T=[n]\setminus S$. No vertex can lie strictly between them in the order, since it would make another absent/present pair that is not complementary. Hence the terminal family is either $C(|A|)$ or that segment with its last vertex $S$ exchanged for its immediate complementary successor $T$.

For odd $n=2m+1$, that exceptional exchange crosses the middle levels: $S=\{m+2,\ldots,2m+1\}$ and $T=\{1,\ldots,m+1\}$. For $m\geq1$, all sets of size at most $m+1$ remain in the neighbourhood after the exchange, since an $(m+1)$-set has at least two lower neighbours and only one was removed. The new $T$ can only add vertices of size $m+2$.

For even $n=2m$, the only consecutive complementary pair in one level is $S=\{1,m+2,\ldots,2m\}$ and $T=\{2,\ldots,m+1\}$. The original segment contains all sets below size $m$ and all $m$-sets containing 1. For $m\geq2$, its neighbourhood contains all sets of size at most $m$ and all $(m+1)$-sets containing 1; every such upper set still has an included lower neighbour after the single removal. The new $T$ can only add further neighbours. The cases $n=1,2$ follow directly, with the exceptional families related to the initial ones by a [graph automorphism](../../../graph.md#graph-automorphism). Thus neither exception improves the neighbourhood, completing the induction.

For the [half-cube vertex-boundary extrema](../../../combinatorics.md#half-cube-vertex-boundary-extrema), if $n=2m+1$, the initial half cube is all sets of size at most $m$; its boundary is the next level, of size $\binom{2m+1}{m+1}$. If $n=2m$, it contains all levels below $m$ and the $m$-sets containing 1. The boundary consists of the $m$-sets avoiding 1 and the $(m+1)$-sets containing 1, giving $2\binom{2m-1}{m}=\binom{2m}{m}$.

No boundary can exceed the $2^{n-1}$ vertices outside a half cube. Taking all vertices of even [Hamming weight](../../../coding-theory.md#hamming-weight) attains that bound, because every odd-weight vertex is adjacent to one of them. Therefore, for $n\geq1$,

$$
\boxed{\min_{|A|=2^{n-1}}|\partial A|=\binom n{\lfloor n/2\rfloor},\qquad
\max_{|A|=2^{n-1}}|\partial A|=2^{n-1}}.
$$

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

**Always true.** Simplicial [initial segments](../../../set.md#initial-segment) are nested: $C(k)\subseteq C(l)$ when $k\leq l$. Taking the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) preserves inclusion, hence $N[C(k)]\subseteq N[C(l)]$ and the claimed size inequality follows. No extremal theorem is needed for this step.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

**False.** The [simplicial vertex boundaries need not increase below half volume](../../../combinatorics.md#simplicial-vertex-boundaries-need-not-increase-below-half-volume). In $Q_3$,

$$
C(3)=\{\varnothing,\{1\},\{2\}\},\qquad
C(4)=C(3)\cup\{\{3\}\}.
$$

Both [closed graph neighbourhoods](../../../graph-theory.md#closed-graph-neighbourhood) consist of all vertices except $\{1,2,3\}$, so both have size seven. Their external [vertex boundaries](../../../graph-theory.md#external-vertex-boundary) therefore have sizes

$$
\boxed{|\partial C(3)|=4>3=|\partial C(4)|},
$$

although $3<4=2^{3-1}$. Adding a vertex already in the neighbourhood can reduce the external [vertex boundary](../../../graph-theory.md#external-vertex-boundary) without enlarging the neighbourhood.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

**False.** [Complementary-size simplicial vertex boundaries can be asymmetric](../../../combinatorics.md#complementary-size-simplicial-vertex-boundaries-can-be-asymmetric). Use $n=7$, $k=63$ and $l=65$, so $k+l=128$.

There are 64 sets of size at most three. The [initial segment](../../../set.md#initial-segment) $C(63)$ contains all of them except the last triple $\{5,6,7\}$. Every four-set has another included triple, so its external [vertex boundary](../../../graph-theory.md#external-vertex-boundary) is that missing triple together with all $\binom74=35$ four-sets: $|\partial C(63)|=36$.

The [initial segment](../../../set.md#initial-segment) $C(65)$ contains all sets of size at most three and the first four-set $\{1,2,3,4\}$. Its external [vertex boundary](../../../graph-theory.md#external-vertex-boundary) has the other 34 four-sets and the three five-sets containing $\{1,2,3,4\}$. Thus

$$
\boxed{|\partial C(63)|=36<37=|\partial C(65)|},
$$

contradicting the proposed inequality.

## 2

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [standard simplicial decomposition of a sphere](../../../algebraic-topology.md#standard-simplicial-decomposition-of-a-sphere) $F^n$ is the boundary of the [cross-polytope](../../../mathematical-optimization.md#cross-polytope) with vertices $\pm e_1,\ldots,\pm e_{n+1}$, identified radially with $S^n$. A face chooses distinct coordinate indices and one sign for each; it never contains an [antipodal pair](../../../geometry-and-topology.md#antipodal-pair).

A [regular antipodal triangulation of a sphere](../../../algebraic-topology.md#regular-antipodal-triangulation-of-a-sphere) is invariant under the [antipodal map](../../../homology.md#antipodal-map) and has the nested coordinate equators $S^0\subset S^1\subset\cdots\subset S^{k-1}$ as subcomplexes. In particular each equator separates its sphere into two triangulated [hemispheres](../../../geometry-and-topology.md#hemisphere). These conditions are preserved by [barycentric subdivision](../../../homology.md#barycentric-subdivision).

For a [simplicial map](../../../algebraic-topology.md#simplicial-map) $f:F\to F^n$, a [positive alternating simplex](../../../algebraic-topology.md#positive-alternating-simplex) of dimension $j$ has distinct image labels

$$
+e_{i_0},-e_{i_1},\ldots,(-1)^je_{i_j},\qquad i_0<\cdots<i_j.
$$

The opposite alternating pattern is negative; all other simplices, including collapsed images, are neutral.

To prove the [antipodal alternating-simplex parity lemma](../../../algebraic-topology.md#antipodal-alternating-simplex-parity-lemma), let $p_j$ count positive $j$-simplices in the equatorial $S^j$. There is exactly one positive vertex in $S^0$, so $p_0=1$. A $j$-simplex has an odd number of positive alternating facets precisely when it is positive or negative alternating. Indeed an alternating sequence has exactly one positive alternating deletion; a nonalternating sequence has either zero or two. For a collapsed image, a positive facet can occur only when exactly one label is repeated; deleting either copy gives two such facets.

Count incidences of positive $(j-1)$-faces with $j$-simplices in one closed [hemisphere](../../../geometry-and-topology.md#hemisphere). Interior faces contribute twice and equatorial faces once. The count modulo two is therefore $p_{j-1}$. It is also the number of positive or negative $j$-simplices in that hemisphere modulo two. Because $f$ is antipodal, each alternating pair $\sigma,-\sigma$ has one positive and one negative member, with one member in each hemisphere. Thus

$$
p_j\equiv p_{j-1}\pmod2.
$$

Induction gives odd $p_k$, proving the existence of a positive $k$-simplex. In particular, an antipodal [simplicial map](../../../algebraic-topology.md#simplicial-map) $F\to F^{k-1}$ is impossible: a positive $k$-simplex would require $k+1$ distinct coordinate labels but only $k$ are available.

The [Borsuk-Ulam theorem](../../../algebraic-topology.md#borsuk-ulam-theorem) states that every [continuous map](../../../topology.md#continuous-map) $g:S^k\to\mathbb R^k$ has some $x$ with $g(x)=g(-x)$. First rule out a continuous antipodal map $h:S^k\to S^{k-1}$ for $k\geq1$. By [uniform continuity](../../../topological-analysis.md#uniform-continuity), take a sufficiently fine regular [barycentric subdivision](../../../homology.md#barycentric-subdivision) so that endpoints of each edge have images less than $2/\sqrt{k}$ apart. Label a vertex by $\operatorname{sgn}(h_i)e_i$, where $i$ is the smallest index maximizing $|h_i|$. Since $h$ is unit length, this maximum is at least $1/\sqrt{k}$; two adjacent vertices cannot have opposite labels. The labels therefore define an antipodal [simplicial map](../../../algebraic-topology.md#simplicial-map) to $F^{k-1}$, contradicting the preceding result.

If the stated [Borsuk-Ulam theorem](../../../algebraic-topology.md#borsuk-ulam-theorem) failed, the map

$$
h(x)=\frac{g(x)-g(-x)}{\|g(x)-g(-x)\|}
$$

would be just such a continuous antipodal map. This proves the required version; $k=0$ is immediate.

For the [Kneser conjecture](../../../graph-theory.md#lovasz-theorem-on-kneser-graphs), equivalently [Lovász theorem on Kneser graphs](../../../graph-theory.md#lovasz-theorem-on-kneser-graphs), the claim is

$$
\boxed{\chi(KG(N,r))=N-2r+2\qquad(N\geq2r\geq2)}.
$$

The [Kneser graph](../../../graph-theory.md#kneser-graph) joins disjoint $r$-subsets of $[N]$. Let $d=N-2r+1$. Colour each $r$-set by its least element in $[d]$ when it has one, and otherwise by one final colour. A colour class indexed by $i$ is an [intersecting family](../../../extremal-set-theory.md#intersecting-family) because all its members contain $i$; the final class lies in a $(2r-1)$-set and is also intersecting. This proves the upper bound $d+1$.

For the lower bound, first deduce the open-cover [Lusternik-Schnirelmann-Borsuk theorem](../../../algebraic-topology.md#lusternik-schnirelmann-theorem). An [open cover](../../../topology.md#open-cover) $U_0,\ldots,U_d$ of $S^d$ admits a continuous [partition of unity](../../../differential-geometry.md#partition-of-unity) $\phi_0,\ldots,\phi_d$ subordinate to it. Apply the [Borsuk-Ulam theorem](../../../algebraic-topology.md#borsuk-ulam-theorem) to $(\phi_1,\ldots,\phi_d)$. Equal values at $x,-x$ and $\sum_i\phi_i=1$ make all values equal. At least one common value is positive, so some $U_i$ contains an [antipodal pair](../../../geometry-and-topology.md#antipodal-pair).

Now suppose the $r$-sets could be coloured with only $d$ colours, each an [intersecting family](../../../extremal-set-theory.md#intersecting-family). Choose $N$ points $v_1,\ldots,v_N\in S^d$ such that every $d+1$ of their vectors are [linearly independent](../../../vector-space.md#linear-independence). For example, normalize $(1,t_i,\ldots,t_i^d)$ for distinct real $t_i$; the [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant) proves this property. The [general-position hemisphere count](../../../geometry-and-topology.md#general-position-hemisphere-count) says that at most $d$ points lie on any equator. Since $N-d=2r-1$, at least one of the opposite [open hemispheres](../../../geometry-and-topology.md#open-hemisphere) determined by $x,-x$ contains an $r$-set of the labelled points.

Let $U_i$ be the open set of directions whose positive [open hemisphere](../../../geometry-and-topology.md#open-hemisphere) contains an $r$-set of colour $i$. It contains no [antipodal pair](../../../geometry-and-topology.md#antipodal-pair), as such a pair would give two disjoint sets of that colour. The compact set $K=S^d\setminus\bigcup_{i=1}^dU_i$ also contains no [antipodal pair](../../../geometry-and-topology.md#antipodal-pair): otherwise each of the two opposite hemispheres would have at most $r-1$ points, contradicting the count $2r-1$.

If $K$ is nonempty, compactness gives a positive [set distance](../../../topological-analysis.md#distance-between-two-sets) between $K$ and $-K$; an open neighbourhood $U_0$ of radius less than half that [set distance](../../../topological-analysis.md#distance-between-two-sets) still has no [antipodal pair](../../../geometry-and-topology.md#antipodal-pair). If $K$ is empty, take $U_0=\varnothing$. In either case $U_0,U_1,\ldots,U_d$ is an [open cover](../../../topology.md#open-cover) with no member containing an [antipodal pair](../../../geometry-and-topology.md#antipodal-pair), contradicting the [Lusternik-Schnirelmann-Borsuk theorem](../../../algebraic-topology.md#lusternik-schnirelmann-theorem). Hence at least $d+1$ colours are required.

## 3

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the uniform [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem): if $p$ is a [prime number](../../../number-theory.md#prime-number), $L\subseteq\mathbb F_p$ has $s$ distinct residues, $s\leq\min\{r,n-r\}$, and an $r$-[uniform set family](../../../extremal-set-theory.md#uniform-set-family) $\mathcal F$ has distinct-member intersection sizes in $L$ modulo $p$ while $r\bmod p\notin L$, then

$$
|\mathcal F|\leq\binom ns.
$$

Here is a [polynomial method in combinatorics](../../../combinatorics.md#polynomial-method-in-combinatorics) proof. For each $A\in\mathcal F$, form the [intersection polynomial](../../../combinatorics.md#intersection-polynomial)

$$
f_A(x)=\prod_{\lambda\in L}\left(\sum_{i\in A}x_i-\lambda\right)
$$

over $\mathbb F_p$, and use [multilinear reduction on the Boolean cube](../../../polynomial.md#multilinear-reduction-on-the-boolean-cube) so its degree is at most $s$. At the [characteristic vector](../../../extremal-set-theory.md#characteristic-vector-of-a-set) of $B\in\mathcal F$, this evaluates to zero for $A\ne B$ and is nonzero for $A=B$. Consequently these evaluation functions are [linearly independent](../../../vector-space.md#linear-independence).

The [low-degree evaluation rank on a uniform layer](../../../extremal-set-theory.md#low-degree-evaluation-rank-on-a-uniform-layer) bounds their space by $\binom ns$. To justify that step without division by a possibly zero residue, form the integer incidence matrix with rows $T\subseteq[n]$, $|T|\leq s$, columns $r$-sets $B$, and entries $\mathbf1_{T\subseteq B}$. Over the [rational numbers](../../../number-theory.md#rational-number), a row with $|T|=j$ equals $\binom{r-j}{s-j}^{-1}$ times the sum of the rows of all $s$-sets containing $T$. Thus its rational [matrix rank](../../../vector-space.md#matrix-rank) is at most $\binom ns$. Every larger minor is an integer [determinant](../../../linear-algebra.md#determinant) equal to zero and stays zero modulo $p$, so the same upper bound holds over $\mathbb F_p$. This proves the theorem.

For the forbidden midpoint problem, split $\mathcal A$ according to whether its members contain coordinate 1. Leave the containing half unchanged; complement every member of the avoiding half. Both resulting families consist of $2p$-sets containing 1, and complementation preserves their internal intersection sizes because

$$
|A^c\cap B^c|=4p-|A|-|B|+|A\cap B|=|A\cap B|.
$$

Within either transformed family, distinct intersections lie between 1 and $2p-1$ and are not $p$. Their residues are therefore in $L=\{1,\ldots,p-1\}$, whereas the set-size residue is $2p\equiv0$. Apply the [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) to each half and add:

$$
\boxed{|\mathcal A|\leq2\binom{4p}{p-1}}.
$$

**The factor 2 comes from splitting into two families.** The unsplit family can contain disjoint sets, whose intersection residue zero equals the set-size residue and prevents this direct application. Removing the shared coordinate after splitting also gives the stronger [complement splitting for forbidden midpoint intersections](../../../extremal-set-theory.md#complement-splitting-for-forbidden-midpoint-intersections) bound $2\binom{4p-1}{p-1}$.

For the construction, fix a $(p+1)$-set $B$ and let $R=[4p]\setminus B$, of size $3p-1$. The [fixed-core construction avoiding midpoint intersections](../../../extremal-set-theory.md#fixed-core-construction-avoiding-midpoint-intersections) is

$$
\mathcal F=\{B\cup X:X\in R^{(p-1)}\},\qquad
\mathcal A=\mathcal F\cup\{A^c:A\in\mathcal F\}.
$$

Two members of $\mathcal F$ intersect in at least $p+1$ points; the same is true for two complements. An intersection across the two halves has size $|X\setminus Y|\leq p-1$. No intersection is $p$. The halves are disjoint because one contains all of $B$ and the other none, so

$$
\boxed{|\mathcal A|=2\binom{3p-1}{p-1}}.
$$

## 4

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [uniform covers theorem](../../../combinatorics.md#uniform-covers-theorem) says that if a multiset $\mathcal C$ of coordinate subsets covers every coordinate exactly $k$ times, then a [Euclidean body](../../../combinatorics.md#euclidean-body) $S\subseteq\mathbb R^n$ satisfies

$$
|S|^k\leq\prod_{A\in\mathcal C}|S_A|,
$$

where $S_A$ is its [coordinate projection of a Euclidean body](../../../combinatorics.md#coordinate-projection-of-a-euclidean-body). Work with bounded Borel bodies, whose projections are [Lebesgue measurable sets](../../../measure-theory.md#lebesgue-measurable-set); an empty-coordinate projection has measure one.

Prove the theorem by induction on dimension, with the one-dimensional case immediate. Slice at the last coordinate, writing $S_t\subseteq\mathbb R^{n-1}$. The subsets $A\setminus\{n\}$ still cover each remaining coordinate $k$ times, so induction gives

$$
|S_t|\leq\prod_{A\in\mathcal C}|(S_t)_{A\setminus\{n\}}|^{1/k}.
$$

For $A$ not containing $n$, the projected slice is contained in $S_A$, giving a constant bound. For $A$ containing $n$, its measure is the slice measure $f_A(t)$ of $S_A$. Exactly $k$ members of $\mathcal C$ contain $n$, counted with multiplicity. Integrate and apply [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) to those $k$ factors:

$$
|S|\leq\left(\prod_{A\not\ni n}|S_A|\right)^{1/k}
\int\prod_{A\ni n}f_A(t)^{1/k}\,dt
\leq\prod_{A\in\mathcal C}|S_A|^{1/k}.
$$

[Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) identifies $\int f_A=|S_A|$, completing the proof. Exact covering is needed for real volumes, which may be smaller than one.

The [Bollobas--Thomason box theorem](../../../combinatorics.md#box-theorem) states that there is an [axis-parallel box](../../../combinatorics.md#axis-parallel-box) $B$ with $|B|=|S|$ and $|B_A|\leq|S_A|$ for every nonempty coordinate subset $A$. Use the [logarithmic linear program for the box theorem](../../../combinatorics.md#logarithmic-linear-program-for-the-box-theorem): if its side lengths are $b_i=e^{x_i}$, maximize $\sum_i x_i$ subject to

$$
\sum_{i\in A}x_i\leq\log|S_A|\qquad(\varnothing\ne A\subseteq[n]).
$$

The [linear program](../../../mathematical-optimization.md#linear-programming) is feasible by choosing all $x_i$ sufficiently negative and is bounded above by the full-set constraint. Its dual minimizes $\sum_A\lambda_A\log|S_A|$ subject to $\lambda_A\geq0$ and $\sum_{A\ni i}\lambda_A=1$ for each $i$: precisely a [fractional uniform cover](../../../combinatorics.md#fractional-uniform-cover).

The dual feasible polytope is nonempty, bounded and defined by integer coefficients, so an optimal extreme point has rational coordinates. Multiply its weights by a common denominator $k$. The resulting integer [uniform cover](../../../combinatorics.md#uniform-cover) and the [uniform covers theorem](../../../combinatorics.md#uniform-covers-theorem) give

$$
k\log|S|\leq\sum_A(k\lambda_A)\log|S_A|.
$$

Thus the dual optimum is at least $\log|S|$; weight one on $A=[n]$ attains equality. [Strong duality](../../../mathematical-optimization.md#strong-duality) gives a primal optimum $\sum_i x_i=\log|S|$. The corresponding box has the required volume and projected-volume bounds, proving the theorem.

For the [Loomis–Whitney theorem](../../../combinatorics.md#loomis-whitney-inequality), take the box supplied by the [Bollobas--Thomason box theorem](../../../combinatorics.md#box-theorem). Each side length occurs in exactly $n-1$ projections omitting one coordinate, so

$$
|S|^{n-1}=|B|^{n-1}
=\prod_{i=1}^n|B_{[n]\setminus\{i\}}|
\leq\prod_{i=1}^n|S_{[n]\setminus\{i\}}|.
$$

This is the [Loomis--Whitney inequality](../../../combinatorics.md#loomis-whitney-inequality).

For the [three projection areas of a volume-one body](../../../combinatorics.md#three-projection-areas-of-a-volume-one-body), necessity is $1=|S|^2\leq abc$. Conversely suppose $abc\geq1$ and set

$$
x=\sqrt{ac/b},\qquad y=\sqrt{ab/c},\qquad z=\sqrt{bc/a}.
$$

The box $[0,x]\times[0,y]\times[0,z]$ has projected areas $a,b,c$ and volume $V=\sqrt{abc}\geq1$. Inside it retain the three slabs

$$
S_t=\{(u,v,w):0\leq u\leq x,\ 0\leq v\leq y,\ 0\leq w\leq z,
\ \min(u/x,v/y,w/z)\leq t\}.
$$

For $t>0$, each projection is the full corresponding rectangle, since the slab in the omitted coordinate supplies every point of that projection. The volume is $V[1-(1-t)^3]$. Choose

$$
t=1-(1-1/V)^{1/3}\in(0,1]
$$

to make the volume one. This is a compact connected union of three positive-thickness boxes. Hence the complete answer is

$$
\boxed{a,b,c>0\quad\text{and}\quad abc\geq1}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
