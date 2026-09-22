<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For disjoint nonempty [vertex](../../../../../../vertex-graph-theory.md) [sets](../../../../../../set-split.md) $U,V$, write $d(U,V)=e(U,V)/(|U||V|)$. A [regular pair of vertex sets](../../../../../../regular-pair-of-vertex-sets.md) is $\varepsilon$-regular if every $U'\subseteq U,V'\subseteq V$ with $|U'|\geq\varepsilon|U|$, $|V'|\geq\varepsilon|V|$ satisfies $|d(U',V')-d(U,V)|\leq\varepsilon$.

The [Szemerédi regularity lemma](../../../../../../szemeredi-regularity-lemma.md) states that, for every $\varepsilon>0$ and [integer](../../../../../../integer.md) $m_0$, there are $M,n_0$ such that every finite simple [graph](../../../../../../graph-split.md) on $n\geq n_0$ [vertices](../../../../../../vertex-graph-theory.md) has a [set partition](../../../../../../set-partition.md)

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_m
$$

with **$m_0\leq m\leq M$, $|V_0|\leq\varepsilon n$, $|V_1|=\cdots=|V_m|$, and at most $\varepsilon m^2$ irregular unordered pairs among the nonexceptional classes**. Prove it for $0<\varepsilon\leq1/2$; larger parameters follow by using a smaller one.

For the [energy-increment proof of Szemerédi regularity](../../../../../../energy-increment-proof-of-szemeredi-regularity.md), keep every exceptional [vertex](../../../../../../vertex-graph-theory.md) as a singleton cell in the [set partition](../../../../../../set-partition.md) used to measure [regularity energy](../../../../../../equitable-regularity-energy.md). Define the [equitable regularity energy](../../../../../../equitable-regularity-energy.md)

$$
q(\mathcal P)=\frac1{n^2}\sum_{U,V\in\mathcal P}|U||V|d(U,V)^2.
$$

The sum is ordered, and on diagonal cells [subset density](../../../../../../density-of-a-finite-subset.md) means the average of the adjacency indicator, with zero on loops. Thus $0\leq q\leq1$. If $U,V$ are refined into $U_a,V_b$, expanding squares gives

$$
\sum_{a,b}|U_a||V_b|d(U_a,V_b)^2-|U||V|d(U,V)^2=\sum_{a,b}|U_a||V_b|[d(U_a,V_b)-d(U,V)]^2\geq0.
$$

The cross term vanishes because the weighted [arithmetic mean](../../../../../../arithmetic-mean.md) of the refined [subset densities](../../../../../../density-of-a-finite-subset.md) is the original [subset density](../../../../../../density-of-a-finite-subset.md). Consequently every [refinement of a set partition](../../../../../../refinement-of-a-set-partition.md) increases or preserves [regularity energy](../../../../../../equitable-regularity-energy.md).

Suppose the current nonexceptional classes have common size $t$ and there are $k$ of them. For each [irregular pair](../../../../../../irregular-pair-of-vertex-sets.md) $V_i,V_j$, choose witnesses $A_{ij},B_{ij}$ of sizes at least $\varepsilon t$ and discrepancy greater than $\varepsilon$. Refine each class by all its incident witness [subsets](../../../../../../subset.md). There are at most $k-1$ cuts in each class and at most $2^k$ resulting atoms. The witness rectangle is a union of refined rectangles. By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), its contribution to the [variance](../../../../../../variance-split.md) identity is at least

$$
|A_{ij}||B_{ij}|[d(A_{ij},B_{ij})-d(V_i,V_j)]^2>\varepsilon^4t^2.
$$

Indeed, the sum of squared deviations on the witness rectangle is at least its total weight times the square of their weighted [arithmetic mean](../../../../../../arithmetic-mean.md). If more than $\varepsilon k^2$ unordered pairs are irregular, summing even just one orientation of each gives

$$
\Delta q>\varepsilon^5\frac{k^2t^2}{n^2}\geq\frac{\varepsilon^5}{4},
$$

provided the exceptional [set](../../../../../../set-split.md) has at most $n/2$ [vertices](../../../../../../vertex-graph-theory.md). This is the strictly positive [regularity energy](../../../../../../equitable-regularity-energy.md) increment.

Restore equal class sizes without losing that increment. Divide every witness atom into blocks of size $\ell=\lfloor t/4^k\rfloor$ and make every leftover [vertex](../../../../../../vertex-graph-theory.md) an exceptional singleton. This is a further [refinement of a set partition](../../../../../../refinement-of-a-set-partition.md), so it cannot decrease $q$. There are at most $k2^k$ atoms, hence fewer than $k2^k\ell\leq n2^{-k}$ newly exceptional [vertices](../../../../../../vertex-graph-theory.md). If $t\geq2\cdot4^k$, then $\ell\geq t/(2\cdot4^k)$, so the number of full blocks is at most $2k4^k$. Each original class produces at least one full block: its leftovers occupy less than $2^k\ell$, whereas $t\geq4^k\ell>2^k\ell$. Thus the new class count is at least $k$.

Choose $R_* =\lceil4\varepsilon^{-5}\rceil+1$, and choose an initial [integer](../../../../../../integer.md) $k_0\geq m_0$ large enough that $R_*2^{-k_0}\leq\varepsilon/2$. Initially partition into $k_0$ equal classes and fewer than $k_0$ exceptional [vertices](../../../../../../vertex-graph-theory.md). Take $n_0$ large enough that this initial exception is at most $\varepsilon n/2$. During at most $R_*$ rounds, the additional exception is at most $R_*n2^{-k_0}\leq\varepsilon n/2$, so it never exceeds $\varepsilon n\leq n/2$.

A bound on class counts is obtained by iterating $k\mapsto2k4^k$ at most $R_*$ times starting at $k_0$; call the resulting bound $M$. Increasing $n_0$ further to satisfy $n_0\geq4M4^M$ guarantees $t\geq n/(2k)\geq2\cdot4^k$ at every round, so all full-block constructions are valid. If the desired regularity had not been reached after $R_*$ refinements, the [regularity energy](../../../../../../equitable-regularity-energy.md) increments would total more than one, impossible. Therefore the process terminates with the required partition and bounds. The singleton treatment of discarded [vertices](../../../../../../vertex-graph-theory.md) is what preserves [regularity energy](../../../../../../equitable-regularity-energy.md) monotonicity during equalization.

## ↑ Ancestors (11)

1. [I](../i.md)
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
