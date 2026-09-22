<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Identify the vertices of the [Boolean hypercube](../../../../../boolean-hypercube.md) $Q_n$ with subsets of $[n]$, adjacent when their [symmetric difference](../../../../../symmetric-difference.md) has size one. Write $N(\mathcal A)$ for the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md), including $\mathcal A$ itself. In [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md), smaller [sets](../../../../../set-split.md) come first, and equal-sized [sets](../../../../../set-split.md) are ordered by [lexicographic order](../../../../../lexicographic-order.md): the least element of the [symmetric difference](../../../../../symmetric-difference.md) belongs to the earlier member. Let $I_m$ denote the first $m$ vertices. The [vertex-isoperimetric inequality in the discrete cube](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) states

$$
\boxed{|N(\mathcal A)|\geq|N(I_{|\mathcal A|})|\qquad(\mathcal A\subseteq Q_n).}
$$

Subtracting $|\mathcal A|$ gives the equivalent assertion for the external vertex boundary.

We first check that $N(I_m)$ is also an initial segment in [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md). Apart from the empty and full cases, $I_m$ consists of complete lower layers and a [lexicographic](../../../../../lexicographic-order.md) initial segment $\mathcal F$ in its top rank $r$. Its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) contains all ranks at most $r$ and the [upper shadow](../../../../../upper-shadow.md) $\nabla\mathcal F$ in rank $r+1$. This [upper shadow](../../../../../upper-shadow.md) is [lexicographic](../../../../../lexicographic-order.md) initial: an $(r+1)$-subset $C$ belongs to it precisely when its first $r$-subset in [lexicographic order](../../../../../lexicographic-order.md), obtained by deleting its largest element, belongs to $\mathcal F$. Taking the first $r$ elements preserves weak [lexicographic order](../../../../../lexicographic-order.md), proving the assertion. This also handles $r=0$, where $N(\{\varnothing\})$ consists of ranks zero and one.

We prove the [vertex-isoperimetric inequality in the discrete cube](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) by [mathematical induction](../../../../../mathematical-induction.md) on $n$, with $n=0,1$ immediate. Fix a coordinate $i$ and write $\mathcal A_0,\mathcal A_1\subseteq Q_{n-1}$ for the sections without and with $i$. The two sections of its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) are

$$
N(\mathcal A)_0=N(\mathcal A_0)\cup\mathcal A_1,\qquad
N(\mathcal A)_1=N(\mathcal A_1)\cup\mathcal A_0.
$$

A [simplicial section compression](../../../../../simplicial-section-compression.md) replaces $\mathcal A_j$ by the initial segment $I_{a_j}$ of size $a_j=|\mathcal A_j|$ in the other coordinates. By the preceding observation, both $N(I_{a_j})$ and $I_{a_{1-j}}$ are initial segments, so their union has size $\max\{|N(I_{a_j})|,a_{1-j}\}$. The [mathematical induction](../../../../../mathematical-induction.md) hypothesis gives

$$
\max\{|N(I_{a_j})|,a_{1-j}\}
\leq\max\{|N(\mathcal A_j)|,a_{1-j}\}
\leq|N(\mathcal A_j)\cup\mathcal A_{1-j}|.
$$

Adding the two section bounds proves that [simplicial section compression](../../../../../simplicial-section-compression.md) cannot increase the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md).

Apply changing [simplicial section compressions](../../../../../simplicial-section-compression.md) until none remains. The sum of the global [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md) positions strictly decreases at each step: within a section the order is exactly the restriction of the global order. Thus the procedure terminates at a [set family](../../../../../set-family.md) $\mathcal B$ every coordinate section of which is initial. We now classify the possible [terminal families for simplicial section compression](../../../../../terminal-families-for-simplicial-section-compression.md), rather than assuming this terminal [set family](../../../../../set-family.md) must be globally initial.

