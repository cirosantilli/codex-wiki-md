<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For disjoint nonempty vertex sets $X,Y$, their [edge density of a bipartite graph](../../../../../../edge-density-of-a-bipartite-graph.md) is

$$
d(X,Y)=\frac{e(X,Y)}{|X||Y|}.
$$

The pair $(X,Y)$ is a [$\varepsilon$-regular pair](../../../../../../regular-pair-of-vertex-sets.md) if

$$
|d(X',Y')-d(X,Y)|\leq\varepsilon
$$

whenever $X'\subseteq X$, $Y'\subseteq Y$, $|X'|\geq\varepsilon|X|$, and $|Y'|\geq\varepsilon|Y|$. A partition $V_0,V_1,\ldots,V_m$ is equitable when $|V_1|=\cdots=|V_m|$; $V_0$ is its exceptional class.

The [Szemerédi regularity lemma](../../../../../../szemeredi-regularity-lemma.md) says that for every $\varepsilon>0$ and $m_0$ there are integers $M,n_0$ such that every graph on at least $n_0$ vertices has an equitable partition

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_m
$$

with

$$
m_0\leq m\leq M,
\qquad |V_0|\leq\varepsilon|V|,
$$

for which all but at most $\varepsilon m^2$ pairs $(V_i,V_j)$, $1\leq i<j\leq m$, are $\varepsilon$-regular.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
