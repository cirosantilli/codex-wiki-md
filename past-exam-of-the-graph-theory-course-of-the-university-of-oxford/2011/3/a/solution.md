<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For disjoint nonempty [sets](../../../../set-split.md) $X,Y$, let $e(X,Y)$ count [edges](../../../../edge-of-a-graph.md) between them. Their [edge](../../../../edge-of-a-graph.md) density is

$$
\boxed{d(X,Y)=\frac{e(X,Y)}{|X||Y|}.}
$$

The pair is $\varepsilon$-regular if every $A\subseteq X$ and $B\subseteq Y$ with $|A|\geq\varepsilon|X|$, $|B|\geq\varepsilon|Y|$ satisfies $|d(A,B)-d(X,Y)|\leq\varepsilon$.

An $\varepsilon$-regular partition has disjoint classes $V_0,V_1,\ldots,V_k$ covering $V(G)$, with $|V_0|\leq\varepsilon|V(G)|$, equal positive sizes $|V_1|=\cdots=|V_k|$, and at most $\varepsilon k^2$ unordered pairs $(V_i,V_j)$ with $1\leq i<j\leq k$ that are not $\varepsilon$-regular. The [set](../../../../set-split.md) $V_0$ is exceptional and its pairs need not satisfy regularity.

[Szemerédi regularity lemma](../../../../szemeredi-regularity-lemma.md) states that for every $\varepsilon>0$ and [integer](../../../../integer-split.md) $m_0\geq1$, there are [integers](../../../../integer-split.md) $M,n_0$ such that every [graph](../../../../graph-split.md) with $n\geq n_0$ [vertices](../../../../vertex-graph-theory.md) has such a partition with

$$
\boxed{m_0\leq k\leq M.}
$$

The bounds depend on $\varepsilon,m_0$, not on the [graph](../../../../graph-split.md) order. Using a strict regularity [inequality](../../../../inequality-mathematics.md) or a slightly different [constant](../../../../constant-mathematics.md) in the allowed pair count gives an equivalent conventional version; the displayed convention will be used below.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
