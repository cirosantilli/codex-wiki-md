# Paper 10

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper10.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper10.pdf)

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

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For an $r$-[uniform set family](../../../extremal-set-theory.md#uniform-set-family) $\mathcal F$, its [lower shadow](../../../extremal-set-theory.md#lower-shadow) is the [set family](../../../extremal-set-theory.md#set-family) of all $(r-1)$-sets contained in a member. Write a positive integer $m$ in its unique [binomial representation](../../../combinatorics.md#combinatorial-number-system)

$$
m=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_j}{j},\qquad
a_r>a_{r-1}>\cdots>a_j\geq j\geq1.
$$

The [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem) states that

$$
\boxed{|\mathcal F|=m\quad\Longrightarrow\quad
|\partial\mathcal F|\geq\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_j}{j-1}.}
$$

For $m=0$ the bound is zero. Equality is attained by the first $m$ $r$-sets in [colexicographic order](../../../extremal-set-theory.md#colexicographic-order). In that order $A$ precedes $B$ when the largest element of their [symmetric difference](../../../set.md#symmetric-difference) belongs to $B$.

Here is a complete [UV-compression proof of the Kruskal-Katona theorem](../../../extremal-set-theory.md#uv-compression-proof-of-the-kruskal-katona-theorem). For disjoint equal-sized [sets](../../../set.md) $U,V$, put $C(A)=(A\setminus V)\cup U$ when $A$ contains every element of $V$ and no element of $U$, and put $C(A)=A$ otherwise. The [UV-compression](../../../extremal-set-theory.md#uv-compression) of a [set family](../../../extremal-set-theory.md#set-family) replaces an eligible $A$ only if its image is absent. It preserves [cardinality](../../../set-theory.md#cardinality): a retained collision keeps both the original [set](../../../set.md) and its already present image.

We first prove the required [Shadow lemma for UV-compressions](../../../extremal-set-theory.md#shadow-lemma-for-uv-compressions). Suppose that, for each $x\in U$, a $y\in V$ can be chosen so the [set family](../../../extremal-set-theory.md#set-family) is fixed by $C_{U\setminus\{x\},V\setminus\{y\}}$. We claim

$$
\partial C_{U,V}(\mathcal F)\subseteq C_{U,V}(\partial\mathcal F).
$$

Consider a [lower shadow](../../../extremal-set-theory.md#lower-shadow) member obtained by deleting $z$ from a moved [set](../../../set.md) $A'=(A\setminus V)\cup U$. If $z\notin U$, it is the compressed image of $A\setminus\{z\}$, an old [lower shadow](../../../extremal-set-theory.md#lower-shadow) member. If $z=x\in U$, the smaller compression of $A$ produces $A'\setminus\{x\}\cup\{y\}$, which is in $\mathcal F$ by the assumed invariance. Thus $A'\setminus\{x\}$ already belongs to the old [lower shadow](../../../extremal-set-theory.md#lower-shadow); it is not eligible to move since it lacks $x$.

It remains to consider a [lower shadow](../../../extremal-set-theory.md#lower-shadow) member $B$ from a retained original member $A=B\cup\{z\}$. If $B$ is not eligible to move, it stays in the compressed [lower shadow](../../../extremal-set-theory.md#lower-shadow). If it is eligible, let $B'=(B\setminus V)\cup U$. When $z\notin U$, retaining the eligible $A$ means its image already belongs to $\mathcal F$, and that image contains $B'$. When $z=x\in U$, the smaller compression of $A$ belongs to $\mathcal F$ and equals $B'\cup\{y\}$. In either case $B'$ is in the old [lower shadow](../../../extremal-set-theory.md#lower-shadow) too. Consequently the collision rule retains $B$ as well. This proves the claimed containment in every case. Since compression preserves [cardinality](../../../set-theory.md#cardinality), it cannot increase [lower shadow](../../../extremal-set-theory.md#lower-shadow) size.

If $\mathcal F$ is not a [colexicographic initial segment](../../../extremal-set-theory.md#colexicographic-initial-segment), an earlier absent [set](../../../set.md) $A$ and a later present [set](../../../set.md) $B$ give $U=A\setminus B$, $V=B\setminus A$ with $\max U<\max V$, and a nontrivial [UV-compression](../../../extremal-set-theory.md#uv-compression). Choose such a compression with $|U|$ smallest. If $|U|>1$, choose $y\in V\setminus\{\max V\}$. For every $x\in U$, the smaller compression still has its largest differing element on the $V$ side and must fix $\mathcal F$ by minimality. If $|U|=1$, the smaller compression is the identity. Thus the [lower shadow](../../../extremal-set-theory.md#lower-shadow) argument applies.

Each nontrivial step strictly decreases the positive integer weight

$$
w(\mathcal F)=\sum_{A\in\mathcal F}\sum_{i\in A}2^i,
$$

because the largest differing coordinate belongs to $V$. Iteration therefore terminates. A terminal [set family](../../../extremal-set-theory.md#set-family) is a [colexicographic initial segment](../../../extremal-set-theory.md#colexicographic-initial-segment), since an earlier gap and a later member would otherwise provide another nontrivial compression. The final [set family](../../../extremal-set-theory.md#set-family) has $m$ members and no larger [lower shadow](../../../extremal-set-theory.md#lower-shadow).

To compute its [lower shadow](../../../extremal-set-theory.md#lower-shadow), take $a_r$ maximal with $\binom{a_r}{r}\leq m$. All $r$-sets of $[a_r]$ occur first. The next block consists of [sets](../../../set.md) containing $a_r+1$ whose remaining $(r-1)$-set runs through the initial segment of length $m-\binom{a_r}{r}$. By [Pascal's identity](../../../combinatorics.md#pascal-s-rule), the remainder is smaller than $\binom{a_r}{r-1}$, so its next leading top index is strictly less than $a_r$. Repeating gives the stated unique [binomial representation](../../../combinatorics.md#combinatorial-number-system). The first block contributes all $\binom{a_r}{r-1}$ $(r-1)$-sets in $[a_r]$ to the [lower shadow](../../../extremal-set-theory.md#lower-shadow). Deleting $a_r+1$ from the next block contributes only [sets](../../../set.md) already counted; deleting another coordinate contributes $a_r+1$ joined to the [lower shadow](../../../extremal-set-theory.md#lower-shadow) of the smaller initial segment. This recursive decomposition gives exactly the displayed sum. The base $r=1$ has [lower shadow](../../../extremal-set-theory.md#lower-shadow) $\{\varnothing\}$ for every nonempty [set family](../../../extremal-set-theory.md#set-family). This completes the proof and the sharpness assertion.

Now let $\mathcal C$ be the [set family](../../../extremal-set-theory.md#set-family) of [vertex](../../../graph.md#vertex-graph-theory) [sets](../../../set.md) of the [graph](../../../graph.md)'s [cliques](../../../graph-theory.md#clique-graph-theory) of order four. Its twice-iterated [lower shadow](../../../extremal-set-theory.md#lower-shadow) consists of [edges](../../../graph-theory.md#edge-of-a-graph) of the [graph](../../../graph.md). If there were at least sixteen such copies, choose a sixteen-member subfamily. The relevant [binomial representation](../../../combinatorics.md#combinatorial-number-system) is

$$
16=\binom64+\binom33.
$$

The proved theorem gives at least $\binom63+\binom32=23$ triples in its first [lower shadow](../../../extremal-set-theory.md#lower-shadow). Apply it again to any twenty-three of those triples, using $23=\binom63+\binom32$. Their [edge](../../../graph-theory.md#edge-of-a-graph) [lower shadow](../../../extremal-set-theory.md#lower-shadow) has at least

$$
\binom62+\binom31=18
$$

members, contradicting the fifteen available [edges](../../../graph-theory.md#edge-of-a-graph). Conversely, the [complete graph](../../../graph-theory.md#complete-graph) $K_6$ has $\binom62=15$ [edges](../../../graph-theory.md#edge-of-a-graph) and $\binom64=15$ copies of $K_4$. Therefore **the maximum number of copies is exactly 15**.

## 2

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take the natural parameter range $1\leq t\leq r\leq n$ and admissible indices $0\leq i\leq r-t$. Larger indices give empty [set families](../../../extremal-set-theory.md#set-family). Write $q=r-t+1$ and [set](../../../set.md) $n_0=\infty$ when discussing the first interval. For the nontrivial interval calculation, $t>1$ and $n>2r-t+1$; all prefixes used below then lie inside the ground [set](../../../set.md).

To compare consecutive [complete-intersection candidate families](../../../extremal-set-theory.md#complete-intersection-candidate-family), put $a=t+2i$ and $b=t+i$. A [set](../../../set.md) in $\mathcal A_{i+1}\setminus\mathcal A_i$ has exactly $b-1$ points in $[a]$ and both of the next two points. A [set](../../../set.md) in $\mathcal A_i\setminus\mathcal A_{i+1}$ has exactly $b$ points in $[a]$ and neither next point. Therefore

$$
G_i=|\mathcal A_{i+1}\setminus\mathcal A_i|
=\binom{t+2i}{t+i-1}\binom{n-t-2i-2}{r-t-i-1},
$$



$$
L_i=|\mathcal A_i\setminus\mathcal A_{i+1}|
=\binom{t+2i}{t+i}\binom{n-t-2i-2}{r-t-i}.
$$

For $0\leq i<r-t$ these quantities are positive in the present range, and cancellation of [binomial coefficients](../../../combinatorics.md#binomial-coefficient) gives

$$
\frac{G_i}{L_i}
=\frac{(t+i)(r-t-i)}{(i+1)(n-r-i-1)}.
$$

The numerator minus the denominator is

$$
(i+1)(n_{i+1}-n),\qquad
n_{i+1}=q\left(2+\frac{t-1}{i+1}\right).
$$

Thus $|\mathcal A_{i+1}|$ is larger, equal or smaller than $|\mathcal A_i|$ according as $n$ is smaller, equal or larger than $n_{i+1}$. Since these thresholds decrease with the index, $n_{k+1}<n<n_k$ implies strict increase up to $\mathcal A_k$ and strict decrease thereafter:

$$
\boxed{\max_i|\mathcal A_i|=|\mathcal A_k|.}
$$

At an interior boundary $n=n_{k+1}$, the two consecutive maxima tie. The interval assertion concerns admissible $k$; taking $k>r-t$ would instead refer to an empty [set family](../../../extremal-set-theory.md#set-family) and is not a valid interpretation.

The [Ahlswede-Khachatrian theorem](../../../extremal-set-theory.md#ahlswede-khachatrian-theorem), in its [cardinality](../../../set-theory.md#cardinality) form, states

$$
\boxed{M(n,r,t)=\max_{0\leq i\leq r-t}|\mathcal A_i|.}
$$

Here $\mathcal A_i$ is interpreted exactly by its intersection with $[t+2i]$, even if that prefix extends beyond $[n]$. Its size can always be written with $m_i=\min\{n,t+2i\}$ as

$$
|\mathcal A_i|=\sum_{j=t+i}^{r}\binom{m_i}{j}\binom{n-m_i}{r-j},
$$

where impossible [binomial coefficients](../../../combinatorics.md#binomial-coefficient) are zero. When $n\leq2r-t$, the whole level is $t$-intersecting and the formula gives $M=\binom nr$. The nontrivial case has $n>2r-t$.

First, each candidate is a [t-intersecting family](../../../extremal-set-theory.md#t-intersecting-family): two members contain at least $2(t+i)-(t+2i)=t$ common points in the prefix. This proves the lower bound for $M$. We now prove the upper bound, using only the compression and generating-family facts expressly allowed in the question.

The first auxiliary fact is that the usual left [coordinate shifts of a set family](../../../extremal-set-theory.md#coordinate-shifts-of-a-set-family) preserve [cardinality](../../../set-theory.md#cardinality) and $t$-intersection. Iterating them produces a [left-compressed set family](../../../extremal-set-theory.md#left-compressed-set-family) of the same size. The shift $S_{ab}$ with $a<b$ replaces $b$ by $a$ only when $b$ is present, $a$ is absent, and the replacement is not already in the [set family](../../../extremal-set-theory.md#set-family). A [set family](../../../extremal-set-theory.md#set-family) is left-compressed when it is fixed by every such shift. Right compression is the reflected notion.

For the second auxiliary fact, a [generating family for a uniform set family](../../../extremal-set-theory.md#generating-family-for-a-uniform-set-family) $\mathcal G$ means a collection of [sets](../../../set.md) of size at most $r$ with

$$
\mathcal F=\{A\in[n]^{(r)}:G\subseteq A\text{ for some }G\in\mathcal G\}.
$$

The permitted [small-support generating lemma for extremal intersecting families](../../../extremal-set-theory.md#small-support-generating-lemma-for-extremal-intersecting-families) is this precise statement: if $\mathcal F$ is a maximum-cardinality left-compressed $t$-intersecting [set family](../../../extremal-set-theory.md#set-family), $n>2r-t$, and

$$
n>(r-t+1)\left(2+\frac{t-1}{j+1}\right)
\quad(j\geq0),
$$

then it has a generating [set family](../../../extremal-set-theory.md#set-family) supported on $[t+2j]$. Reflection gives the same assertion for a right-compressed extremal [set family](../../../extremal-set-theory.md#set-family), with the supporting interval at the right end. These two auxiliary results are being used as permitted lemmas; the extremal conclusion of the theorem is established in the remaining argument.

Choose a maximum left-compressed [set family](../../../extremal-set-theory.md#set-family) $\mathcal F$. Its complement [set family](../../../extremal-set-theory.md#set-family)

$$
\mathcal F^*=\{[n]\setminus A:A\in\mathcal F\}
$$

is right-compressed, has uniformity $r'=n-r$ and intersection parameter $t'=n-2r+t$, and is extremal for those parameters. Indeed

$$
|([n]\setminus A)\cap([n]\setminus B)|=n-2r+|A\cap B|,
$$

so complementation gives a cardinality-preserving bijection between the two classes of intersecting [set families](../../../extremal-set-theory.md#set-family). Notice that $r'-t'+1=q$ too.

We need a compatibility observation, which we prove. If $G$ generates $\mathcal F$ and $H$ generates $\mathcal F^*$, then

$$
\boxed{|G\cup H|\geq n-r+t.}
$$

Otherwise extend $G\cup H$ to a [set](../../../set.md) $T$ of size $n-r+t-1$. This size is at least both $r$ and $n-r$ because $n\geq2r-t+1$ and $t\geq1$. Choose an $r$-set $A\subseteq T$ containing $G$, and an $(n-r)$-set $B\subseteq T$ containing $H$. Their generating properties imply $A,[n]\setminus B\in\mathcal F$, but

$$
|A\cap([n]\setminus B)|=|A\cup B|-|B|
\leq(n-r+t-1)-(n-r)=t-1,
$$

a contradiction. This [compatibility bound for complementary generating families](../../../extremal-set-theory.md#compatibility-bound-for-complementary-generating-families) is the link between the two compression directions.

Suppose first that $t>1$ and $n>2r-t+1$ lies strictly between $n_{k+1}$ and $n_k$. Put $m=t+2k$ and $h=r-t-k$. The small-support lemma gives generators $\mathcal G$ for $\mathcal F$ supported on $[m]$. It also gives generators $\mathcal H$ for $\mathcal F^*$ supported on $[m+1,n]$. For completeness, the dual inequality required here is

$$
n>q\left(2+\frac{t'-1}{h+1}\right).
$$

Writing $D=n-2q$, it is equivalent to $kD<q(t-1)$, exactly the upper interval inequality $n<n_k$; for $k=0$ it follows from $t>1$. The dual support length is $t'+2h=n-m$.

Either every $G\in\mathcal G$ has $|G|\geq t+k$, or every $H\in\mathcal H$ has $|H|\geq n-r-k$. If neither assertion held, a pair of smaller generators would have union size at most

$$
(t+k-1)+(n-r-k-1)=n-r+t-2,
$$

contradicting the compatibility bound. In the first alternative, every member of $\mathcal F$ has at least $t+k$ points in $[m]$, so $\mathcal F\subseteq\mathcal A_k$. In the second alternative, each complement has at least $n-r-k$ points in $[m+1,n]$, leaving its original [set](../../../set.md) with at most $r-t-k$ points there; again $\mathcal F\subseteq\mathcal A_k$. Therefore $M\leq|\mathcal A_k|$, proving the theorem in every strict interval.

At an interior boundary $n=n_{k+1}$, with $0\leq k\leq r-t-1$, apply the small-support lemma at index $k+1$ to the original [set family](../../../extremal-set-theory.md#set-family), since $n>n_{k+2}$. Its generators are supported on $[t+2k+2]$. The dual generators are still supported on $[t+2k+1,n]$, by the same dual calculation with $h=r-t-k$. Either all original generators have size at least $t+k+1$, or all dual generators have size at least $n-r-k$: failure of both would give union size at most $n-r+t-1$, again impossible. The first alternative places $\mathcal F$ inside $\mathcal A_{k+1}$, and the second places it inside $\mathcal A_k$. The comparison already proved gives $|\mathcal A_k|=|\mathcal A_{k+1}|$, so the common size is $M$.

It remains to cover the endpoint cases, not to assume them implicitly. For $t=1$ and $n>2r$, the small-support lemma with $j=0$ puts an extremal left-compressed [set family](../../../extremal-set-theory.md#set-family)'s generators inside $\{1\}$. Its members must all contain one, giving $M\leq\binom{n-1}{r-1}$, attained by $\mathcal A_0$. For $t=1$, $n=2r$, at most one member of each complementary pair can occur, so $M\leq\tfrac12\binom{2r}{r}=\binom{2r-1}{r-1}$, again attained by $\mathcal A_0$. If $n<2r$, the whole level is intersecting.

For $t>1$ and $n=2r-t+1$, complementation changes the problem into a one-intersection problem with uniformity $q=r-t+1$. Since $n=2q+t-1>2q$, the preceding case gives

$$
M(n,r,t)=\binom{n-1}{q-1}=\binom{n-1}{r},
$$

attained by $\mathcal A_{r-t}$, the [set family](../../../extremal-set-theory.md#set-family) of $r$-sets avoiding the final point. For $n\leq2r-t$, every two $r$-sets meet in at least $2r-n\geq t$, so $M=\binom nr$ and $\mathcal A_{r-t}$ is the whole level. Finally, $t=r$ gives $M=1$ directly. These cases, the strict intervals and their boundaries cover all $1\leq t\leq r\leq n$, completing the proof of the stated maximum formula.

## 3

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An $r$-[uniform hypergraph](../../../hypergraph.md#uniform-hypergraph) is [strongly saturated with respect to a complete uniform hypergraph](../../../hypergraph.md#strong-saturation-of-a-uniform-hypergraph) of order $r+t$ if adding any missing [edge](../../../graph-theory.md#edge-of-a-graph) creates a new [complete uniform hypergraph](../../../hypergraph.md#complete-uniform-hypergraph) on $r+t$ [vertices](../../../graph.md#vertex-graph-theory) containing that [edge](../../../graph-theory.md#edge-of-a-graph). Equivalently, for every missing $r$-set $e$, there is an $(r+t)$-set $T\supseteq e$ for which all other $r$-subsets are [edges](../../../graph-theory.md#edge-of-a-graph). Existing complete subhypergraphs are allowed in this strong-saturation definition.

We prove the bound by an [exterior-power quotient bound for strong hypergraph saturation](../../../hypergraph.md#exterior-power-quotient-bound-for-strong-hypergraph-saturation). Assume $r,t\geq1$ and $n\geq r+t$. Let $V=\mathbb R^n$ with [basis](../../../vector-space.md#basis) $e_1,\ldots,e_n$. Choose distinct real numbers $a_1,\ldots,a_n$ and let $U$ be the kernel of the $t\times n$ matrix whose column $i$ is

$$
(1,a_i,\ldots,a_i^{t-1})^\mathsf T.
$$

Every $t$ columns are [linearly independent](../../../vector-space.md#linear-independence) by the [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant), so $\dim U=n-t$. Form the [quotient vector space](../../../vector-space.md#quotient-vector-space)

$$
W=\bigwedge^rV\big/\bigwedge^rU,\qquad
\dim W=\binom nr-\binom{n-t}{r}.
$$

For each $r$-set $e=\{i_1<\cdots<i_r\}$, let $v_e$ be the image in $W$ of the [exterior product](../../../linear-algebra.md#exterior-product) $e_{i_1}\wedge\cdots\wedge e_{i_r}$. These images [span](../../../vector-space.md#linear-span) $W$.

For an $(r+t)$-set $T$, let $V_T$ be its coordinate subspace. The matrix restricted to $T$ has rank $t$, so $U\cap V_T$ has [dimension](../../../vector-space.md#dimension-vector-space) $r$. The wedge of a [basis](../../../vector-space.md#basis) of this intersection is a nonzero vector

$$
\alpha_T=\sum_{e\in T^{(r)}}c_e\,e_{i_1}\wedge\cdots\wedge e_{i_r}
\quad\text{in }\bigwedge^rU.
$$

Every coefficient $c_e$ is nonzero. Indeed, projection from $U\cap V_T$ onto the $r$ coordinates in $e$ is an isomorphism: a vector in its kernel would be supported on $T\setminus e$, where the $t$ columns are independent, and hence would be zero. That projection's determinant is precisely the corresponding wedge coefficient. Thus, in the [quotient vector space](../../../vector-space.md#quotient-vector-space),

$$
\sum_{e\in T^{(r)}}c_e v_e=0\qquad(c_e\ne0).
$$

For a missing [edge](../../../graph-theory.md#edge-of-a-graph), choose its strong-saturation witness $T$. All other vectors in this relation come from present [edges](../../../graph-theory.md#edge-of-a-graph), so the missing [edge](../../../graph-theory.md#edge-of-a-graph)'s vector is in their [span](../../../vector-space.md#linear-span). Consequently the present-edge vectors already [span](../../../vector-space.md#linear-span) all of $W$. Their number is at least its [dimension](../../../vector-space.md#dimension-vector-space):

$$
\boxed{|E(H)|\geq\binom nr-\binom{n-t}{r}.}
$$

This is sharp. Take all $r$-sets that meet a fixed $t$-set $D$. A missing [edge](../../../graph-theory.md#edge-of-a-graph) $e$ is disjoint from $D$, and on $e\cup D$ every other $r$-set meets $D$; adding $e$ completes the required [clique](../../../graph-theory.md#clique-graph-theory). The number of [edges](../../../graph-theory.md#edge-of-a-graph) is exactly the boxed difference. If $r\leq n<r+t$, no missing [edge](../../../graph-theory.md#edge-of-a-graph) could have a witness, so a strongly saturated [hypergraph](../../../hypergraph.md) must be complete; the substantive construction above is for the usual range $n\geq r+t$.

For the set-pair problem, write $m=|I|$ and choose $x_i\in R_i\cap S_i$. If $i\ne j$, the cross-disjointness implies that $x_i$ is in neither $R_j$ nor $S_j$. In particular, the witnesses are distinct. Let $D=\{x_i:i\in I\}$; each $R_i$ and $S_i$ contains exactly its own witness from $D$.

Choose two different indices $i,j$. The [sets](../../../set.md) $R_i\setminus\{x_i\}$ and $S_j\setminus\{x_j\}$ are disjoint, lie outside $D$, and have sizes $r-1$ and $s-1$. Hence

$$
n-m\geq(r-1)+(s-1),\qquad
\boxed{|I|\leq n-r-s+2.}
$$

For equality, partition the ground [set](../../../set.md) into disjoint [sets](../../../set.md) $P,Q,D$ with sizes $r-1,s-1,n-r-s+2$, respectively, and enumerate $D$ as $x_1,\ldots,x_m$. [Set](../../../set.md)

$$
\boxed{R_i=P\cup\{x_i\},\qquad S_i=Q\cup\{x_i\}.}
$$

Then $R_i\cap S_j$ is $\{x_i\}$ for $i=j$ and empty otherwise. This realizes equality whenever the bound permits $m\geq2$. The argument is a [diagonal-intersection set-pair bound](../../../extremal-set-theory.md#diagonal-intersection-set-pair-bound), with no additional assumptions on intersections among the $R_i$ or among the $S_i$.

## 4

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [set family](../../../extremal-set-theory.md#set-family) [shatters a set](../../../extremal-set-theory.md#set-shattering) $Z$ when its traces on $Z$ include all of $\mathcal P(Z)$. The [Sauer-Shelah lemma](../../../foundations-of-mathematics.md#sauer-shelah-lemma) says that a [set family](../../../extremal-set-theory.md#set-family) $\mathcal F\subseteq\mathcal P([n])$ which shatters no $k$-set satisfies

$$
\boxed{|\mathcal F|\leq\sum_{i=0}^{k-1}\binom ni.}
$$

Equivalently, if $|\mathcal F|$ exceeds this sum, it shatters a $k$-set. [Binomial coefficients](../../../combinatorics.md#binomial-coefficient) with index greater than $n$ are zero; if $k>n$ the inequality reduces to the whole-power-set bound. The [VC dimension](../../../foundations-of-mathematics.md#vc-dimension) formulation puts $k=d+1$.

We give the full inductive proof. Split $\mathcal F$ according to the last coordinate, deleting that coordinate from the present section, and write these two [set families](../../../extremal-set-theory.md#set-family) on $[n-1]$ as $\mathcal F_0,\mathcal F_1$. Put

$$
\mathcal C=\mathcal F_0\cup\mathcal F_1,\qquad
\mathcal D=\mathcal F_0\cap\mathcal F_1.
$$

The [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) gives $|\mathcal F|=|\mathcal C|+|\mathcal D|$. If $\mathcal C$ shattered a $k$-set, then $\mathcal F$ would shatter it too. If $\mathcal D$ shattered a $(k-1)$-set $Z$, both versions of each required trace, with and without the last coordinate, would occur in $\mathcal F$, which would shatter $Z\cup\{n\}$. Thus the two [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) bounds apply:

$$
|\mathcal F|\leq\sum_{i=0}^{k-1}\binom{n-1}{i}
+\sum_{i=0}^{k-2}\binom{n-1}{i}
=\sum_{i=0}^{k-1}\binom ni,
$$

using [Pascal's identity](../../../combinatorics.md#pascal-s-rule). For $n=0$ the [set family](../../../extremal-set-theory.md#set-family) has at most one member. For $k=1$, the intersection section must be empty, since any nonempty [set family](../../../extremal-set-theory.md#set-family) shatters the empty [set](../../../set.md). These supply the [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) bases; the forbidden-empty-set case has an empty [set family](../../../extremal-set-theory.md#set-family) and an empty sum. Sharpness is attained by all [subsets](../../../set.md#subset) of size at most $k-1$, which cannot shatter a $k$-set.

Now fix $k\geq1$ in the infinite-ground-set problem. Choose, using the hypothesis with $2k$, a [set](../../../set.md) $Y$ of size $2k$ with at least $2^{2k-1}$ distinct traces. If its trace [set family](../../../extremal-set-theory.md#set-family) shattered no $k$-set, the [Sauer-Shelah lemma](../../../foundations-of-mathematics.md#sauer-shelah-lemma) would give

$$
|\mathcal A_{|Y}|\leq\sum_{i=0}^{k-1}\binom{2k}{i}
=\frac{2^{2k}-\binom{2k}{k}}2
<2^{2k-1},
$$

a contradiction. Therefore some $Z\subseteq Y$ of size $k$ is shattered by the trace [set family](../../../extremal-set-theory.md#set-family), and hence by $\mathcal A$ itself. Thus **every finite shattering size occurs**. The use of $2k$ makes the contradiction strict, even though the hypothesis only gives a half-power-set lower bound.

An infinite realization does not follow. For a concrete [unbounded finite shattering without an infinite universal trace](../../../extremal-set-theory.md#unbounded-finite-shattering-without-an-infinite-universal-trace) construction, partition $X=\mathbb N$ into disjoint finite blocks

$$
B_j=\left\{\frac{j(j-1)}2+1,\ldots,\frac{j(j+1)}2\right\},\qquad |B_j|=j,
$$

and take

$$
\boxed{\mathcal A=\bigcup_{j\geq1}\mathcal P(B_j).}
$$

Every member is finite. Given $k$, choose $Y=B_k$; its trace [set family](../../../extremal-set-theory.md#set-family) is the full [power set](../../../set.md#power-set), so it has $2^k\geq2^{k-1}$ members and is shattered. However, an infinite $Z$ cannot be contained in one finite block. Choose $x,y\in Z$ from different blocks. No member of $\mathcal A$ contains both, so $\{x,y\}$ is not a trace on $Z$. Consequently **there need not be an infinite $Z$ whose traces contain every finite [subset](../../../set.md#subset) of $Z$**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
