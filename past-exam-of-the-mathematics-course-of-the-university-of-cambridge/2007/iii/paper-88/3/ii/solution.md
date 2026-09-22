<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First derive the [triangle removal lemma](../../../../../../triangle-removal-lemma.md) from the [Szemerédi regularity lemma](../../../../../../szemeredi-regularity-lemma.md). Given an allowed deletion fraction $0<\eta<1$, take $d=\eta/10$, $m_0=\lceil10/\eta\rceil$, and $0<\varepsilon\leq\min(d/4,\eta/100,1/8)$. Apply part (i), with upper class bound $M$. Delete [edges](../../../../../../edge-of-a-graph.md) incident with $V_0$, inside each nonexceptional class, between [irregular pairs](../../../../../../irregular-pair-of-vertex-sets.md), and between [regular pairs](../../../../../../regular-pair-of-vertex-sets.md) of [subset density](../../../../../../density-of-a-finite-subset.md) less than $d$. Their total number is at most

$$
\left(2\varepsilon+\frac1{2m_0}+\frac d2\right)n^2<\eta n^2.
$$

These four terms are bounded respectively by $\varepsilon n^2$, $n^2/(2m_0)$, $\varepsilon n^2$, and $dn^2/2$.

If a [triangle in a graph](../../../../../../triangle-in-a-graph.md) remains, its three [vertices](../../../../../../vertex-graph-theory.md) lie in three distinct equal classes, all three [regular pairs](../../../../../../regular-pair-of-vertex-sets.md) with [subset density](../../../../../../density-of-a-finite-subset.md) at least $d$. The permitted [regular triangle counting lemma](../../../../../../regular-triangle-counting-lemma.md) gives at least $(d^3/4)t^3$ [triangles in a graph](../../../../../../triangle-in-a-graph.md) in the original [graph](../../../../../../graph-split.md), where $t$ is the class size. This lower bound can also be checked directly: all but $2\varepsilon t$ [vertices](../../../../../../vertex-graph-theory.md) of the first class have at least $(d-\varepsilon)t$ neighbors in each of the other two. Those neighborhoods are large enough to use the [regular pair](../../../../../../regular-pair-of-vertex-sets.md) condition on the remaining pair, giving at least $(d-\varepsilon)^3t^2$ [edges](../../../../../../edge-of-a-graph.md) between them. Hence the total is at least $(1-2\varepsilon)(d-\varepsilon)^3t^3\geq(d^3/4)t^3$.

Since $t\geq n/(2M)$, a surviving [triangle in a graph](../../../../../../triangle-in-a-graph.md) forces at least $d^3n^3/(32M^3)$ original [triangles in a graph](../../../../../../triangle-in-a-graph.md). Thus a [graph](../../../../../../graph-split.md) with fewer than $\xi n^3$ [triangles in a graph](../../../../../../triangle-in-a-graph.md), where $\xi=d^3/(64M^3)>0$, can be made [triangle-free](../../../../../../triangle-free-graph.md) by deleting fewer than $\eta n^2$ [edges](../../../../../../edge-of-a-graph.md), for all sufficiently large $n$. This proves the removal lemma needed here.

Now use the [triangle-removal proof of Roth theorem](../../../../../../triangle-removal-proof-of-roth-theorem.md). Fix a [subset density](../../../../../../density-of-a-finite-subset.md) lower bound $\delta>0$ and suppose $A\subseteq[N]$, $|A|\geq\delta N$, has no nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md). Set $m=2N+1$ and $G=\mathbb Z_m$. Use three disjoint copies $X,Y,Z$ of $G$ and put [edges](../../../../../../edge-of-a-graph.md) according to

$$
xy\in E\iff y-x\in A,\qquad yz\in E\iff z-y\in A,\qquad xz\in E\iff (z-x)/2\in A.
$$

Division by two is valid because $m$ is odd. A [triangle in a graph](../../../../../../triangle-in-a-graph.md) corresponds to $a=y-x$, $b=z-y$, $c=(z-x)/2$ with $a,b,c\in A$ and $a+b=2c$. Since $A\subseteq[N]$ and $|a+b-2c|<m$, this congruence is an [integer](../../../../../../integer.md) equality. Progression-freeness therefore forces $a=b=c$.

Every [triangle in a graph](../../../../../../triangle-in-a-graph.md) is consequently of the form $(x,x+a,x+2a)$ with $x\in G,a\in A$, so there are exactly $m|A|$ [triangles in a graph](../../../../../../triangle-in-a-graph.md). These [triangles in a graph](../../../../../../triangle-in-a-graph.md) are edge-disjoint: an $XY$ [edge](../../../../../../edge-of-a-graph.md) determines $(x,a)$; a $YZ$ [edge](../../../../../../edge-of-a-graph.md) determines $a$ and then $x$; and an $XZ$ [edge](../../../../../../edge-of-a-graph.md) determines $a=(z-x)/2$ and $x$. Eliminating them all requires at least $m|A|$ [edge](../../../../../../edge-of-a-graph.md) deletions.

The [graph](../../../../../../graph-split.md) has $3m$ [vertices](../../../../../../vertex-graph-theory.md) but only $m|A|\leq mN=O(m^2)$ [triangles in a graph](../../../../../../triangle-in-a-graph.md). Take $\eta=\delta/100$. For large enough $N$ its [triangle in a graph](../../../../../../triangle-in-a-graph.md) count is below $\xi(3m)^3$, so removal requires fewer than $\eta(3m)^2=9\delta m^2/100$ deletions. Yet

$$
m|A|\geq\delta mN\geq\frac{\delta m^2}{3}>\frac{9\delta m^2}{100},
$$

a contradiction. Therefore **every fixed positive-density [subset](../../../../../../subset.md) of a sufficiently long interval contains a nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md)**.

This proves the qualitative [Roth theorem on three-term arithmetic progressions](../../../../../../roth-theorem-on-three-term-arithmetic-progressions.md). The quantitative bound from part 2(i) came from the explicit Fourier iteration; the regularity-removal argument gives a density-dependent threshold without that double-logarithmic estimate.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
