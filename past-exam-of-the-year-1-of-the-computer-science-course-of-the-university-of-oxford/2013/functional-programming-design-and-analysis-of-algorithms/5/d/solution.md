<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret the source's $m$ as the maximum finite [shortest-path distance](../../../../../shortest-path-distance.md) among reachable pairs, taking $m=0$ when only length-zero [graph paths](../../../../../path-in-a-graph.md) are needed. This is the length bound required for [reflexive transitive closure](../../../../../reflexive-transitive-closure.md). A directed [graph cycle](../../../../../cycle-in-a-graph.md) permits arbitrarily long [walks](../../../../../walk-in-a-graph.md), so the maximum length of all possible [walks](../../../../../walk-in-a-graph.md) would not be a finite termination parameter.[p. 6, Question 5(d), phrase “maximum path length in the transitive closure”](../../../../../functional-programming-design-and-analysis-of-algorithms-examination-paper-by-the-university-of-oxford-2013.md)

For the elementary dense implementation, each [Boolean matrix multiplication](../../../../../boolean-matrix-multiplication.md) evaluates all $n^3$ triples $(i,t,j)$, with no early exit. Each equality test costs $O(n^2)$. Starting from $P_1$, the algorithm reaches $P_m$ after $m-1$ updates when $m\geq1$, then performs one further update to detect stability. Consequently, for $n\geq2$,

$$
\boxed{T_{\mathrm{extend}}=\Theta(n^3\max\{1,m\}),\qquad \text{auxiliary space}=\Theta(n^2).}
$$

For the usual nontrivial case $m\geq1$, this is $\Theta(mn^3)$. Since $m\leq n-1$, the overall worst case is $\Theta(n^4)$. This bound is tight for this implementation: the directed chain $0\to1\to\cdots\to n-1$ has $m=n-1$ and gains previously unknown pairs at every length until then, while every update scans all triples. This tightness does not claim an inherent lower bound for the [reflexive transitive closure](../../../../../reflexive-transitive-closure.md) problem; it concerns the specified repeated-extension [algorithm](../../../../../algorithm-split.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
