# Paper 10

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_10.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_10.pdf)

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

Write $[n]^{(r)}$ for the rank-$r$ [uniform layer of the Boolean cube](../../../extremal-set-theory.md#uniform-layer-of-the-boolean-cube). For a [uniform set family](../../../extremal-set-theory.md#uniform-set-family) $\mathcal F\subseteq[n]^{(r)}$, with $1\leq r\leq n$, let $\partial\mathcal F$ be its [lower shadow](../../../extremal-set-theory.md#lower-shadow). The **[Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality)** is

$$
\boxed{\frac{|\partial\mathcal F|}{\binom n{r-1}}\geq\frac{|\mathcal F|}{\binom nr}}.
$$

For its proof, count incidences $(B,A)$ with $A\in\mathcal F$, $B\subset A$, and $|B|=r-1$. Each member of $\mathcal F$ contributes $r$ incidences, while each member of the [lower shadow](../../../extremal-set-theory.md#lower-shadow) contributes at most $n-r+1$. Thus $r|\mathcal F|\leq(n-r+1)|\partial\mathcal F|$, which is the displayed bound by the ratio of consecutive [binomial coefficients](../../../combinatorics.md#binomial-coefficient). Complementing every set gives the corresponding [upper shadow](../../../extremal-set-theory.md#upper-shadow) bound, $|\nabla\mathcal F|/\binom n{r+1}\geq|\mathcal F|/\binom nr$ for $r<n$.

For an [antichain](../../../extremal-set-theory.md#antichain) $\mathcal A$ in the [Boolean lattice](../../../extremal-set-theory.md#boolean-lattice), the **[LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality)** is

$$
\boxed{\sum_{r=0}^n\frac{|\mathcal A\cap[n]^{(r)}|}{\binom nr}\leq1}.
$$

Here is the proof using the [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality). Denote the rank-$r$ part by $\mathcal A_r$, and let $\mathcal D_r$ consist of the $r$-sets containing some member of $\mathcal A$ of size at most $r$. These families satisfy

$$
\mathcal D_r=\mathcal A_r\mathbin{\dot\cup}\nabla\mathcal D_{r-1}\quad(1\leq r\leq n),\qquad \mathcal D_0=\mathcal A_0.
$$

The union is disjoint because a member of the [antichain](../../../extremal-set-theory.md#antichain) cannot contain a strictly smaller member. Apply the [upper shadow](../../../extremal-set-theory.md#upper-shadow) form of the [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) to $\mathcal D_{r-1}$:

$$
\frac{|\mathcal D_r|}{\binom nr}\geq\frac{|\mathcal A_r|}{\binom nr}+\frac{|\mathcal D_{r-1}|}{\binom n{r-1}}.
$$

Iterating gives a bound for the entire sum by $|\mathcal D_n|/\binom nn\leq1$. This also covers the empty [antichain](../../../extremal-set-theory.md#antichain) and an [antichain](../../../extremal-set-theory.md#antichain) containing the empty set.

For the second proof, each [permutation](../../../combinatorics.md#permutation) of $[n]$ specifies a [maximal chain in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) by taking its successive prefixes. There are $n!$ such [maximal chains in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice), and a fixed $r$-set belongs to $r!(n-r)!$ of them. A [maximal chain in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) meets an [antichain](../../../extremal-set-theory.md#antichain) at most once. [Double counting](../../../combinatorics.md#double-counting-proof-technique) these incidences therefore gives $\sum_r|\mathcal A_r|r!(n-r)!\leq n!$, exactly the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality).

The **[Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem)** says that an [antichain](../../../extremal-set-theory.md#antichain) in $\mathcal P([n])$ has at most $\binom n{\lfloor n/2\rfloor}$ members; a full middle rank attains this bound. Indeed, every [binomial coefficient](../../../combinatorics.md#binomial-coefficient) $\binom nr$ is at most the central one, so the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality) gives

$$
\frac{|\mathcal A|}{\binom n{\lfloor n/2\rfloor}}\leq\sum_r\frac{|\mathcal A_r|}{\binom nr}\leq1.
$$

Now let $\mathcal F$ be an [intersection-free uniform set family](../../../extremal-set-theory.md#intersection-free-uniform-set-family). If it is empty, there is nothing to prove. Fix $X\in\mathcal F$ and consider the traces

$$
\mathcal T=\{X\cap A:A\in\mathcal F\setminus\{X\}\}\subseteq\mathcal P(X).
$$

If $A,B\ne X$ are distinct and $X\cap A\subseteq X\cap B$, then $X\cap A\subseteq B$. This contradicts the defining restriction on the three distinct members $X,A,B$. The intersection has size less than $r$, so it is a proper subset of $B$ even if the printed subset symbol is interpreted strictly. In particular, equal traces are impossible, and the traces form an [antichain](../../../extremal-set-theory.md#antichain). Thus $|\mathcal T|=|\mathcal F|-1$. Applying the [Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem) to the $r$-element ground set $X$ proves the [antichain trace bound for intersection-free families](../../../extremal-set-theory.md#antichain-trace-bound-for-intersection-free-families)

$$
\boxed{|\mathcal F|\leq1+\binom r{\lfloor r/2\rfloor}}.
$$

The argument also handles $r=0$: a [uniform set family](../../../extremal-set-theory.md#uniform-set-family) then has at most one member.

## 2

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The **[Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem)** states that a [colexicographic initial segment](../../../extremal-set-theory.md#colexicographic-initial-segment) minimizes the [lower shadow](../../../extremal-set-theory.md#lower-shadow) of a [uniform set family](../../../extremal-set-theory.md#uniform-set-family) of prescribed size. Its numerical form is as follows. For $m>0$, write the unique [combinatorial number system](../../../combinatorics.md#combinatorial-number-system) expansion

$$
m=\binom{a_r}r+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}s,\qquad a_r>a_{r-1}>\cdots>a_s\geq s\geq1.
$$

Every $\mathcal F\subseteq[n]^{(r)}$ of size $m$ satisfies

$$
\boxed{|\partial\mathcal F|\geq\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}}.
$$

The empty family has empty [lower shadow](../../../extremal-set-theory.md#lower-shadow). Equality is attained by the first $m$ $r$-sets in [colexicographic order](../../../extremal-set-theory.md#colexicographic-order), where the largest differing element belongs to the later set. Iterating the [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem) shows that the same [colexicographic initial segment](../../../extremal-set-theory.md#colexicographic-initial-segment) minimizes every [iterated lower shadow](../../../extremal-set-theory.md#iterated-lower-shadow).

For $1\leq r<n/2$, the **[Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem)** gives

$$
\boxed{|\mathcal F|\leq\binom{n-1}{r-1}}
$$

for an [intersecting family](../../../extremal-set-theory.md#intersecting-family) $\mathcal F\subseteq[n]^{(r)}$. All $r$-sets containing one prescribed point show that the bound is sharp.

For the proof from the [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem), put $k=n-r$ and form the complement family $\mathcal G=\{[n]\setminus A:A\in\mathcal F\}\subseteq[n]^{(k)}$. Let $\mathcal S$ be its rank-$r$ [iterated lower shadow](../../../extremal-set-theory.md#iterated-lower-shadow). No member $B\in\mathcal F$ belongs to $\mathcal S$: containment in $[n]\setminus A$ would give $A\cap B=\varnothing$, impossible for an [intersecting family](../../../extremal-set-theory.md#intersecting-family) of nonempty sets. Hence

$$
|\mathcal F|+|\mathcal S|\leq\binom nr.
$$

Suppose $|\mathcal F|>\binom{n-1}{r-1}=\binom{n-1}k$. The first $\binom{n-1}k$ members of the [colexicographic order](../../../extremal-set-theory.md#colexicographic-order) are all $k$-sets of $[n-1]$. Their rank-$r$ [iterated lower shadow](../../../extremal-set-theory.md#iterated-lower-shadow) is all $r$-sets of $[n-1]$, since $r<k$. The next $k$-set contains $n$ and has an $r$-subset containing $n$, so taking even one more member strictly enlarges that [iterated lower shadow](../../../extremal-set-theory.md#iterated-lower-shadow). By the iterated [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem), $|\mathcal S|>\binom{n-1}r$. Together with $|\mathcal F|>\binom{n-1}{r-1}$ this contradicts [Pascal's identity](../../../combinatorics.md#pascal-s-rule) and the preceding inequality. This proves the [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem).

For the [Katona circle method](../../../extremal-set-theory.md#katona-circle-method) proof, fix a [cyclic ordering](../../../combinatorics.md#cyclic-ordering) of $[n]$. A [cyclic interval](../../../combinatorics.md#cyclic-interval) of length $r$ is specified by its final position. If no such interval belongs to $\mathcal F$, the bound below is automatic. Otherwise rotate one selected interval so that it ends at position $n$, and thus occupies positions $n-r+1,\ldots,n$. Intervals ending at positions $r,\ldots,n-r$ are disjoint from it and cannot be selected. Among the remaining endpoints, pair $j$ with $n-r+j$ for $1\leq j\leq r-1$. The corresponding intervals are disjoint when $n\geq2r$, so at most one interval per pair is selected. Together with the interval ending at $n$, this gives the [cyclic interval intersection bound](../../../extremal-set-theory.md#cyclic-interval-intersection-bound) of $r$ selected intervals.

Choose a uniformly random [permutation](../../../combinatorics.md#permutation) and read its positions cyclically. A fixed $r$-set is a [cyclic interval](../../../combinatorics.md#cyclic-interval) with probability $n/\binom nr$: each cyclic position gives a uniformly distributed $r$-set, and for $r<n$ the $n$ intervals are distinct. Summing over $\mathcal F$, the [expected value](../../../probability-theory.md#expected-value) of the number of selected intervals is $n|\mathcal F|/\binom nr$. The [cyclic interval intersection bound](../../../extremal-set-theory.md#cyclic-interval-intersection-bound) makes this at most $r$, giving $|\mathcal F|\leq(r/n)\binom nr=\binom{n-1}{r-1}$.

Finally apply the [Katona circle method](../../../extremal-set-theory.md#katona-circle-method) to an arbitrary [antichain](../../../extremal-set-theory.md#antichain) $\mathcal A$. If it contains $\varnothing$ or $[n]$, it has exactly one member and the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality) holds with equality. Otherwise all its members have sizes $1,\ldots,n-1$. In a fixed [cyclic ordering](../../../combinatorics.md#cyclic-ordering), the [cyclic intervals](../../../combinatorics.md#cyclic-interval) sharing a final position form a nested chain as their lengths increase. At most one of them can belong to the [antichain](../../../extremal-set-theory.md#antichain). Summing over the $n$ final positions proves the [cyclic interval antichain bound](../../../extremal-set-theory.md#cyclic-interval-antichain-bound) of $n$ intervals. Taking the [expected value](../../../probability-theory.md#expected-value) over a uniformly random [permutation](../../../combinatorics.md#permutation) gives

$$
n\sum_{r=1}^{n-1}\frac{|\mathcal A\cap[n]^{(r)}|}{\binom nr}\leq n.
$$

After division by $n$, this is **the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality) proved by cyclic intervals**. The case $n=0$ consists only of the empty set and is immediate.

## 3

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Identify the [hypercube graph](../../../graph.md#hypercube-graph) $Q_n$ with $\mathcal P([n])$, joining two sets when their [symmetric difference](../../../set.md#symmetric-difference) has size one. Write $N[A]$ for the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) of $A$, and $N_t[A]$ for its radius-$t$ neighbourhood in [Hamming distance](../../../coding-theory.md#hamming-distance). In the [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube), smaller sets come first, with [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) within each rank: the smallest differing coordinate belongs to the earlier set. Let $I_m$ be the first $m$ vertices in this order. **[Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube)** is

$$
\boxed{|N[A]|\geq|N[I_{|A|}]|}.
$$

Equivalently, $I_m$ minimizes the [external vertex boundary](../../../graph-theory.md#external-vertex-boundary) at fixed size. We will also obtain $|N_t[A]|\geq|N_t[I_{|A|}]|$ for every integer $t\geq0$.

Here is a complete proof by [simplicial section compression](../../../combinatorics.md#simplicial-section-compression). First note two properties of the [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube). Its restriction to either face obtained by fixing one coordinate is the corresponding order on the smaller [hypercube graph](../../../graph.md#hypercube-graph). Also, the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) of an [initial segment](../../../set.md#initial-segment) is an [initial segment](../../../set.md#initial-segment). To verify the latter, a nonempty [initial segment](../../../set.md#initial-segment) contains every level below its last level $r$, and a [lexicographic](../../../extremal-set-theory.md#lexicographic-order) prefix $\mathcal L$ at level $r$. For $r\geq1$, its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) contains every set of size at most $r$, and its only further members are the [upper shadow](../../../extremal-set-theory.md#upper-shadow) of $\mathcal L$. An $(r+1)$-set lies in this [upper shadow](../../../extremal-set-theory.md#upper-shadow) exactly when its lexicographically earliest $r$-subset lies in $\mathcal L$. That earliest subset is obtained by deleting the largest element. These earliest subsets vary monotonically in [lexicographic order](../../../extremal-set-theory.md#lexicographic-order), so the [upper shadow](../../../extremal-set-theory.md#upper-shadow) is another [lexicographic](../../../extremal-set-theory.md#lexicographic-order) prefix. For $r=0$, the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) of $\{\varnothing\}$ is the union of levels zero and one. The empty [initial segment](../../../set.md#initial-segment) causes no exception.

Induct on $n$, with $n=0,1$ immediate. Fix a coordinate $i$ and write the sections of $A$ as $A_0,A_1\subseteq Q_{n-1}$, deleting $i$ from the latter section. Replace them by the [initial segments](../../../set.md#initial-segment) $I_a,I_b$ with $a=|A_0|$, $b=|A_1|$. The sections of the old [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) are

$$
(N[A])_0=N[A_0]\cup A_1,\qquad (N[A])_1=N[A_1]\cup A_0.
$$

By induction their sizes are at least $\max\{|N[I_a]|,b\}$ and $\max\{|N[I_b]|,a\}$, respectively. These are exactly the sizes of the new sections, because both sets in each new union are [initial segments](../../../set.md#initial-segment) and hence nested. Thus [simplicial section compression](../../../combinatorics.md#simplicial-section-compression) preserves size and never enlarges the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood).

Repeatedly compress any section that is not already an [initial segment](../../../set.md#initial-segment). Every change strictly reduces the sum of the global simplicial positions of the included vertices. This nonnegative integer decreases only finitely often, so the process ends at a family $B$ whose sections in every coordinate are [initial segments](../../../set.md#initial-segment). If $B$ itself is an [initial segment](../../../set.md#initial-segment), the induction is complete. Otherwise choose the earliest absent vertex $X$ and the latest present vertex $Y$, with $X\prec Y$. They cannot agree in any coordinate: agreement would put them in one compressed section, where an earlier absent vertex cannot precede a later present one. Hence $Y=X^c$. Nor can a vertex $Z$ lie between them: if $Z$ is present, pairing it with $X$ would force $Z=X^c=Y$; if absent, pairing it with $Y$ would force $Z=Y^c=X$. Thus $X,Y$ are consecutive, and $B$ is obtained from $I_{|B|}$ by replacing its last vertex $X$ with the next vertex $Y$.

There are only two possibilities for these [terminal families for simplicial section compression](../../../combinatorics.md#terminal-families-for-simplicial-section-compression). If $|X|<|Y|$, consecutiveness makes $X$ the last $k$-set and $Y$ the first $(k+1)$-set. Complementarity forces $n=2k+1$, $X=\{k+2,\ldots,2k+1\}$ and $Y=\{1,\ldots,k+1\}$. For $n\geq3$, the corresponding $B$ contains all sets of size at most $k$ except $X$, and additionally $Y$. Every $(k+1)$-set has at least two $k$-subsets, so at least one belongs to $B$. The missing $X$ has a $(k-1)$-subset in $B$. Consequently $N[B]$ contains every set of size at most $k+1$, which is exactly $N[I_{|B|}]$.

If $|X|=|Y|$, then $n=2k$. Since $X,Y$ are complementary, the smaller one contains coordinate $1$. Consecutiveness forces $X$ to be the last $k$-set containing $1$, and $Y$ the first $k$-set avoiding $1$:

$$
X=\{1,k+2,\ldots,2k\},\qquad Y=\{2,\ldots,k+1\}.
$$

The [initial segment](../../../set.md#initial-segment) consists of all sets of size less than $k$ and all $k$-sets containing $1$. Its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) contains all sets of size at most $k$ and all $(k+1)$-sets containing $1$. For $k\geq2$, each such $(k+1)$-set has $k\geq2$ $k$-subsets containing $1$, so removing only $X$ leaves one in $B$. All sets of size at most $k$ are still in $N[B]$, because all levels below $k$ belong to $B$. Hence again $N[I_{|B|}]\subseteq N[B]$. For $k=1$, the two families are related by exchanging coordinates and both have the whole $Q_2$ as their [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood). These comparisons finish the induction and prove [Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube).

For the radius-$t$ version, repeatedly use the one-step result. At each step the comparison family remains an [initial segment](../../../set.md#initial-segment), and its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) is monotone in its size. If $|N_{t-1}[A]|\geq|N_{t-1}[I_m]|$, applying [Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) to $N_{t-1}[A]$ therefore gives $|N_t[A]|\geq|N_t[I_m]|$. Induction on $t$ proves the asserted extension.

A **[Lévy family of graphs](../../../probability-theory.md#levy-family-of-graphs)** has vanishing [concentration of measure](../../../probability-theory.md#concentration-of-measure) functions after distances have been scaled by the graph diameter. More explicitly, for connected finite [graphs](../../../graph.md) $G_n$ of diameter $D_n$, use normalized [graph distance](../../../graph-theory.md#distance-graph-theory) $d_n=d_{G_n}/D_n$ and uniform [probability measure](../../../probability-theory.md#probability-measure). For every fixed $\varepsilon>0$, require

$$
\alpha_n(\varepsilon):=\sup_{|A|\geq|V(G_n)|/2}\left(1-\frac{|N_{\lfloor\varepsilon D_n\rfloor}[A]|}{|V(G_n)|}\right)\longrightarrow0.
$$

For $Q_n$ this normalization is [normalized Hamming distance](../../../coding-theory.md#normalized-hamming-distance) $d_H/n$, since its diameter is $n$.

If $|A|\geq2^{n-1}$, the corresponding [initial segment](../../../set.md#initial-segment) contains the [Hamming ball](../../../coding-theory.md#hamming-ball) about $\varnothing$ of radius $b_n=\lfloor(n-1)/2\rfloor$. The radius-$t$ version of [Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) implies

$$
1-\frac{|N_t[A]|}{2^n}\leq\mathbb P\{Z_n>b_n+t\},\qquad Z_n\sim\operatorname{Bin}(n,1/2).
$$

Use the precise [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) $\mathbb P(Z_n-n/2\geq u)\leq\exp(-2u^2/n)$ for $u\geq0$. One can also derive this estimate directly: the [moment-generating function](../../../probability-theory.md#moment-generating-function) of $Z_n-n/2$ is $\cosh(\lambda/2)^n\leq\exp(n\lambda^2/8)$; the exponential [Markov inequality](../../../probability-inequality.md#markov-inequality) followed by minimization at $\lambda=4u/n$ gives the bound. With $t=\lfloor\varepsilon n\rfloor$, we have $b_n+t\geq n/2+\varepsilon n-2$. Thus, whenever $\varepsilon n>2$,

$$
\boxed{\alpha_n(\varepsilon)\leq\exp\left(-\frac{2(\varepsilon n-2)^2}{n}\right)\longrightarrow0}.
$$

This proves that the [hypercube graphs](../../../graph.md#hypercube-graph) form a [Lévy family of graphs](../../../probability-theory.md#levy-family-of-graphs). The stronger fixed-positive-mass formulation follows as well. For any $a>0$, choose $c$ with $1/(4c^2)<a$. The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) for $Z_n$, whose [variance](../../../variance.md) is $n/4$, makes the [Hamming ball](../../../coding-theory.md#hamming-ball) of radius $\lfloor n/2-c\sqrt n\rfloor$ have fewer than $a2^n$ vertices. An [initial segment](../../../set.md#initial-segment) of size at least $a2^n$ contains that ball. Enlarging by $\lfloor\varepsilon n\rfloor$ and using the same [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) gives a complement proportion tending to zero uniformly over all such $A$. The normalization matters: with unscaled unit [Hamming distance](../../../coding-theory.md#hamming-distance), cubes do not satisfy the metric version at every fixed radius; for a radius below one, a half-cube has no enlargement.

**Equality in [Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) does not determine a [down-set](../../../extremal-set-theory.md#down-set) up to isomorphism.** In $Q_4$, take

$$
A=\{\varnothing,\{1\},\{2\},\{3\},\{4\},\{1,2\},\{2,3\},\{3,4\},\{1,4\}\}.
$$

This is a [down-set](../../../extremal-set-theory.md#down-set) of size nine. Its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) contains every set of size at most two, because all singletons belong to $A$. Every triple contains an edge of the four-cycle among the listed pairs, so every triple also belongs to $N[A]$. The four-element set does not. Hence $|N[A]|=1+4+6+4=15$.

The size-nine [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube) [initial segment](../../../set.md#initial-segment) is all sets of size at most one together with the pairs $12,13,14,23$. Every triple contains one of these pairs, and the four-element set is again absent from its [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood). Its neighbourhood therefore also has size $15$, proving extremality of $A$. Nevertheless the induced [graphs](../../../graph.md) are not isomorphic: in $A$, the empty set has degree four, the four singletons have degree three, and the four pairs have degree two. The [initial segment](../../../set.md#initial-segment) has two vertices of degree four, namely $\varnothing$ and $\{1\}$. Since a [graph automorphism](../../../graph.md#graph-automorphism) preserves induced [degree of a vertex](../../../graph-theory.md#degree-graph-theory), no automorphism of the cube can carry one family to the other. This gives **[nonunique down-set extremizers for Harper theorem](../../../combinatorics.md#nonunique-down-set-extremizers-for-harper-theorem)** even under the stronger test of induced graph isomorphism.

## 4

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The general modular form, the **[nonuniform Frankl-Wilson theorem](../../../extremal-set-theory.md#nonuniform-frankl-wilson-theorem)**, can be stated as follows. Let $p$ be a [prime number](../../../number-theory.md#prime-number), and let $L\subseteq\mathbb F_p$ have $s$ elements. Suppose $\mathcal F\subseteq\mathcal P([n])$ has $|A|\bmod p\notin L$ for every member, while $|A\cap B|\bmod p\in L$ for any distinct members. Then

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^{\min(s,n)}\binom nj}.
$$

The uniform [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) sharpens this to $|\mathcal F|\leq\binom ns$ when all members have size $k$ and $0\leq s\leq\min\{k,n-k\}$. Both forms require a prime modulus and exclusion of the self-intersection residue.

For the general proof, work over the [finite field](../../../algebra.md#finite-field) $\mathbb F_p$. Associate to each member $A$ the [intersection polynomial](../../../combinatorics.md#intersection-polynomial)

$$
f_A(x)=\prod_{\ell\in L}\left(\sum_{i\in A}x_i-\ell\right).
$$

At the [characteristic vectors of sets](../../../extremal-set-theory.md#characteristic-vector-of-a-set) $\mathbf1_B$, this is zero if $B\ne A$, and nonzero if $B=A$. Thus these [polynomials](../../../polynomial.md), regarded as functions on the [Boolean hypercube](../../../combinatorics.md#boolean-hypercube), are [linearly independent](../../../vector-space.md#linear-independence): evaluating any relation at $\mathbf1_A$ isolates its coefficient. Apply [multilinear reduction on the Boolean cube](../../../polynomial.md#multilinear-reduction-on-the-boolean-cube), replacing every positive power of a variable by that variable. Values on the [Boolean hypercube](../../../combinatorics.md#boolean-hypercube) remain unchanged, and the resulting [multilinear polynomials](../../../polynomial.md#multilinear-polynomial) have degree at most $s$. Their ambient space has a [monomial basis](../../../vector-space.md#monomial-basis) consisting of $x_S=\prod_{i\in S}x_i$ for $|S|\leq s$, with dimension $\sum_{j=0}^{\min(s,n)}\binom nj$. This proves the general bound, including $s=0$.

For completeness, obtain the uniform sharpening without dividing by factorials in a [finite field](../../../algebra.md#finite-field). For $s\geq1$ put $a=k\bmod p$ and $g(x)=\sum_i x_i-a$. The functions $x_Sg$ with $|S|<s$ are [linearly independent](../../../vector-space.md#linear-independence). Indeed, a relation gives $gh=0$ with $\deg h<s$, so $h$ is supported only on weights in $H=\{j\in[0,n]:j\equiv a\pmod p\}$. With boundary weights $-1,n+1$, this set has a gap of at least $s+1$: either consecutive allowed weights differ by $p\geq s+1$, or its terminal gap does, since $n\geq k+s\geq a+s$. The alternating sum of $h$ over any interval of $s$ free coordinates vanishes by its degree. Across that gap only one endpoint level can contribute, forcing $h$ to vanish there. Delete that level and repeat across the enlarged gap until $H$ is empty. Hence $h=0$, and independence of the square-free [monomials](../../../polynomial.md#monomial) gives the claim. Adjoin these functions to the $f_A$. Evaluation at each family vector eliminates the coefficients of $f_A$, since $g$ vanishes there; the claim eliminates all remaining coefficients. Counting dimensions yields

$$
|\mathcal F|+\sum_{j=0}^{s-1}\binom nj\leq\sum_{j=0}^s\binom nj,\qquad\boxed{|\mathcal F|\leq\binom ns}.
$$

The case $s=0$ permits at most one member directly. The gap argument is an instance of the [modular layer vanishing lemma](../../../extremal-set-theory.md#modular-layer-vanishing-lemma).

For the final application, enumerate the distinct sets as $A_1,\ldots,A_m$ and let $v_i=\mathbf1_{A_i}\in\mathbb R^n$ be their [characteristic vectors of sets](../../../extremal-set-theory.md#characteristic-vector-of-a-set). If $m\leq1$, the desired bound is immediate for $n\geq1$. Otherwise $|A_i|\geq k$, because $A_i$ intersects another member in $k$ points. At most one member can have size $k$: two distinct $k$-sets cannot have intersection size $k$. The [Gram matrix](../../../linear-algebra.md#gram-matrix) of these vectors is

$$
G=k\mathbf1\mathbf1^{\mathsf T}+\operatorname{diag}(|A_1|-k,\ldots,|A_m|-k).
$$

For real coefficients $c_i$,

$$
\left\|\sum_i c_iv_i\right\|^2=c^{\mathsf T}Gc=k\left(\sum_i c_i\right)^2+\sum_i(|A_i|-k)c_i^2.
$$

All terms are nonnegative, with $k>0$. If the expression vanishes, every coefficient corresponding to a set of size greater than $k$ is zero. At most one coefficient remains, and the first term forces it to be zero as well. Thus the [characteristic vectors of sets](../../../extremal-set-theory.md#characteristic-vector-of-a-set) are [linearly independent](../../../vector-space.md#linear-independence) in $\mathbb R^n$, proving the **[constant-intersection family bound](../../../extremal-set-theory.md#constant-intersection-family-bound)**

$$
\boxed{m\leq n}.
$$

This proof explicitly covers the possible member of size exactly $k$; assuming all diagonal corrections were strictly positive would miss that case. Positivity of $k$ is essential: when $k=0$, the empty set and all $n$ singleton sets give $n+1$ members.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