If $X<Y$, $X\notin\mathcal B$ and $Y\in\mathcal B$, then $X,Y$ cannot agree in any coordinate, since that coordinate section would have an omitted earlier member and an included later one. Therefore $Y=X^c$. Let $X$ be the first omitted vertex and $Y$ the last included vertex. If $\mathcal B$ is noninitial, $X<Y$ and $Y=X^c$. Any vertex $Z$ strictly between them would have to be included, since an omitted $Z$ paired with $Y$ would have to equal $Y^c=X$. But it would also have to be omitted, since an included $Z$ paired with $X$ would have to equal $X^c=Y$. Thus there is no such $Z$: $X,Y$ are consecutive complementary vertices. Everything before $X$ is included and everything after $Y$ omitted. Hence $\mathcal B$ is obtained from the initial segment of its size by replacing $X$ with its immediate successor $X^c$.

There are only two forms of this exception. If $n=2r+1$, consecutive complementary vertices must straddle ranks $r,r+1$; otherwise an intermediate rank or a further vertex in one of their ranks separates them. They are consequently

$$
X=\{r+2,\ldots,2r+1\},\qquad Y=\{1,\ldots,r+1\},
$$

with $X$ the last $r$-subset and $Y$ the first $(r+1)$-subset. The corresponding initial segment is all ranks at most $r$. For $r\geq1$, the omitted $X$ remains in $N(\mathcal B)$ through a lower neighbour, and every $(r+1)$-subset has at least two $r$-subsets, only one of which was omitted. Thus $N(\mathcal B)$ contains every rank at most $r+1$, namely $N(I_{|\mathcal B|})$. For $r=0$ both singleton [closed graph neighbourhoods](../../../../../closed-graph-neighbourhood.md) are the whole $Q_1$.

If $n=2r$, the two complementary vertices must both have rank $r$. The [complement](../../../../../complement-of-a-set.md) map reverses the [lexicographic order](../../../../../lexicographic-order.md) in that rank, so a consecutive complementary pair must be its central pair. Exactly half the $r$-subsets contain $1$, and all of those precede those missing $1$. Therefore the pair is

$$
X=\{1,r+2,\ldots,2r\},\qquad Y=\{2,\ldots,r+1\}.
$$

Here $I_{|\mathcal B|}$ comprises all ranks below $r$ and all $r$-subsets containing $1$. For $r\geq2$, $N(\mathcal B)$ contains every rank at most $r$, because all lower ranks were retained. Every $(r+1)$-subset containing $1$ has $r\geq2$ different $r$-subsets containing $1$, so deletion of the one member $X$ removes no vertex of the [upper shadow](../../../../../upper-shadow.md). Consequently $N(\mathcal B)\supseteq N(I_{|\mathcal B|})$. For $r=1$, the two [closed graph neighbourhoods](../../../../../closed-graph-neighbourhood.md) both have size three in $Q_2$. These cases exhaust the exceptions. Since the successive [simplicial section compressions](../../../../../simplicial-section-compression.md) never increased the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md), this proves the [vertex-isoperimetric inequality in the discrete cube](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md).

The same argument gives all integer radii. Write $N^t$ for $t$ repetitions of the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md). Its application to an initial segment is again initial; the sizes of these initial segments are monotone in the original size. Inducting on $t$ therefore gives

$$
|N^t(\mathcal A)|\geq|N^t(I_{|\mathcal A|})|.
$$

