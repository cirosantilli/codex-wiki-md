# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper14.pdf)

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

Write $\binom{[n]}k$ for the $k$th [uniform layer of the Boolean cube](../../../extremal-set-theory.md#uniform-layer-of-the-boolean-cube). For $\mathcal F\subseteq\binom{[n]}k$, $1\leq k\leq n$, its [lower shadow](../../../extremal-set-theory.md#lower-shadow) is $\partial\mathcal F=\{B:|B|=k-1,\ B\subset A\text{ for some }A\in\mathcal F\}$. The [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) states

$$
\boxed{\frac{|\partial\mathcal F|}{\binom n{k-1}}\geq\frac{|\mathcal F|}{\binom nk}.}
$$

To prove it, count pairs $(B,A)$ with $A\in\mathcal F$, $B\subset A$ and $|B|=k-1$. Each $A$ contributes $k$ pairs; each member of the [lower shadow](../../../extremal-set-theory.md#lower-shadow) contributes at most $n-k+1$. Thus $k|\mathcal F|\leq(n-k+1)|\partial\mathcal F|$, which is exactly the displayed [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality). The corresponding [upper shadow](../../../extremal-set-theory.md#upper-shadow) inequality follows either by taking [complements](../../../set.md#complement-of-a-set) or by counting upward inclusion pairs.

For an [antichain](../../../extremal-set-theory.md#antichain) $\mathcal A\subseteq\mathcal P([n])$, put $\mathcal A_k=\mathcal A\cap\binom{[n]}k$. The [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality) is

$$
\boxed{\sum_{k=0}^n\frac{|\mathcal A_k|}{\binom nk}\leq1.}
$$

For the first proof, set $\mathcal B_n=\mathcal A_n$ and recursively $\mathcal B_k=\mathcal A_k\cup\partial\mathcal B_{k+1}$. Every member of $\mathcal B_{k+1}$ is a subset of an original member of $\mathcal A$ of size at least $k+1$. Consequently $\mathcal A_k$ and $\partial\mathcal B_{k+1}$ are disjoint: otherwise one original member would properly contain another, contradicting the [antichain](../../../extremal-set-theory.md#antichain) condition. The [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) now gives

$$
\frac{|\mathcal B_k|}{\binom nk}
\geq\frac{|\mathcal A_k|}{\binom nk}
+\frac{|\mathcal B_{k+1}|}{\binom n{k+1}}.
$$

Iterating down to $k=0$ bounds the desired sum by $|\mathcal B_0|\leq1$, proving the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality).

For the second proof, a [permutation](../../../combinatorics.md#permutation) $(i_1,\ldots,i_n)$ determines a [maximal chain in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) through the successive initial subsets $\varnothing,\{i_1\},\ldots,[n]$. A member $A$ of size $k$ lies on exactly $k!(n-k)!$ of these $n!$ [maximal chains in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice). An [antichain](../../../extremal-set-theory.md#antichain) meets each such [chain in a partially ordered set](../../../set.md#chain-in-a-partially-ordered-set) at most once. Counting its incidences with the [maximal chains in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) therefore yields $\sum_{A\in\mathcal A}|A|!(n-|A|)!\leq n!$. Division by $n!$ is the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality) again.

The [Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem) says that an [antichain](../../../extremal-set-theory.md#antichain) has at most $M=\binom n{\lfloor n/2\rfloor}$ members. Indeed $\binom nk\leq M$ for every $k$, so

$$
\frac{|\mathcal A|}{M}\leq\sum_k\frac{|\mathcal A_k|}{\binom nk}\leq1.
$$

The middle [uniform layer of the Boolean cube](../../../extremal-set-theory.md#uniform-layer-of-the-boolean-cube) attains the bound. For [equality in Sperner theorem](../../../extremal-set-theory.md#equality-in-sperner-theorem), equality throughout forces every member to lie in a layer of maximum size. If $n=2k$, this forces $\mathcal A=\binom{[n]}k$.

If $n=2k+1$, only ranks $k$ and $k+1$ are possible. Let $\mathcal L=\mathcal A_k$, $\mathcal U=\mathcal A_{k+1}$, and $\mathcal S=\nabla\mathcal L$ be the [upper shadow](../../../extremal-set-theory.md#upper-shadow). The [antichain](../../../extremal-set-theory.md#antichain) condition gives $\mathcal U\cap\mathcal S=\varnothing$. The [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) for the two equally sized middle layers gives $|\mathcal S|\geq|\mathcal L|$, while $|\mathcal L|+|\mathcal U|=M$ forces $|\mathcal S|=|\mathcal L|$ and $\mathcal U=\binom{[n]}{k+1}\setminus\mathcal S$.

Consider the inclusion [bipartite graph](../../../graph-theory.md#bipartite-graph) between these two middle layers. It is a $(k+1)$-[regular graph](../../../graph-theory.md#regular-graph). Since $|\mathcal S|=|\mathcal L|$, all $(k+1)|\mathcal S|$ edges incident to $\mathcal S$ must come from $\mathcal L$; there are no edges from its complement on the lower side into $\mathcal S$. This [bipartite graph](../../../graph-theory.md#bipartite-graph) is a [connected graph](../../../graph.md#connected-graph): any two $k$-subsets can be joined by single-element exchanges, and each exchange passes through their common $(k+1)$-superset; every upper vertex has a lower neighbour. For $k=0$ it is just one edge. Hence either $\mathcal L=\varnothing$ or $\mathcal L$ is the whole lower layer. We have proved the complete classification:

$$
\boxed{\mathcal A=\binom{[n]}{\lfloor n/2\rfloor}\quad\text{or}\quad\mathcal A=\binom{[n]}{\lceil n/2\rceil}.}
$$

The two possibilities coincide for even $n$; for $n=0$ the unique maximum [antichain](../../../extremal-set-theory.md#antichain) is $\{\varnothing\}$.

Finally enumerate the members of the [separating set system](../../../extremal-set-theory.md#separating-set-system) as $A_1,\ldots,A_m$ and encode each point $i\in[n]$ by $T_i=\{a\in[m]:i\in A_a\}$. Separation of the ordered pair $(i,j)$ means $T_i\setminus T_j\ne\varnothing$. Applying the hypothesis also to $(j,i)$ shows that the $n$ [sets](../../../set.md) $T_i$ are distinct and pairwise incomparable. They form an [antichain](../../../extremal-set-theory.md#antichain) in $\mathcal P([m])$, so the [Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem) immediately gives

$$
\boxed{n\leq\binom m{\lfloor m/2\rfloor}.}
$$

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem) asserts that, for $1\leq r<n/2$, every [intersecting family](../../../extremal-set-theory.md#intersecting-family) $\mathcal A\subseteq\binom{[n]}r$ satisfies

$$
\boxed{|\mathcal A|\leq\binom{n-1}{r-1}.}
$$

The bound is attained by the [set family](../../../extremal-set-theory.md#set-family) of all $r$-subsets containing one prescribed point. Here [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) means that $X<Y$ when the smallest element of their [symmetric difference](../../../set.md#symmetric-difference) belongs to $X$.

The first $M=\binom{n-1}{r-1}$ members in [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) are exactly those containing $1$. An initial segment longer than $M$ contains all of them and also the first member avoiding $1$, namely $B=\{2,\ldots,r+1\}$. There is an $r$-subset containing $1$ and disjoint from $B$: choose its other $r-1$ elements from $\{r+2,\ldots,n\}$, which has $n-r-1\geq r-1$ elements. Consequently any longer [lexicographic](../../../extremal-set-theory.md#lexicographic-order) initial segment fails to be an [intersecting family](../../../extremal-set-theory.md#intersecting-family). Thus preservation of the [intersection](../../../set.md#set-intersection) property upon replacing a [set family](../../../extremal-set-theory.md#set-family) by the equally large [lexicographic](../../../extremal-set-theory.md#lexicographic-order) initial segment proves the displayed bound.

Here is a direct [UV-compression](../../../extremal-set-theory.md#uv-compression) proof of that preservation statement. For disjoint nonempty [sets](../../../set.md) $U,V$ with $|U|=|V|$ and $\min U<\min V$, an eligible member $A$ contains $V$ and misses $U$; its proposed image is $A'=(A\setminus V)\cup U$. The [UV-compression](../../../extremal-set-theory.md#uv-compression) moves $A$ to $A'$ only if $A'$ is not already present. Each eligible pair is either kept as a pair or moved from its later to its earlier member, so this operation preserves cardinality and uniformity and strictly decreases the sum of [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) positions whenever it changes the [set family](../../../extremal-set-theory.md#set-family).

The essential [intersection-preserving lexicographic UV-compression](../../../extremal-set-theory.md#intersection-preserving-lexicographic-uv-compression) lemma is that this operation preserves an [intersecting family](../../../extremal-set-theory.md#intersecting-family) whenever all smaller lexicographically improving [UV-compressions](../../../extremal-set-theory.md#uv-compression) already leave that [set family](../../../extremal-set-theory.md#set-family) unchanged. Suppose instead that the compressed [set family](../../../extremal-set-theory.md#set-family) has disjoint members. At least one, say $A'$, must be newly moved. Both newly moved members would contain $U$, so the other, $B$, is a retained old member. Write $A=(A'\setminus U)\cup V$ for the old preimage. Since $A'\cap B=\varnothing$, we have $B\cap U=\varnothing$ and $(A\setminus V)\cap B=\varnothing$. Old intersectingness forces

$$
V'=V\cap B\ne\varnothing.
$$

If $V'=V$, then $B$ was eligible for the same [UV-compression](../../../extremal-set-theory.md#uv-compression). Since it was retained, $B'=(B\setminus V)\cup U$ was already present. But $A\cap B'=\varnothing$, contradicting old intersectingness.

Otherwise $0<|V'|<|V|$. Choose $U'\subset U$ with $|U'|=|V'|$ and $\min U\in U'$. This is a smaller improving pair, since $\min U'=\min U<\min V\leq\min V'$. The old member $A$ is eligible for its [UV-compression](../../../extremal-set-theory.md#uv-compression). The assumed stability therefore forces $A''=(A\setminus V')\cup U'$ to be present already. Yet its portion outside $V$ misses $B$, its remaining portion $V\setminus V'$ misses $B$, and $U'$ misses $B$. Thus $A''\cap B=\varnothing$, the required contradiction. This proves the lemma, including the size-one case, where only the first alternative can arise.

Starting with $\mathcal A$, repeatedly choose a changing improving [UV-compression](../../../extremal-set-theory.md#uv-compression) with the smallest possible $|U|$. The lemma applies at each step because every smaller improving [UV-compression](../../../extremal-set-theory.md#uv-compression) is then unchanged. Thus every intermediate [set family](../../../extremal-set-theory.md#set-family) is intersecting. The strictly decreasing nonnegative integer sum of [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) positions ensures termination. If the terminal [set family](../../../extremal-set-theory.md#set-family) were not an initial segment, there would be a missing $X$ earlier than a present $Y$. Taking $U=X\setminus Y$ and $V=Y\setminus X$ gives equally sized nonempty disjoint [sets](../../../set.md) with $\min U<\min V$, and moves $Y$ to the missing $X$. That contradicts termination. The terminal [set family](../../../extremal-set-theory.md#set-family) is therefore exactly the equally large [lexicographic](../../../extremal-set-theory.md#lexicographic-order) initial segment, and it is intersecting. **This proves the required lexicographic statement directly, and hence the [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem).**

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Identify the vertices of the [Boolean hypercube](../../../combinatorics.md#boolean-hypercube) $Q_n$ with subsets of $[n]$, adjacent when their [symmetric difference](../../../set.md#symmetric-difference) has size one. Write $N(\mathcal A)$ for the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood), including $\mathcal A$ itself. In [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube), smaller [sets](../../../set.md) come first, and equal-sized [sets](../../../set.md) are ordered by [lexicographic order](../../../extremal-set-theory.md#lexicographic-order): the least element of the [symmetric difference](../../../set.md#symmetric-difference) belongs to the earlier member. Let $I_m$ denote the first $m$ vertices. The [vertex-isoperimetric inequality in the discrete cube](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) states

$$
\boxed{|N(\mathcal A)|\geq|N(I_{|\mathcal A|})|\qquad(\mathcal A\subseteq Q_n).}
$$

Subtracting $|\mathcal A|$ gives the equivalent assertion for the external vertex boundary.

We first check that $N(I_m)$ is also an initial segment in [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube). Apart from the empty and full cases, $I_m$ consists of complete lower layers and a [lexicographic](../../../extremal-set-theory.md#lexicographic-order) initial segment $\mathcal F$ in its top rank $r$. Its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) contains all ranks at most $r$ and the [upper shadow](../../../extremal-set-theory.md#upper-shadow) $\nabla\mathcal F$ in rank $r+1$. This [upper shadow](../../../extremal-set-theory.md#upper-shadow) is [lexicographic](../../../extremal-set-theory.md#lexicographic-order) initial: an $(r+1)$-subset $C$ belongs to it precisely when its first $r$-subset in [lexicographic order](../../../extremal-set-theory.md#lexicographic-order), obtained by deleting its largest element, belongs to $\mathcal F$. Taking the first $r$ elements preserves weak [lexicographic order](../../../extremal-set-theory.md#lexicographic-order), proving the assertion. This also handles $r=0$, where $N(\{\varnothing\})$ consists of ranks zero and one.

We prove the [vertex-isoperimetric inequality in the discrete cube](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $n$, with $n=0,1$ immediate. Fix a coordinate $i$ and write $\mathcal A_0,\mathcal A_1\subseteq Q_{n-1}$ for the sections without and with $i$. The two sections of its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) are

$$
N(\mathcal A)_0=N(\mathcal A_0)\cup\mathcal A_1,\qquad
N(\mathcal A)_1=N(\mathcal A_1)\cup\mathcal A_0.
$$

A [simplicial section compression](../../../combinatorics.md#simplicial-section-compression) replaces $\mathcal A_j$ by the initial segment $I_{a_j}$ of size $a_j=|\mathcal A_j|$ in the other coordinates. By the preceding observation, both $N(I_{a_j})$ and $I_{a_{1-j}}$ are initial segments, so their union has size $\max\{|N(I_{a_j})|,a_{1-j}\}$. The [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) hypothesis gives

$$
\max\{|N(I_{a_j})|,a_{1-j}\}
\leq\max\{|N(\mathcal A_j)|,a_{1-j}\}
\leq|N(\mathcal A_j)\cup\mathcal A_{1-j}|.
$$

Adding the two section bounds proves that [simplicial section compression](../../../combinatorics.md#simplicial-section-compression) cannot increase the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood).

Apply changing [simplicial section compressions](../../../combinatorics.md#simplicial-section-compression) until none remains. The sum of the global [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube) positions strictly decreases at each step: within a section the order is exactly the restriction of the global order. Thus the procedure terminates at a [set family](../../../extremal-set-theory.md#set-family) $\mathcal B$ every coordinate section of which is initial. We now classify the possible [terminal families for simplicial section compression](../../../combinatorics.md#terminal-families-for-simplicial-section-compression), rather than assuming this terminal [set family](../../../extremal-set-theory.md#set-family) must be globally initial.

If $X<Y$, $X\notin\mathcal B$ and $Y\in\mathcal B$, then $X,Y$ cannot agree in any coordinate, since that coordinate section would have an omitted earlier member and an included later one. Therefore $Y=X^c$. Let $X$ be the first omitted vertex and $Y$ the last included vertex. If $\mathcal B$ is noninitial, $X<Y$ and $Y=X^c$. Any vertex $Z$ strictly between them would have to be included, since an omitted $Z$ paired with $Y$ would have to equal $Y^c=X$. But it would also have to be omitted, since an included $Z$ paired with $X$ would have to equal $X^c=Y$. Thus there is no such $Z$: $X,Y$ are consecutive complementary vertices. Everything before $X$ is included and everything after $Y$ omitted. Hence $\mathcal B$ is obtained from the initial segment of its size by replacing $X$ with its immediate successor $X^c$.

There are only two forms of this exception. If $n=2r+1$, consecutive complementary vertices must straddle ranks $r,r+1$; otherwise an intermediate rank or a further vertex in one of their ranks separates them. They are consequently

$$
X=\{r+2,\ldots,2r+1\},\qquad Y=\{1,\ldots,r+1\},
$$

with $X$ the last $r$-subset and $Y$ the first $(r+1)$-subset. The corresponding initial segment is all ranks at most $r$. For $r\geq1$, the omitted $X$ remains in $N(\mathcal B)$ through a lower neighbour, and every $(r+1)$-subset has at least two $r$-subsets, only one of which was omitted. Thus $N(\mathcal B)$ contains every rank at most $r+1$, namely $N(I_{|\mathcal B|})$. For $r=0$ both singleton [closed graph neighbourhoods](../../../graph-theory.md#closed-graph-neighbourhood) are the whole $Q_1$.

If $n=2r$, the two complementary vertices must both have rank $r$. The [complement](../../../set.md#complement-of-a-set) map reverses the [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) in that rank, so a consecutive complementary pair must be its central pair. Exactly half the $r$-subsets contain $1$, and all of those precede those missing $1$. Therefore the pair is

$$
X=\{1,r+2,\ldots,2r\},\qquad Y=\{2,\ldots,r+1\}.
$$

Here $I_{|\mathcal B|}$ comprises all ranks below $r$ and all $r$-subsets containing $1$. For $r\geq2$, $N(\mathcal B)$ contains every rank at most $r$, because all lower ranks were retained. Every $(r+1)$-subset containing $1$ has $r\geq2$ different $r$-subsets containing $1$, so deletion of the one member $X$ removes no vertex of the [upper shadow](../../../extremal-set-theory.md#upper-shadow). Consequently $N(\mathcal B)\supseteq N(I_{|\mathcal B|})$. For $r=1$, the two [closed graph neighbourhoods](../../../graph-theory.md#closed-graph-neighbourhood) both have size three in $Q_2$. These cases exhaust the exceptions. Since the successive [simplicial section compressions](../../../combinatorics.md#simplicial-section-compression) never increased the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood), this proves the [vertex-isoperimetric inequality in the discrete cube](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube).

The same argument gives all integer radii. Write $N^t$ for $t$ repetitions of the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood). Its application to an initial segment is again initial; the sizes of these initial segments are monotone in the original size. Inducting on $t$ therefore gives

$$
|N^t(\mathcal A)|\geq|N^t(I_{|\mathcal A|})|.
$$

For the concentration question, use uniform [probability measure](../../../probability-theory.md#probability-measure) on a finite [connected graph](../../../graph.md#connected-graph) and normalize its [graph distance](../../../graph-theory.md#distance-graph-theory) by its [graph diameter](../../../graph-theory.md#graph-diameter). A sequence is a [Lévy family of graphs](../../../probability-theory.md#levy-family-of-graphs) if, for every fixed $\varepsilon>0$ and $\delta>0$, the radius-$\varepsilon$ neighbourhood of every [set](../../../set.md) of measure at least $\delta$ has measure tending to one, uniformly over those [sets](../../../set.md). One may equivalently require this only for [sets](../../../set.md) of measure at least one half. To see the reverse implication, first the radius-$\varepsilon/2$ neighbourhood of every positive-density [set](../../../set.md) must eventually have measure greater than one half. Otherwise its [complement](../../../set.md#complement-of-a-set) has measure at least one half, while the radius-$\varepsilon/4$ neighbourhood of that [complement](../../../set.md#complement-of-a-set) misses the original positive-density [set](../../../set.md), contradicting the half-measure condition. Apply the half-measure condition once more to the radius-$\varepsilon/2$ neighbourhood, enlarging it by another $\varepsilon/2$, to obtain the full claim. The metric normalization is essential here.

For $Q_n$, the [graph diameter](../../../graph-theory.md#graph-diameter) is $n$. A uniformly chosen vertex has size $Z_n$ with [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) $\operatorname{Bin}(n,1/2)$, [expectation](../../../probability-theory.md#expected-value) $n/2$ and [variance](../../../variance.md) $n/4$. Fix $\delta>0$ and choose $C>0$ so that $1/(4C^2)<\delta$. By [Chebyshev's inequality](../../../probability-inequality.md#chebyshev-inequality),

$$
\Pr\{Z_n\leq n/2-C\sqrt n\}\leq\frac1{4C^2}<\delta.
$$

For sufficiently large $n$, put $k_n=\lfloor n/2-C\sqrt n\rfloor\geq0$. Every initial segment of measure at least $\delta$ contains the complete ranks through $k_n$. Its radius-$t$ [graph neighbourhood](../../../graph-theory.md#graph-neighbourhood) therefore contains every rank at most $k_n+t$. Taking $t=\lfloor\varepsilon n\rfloor$, the all-radius [vertex-isoperimetric inequality in the discrete cube](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) gives, uniformly for $|\mathcal A|\geq\delta2^n$,

$$
1-\frac{|N^t(\mathcal A)|}{2^n}
\leq\Pr\{Z_n>k_n+t\}
\leq\frac{n}{4(\varepsilon n-C\sqrt n-2)^2}\longrightarrow0.
$$

The last [Chebyshev's inequality](../../../probability-inequality.md#chebyshev-inequality) is used only when its denominator has positive square root. These are precisely the radius-$\varepsilon$ neighbourhoods in the normalized [graph distance](../../../graph-theory.md#distance-graph-theory). **The discrete cubes form a [Lévy family](../../../probability-theory.md#levy-family-of-graphs).** In fact, taking $t=\lfloor n^{3/4}\rfloor$ in the same bound makes the omitted measure $O(n^{-1/2})$ for each fixed $\delta$: a radius that is $o(n)$ already suffices.

For fixed $d\geq1$, the nearest-neighbour grid $[n]^d$ has [graph distance](../../../graph-theory.md#distance-graph-theory) $\sum_i|x_i-y_i|$ and [graph diameter](../../../graph-theory.md#graph-diameter) $d(n-1)$. Take the slab $\mathcal A_n=\{x:x_1\leq\lceil n/2\rceil\}$, whose uniform measure is at least one half. Its integer radius-$t$ [graph neighbourhood](../../../graph-theory.md#graph-neighbourhood) is exactly $\{x:x_1\leq\min(n,\lceil n/2\rceil+t)\}$: changing the first coordinate alone attains the minimum distance to the slab. For $0<\varepsilon<1/(2d)$ and $t=\lfloor\varepsilon d(n-1)\rfloor$, the omitted proportion tends to

$$
\boxed{\frac12-\varepsilon d>0.}
$$

Thus there is [failure of concentration in fixed-dimensional grids](../../../probability-theory.md#failure-of-concentration-in-fixed-dimensional-grids), and **the fixed-dimensional grids do not form a [Lévy family](../../../probability-theory.md#levy-family-of-graphs)** with normalized graph distance.

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) in its uniform form says: let $p$ be a [prime number](../../../number-theory.md#prime-number), let $L\subseteq\mathbb F_p$ have size $s\leq\min(k,n-k)$, and let $\mathcal F\subseteq\binom{[n]}k$ have $k\bmod p\notin L$, while $|A\cap B|\bmod p\in L$ for every distinct pair of members. Then

$$
\boxed{|\mathcal F|\leq\binom ns.}
$$

The modular-intersection, nonuniform form of the [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) is as follows. Let $p$ be a [prime number](../../../number-theory.md#prime-number), let $L\subseteq\mathbb F_p$ have $s$ elements, and let $\mathcal F\subseteq\mathcal P([n])$ satisfy $|A|\bmod p\notin L$ for each $A\in\mathcal F$, whereas $|A\cap B|\bmod p\in L$ for distinct $A,B\in\mathcal F$. Then

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^{\min(s,n)}\binom nj.}
$$

This [nonuniform Frankl-Wilson theorem](../../../extremal-set-theory.md#nonuniform-frankl-wilson-theorem) allows different sizes and different diagonal residues; in particular it applies when all sizes have one common residue outside $L$.

To prove it by the [polynomial method in combinatorics](../../../combinatorics.md#polynomial-method-in-combinatorics), work over the [finite field](../../../algebra.md#finite-field) $\mathbb F_p$ and associate to each member the [intersection polynomial](../../../combinatorics.md#intersection-polynomial)

$$
P_A(x_1,\ldots,x_n)=\prod_{\ell\in L}\left(\sum_{i\in A}x_i-\ell\right).
$$

Replace each positive power of $x_i$ in its expansion by $x_i$ to obtain its [multilinear reduction on the Boolean cube](../../../polynomial.md#multilinear-reduction-on-the-boolean-cube) $\widetilde P_A$. This preserves evaluation on every [characteristic vector](../../../extremal-set-theory.md#characteristic-vector-of-a-set), whose coordinates are zero or one, and leaves degree at most $s$. At the [characteristic vector](../../../extremal-set-theory.md#characteristic-vector-of-a-set) $\mathbf1_B$,

$$
\widetilde P_A(\mathbf1_B)=\prod_{\ell\in L}(|A\cap B|-\ell).
$$

It is zero for distinct $A,B$, and nonzero for $B=A$ by the diagonal hypothesis. If $\sum_{A\in\mathcal F}c_A\widetilde P_A=0$, evaluating at each $\mathbf1_B$ forces $c_B=0$. Thus the [multilinear polynomials](../../../polynomial.md#multilinear-polynomial) are [linearly independent](../../../vector-space.md#linear-independence). They belong to the [vector space](../../../vector-space.md) with [basis](../../../vector-space.md#basis) the square-free [monomials](../../../polynomial.md#monomial) $\prod_{i\in S}x_i$ for $|S|\leq s$, whose [dimension](../../../vector-space.md#dimension-vector-space) is the displayed sum. This proves the nonuniform form, including $s=0$, where distinct members are impossible and the empty product is one.

For the sharp uniform form, we need the [low-degree evaluation rank on a uniform layer](../../../extremal-set-theory.md#low-degree-evaluation-rank-on-a-uniform-layer). Form the integer [matrix](../../../vector-space.md#matrix) $M$ whose rows are indexed by $S\subseteq[n]$ with $|S|\leq s$, columns by $k$-subsets $T$, and entries $M_{S,T}=\mathbf1_{S\subseteq T}$. These are evaluations of the square-free [monomials](../../../polynomial.md#monomial). Over the [rational numbers](../../../number-theory.md#rational-number), the row of a $j$-subset $S$ satisfies

$$
\sum_{\substack{R\supseteq S\\|R|=s}}M_{R,T}
=\binom{k-j}{s-j}M_{S,T}\qquad\text{for every }T.
$$

Indeed, when $S\subseteq T$ the left side counts the $s$-subsets between $S$ and $T$, and otherwise both sides vanish. Since $s\leq k$, the coefficient is a positive integer. Thus the degree-$s$ rows span all the rows over the [rational numbers](../../../number-theory.md#rational-number), giving $\operatorname{rank}_{\mathbb Q}M\leq\binom ns$. Every square submatrix of larger size has integer [determinant](../../../linear-algebra.md#determinant) zero, so its [determinant](../../../linear-algebra.md#determinant) remains zero modulo $p$. Hence

$$
\operatorname{rank}_{\mathbb F_p}M\leq\operatorname{rank}_{\mathbb Q}M\leq\binom ns.
$$

This reduction of [matrix rank](../../../vector-space.md#matrix-rank) is the reason one must not try to divide by $\binom{k-j}{s-j}$ directly in $\mathbb F_p$.

The evaluations of the $\widetilde P_A$ on the $k$th [uniform layer of the Boolean cube](../../../extremal-set-theory.md#uniform-layer-of-the-boolean-cube) lie in the row [linear span](../../../vector-space.md#linear-span) of $M$ over $\mathbb F_p$. They are [linearly independent](../../../vector-space.md#linear-independence) as functions there, because restriction to the columns corresponding to $\mathcal F$ still gives the nonzero diagonal evaluation matrix. Their number is consequently at most $\binom ns$. This completes the proof of the uniform [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) as well.

For the odd-cardinality problem the sharper [Oddtown theorem](../../../extremal-set-theory.md#oddtown-theorem) follows directly from [linear algebra](../../../linear-algebra.md). Let $v_A=\mathbf1_A\in\mathbb F_2^n$ be the [characteristic vector](../../../extremal-set-theory.md#characteristic-vector-of-a-set). The parity conditions say

$$
v_A\cdot v_B=0\quad(A\ne B),\qquad v_A\cdot v_A=1.
$$

For any [linear combination](../../../vector-space.md#linear-combination) $\sum_A c_Av_A=0$, take its [dot product](../../../linear-algebra.md#dot-product) with $v_B$. All off-diagonal terms vanish, leaving $c_B=0$. Hence these vectors are [linearly independent](../../../vector-space.md#linear-independence) in an $n$-dimensional [vector space](../../../vector-space.md), giving

$$
\boxed{|\mathcal A|\leq n.}
$$

The singleton [sets](../../../set.md) show that the bound can be attained. Notice why the constant term in the general [nonuniform Frankl-Wilson theorem](../../../extremal-set-theory.md#nonuniform-frankl-wilson-theorem) is unnecessary here: these [dot products](../../../linear-algebra.md#dot-product) already give a diagonal evaluation matrix using only the $n$ coordinate functions.

For even $n$, partition $[n]$ into the pairs $\{1,2\},\{3,4\},\ldots,\{n-1,n\}$ and take every union of a selection of these pairs. This gives exactly $2^{n/2}$ distinct [sets](../../../set.md), including the empty [set](../../../set.md). Each has even size; every pairwise [intersection](../../../set.md#set-intersection) is again a union of entire pairs and therefore has even size. **This attains the proposed bound.**

For any [set family](../../../extremal-set-theory.md#set-family) satisfying the even-cardinality conditions, let $W$ be the [linear span](../../../vector-space.md#linear-span) of its [characteristic vectors](../../../extremal-set-theory.md#characteristic-vector-of-a-set) over $\mathbb F_2$. Now the self-[dot products](../../../linear-algebra.md#dot-product) vanish as well as the off-diagonal ones. By [bilinearity](../../../linear-algebra.md#bilinearity), $u\cdot v=0$ for all $u,v\in W$, so $W\subseteq W^\perp$: it is a [self-orthogonal binary subspace](../../../coding-theory.md#self-orthogonal-binary-subspace).

For completeness the standard [bilinear form](../../../linear-algebra.md#bilinear-form) on $\mathbb F_2^n$ is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form), because a vector orthogonal to every coordinate vector has every coordinate zero. Thus the map $v\mapsto(w\mapsto v\cdot w)$ from $\mathbb F_2^n$ onto the [dual space](../../../linear-algebra.md#dual-space) $W^*$ is surjective: every [linear functional](../../../linear-algebra.md#linear-functional) on $W$ extends to the whole [vector space](../../../vector-space.md) by extending a [basis](../../../vector-space.md#basis), and every such functional on $\mathbb F_2^n$ is a [dot product](../../../linear-algebra.md#dot-product) with a vector. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $W^\perp$. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) consequently gives $\dim W^\perp=n-\dim W$. The inclusion $W\subseteq W^\perp$ implies $\dim W\leq n/2$. Finally, distinct members have distinct [characteristic vectors](../../../extremal-set-theory.md#characteristic-vector-of-a-set), all in $W$, and a $k$-dimensional [vector space](../../../vector-space.md) over $\mathbb F_2$ has exactly $2^k$ elements. Therefore

$$
\boxed{|\mathcal A|\leq|W|=2^{\dim W}\leq2^{n/2}.}
$$

This proves the [Eventown theorem](../../../extremal-set-theory.md#eventown-theorem) and also explains the suggested [dimension](../../../vector-space.md#dimension-vector-space) contradiction if the [set family](../../../extremal-set-theory.md#set-family) had more than $2^{n/2}$ members.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
