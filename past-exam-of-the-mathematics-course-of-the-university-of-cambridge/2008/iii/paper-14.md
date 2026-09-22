# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper14.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Choose a uniformly random [permutation](../../../combinatorics.md#permutation) of $[n]$ and take its initial segments. This produces a [Uniformly random maximal chain in a Boolean lattice](../../../extremal-set-theory.md#uniformly-random-maximal-chain-in-a-boolean-lattice). A fixed $r$-set belongs to this chain with [probability](../../../probability-theory.md#probability) $r!(n-r)!/n!=\binom nr^{-1}$. An [antichain](../../../extremal-set-theory.md#antichain) meets the chain at most once, so taking the [expected value](../../../probability-theory.md#expected-value) of the number of meetings proves the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality):

$$
\boxed{\sum_{r=0}^n\frac{|\mathcal A\cap[n]^{(r)}|}{\binom nr}\le1.}
$$

In particular the [Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem) bound follows by multiplying each summand by at most the largest [binomial coefficient](../../../combinatorics.md#binomial-coefficient).

For the [vector](../../../vector-space.md#vector) request, an ordering by ordinary [subset](../../../set.md#subset) need not work: distinct [vectors](../../../vector-space.md#vector) may cancel. Instead, write $s_A=\sum_{i\in A}x_i$ and construct a [separated block decomposition for vector subset sums](../../../extremal-set-theory.md#separated-block-decomposition-for-vector-subset-sums). A block is separated if distinct labeled members have [subset](../../../set.md#subset) sums at distance at least one. We prove that the labeled [subsets](../../../set.md#subset) of $[n]$ can be partitioned into separated blocks, with

$$
b_{n,r}=\binom nr-\binom n{r-1}
$$

blocks of size $n-2r+1$, for $0\le r\le\lfloor n/2\rfloor$, with $\binom n{-1}=0$.

For $n=0$ the one [subset](../../../set.md#subset) forms one block. Suppose a block of sums $z_1,\ldots,z_\ell$ has already been constructed for $n-1$ [vectors](../../../vector-space.md#vector), and let $x=x_n$. Choose $z_*$ minimizing $z_j\cdot x$ in the block. Replace the two copies of the block, with and without the new coordinate, by the following two blocks:

$$
\{z_1+x,\ldots,z_\ell+x,z_*\},\qquad
\{z_j:j\ne *\}.
$$

The old labels are retained, so these partition the two copies even if equal sums occur in different blocks. Translation preserves separation in the first translated portion, and the second block is a [subset](../../../set.md#subset) of the old separated block. For the new cross pairs, [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\|z_j+x-z_*\|\ge\frac{(z_j-z_*+x)\cdot x}{\|x\|}
\ge\|x\|\ge1.
$$

Thus both new blocks are separated. Their sizes are $\ell+1$ and $\ell-1$, omitting an empty block. The resulting size-profile recurrence is $b_{n,r}=b_{n-1,r}+b_{n-1,r-1}$, and Pascal's identity verifies the displayed binomial-difference formula, including the even middle boundary. The total number of blocks telescopes to $\binom n{\lfloor n/2\rfloor}$.

A signed sum associated with $A=\{i:\epsilon_i=1\}$ is $2s_A-\sum_i x_i$. If two signed sums lie in the [open ball](../../../topology.md#open-ball) of radius one, their difference has [norm](../../../functional-analysis.md#norm) less than two, so their [subset](../../../set.md#subset) sums have distance less than one. At most one can therefore lie in any separated block. Hence the [Littlewood-Offord inequality](../../../extremal-set-theory.md#littlewood-offord-inequality) is

$$
\boxed{\#\left\{\epsilon\in\{-1,1\}^n:\left\|\sum_i\epsilon_ix_i-a\right\|<1\right\}
\le\binom n{\lfloor n/2\rfloor}.}
$$

The counting is by sign choices, not by distinct numerical values of the sums. The open-ball condition handles the equality-distance boundary correctly.

For the last request take real coefficients. Absorb their signs into the choices $\epsilon_i$, so all coefficients are positive and at least one. A signed-sum [real interval](../../../real-analysis.md#interval-mathematics) of length four corresponds to a subset-sum [real interval](../../../real-analysis.md#interval-mathematics) of length two. A strict three-member inclusion chain $A\subsetneq B\subsetneq C$ would have $s_C-s_A\ge2$, which cannot occur in that open [real interval](../../../real-analysis.md#interval-mathematics). Thus its [set family](../../../extremal-set-theory.md#set-family) is a [k-Sperner family](../../../extremal-set-theory.md#k-sperner-family) with $k=2$. Every [maximal chain in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) meets it at most twice, yielding $\sum_r |\mathcal F_r|/\binom nr\le2$. Write $f_r=|\mathcal F_r|/\binom nr$, so $0\le f_r\le1$ and $\sum_r f_r\le2$. If $B_1\ge B_2$ are the two largest [binomial coefficients](../../../combinatorics.md#binomial-coefficient) and $f_*$ is the fraction at a largest level, then $|\mathcal F|\le B_1f_*+B_2(2-f_*)\le B_1+B_2$. This proves the [two-level Littlewood-Offord bound](../../../extremal-set-theory.md#two-level-littlewood-offord-bound):

$$
\boxed{\binom n{\lfloor n/2\rfloor}+\binom n{\lfloor(n-1)/2\rfloor}\quad(n\ge1).}
$$

It is the greatest possible number uniformly over choices of coefficients and center. For even $n=2m$, take every coefficient equal to one and center $a=-1$: the [real interval](../../../real-analysis.md#interval-mathematics) $(-3,1)$ contains the sum levels $-2,0$, of multiplicities $\binom n{m-1},\binom nm$. For odd $n=2m+1$, take center zero, giving levels $-1,1$, each of multiplicity $\binom nm$. These attain the bound. For $n=0$ the only sign choice gives the separate maximum one. Attainment here is at the exhibited centers; it need not hold at every prescribed center.

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Assume first $1\le t\le n$, and write $d=n-t$. The sharp [nonuniform t-intersecting family bound](../../../extremal-set-theory.md#nonuniform-t-intersecting-family-bound) is

$$
\boxed{|\mathcal A|\le
\begin{cases}
\displaystyle\sum_{i=0}^q\binom ni,&d=2q,\\[3pt]
\displaystyle2\sum_{i=0}^q\binom{n-1}i,&d=2q+1.
\end{cases}}
$$

We prove the bound by deriving the needed [Kleitman diametric theorem](../../../extremal-set-theory.md#kleitman-diametric-theorem). Identify [subsets](../../../set.md#subset) with binary words, with [Hamming distance](../../../coding-theory.md#hamming-distance) $|A\triangle B|$. Let $D(n,d)$ be the two expressions above. A [set family](../../../extremal-set-theory.md#set-family) of [Hamming diameter](../../../coding-theory.md#diameter-of-a-set-family) at most $d<n$ has size at most $D(n,d)$, as follows.

First apply [downward coordinate compression](../../../extremal-set-theory.md#downward-coordinate-compression): delete coordinate $i$ from a member only when its deletion is not already present. This preserves size and cannot increase the [Hamming diameter](../../../coding-theory.md#diameter-of-a-set-family). The only possible increased distance would be between a newly lowered member $A\setminus\{i\}$ and a retained member $B$ containing $i$. The deletion $B\setminus\{i\}$ must have belonged to the old [set family](../../../extremal-set-theory.md#set-family), or $B$ would have been lowered too. The old pair $A,B\setminus\{i\}$ has precisely that increased distance, proving it was already allowed. Repeated downward compressions terminate in a [down-set](../../../extremal-set-theory.md#down-set).

Next apply all [elementary set shifts](../../../extremal-set-theory.md#elementary-set-shift) $S_{ij}$ with $i<j$. They preserve size and [Hamming diameter](../../../coding-theory.md#diameter-of-a-set-family). If shifting one member but retaining the other increased their distance, the retained member must contain $j$ but not $i$; its shifted partner was already present, and the old pair with that partner has the same distance. These shifts preserve the [down-set](../../../extremal-set-theory.md#down-set) property: a [subset](../../../set.md#subset) of a shifted member either was already present or is obtained by shifting its corresponding old [subset](../../../set.md#subset). For a retained member, a [subset](../../../set.md#subset) cannot disappear, because the shifted partner of that [subset](../../../set.md#subset) is also a [subset](../../../set.md#subset) of the member or of its retained shifted partner. Repeated shifts terminate, since the sum of the selected coordinate labels decreases whenever a change occurs. We now have a shifted [down-set](../../../extremal-set-theory.md#down-set) $\mathcal F$ of the same size and [Hamming diameter](../../../coding-theory.md#diameter-of-a-set-family).

Split it into sections on $[n-1]$:

$$
\mathcal F_0=\{A:n\notin A,\ A\in\mathcal F\},\qquad
\mathcal F_1=\{A:A\cup\{n\}\in\mathcal F\}.
$$

The first section has [Hamming diameter](../../../coding-theory.md#diameter-of-a-set-family) at most $d$. We claim the second has [Hamming diameter](../../../coding-theory.md#diameter-of-a-set-family) at most $d-2$. For $X,Y\in\mathcal F_1$, downward closure gives $X\setminus Y,Y\in\mathcal F_1$. Compare $(X\setminus Y)\cup\{n\}$ with $Y\in\mathcal F_0$. Their distance is $|X\cup Y|+1$, so $|X\cup Y|\le d-1<n-1$. Choose $i<n$ outside their union. Shiftedness puts $X\cup\{i\}$ in $\mathcal F_0$, while $Y\cup\{n\}$ is a member of $\mathcal F$. Their distance is $|X\triangle Y|+2$, proving the claim. For $d<2$ this argument forces $\mathcal F_1$ to be empty.

The induction now gives

$$
|\mathcal F|\le D(n-1,d)+D(n-1,d-2)=D(n,d),
$$

where negative-diameter [set families](../../../extremal-set-theory.md#set-family) are empty. The equality of the numerical expressions is Pascal's identity. The base case $d=0$ has at most one member. At the boundary $d=n-1$, at most one member of each complementary pair is allowed, giving $2^{n-1}$, which equals $D(n,n-1)$ by binomial symmetry. For the remaining cases $1\le d\le n-2$, both section bounds belong to smaller-dimensional induction cases. This completes the diametric proof.

For a $t$-intersecting [set family](../../../extremal-set-theory.md#set-family),

$$
|A\triangle B|=|A\cup B|-|A\cap B|\le n-t=d,
$$

so the theorem applies. For $d=2q$, equality is attained by all [sets](../../../set.md) of size at least $n-q$, since two such [sets](../../../set.md) intersect in at least $n-2q=t$ elements. For $d=2q+1$, take all [sets](../../../set.md) of size at least $n-q$, and also all $(n-q-1)$-sets avoiding one fixed point. Two of these smaller [sets](../../../set.md) intersect in at least $2(n-q-1)-(n-1)=t$ points; a smaller and a larger [set](../../../set.md) intersect in at least $t$; two larger [sets](../../../set.md) intersect in at least $t+1$. The size of this [set family](../../../extremal-set-theory.md#set-family) is

$$
\sum_{i=0}^q\binom ni+\binom{n-1}q
=2\sum_{i=0}^q\binom{n-1}i,
$$

so it attains the odd bound. If $t=0$, the full power [set](../../../set.md) is admissible; if $t>n$, the only admissible [set family](../../../extremal-set-theory.md#set-family) is empty.

**Every maximal 1-intersecting [set family](../../../extremal-set-theory.md#set-family) attains $2^{n-1}$, for $n\ge1$.** Such a [set family](../../../extremal-set-theory.md#set-family) is an [up-set](../../../extremal-set-theory.md#up-set), since adding a superset preserves [set intersections](../../../set.md#set-intersection). It contains $[n]$ and omits the empty [set](../../../set.md). It contains at most one member of any complementary pair. If neither of two nonempty complements $A,A^c$ were present, maximality would give a member $B$ disjoint from $A$; upward closure would then include $A^c$, a contradiction. Thus it chooses precisely one member of each complementary pair, as in [maximal intersecting families choose one member of every complementary pair](../../../extremal-set-theory.md#maximal-intersecting-families-choose-one-member-of-every-complementary-pair).

**Not every maximal 2-intersecting [set family](../../../extremal-set-theory.md#set-family) attains the bound.** On four points, let $\mathcal A=\{A:\{1,2\}\subseteq A\}$. This [set family](../../../extremal-set-theory.md#set-family) has four members and is maximal: every missing [set](../../../set.md) meets its member $\{1,2\}$ in at most one point. The sharp bound is $1+4=5$, attained by all [sets](../../../set.md) of size at least three. This proves [maximal intersection does not imply maximum size](../../../extremal-set-theory.md#maximal-intersection-does-not-imply-maximum-size).

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

All [graphs](../../../graph.md) here are finite and simple. For the [strong graph product](../../../graph.md#strong-product-of-graphs) $G\boxtimes H$, two distinct [graph vertex](../../../graph.md#vertex-graph-theory) pairs are adjacent if in each coordinate the entries are equal or adjacent. Use $G^{\boxtimes m}$ for its [strong graph power](../../../graph.md#strong-graph-power); the exam's $G^m$ means this product power, not the distance-based [graph power](../../../graph.md#graph-power). The [Shannon capacity of a graph](../../../graph.md#shannon-capacity-of-a-graph) is

$$
\boxed{c(G)=\sup_{m\ge1}\alpha(G^{\boxtimes m})^{1/m}
=\lim_{m\to\infty}\alpha(G^{\boxtimes m})^{1/m},}
$$

where $\alpha$ is the [independence number](../../../graph-theory.md#independence-number). Products of [independent sets](../../../graph-theory.md#independent-set-graph-theory) are independent, so $a_{r+s}\ge a_ra_s$ for $a_m=\alpha(G^{\boxtimes m})$. To see why the limit exists, fix $r$ and write $m=qr+s$, $0\le s<r$. Then $a_m\ge a_r^q$, using $a_s\ge1$ and $a_0=1$, so $\liminf_m (\log a_m)/m\ge(\log a_r)/r$. Take the supremum over $r$; the reverse upper bound holds termwise. This proves the required form of [Fekete lemma](../../../real-analysis.md#fekete-s-lemma). For the empty [graph](../../../graph.md) on no [graph vertices](../../../graph.md#vertex-graph-theory) one [sets](../../../set.md) [graph capacity](../../../graph.md#shannon-capacity-of-a-graph) zero separately.

Associativity of the [strong product](../../../graph.md#strong-product-of-graphs) gives

$$
c(G\boxtimes G)=\lim_m\alpha(G^{\boxtimes 2m})^{1/m}
=\left(\lim_m\alpha(G^{\boxtimes 2m})^{1/(2m)}\right)^2
=\boxed{c(G)^2}.
$$

An [orthonormal representation of a graph](../../../graph-theory.md#orthonormal-representation-of-a-graph) assigns a real [unit vector](../../../vector-space.md#unit-vector) $u_v$ to each [graph vertex](../../../graph.md#vertex-graph-theory), with $u_v\perp u_w$ whenever distinct [graph vertices](../../../graph.md#vertex-graph-theory) $v,w$ are nonadjacent. Adjacent [graph vertices](../../../graph.md#vertex-graph-theory) need not receive orthogonal [vectors](../../../vector-space.md#vector). A handle is a [unit vector](../../../vector-space.md#unit-vector) $h$. The handle formulation of the [Lovász theta function](../../../graph-theory.md#lovasz-number) is

$$
\vartheta(G)=\inf_{\{u_v\},\,\|h\|=1}\max_v\frac1{|h\cdot u_v|^2},
$$

with a zero denominator giving infinity. Representations may use any finite-dimensional Euclidean space. This is the usual [Lovász number](../../../graph-theory.md#lovasz-number) in its orthonormal-representation formulation.

For an [independent set](../../../graph-theory.md#independent-set-graph-theory) $I$, the [vectors](../../../vector-space.md#vector) $u_v$, $v\in I$, are mutually orthonormal. Directly,

$$
0\le\left\|h-\sum_{v\in I}(h\cdot u_v)u_v\right\|^2
=1-\sum_{v\in I}|h\cdot u_v|^2.
$$

If $T=\max_v|h\cdot u_v|^{-2}$ is finite, every summand is at least $1/T$, giving $|I|\le T$. For a [strong power](../../../graph.md#strong-graph-power), use the [vectors](../../../vector-space.md#vector) and handle

$$
u_{(v_1,\ldots,v_m)}=u_{v_1}\otimes\cdots\otimes u_{v_m},\qquad
h_m=h^{\otimes m}.
$$

Their [norms](../../../functional-analysis.md#norm) are one. Nonadjacency of two distinct words means a coordinate has distinct nonadjacent entries, so the corresponding tensor [inner product](../../../linear-algebra.md#inner-product) has a zero factor. The handle [inner products](../../../linear-algebra.md#inner-product) satisfy

$$
|h_m\cdot u_{(v_1,\ldots,v_m)}|^2=\prod_{i=1}^m|h\cdot u_{v_i}|^2\ge T^{-m}.
$$

Applying the preceding calculation gives $\alpha(G^{\boxtimes m})\le T^m$. Taking roots, then the infimum over representations and handles, proves

$$
\boxed{c(G)\le\vartheta(G).}
$$

This is the [tensor-product capacity bound from an orthonormal representation](../../../graph-theory.md#tensor-product-capacity-bound-from-an-orthonormal-representation), and the displayed projection calculation supplies [Bessel inequality](../../../hilbert-space.md#bessel-s-inequality) explicitly.

For $C_5$, label [graph vertices](../../../graph.md#vertex-graph-theory) by $\mathbb Z/5\mathbb Z$, with edges at differences $\pm1$. The five words

$$
\{(j,2j):j\in\mathbb Z/5\mathbb Z\}
$$

are independent in its strong square: a difference $\pm1$ in the first coordinate produces a nonedge difference $\pm2$ in the second, while a first-coordinate difference $\pm2$ is already a nonedge. Hence $c(C_5)\ge\sqrt5$.

<a id="3/image-five-independent-words-in-the-strong-square-of-the-pentagon"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14-pentagon-code.png)

**[Figure 1](#3/image-five-independent-words-in-the-strong-square-of-the-pentagon). Five independent words in the strong square of the pentagon**.

For the matching upper bound [set](../../../set.md) $\rho=1/\sqrt5$, $h=(0,0,1)$, and

$$
u_j=\left(\sqrt{1-\rho}\cos\frac{2\pi j}5,
\sqrt{1-\rho}\sin\frac{2\pi j}5,\sqrt\rho\right).
$$

Each [vector](../../../vector-space.md#vector) is unit. For a nonedge, the angle difference is $\pm4\pi/5$, and

$$
u_j\cdot u_{j+2}=(1-\rho)\cos(4\pi/5)+\rho=0,
$$

because $\cos(4\pi/5)=-(1+\sqrt5)/4$ and $\rho=1/\sqrt5$. Thus these [vectors](../../../vector-space.md#vector) form an [orthonormal representation](../../../graph-theory.md#orthonormal-representation-of-a-graph). The handle has $|h\cdot u_j|^2=\rho$, giving $\vartheta(C_5)\le1/\rho=\sqrt5$. Together the two bounds prove the [pentagon capacity code](../../../graph.md#pentagon-capacity-code) result

$$
\boxed{c(C_5)=\vartheta(C_5)=\sqrt5.}
$$

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $U=G\sqcup\bar G$, with the two copies of the [graph vertex](../../../graph.md#vertex-graph-theory) [set](../../../set.md) distinguished. In $G\boxtimes\bar G$, the diagonal pairs $(v,v)$ form an [independent set](../../../graph-theory.md#independent-set-graph-theory) of size $n$: for $v\ne w$, their adjacency cannot hold in both a [graph](../../../graph.md) and its [complement graph](../../../graph-theory.md#complement-graph). There is another such diagonal [set](../../../set.md) in $\bar G\boxtimes G$. These two types lie in different components of $U^{\boxtimes2}$, so their [set union](../../../set.md#set-union) is independent. Thus

$$
\alpha(U^{\boxtimes2})\ge2n,\qquad\boxed{c(U)\ge\sqrt{2n},}
$$

which proves the printed bound.

A stronger [complement-pair capacity gain](../../../graph.md#complement-pair-capacity-gain) will make the strict inequality transparent. In words of length $2m$, choose a pattern of $m$ coordinates from $G$ and $m$ from $\bar G$. Match the $i$th coordinate of the first type with the $i$th of the second type, and put the same [graph vertex](../../../graph.md#vertex-graph-theory) label in each pair. This gives $n^m$ independent words for each pattern: if two label tuples differ, their differing pair has a nonedge in one of the two complementary [graphs](../../../graph.md). Codes belonging to distinct patterns are mutually nonadjacent, since some coordinate lies in different components of the disjoint [set union](../../../set.md#set-union). Consequently

$$
\alpha(U^{\boxtimes2m})\ge\binom{2m}m n^m.
$$

The inequalities $4^m/(2m+1)\le\binom{2m}m\le4^m$ show that its $2m$th root tends to two. Therefore

$$
\boxed{c(G\sqcup\bar G)\ge2\sqrt n.}
$$

This strengthens, rather than changes, the bound requested in the PDF.

For a [polynomial representation of a graph](../../../graph.md#polynomial-representation-of-a-graph) over a [field](../../../algebra.md#field) $F$, choose points $a_v\in F^r$ and [polynomials](../../../polynomial.md) $f_v\in M$, where $M\subseteq F[z_1,\ldots,z_r]$ is a finite-dimensional [vector](../../../vector-space.md#vector) space, such that

$$
f_v(a_v)\ne0,\qquad f_v(a_w)=0\quad\text{whenever }v\ne w\text{ are nonadjacent}.
$$

No condition is imposed at adjacent pairs. To bound a [strong power](../../../graph.md#strong-graph-power), put its [polynomials](../../../polynomial.md) in disjoint variable blocks:

$$
F_{(v_1,\ldots,v_m)}(z^{(1)},\ldots,z^{(m)})
=\prod_{i=1}^m f_{v_i}(z^{(i)}).
$$

They lie in a [polynomial](../../../polynomial.md) space canonically identified with $M^{\otimes m}$, of [dimension](../../../vector-space.md#dimension-vector-space) $(\dim_F M)^m$. For an [independent set](../../../graph-theory.md#independent-set-graph-theory) of words, evaluation of their [polynomials](../../../polynomial.md) at their associated point tuples is a diagonal matrix with nonzero diagonal: distinct words have a nonedge coordinate, which supplies a zero factor. The [polynomials](../../../polynomial.md) in that [independent set](../../../graph-theory.md#independent-set-graph-theory) are therefore linearly independent, since evaluating any linear relation at each tuple forces its corresponding coefficient to be zero. Hence

$$
\alpha(G^{\boxtimes m})\le(\dim_F M)^m,
\qquad\boxed{c(G)\le\dim_F M.}
$$

This is the [polynomial](../../../polynomial.md) form of the [Haemers rank bound](../../../graph.md#haemers-rank-bound), proved here by evaluations and [tensor products](../../../linear-algebra.md#tensor-product) rather than assumed.

For an explicit counterexample, let the [graph vertices](../../../graph.md#vertex-graph-theory) of $G$ be the five-element [subsets](../../../set.md#subset) of $[20]$. Join distinct $A,B$ exactly when $|A\cap B|$ is odd. There are $n=\binom{20}5=15504$ [graph vertices](../../../graph.md#vertex-graph-theory). Over $\mathbb F_2$, take $a_B=\mathbf1_B$ and

$$
f_A(z)=\sum_{i\in A}z_i.
$$

At the diagonal $f_A(a_A)=5=1$ in the [field](../../../algebra.md#field). At a distinct nonedge the [set intersection](../../../set.md#set-intersection) is even, so $f_A(a_B)=0$. These [polynomials](../../../polynomial.md) lie in the twenty-dimensional space spanned by $z_1,\ldots,z_{20}$, proving **$c(G)\le20$**.

Represent the [complement graph](../../../graph-theory.md#complement-graph) over $\mathbb F_3$, using the same [indicator vectors](../../../measure-theory.md#indicator-vector) and

$$
g_A(z)=\sum_{\{i,j\}\subseteq A}z_iz_j.
$$

Its evaluation at $a_B$ is $\binom{|A\cap B|}2$. The diagonal value is $\binom52=10=1$ modulo three. Distinct nonedges of $\bar G$ are edges of $G$, so the [set intersection](../../../set.md#set-intersection) size is one or three. Their evaluations are respectively zero and $\binom32=3=0$ modulo three. The [polynomials](../../../polynomial.md) belong to the space spanned by the squarefree quadratic monomials $z_iz_j$, $i<j$, of [dimension](../../../vector-space.md#dimension-vector-space) $\binom{20}2=190$. Therefore **$c(\bar G)\le190$**.

The [graph capacity](../../../graph.md#shannon-capacity-of-a-graph) inequalities are real-number bounds regardless of which [field](../../../algebra.md#field) supplies the [polynomial representation of a graph](../../../graph.md#polynomial-representation-of-a-graph). Combining them with the stronger [set union](../../../set.md#set-union) lower bound gives

$$
\boxed{c(G\sqcup\bar G)\ge2\sqrt{15504}>210\ge c(G)+c(\bar G),}
$$

since $4\cdot15504=62016>210^2=44100$. This proves [nonadditivity of Shannon capacity](../../../graph.md#nonadditivity-of-shannon-capacity) for the [graph](../../../graph.md) just defined, with both individual upper bounds calculated explicitly.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
