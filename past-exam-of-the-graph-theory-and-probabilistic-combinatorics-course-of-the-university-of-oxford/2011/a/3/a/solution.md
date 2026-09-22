<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For disjoint nonempty [sets](../../../../../set-split.md) $X,Y$, let $e(X,Y)$ count [edges](../../../../../edge-of-a-graph.md) between them. Their [edge](../../../../../edge-of-a-graph.md) density is

$$
\boxed{d(X,Y)=\frac{e(X,Y)}{|X||Y|}.}
$$

The pair is $\varepsilon$-regular if every $A\subseteq X$ and $B\subseteq Y$ with $|A|\geq\varepsilon|X|$, $|B|\geq\varepsilon|Y|$ satisfies $|d(A,B)-d(X,Y)|\leq\varepsilon$.

An $\varepsilon$-regular partition has disjoint classes $V_0,V_1,\ldots,V_k$ covering $V(G)$, with $|V_0|\leq\varepsilon|V(G)|$, equal positive sizes $|V_1|=\cdots=|V_k|$, and at most $\varepsilon k^2$ unordered pairs $(V_i,V_j)$ with $1\leq i<j\leq k$ that are not $\varepsilon$-regular. The [set](../../../../../set-split.md) $V_0$ is exceptional and its pairs need not satisfy regularity.

[Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) states that for every $\varepsilon>0$ and [integer](../../../../../integer-split.md) $m_0\geq1$, there are [integers](../../../../../integer-split.md) $M,n_0$ such that every [graph](../../../../../graph-split.md) with $n\geq n_0$ [vertices](../../../../../vertex-graph-theory.md) has such a partition with

$$
\boxed{m_0\leq k\leq M.}
$$

The bounds depend on $\varepsilon,m_0$, not on the [graph](../../../../../graph-split.md) order. Using a strict regularity [inequality](../../../../../inequality-mathematics.md) or a slightly different [constant](../../../../../constant-mathematics.md) in the allowed pair count gives an equivalent conventional version; the displayed convention will be used below.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
