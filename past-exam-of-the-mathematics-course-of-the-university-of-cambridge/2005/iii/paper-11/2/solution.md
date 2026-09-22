<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the equitable form of the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md). For $0<\varepsilon<1/2$ and a prescribed lower bound $m_0$, there are $M,n_0$ such that every sufficiently large [graph](../../../../../graph-split.md) admits a [set partition](../../../../../set-partition.md)

$$
V(G)=V_0\sqcup V_1\sqcup\cdots\sqcup V_k,
\quad m_0\le k\le M,\quad |V_0|\le\varepsilon n,\quad |V_1|=\cdots=|V_k|,
$$

with at most $\varepsilon k^2$ unordered [irregular pairs](../../../../../irregular-pair-of-vertex-sets.md) among the nonexceptional cells. A [uniform pair](../../../../../regular-pair-of-vertex-sets.md) here means a [regular pair of vertex sets](../../../../../regular-pair-of-vertex-sets.md). Larger values of $\varepsilon$ follow from a smaller parameter, so the stated restriction loses nothing.

For the proof, retain the exceptional [vertices](../../../../../vertex-graph-theory.md) as singleton cells in an auxiliary [set partition](../../../../../set-partition.md) $\mathcal P$. Define its [regularity energy](../../../../../equitable-regularity-energy.md) by the ordered sum

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2.
$$

For diagonal rectangles the [adjacency matrix of a graph](../../../../../adjacency-matrix.md) defines $d(A,A)$; diagonal terms are included. Thus $0\le q\le1$. If $A\times B$ is split into rectangles of densities $d_{uv}$ and sizes $w_{uv}$, their weighted mean is $d=d(A,B)$. Expanding squares proves the [refinement variance identity for regularity energy](../../../../../refinement-variance-identity-for-regularity-energy.md):

$$
\sum_{u,v}w_{uv}d_{uv}^2-|A||B|d^2
=\sum_{u,v}w_{uv}(d_{uv}-d)^2\ge0.
$$

Every refinement therefore increases or preserves energy.

Suppose equal cells $V_i,V_j$ of size $m$ are $\varepsilon$-irregular. Choose witnesses $X\subseteq V_i$, $Y\subseteq V_j$ of sizes at least $\varepsilon m$, whose density differs from $d(V_i,V_j)$ by more than $\varepsilon$. Refine the cells so that these witnesses are unions of refined atoms. Applying the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) inside $X\times Y$ gives an increase, for this oriented rectangle, greater than

$$
\frac{|X||Y|}{n^2}|d(X,Y)-d(V_i,V_j)|^2
\ge\frac{\varepsilon^4m^2}{n^2}.
$$

Choose witnesses simultaneously for every [irregular pair](../../../../../irregular-pair-of-vertex-sets.md). Each original cell is cut by at most $k-1$ witness sets and has at most $2^k$ atoms. If more than $\varepsilon k^2$ unordered pairs are irregular, both orientations contribute, giving

$$
\Delta q>2\varepsilon^5\left(\frac{km}{n}\right)^2\ge\frac{\varepsilon^5}{2},
$$

as long as the exceptional set has at most $n/2$ [vertices](../../../../../vertex-graph-theory.md).

To restore equal sizes without sacrificing this increase, use [equalization with a controlled exceptional set](../../../../../equalization-with-a-controlled-exceptional-set.md). Cut every witness atom into blocks of size $\ell=\lfloor m/4^k\rfloor$, leaving fewer than $\ell$ unused [vertices](../../../../../vertex-graph-theory.md) in each atom. Make each unused vertex a singleton exceptional cell. This is a further refinement, so there is **no energy loss**. The number newly exceptional is at most

$$
k2^k\ell\le km2^{-k}\le n2^{-k}.
$$

When $m\ge2\cdot4^k$, the new nonexceptional cell count $k'$ is at most $4k4^k$: indeed $\ell\ge m/(2\cdot4^k)$ and $n/m\le2k$. It is at least $k$, since each old cell supplies at least $4^k-2^k\ge1$ blocks.

Let $L=\lceil2\varepsilon^{-5}\rceil+1$. Choose the initial count $k_0\ge m_0$ so large that $L2^{-k_0}\le\varepsilon/2$, and begin with $k_0$ equal cells and fewer than $k_0$ leftover [vertices](../../../../../vertex-graph-theory.md). Take $n_0$ large enough that these initial leftovers are at most $\varepsilon n/2$. Iterate the bound $k\mapsto4k4^k$ for $L$ rounds to obtain a finite number $M$. Increase $n_0$ further to ensure $n\ge4M4^M$. Then every cell size encountered satisfies $m\ge n/(2M)\ge2\cdot4^k$, so every equalization is legitimate. The total exception budget is at most $\varepsilon n$, because the initial losses use half the budget and all later losses sum to at most $Ln2^{-k_0}$. Energy cannot increase by more than one, so $L$ failing rounds are impossible. The process must stop with at most $\varepsilon k^2$ irregular pairs. This proves the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md), including the bounded cell count, equitability and exceptional-set control.

For the dense-pair application, apply this proof with $\eta=1/100$ and $m_0=100$. Suppose every $\eta$-[regular pair](../../../../../regular-pair-of-vertex-sets.md) of nonexceptional cells has density at most $1/4$. [Edges](../../../../../edge-of-a-graph.md) touching $V_0$ number at most $\eta n^2$. [Edges](../../../../../edge-of-a-graph.md) inside nonexceptional cells number at most $km^2/2\le n^2/(2m_0)$. The at most $\eta k^2$ irregular cell pairs contribute at most $\eta n^2$. Finally the regular cross-cell pairs contribute at most $k(k-1)m^2/8\le n^2/8$. Therefore

$$
e(G)\le\left(\frac18+2\eta+\frac1{2m_0}\right)n^2
=\frac3{20}n^2<\frac16n^2,
$$

a contradiction. Some regular pair $(U,W)$ consequently has density greater than $1/4$. It is also a $1/8$-[uniform pair](../../../../../regular-pair-of-vertex-sets.md), since subsets of relative size at least $1/8$ qualify in the stronger $\eta$-regularity condition. The common cell size satisfies $m\ge(1-\eta)n/M\ge n/(2M)$. Thus the [dense regular pair from edge surplus](../../../../../dense-regular-pair-from-edge-surplus.md) gives

$$
\boxed{|U|=|W|\ge cn,\qquad d(U,W)>1/4,\qquad (U,W)\text{ is }1/8\text{-uniform}.}
$$

This first proves the assertion for $n\ge n_0$. For the finitely many smaller possible orders, choose the endpoints of any edge as singleton sets: the pair has density one and is regular for every positive parameter. Taking $c=\min\{1/(2M),1/n_0\}>0$ includes these cases as well.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