For the concentration question, use uniform [probability measure](../../../../../probability-measure.md) on a finite [connected graph](../../../../../connected-graph.md) and normalize its [graph distance](../../../../../distance-graph-theory.md) by its [graph diameter](../../../../../graph-diameter.md). A sequence is a [Lévy family of graphs](../../../../../levy-family-of-graphs.md) if, for every fixed $\varepsilon>0$ and $\delta>0$, the radius-$\varepsilon$ neighbourhood of every [set](../../../../../set-split.md) of measure at least $\delta$ has measure tending to one, uniformly over those [sets](../../../../../set-split.md). One may equivalently require this only for [sets](../../../../../set-split.md) of measure at least one half. To see the reverse implication, first the radius-$\varepsilon/2$ neighbourhood of every positive-density [set](../../../../../set-split.md) must eventually have measure greater than one half. Otherwise its [complement](../../../../../complement-of-a-set.md) has measure at least one half, while the radius-$\varepsilon/4$ neighbourhood of that [complement](../../../../../complement-of-a-set.md) misses the original positive-density [set](../../../../../set-split.md), contradicting the half-measure condition. Apply the half-measure condition once more to the radius-$\varepsilon/2$ neighbourhood, enlarging it by another $\varepsilon/2$, to obtain the full claim. The metric normalization is essential here.

For $Q_n$, the [graph diameter](../../../../../graph-diameter.md) is $n$. A uniformly chosen vertex has size $Z_n$ with [binomial distribution](../../../../../binomial-distribution.md) $\operatorname{Bin}(n,1/2)$, [expectation](../../../../../expected-value.md) $n/2$ and [variance](../../../../../variance-split.md) $n/4$. Fix $\delta>0$ and choose $C>0$ so that $1/(4C^2)<\delta$. By [Chebyshev's inequality](../../../../../chebyshev-inequality.md),

$$
\Pr\{Z_n\leq n/2-C\sqrt n\}\leq\frac1{4C^2}<\delta.
$$

For sufficiently large $n$, put $k_n=\lfloor n/2-C\sqrt n\rfloor\geq0$. Every initial segment of measure at least $\delta$ contains the complete ranks through $k_n$. Its radius-$t$ [graph neighbourhood](../../../../../graph-neighbourhood.md) therefore contains every rank at most $k_n+t$. Taking $t=\lfloor\varepsilon n\rfloor$, the all-radius [vertex-isoperimetric inequality in the discrete cube](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) gives, uniformly for $|\mathcal A|\geq\delta2^n$,

$$
1-\frac{|N^t(\mathcal A)|}{2^n}
\leq\Pr\{Z_n>k_n+t\}
\leq\frac{n}{4(\varepsilon n-C\sqrt n-2)^2}\longrightarrow0.
$$

The last [Chebyshev's inequality](../../../../../chebyshev-inequality.md) is used only when its denominator has positive square root. These are precisely the radius-$\varepsilon$ neighbourhoods in the normalized [graph distance](../../../../../distance-graph-theory.md). **The discrete cubes form a [Lévy family](../../../../../levy-family-of-graphs.md).** In fact, taking $t=\lfloor n^{3/4}\rfloor$ in the same bound makes the omitted measure $O(n^{-1/2})$ for each fixed $\delta$: a radius that is $o(n)$ already suffices.

For fixed $d\geq1$, the nearest-neighbour grid $[n]^d$ has [graph distance](../../../../../distance-graph-theory.md) $\sum_i|x_i-y_i|$ and [graph diameter](../../../../../graph-diameter.md) $d(n-1)$. Take the slab $\mathcal A_n=\{x:x_1\leq\lceil n/2\rceil\}$, whose uniform measure is at least one half. Its integer radius-$t$ [graph neighbourhood](../../../../../graph-neighbourhood.md) is exactly $\{x:x_1\leq\min(n,\lceil n/2\rceil+t)\}$: changing the first coordinate alone attains the minimum distance to the slab. For $0<\varepsilon<1/(2d)$ and $t=\lfloor\varepsilon d(n-1)\rfloor$, the omitted proportion tends to

$$
\boxed{\frac12-\varepsilon d>0.}
$$

Thus there is [failure of concentration in fixed-dimensional grids](../../../../../failure-of-concentration-in-fixed-dimensional-grids.md), and **the fixed-dimensional grids do not form a [Lévy family](../../../../../levy-family-of-graphs.md)** with normalized graph distance.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
