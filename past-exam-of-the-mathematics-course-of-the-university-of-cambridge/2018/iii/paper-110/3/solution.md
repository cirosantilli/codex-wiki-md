<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Statement and definitions.** For disjoint nonempty sets $A,B$ of [vertices](../../../../../vertex-graph-theory.md), their [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) is $d(A,B)=e(A,B)/(|A||B|)$. They form a [regular pair of vertex sets](../../../../../regular-pair-of-vertex-sets.md), or an $\varepsilon$-uniform pair, if

$$
|d(X,Y)-d(A,B)|\leq\varepsilon
$$

whenever $X\subseteq A$, $Y\subseteq B$, $|X|\geq\varepsilon|A|$ and $|Y|\geq\varepsilon|B|$.

The [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) states that for every $\varepsilon>0$ and positive integer $m_0$, there are integers $M,n_0$ such that every [graph](../../../../../graph-split.md) of order $n\geq n_0$ has a [set partition](../../../../../set-partition.md)

$$
V(G)=V_0\sqcup V_1\sqcup\cdots\sqcup V_k
$$

with $m_0\leq k\leq M$, $|V_0|\leq\varepsilon n$, equal nonzero sizes $|V_1|=\cdots=|V_k|$, and at most $\varepsilon k^2$ unordered pairs $(V_i,V_j)$, $1\leq i<j\leq k$, that fail to be $\varepsilon$-uniform. It is enough to prove this for $0<\varepsilon\leq1/2$, since decreasing the parameter strengthens the conclusion.

**Energy increment.** For the proof, regard each exceptional [vertex](../../../../../vertex-graph-theory.md) as a singleton part and use the [equitable regularity energy](../../../../../equitable-regularity-energy.md)

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2.
$$

The sum is over ordered pairs, including diagonal pairs; for those pairs define $d$ as the mean adjacency indicator on $A\times B$. Thus $0\leq q\leq1$. Under a refinement, the subrectangle densities have the original density as their weighted mean. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), equivalently the nonnegativity of their weighted [variance](../../../../../variance-split.md), gives $q(\mathcal P')\geq q(\mathcal P)$.

Suppose there are more than $\varepsilon k^2$ irregular pairs, with main cell size $m$. For each such pair choose witnesses $X\subseteq V_i$, $Y\subseteq V_j$ of sizes at least $\varepsilon m$ and with $|d(X,Y)-d(V_i,V_j)|>\varepsilon$. Refine every main cell by all its witness subsets. Each splits into at most $2^{k-1}$ atoms, and we may use the larger bound $2^k$.

For an ordered irregular rectangle, write its refined densities as $d_{ab}$ and relative areas as $w_{ab}$. The energy gain on that rectangle is

$$
\frac{m^2}{n^2}\sum_{a,b}w_{ab}(d_{ab}-d(V_i,V_j))^2.
$$

The witness rectangle has relative area at least $\varepsilon^2$. Applying the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to the subrectangles it contains shows that this expression is greater than $\varepsilon^4m^2/n^2$. There are two orientations of each irregular pair. Since $km=n-|V_0|\geq n/2$, the total gain is greater than

$$
2\varepsilon^5\frac{k^2m^2}{n^2}\geq\varepsilon^5/2.
$$

**Restoring equal sizes without losing energy.** Put $\ell=\lfloor m/4^k\rfloor$, assuming $m\geq2\cdot4^k$. Split every refined atom into sets of size $\ell$, putting its leftover fewer than $\ell$ [vertices](../../../../../vertex-graph-theory.md) into the exceptional set as singleton parts. This is a further refinement, so the energy cannot decrease. The number of new exceptional [vertices](../../../../../vertex-graph-theory.md) is at most

$$
k2^k\ell\leq km/2^k\leq n/2^k.
$$

The number $k'$ of new main cells satisfies

$$
k\leq k'\leq\frac{km}{\ell}\leq2k4^k.
$$

For the first inequality, in each old cell the leftovers have total size less than $2^k\ell<m$, so at least one full chunk survives. All previous exceptional singleton parts are kept. Treating leftovers as singleton parts is what makes the energy increment survive equitabilization exactly.

Take $S=\lceil2\varepsilon^{-5}\rceil+1$ and choose $k_0\geq m_0$ so large that $S2^{-k_0}\leq\varepsilon/2$. Start with $k_0$ equal main cells, with fewer than $k_0$ exceptional [vertices](../../../../../vertex-graph-theory.md). Define a finite bound $M$ by iterating $x\mapsto2x4^x$ a total of $S$ times, starting from $k_0$. Choose $n_0$ sufficiently large that $k_0\leq\varepsilon n/2$ and $n/(2M)\geq2\cdot4^M$ whenever $n\geq n_0$.

At each of the first $S$ refinements, the exceptional set has size at most

$$
k_0+S n2^{-k_0}\leq\varepsilon n,
$$

the cell count is between $k_0$ and $M$, and $m\geq n/(2M)$, so all the chunk sizes above are valid. But $S$ unsuccessful refinements would raise $q$ by more than $S\varepsilon^5/2>1$, which is impossible. Thus the procedure terminates at a partition satisfying the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md).

