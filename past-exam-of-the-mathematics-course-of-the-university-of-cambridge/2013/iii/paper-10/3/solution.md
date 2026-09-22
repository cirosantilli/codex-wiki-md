<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Identify the [hypercube graph](../../../../../hypercube-graph.md) $Q_n$ with $\mathcal P([n])$, joining two sets when their [symmetric difference](../../../../../symmetric-difference.md) has size one. Write $N[A]$ for the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) of $A$, and $N_t[A]$ for its radius-$t$ neighbourhood in [Hamming distance](../../../../../hamming-distance.md). In the [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md), smaller sets come first, with [lexicographic order](../../../../../lexicographic-order.md) within each rank: the smallest differing coordinate belongs to the earlier set. Let $I_m$ be the first $m$ vertices in this order. **[Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md)** is

$$
\boxed{|N[A]|\geq|N[I_{|A|}]|}.
$$

Equivalently, $I_m$ minimizes the [external vertex boundary](../../../../../external-vertex-boundary.md) at fixed size. We will also obtain $|N_t[A]|\geq|N_t[I_{|A|}]|$ for every integer $t\geq0$.

Here is a complete proof by [simplicial section compression](../../../../../simplicial-section-compression.md). First note two properties of the [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md). Its restriction to either face obtained by fixing one coordinate is the corresponding order on the smaller [hypercube graph](../../../../../hypercube-graph.md). Also, the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) of an [initial segment](../../../../../initial-segment.md) is an [initial segment](../../../../../initial-segment.md). To verify the latter, a nonempty [initial segment](../../../../../initial-segment.md) contains every level below its last level $r$, and a [lexicographic](../../../../../lexicographic-order.md) prefix $\mathcal L$ at level $r$. For $r\geq1$, its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) contains every set of size at most $r$, and its only further members are the [upper shadow](../../../../../upper-shadow.md) of $\mathcal L$. An $(r+1)$-set lies in this [upper shadow](../../../../../upper-shadow.md) exactly when its lexicographically earliest $r$-subset lies in $\mathcal L$. That earliest subset is obtained by deleting the largest element. These earliest subsets vary monotonically in [lexicographic order](../../../../../lexicographic-order.md), so the [upper shadow](../../../../../upper-shadow.md) is another [lexicographic](../../../../../lexicographic-order.md) prefix. For $r=0$, the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) of $\{\varnothing\}$ is the union of levels zero and one. The empty [initial segment](../../../../../initial-segment.md) causes no exception.

Induct on $n$, with $n=0,1$ immediate. Fix a coordinate $i$ and write the sections of $A$ as $A_0,A_1\subseteq Q_{n-1}$, deleting $i$ from the latter section. Replace them by the [initial segments](../../../../../initial-segment.md) $I_a,I_b$ with $a=|A_0|$, $b=|A_1|$. The sections of the old [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) are

$$
(N[A])_0=N[A_0]\cup A_1,\qquad (N[A])_1=N[A_1]\cup A_0.
$$

By induction their sizes are at least $\max\{|N[I_a]|,b\}$ and $\max\{|N[I_b]|,a\}$, respectively. These are exactly the sizes of the new sections, because both sets in each new union are [initial segments](../../../../../initial-segment.md) and hence nested. Thus [simplicial section compression](../../../../../simplicial-section-compression.md) preserves size and never enlarges the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md).

Repeatedly compress any section that is not already an [initial segment](../../../../../initial-segment.md). Every change strictly reduces the sum of the global simplicial positions of the included vertices. This nonnegative integer decreases only finitely often, so the process ends at a family $B$ whose sections in every coordinate are [initial segments](../../../../../initial-segment.md). If $B$ itself is an [initial segment](../../../../../initial-segment.md), the induction is complete. Otherwise choose the earliest absent vertex $X$ and the latest present vertex $Y$, with $X\prec Y$. They cannot agree in any coordinate: agreement would put them in one compressed section, where an earlier absent vertex cannot precede a later present one. Hence $Y=X^c$. Nor can a vertex $Z$ lie between them: if $Z$ is present, pairing it with $X$ would force $Z=X^c=Y$; if absent, pairing it with $Y$ would force $Z=Y^c=X$. Thus $X,Y$ are consecutive, and $B$ is obtained from $I_{|B|}$ by replacing its last vertex $X$ with the next vertex $Y$.

There are only two possibilities for these [terminal families for simplicial section compression](../../../../../terminal-families-for-simplicial-section-compression.md). If $|X|<|Y|$, consecutiveness makes $X$ the last $k$-set and $Y$ the first $(k+1)$-set. Complementarity forces $n=2k+1$, $X=\{k+2,\ldots,2k+1\}$ and $Y=\{1,\ldots,k+1\}$. For $n\geq3$, the corresponding $B$ contains all sets of size at most $k$ except $X$, and additionally $Y$. Every $(k+1)$-set has at least two $k$-subsets, so at least one belongs to $B$. The missing $X$ has a $(k-1)$-subset in $B$. Consequently $N[B]$ contains every set of size at most $k+1$, which is exactly $N[I_{|B|}]$.

If $|X|=|Y|$, then $n=2k$. Since $X,Y$ are complementary, the smaller one contains coordinate $1$. Consecutiveness forces $X$ to be the last $k$-set containing $1$, and $Y$ the first $k$-set avoiding $1$:

$$
X=\{1,k+2,\ldots,2k\},\qquad Y=\{2,\ldots,k+1\}.
$$

