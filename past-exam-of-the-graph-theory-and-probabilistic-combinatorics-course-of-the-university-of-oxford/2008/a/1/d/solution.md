<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Add $s$ adjacent to every vertex of $V_1$ and $t$ adjacent to every vertex of $V_2$. Suppose an $s$–$t$ separator $C$ has fewer than $n$ vertices. It cannot contain all of either class. Choose $x\in V_1\setminus C$ and $y\in V_2\setminus C$. No edge can join the remaining two classes, since it would give a three-edge $s$–$t$ path. Hence every neighbour of $x$ lies in $C\cap V_2$, and every neighbour of $y$ lies in $C\cap V_1$. The minimum-degree bound implies

$$
|C|\ge|C\cap V_1|+|C\cap V_2|\ge n/2+n/2=n,
$$

a contradiction. [Menger's theorem](../../../../../menger-theorem.md) therefore gives $n$ internally vertex-disjoint $s$–$t$ paths. Each uses at least one vertex of each original class, and only $n$ vertices are available in each class. Every path must consequently use exactly one of each. Their middle edges form **a [perfect matching](../../../../../perfect-matching.md)**.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
