# Mantel theorem

↑ **Parent:** [Extremal number](extremal-number.md)

The [complete bipartite graph](complete-bipartite-graph.md) $K_{3,3}$ has [vertex sets](vertex-set.md) $A=\{a_1,a_2,a_3\}$ and $B=\{b_1,b_2,b_3\}$, with every [edge](edge-of-a-graph.md) between $A$ and $B$ and none inside either part. Its six [vertices](vertex-graph-theory.md) support $3\cdot3=9$ [edges](edge-of-a-graph.md) and no [triangles in a graph](triangle-in-a-graph.md): among any three [vertices](vertex-graph-theory.md), two belong to the same [independent set](independent-set-graph-theory.md) and have no joining [edge](edge-of-a-graph.md).

<a id="image-the-sharp-nine-edge-triangle-free-graph-k-3-3-and-the-three-triangles-in-a-graph-created-by-adding-a-1a-2"></a>
![](mantel-bipartite-bound-and-extra-edge.png)

**[Figure 1](#image-the-sharp-nine-edge-triangle-free-graph-k-3-3-and-the-three-triangles-in-a-graph-created-by-adding-a-1a-2). The sharp nine-edge triangle-free graph $K_{3,3}$ and the three triangles in a graph created by adding $a_1a_2$**.

Add the single [edge](edge-of-a-graph.md) $a_1a_2$. Each $b_j$ is a [common neighbour](common-neighbour.md) of its endpoints, producing the [triangle in a graph](triangle-in-a-graph.md) $a_1a_2b_j$. These are exactly the three new [triangles in a graph](triangle-in-a-graph.md), because every [triangle in a graph](triangle-in-a-graph.md) must use the only [edge](edge-of-a-graph.md) inside a part. The new count is ten [edges](edge-of-a-graph.md); nine was the last possible count without a [triangle in a graph](triangle-in-a-graph.md) on six [vertices](vertex-graph-theory.md).

In general, every [simple graph](simple-graph.md) with a [finite set](finite-set.md) of $n\geq0$ [vertices](vertex-graph-theory.md) that is [triangle-free](triangle-free-graph.md) has at most

$$
m\leq\left\lfloor\frac{n^2}{4}\right\rfloor
$$

[edges](edge-of-a-graph.md). This is the $r=2$ case of [Turán's theorem](turan-s-theorem.md), with forbidden [clique](clique-graph-theory.md) $K_3$. Equality holds exactly for the balanced [complete bipartite graph](complete-bipartite-graph.md) $K_{\lfloor n/2\rfloor,\lceil n/2\rceil}$, up to [graph isomorphism](graph-isomorphism.md); empty parts are allowed for $n<2$.[third electronic edition (2005), §7.1, printed p. 165, Theorem 7.1.1 and the definition of Turán graphs, specialized to the forbidden graph K3](graph-theory-by-reinhard-diestel.md)

The [floor function](floor-function.md) gives the exact [integer](integer-split.md) bound. Splitting $n$ [vertices](vertex-graph-theory.md) into two [independent sets](independent-set-graph-theory.md) of sizes $a$ and $n-a$, and putting in every cross [edge](edge-of-a-graph.md), gives

$$
a(n-a)=\frac{n^2}{4}-\left(a-\frac n2\right)^2.
$$

The count is largest when $a$ is an [integer](integer-split.md) nearest $n/2$. For $n=2k$ it is $k^2$; for $n=2k+1$ it is $k(k+1)$. Both equal $\lfloor n^2/4\rfloor$. This proves attainability for every $n$, including the empty [graph](graph-split.md).

A short proof of the upper bound uses [degrees of vertices](degree-graph-theory.md). In a [triangle-free graph](triangle-free-graph.md), the endpoints $u,v$ of an [edge](edge-of-a-graph.md) have disjoint [vertex neighbourhoods](vertex-neighbourhood.md): a [common neighbour](common-neighbour.md) would complete a [triangle in a graph](triangle-in-a-graph.md). Thus $d(u)+d(v)\leq n$. Summing over [edges](edge-of-a-graph.md) counts $d(v)$ once for each of the $d(v)$ [edges](edge-of-a-graph.md) incident to $v$, giving

$$
\sum_{v\in V}d(v)^2=\sum_{uv\in E}(d(u)+d(v))\leq nm.
$$

For $n>0$, the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) and [handshaking lemma](degree-sum-formula.md) yield

$$
4m^2=\left(\sum_{v\in V}d(v)\right)^2\leq n\sum_{v\in V}d(v)^2\leq n^2m.
$$

If $m>0$, division gives $m\leq n^2/4$; $m=0$ is immediate. Since $m$ is an [integer](integer-split.md), apply the [floor function](floor-function.md). The case $n=0$ is immediate too. This proves the bound; the full equality characterization follows from [Turán's theorem](turan-s-theorem.md).

The useful reversal is that more than $\lfloor n^2/4\rfloor$ [edges](edge-of-a-graph.md) force a [triangle in a graph](triangle-in-a-graph.md), whatever their placement. A global count certifies a local pattern. The extremizer is [bipartite](bipartite-graph-split.md), but a [triangle-free graph](triangle-free-graph.md) need not be [bipartite](bipartite-graph-split.md): a five-[vertex](vertex-graph-theory.md) [graph cycle](cycle-in-a-graph.md) has five [edges](edge-of-a-graph.md), below the bound of six. Historically, [Willem Mantel](willem-mantel.md) posed the triangle-exclusion question in 1907.[Robbert Fokkink, Wie weet wie Willem Wijthoff was?, Nieuw Archief voor Wiskunde 5/17(4), December 2016, printed p. 279, Wythoffs bewijs van de stelling van Mantel: attribution of problem 28 in 1907](wie-weet-wie-willem-wijthoff-was-by-robbert-fokkink.md)

**Table of contents**

- [Triangle lower bound one edge above the Mantel threshold](triangle-lower-bound-one-edge-above-the-mantel-threshold.md)

## ↑ Ancestors (7)

1. [Extremal number](extremal-number.md)
2. [Extremal graph theory](extremal-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/17g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/17g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/17f/a/solution.md)
- [Triangle deletion in the alteration method](triangle-deletion-in-the-alteration-method.md)
- [Turán's theorem](turan-s-theorem.md)