**Three linearly large uniform sets.** Apply the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) with

$$
\varepsilon=10^{-5},\qquad m_0=1000,\qquad d_0=10^{-3}.
$$

For $n\geq n_0$, delete all [edges](../../../../../edge-of-a-graph.md) touching $V_0$, all internal main-cell [edges](../../../../../edge-of-a-graph.md), all [edges](../../../../../edge-of-a-graph.md) of irregular pairs, and all [edges](../../../../../edge-of-a-graph.md) of regular pairs whose [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) is less than $d_0$. The respective losses are bounded by

$$
\varepsilon n^2,\qquad \frac{n^2}{2m_0},\qquad \varepsilon n^2,\qquad \frac{d_0n^2}{2}.
$$

Thus the total loss is at most $0.00102n^2$, and the remaining [graph](../../../../../graph-split.md) has at least

$$
(0.255-0.00102)n^2=0.25398n^2>n^2/4
$$

[edges](../../../../../edge-of-a-graph.md). Form the [reduced graph of a regularity partition](../../../../../reduced-graph-of-a-regularity-partition.md) $R$, joining two main cells precisely when they are $\varepsilon$-uniform and have [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) at least $d_0$. If their common size is $m$, the remaining [edge](../../../../../edge-of-a-graph.md) count is at most $e(R)m^2$. Since $km\leq n$, we obtain $e(R)>k^2/4$. The [Mantel theorem](../../../../../mantel-theorem.md) gives a [triangle in a graph](../../../../../triangle-in-a-graph.md) in $R$. Its three cells $U_1,U_2,U_3$ have the required pairwise density and are $10^{-3}$-uniform: an $\varepsilon$-uniform pair is uniform for any larger parameter.

Each selected cell has size $m\geq(1-\varepsilon)n/M$. Choose

$$
c=\min\left\{\frac{1-\varepsilon}{2M},\frac1{n_0}\right\}>0.
$$

For $n<n_0$, the [Mantel theorem](../../../../../mantel-theorem.md) gives a [triangle in a graph](../../../../../triangle-in-a-graph.md) in the original [graph](../../../../../graph-split.md), since its [edge](../../../../../edge-of-a-graph.md) count exceeds $n^2/4$; take its three singleton [vertices](../../../../../vertex-graph-theory.md). Their pairs have density one and are uniform for every positive parameter, and $1>cn$. Therefore in all cases

$$
\boxed{|U_i|>cn,\quad (U_i,U_j)\text{ is }10^{-3}\text{-uniform},\quad d(U_i,U_j)\geq10^{-3}.}
$$

The constant is absolute; the energy proof gives a very large bound for $M$, which does not affect its positivity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