The [initial segment](../../../../../initial-segment.md) consists of all sets of size less than $k$ and all $k$-sets containing $1$. Its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) contains all sets of size at most $k$ and all $(k+1)$-sets containing $1$. For $k\geq2$, each such $(k+1)$-set has $k\geq2$ $k$-subsets containing $1$, so removing only $X$ leaves one in $B$. All sets of size at most $k$ are still in $N[B]$, because all levels below $k$ belong to $B$. Hence again $N[I_{|B|}]\subseteq N[B]$. For $k=1$, the two families are related by exchanging coordinates and both have the whole $Q_2$ as their [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md). These comparisons finish the induction and prove [Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md).

For the radius-$t$ version, repeatedly use the one-step result. At each step the comparison family remains an [initial segment](../../../../../initial-segment.md), and its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) is monotone in its size. If $|N_{t-1}[A]|\geq|N_{t-1}[I_m]|$, applying [Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) to $N_{t-1}[A]$ therefore gives $|N_t[A]|\geq|N_t[I_m]|$. Induction on $t$ proves the asserted extension.

A **[Lévy family of graphs](../../../../../levy-family-of-graphs.md)** has vanishing [concentration of measure](../../../../../concentration-of-measure.md) functions after distances have been scaled by the graph diameter. More explicitly, for connected finite [graphs](../../../../../graph-split.md) $G_n$ of diameter $D_n$, use normalized [graph distance](../../../../../distance-graph-theory.md) $d_n=d_{G_n}/D_n$ and uniform [probability measure](../../../../../probability-measure.md). For every fixed $\varepsilon>0$, require

$$
\alpha_n(\varepsilon):=\sup_{|A|\geq|V(G_n)|/2}\left(1-\frac{|N_{\lfloor\varepsilon D_n\rfloor}[A]|}{|V(G_n)|}\right)\longrightarrow0.
$$

For $Q_n$ this normalization is [normalized Hamming distance](../../../../../normalized-hamming-distance.md) $d_H/n$, since its diameter is $n$.

If $|A|\geq2^{n-1}$, the corresponding [initial segment](../../../../../initial-segment.md) contains the [Hamming ball](../../../../../hamming-ball.md) about $\varnothing$ of radius $b_n=\lfloor(n-1)/2\rfloor$. The radius-$t$ version of [Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) implies

$$
1-\frac{|N_t[A]|}{2^n}\leq\mathbb P\{Z_n>b_n+t\},\qquad Z_n\sim\operatorname{Bin}(n,1/2).
$$

Use the precise [Hoeffding inequality](../../../../../hoeffding-inequality.md) $\mathbb P(Z_n-n/2\geq u)\leq\exp(-2u^2/n)$ for $u\geq0$. One can also derive this estimate directly: the [moment-generating function](../../../../../moment-generating-function.md) of $Z_n-n/2$ is $\cosh(\lambda/2)^n\leq\exp(n\lambda^2/8)$; the exponential [Markov inequality](../../../../../markov-inequality.md) followed by minimization at $\lambda=4u/n$ gives the bound. With $t=\lfloor\varepsilon n\rfloor$, we have $b_n+t\geq n/2+\varepsilon n-2$. Thus, whenever $\varepsilon n>2$,

$$
\boxed{\alpha_n(\varepsilon)\leq\exp\left(-\frac{2(\varepsilon n-2)^2}{n}\right)\longrightarrow0}.
$$

This proves that the [hypercube graphs](../../../../../hypercube-graph.md) form a [Lévy family of graphs](../../../../../levy-family-of-graphs.md). The stronger fixed-positive-mass formulation follows as well. For any $a>0$, choose $c$ with $1/(4c^2)<a$. The [Chebyshev inequality](../../../../../chebyshev-inequality.md) for $Z_n$, whose [variance](../../../../../variance-split.md) is $n/4$, makes the [Hamming ball](../../../../../hamming-ball.md) of radius $\lfloor n/2-c\sqrt n\rfloor$ have fewer than $a2^n$ vertices. An [initial segment](../../../../../initial-segment.md) of size at least $a2^n$ contains that ball. Enlarging by $\lfloor\varepsilon n\rfloor$ and using the same [Hoeffding inequality](../../../../../hoeffding-inequality.md) gives a complement proportion tending to zero uniformly over all such $A$. The normalization matters: with unscaled unit [Hamming distance](../../../../../hamming-distance.md), cubes do not satisfy the metric version at every fixed radius; for a radius below one, a half-cube has no enlargement.

**Equality in [Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) does not determine a [down-set](../../../../../down-set.md) up to isomorphism.** In $Q_4$, take

$$
A=\{\varnothing,\{1\},\{2\},\{3\},\{4\},\{1,2\},\{2,3\},\{3,4\},\{1,4\}\}.
$$

This is a [down-set](../../../../../down-set.md) of size nine. Its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) contains every set of size at most two, because all singletons belong to $A$. Every triple contains an edge of the four-cycle among the listed pairs, so every triple also belongs to $N[A]$. The four-element set does not. Hence $|N[A]|=1+4+6+4=15$.

The size-nine [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md) [initial segment](../../../../../initial-segment.md) is all sets of size at most one together with the pairs $12,13,14,23$. Every triple contains one of these pairs, and the four-element set is again absent from its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md). Its neighbourhood therefore also has size $15$, proving extremality of $A$. Nevertheless the induced [graphs](../../../../../graph-split.md) are not isomorphic: in $A$, the empty set has degree four, the four singletons have degree three, and the four pairs have degree two. The [initial segment](../../../../../initial-segment.md) has two vertices of degree four, namely $\varnothing$ and $\{1\}$. Since a [graph automorphism](../../../../../graph-automorphism.md) preserves induced [degree of a vertex](../../../../../degree-graph-theory.md), no automorphism of the cube can carry one family to the other. This gives **[nonunique down-set extremizers for Harper theorem](../../../../../nonunique-down-set-extremizers-for-harper-theorem.md)** even under the stronger test of induced graph isomorphism.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
