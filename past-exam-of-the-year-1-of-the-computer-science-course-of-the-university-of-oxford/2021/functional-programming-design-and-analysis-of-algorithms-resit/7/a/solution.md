<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a global clock starting at zero, incrementing once on discovery and once on finish. Scan starting [vertices](../../../../../vertex-graph-theory.md) and each [adjacency list](../../../../../adjacency-list.md) in increasing numerical order. The first search descends through $1,2,5,7,4$, returns from $4$, and then visits $6$ from $7$. After that search finishes, the unvisited [vertex](../../../../../vertex-graph-theory.md) $3$ starts a second tree.

$$
\begin{array}{c|rrrrrrr}
v&1&2&3&4&5&6&7\\\hline
\pi(v)&-&1&-&7&2&7&5\\
d(v)&1&2&13&5&3&7&4\\
f(v)&12&11&14&6&10&8&9
\end{array}
$$

A dash denotes a root with no predecessor. **$2\to6$ is a forward [edge](../../../../../edge-of-a-graph.md)**: [vertex](../../../../../vertex-graph-theory.md) $6$ is a proper descendant of $2$, but its predecessor is $7$. Its interval satisfies $d(2)<d(6)<f(6)<f(2)$. **$4\to1$ is a back [edge](../../../../../edge-of-a-graph.md)**, because $1$ is still an active ancestor when it is examined. The other non-tree [edge](../../../../../edge-of-a-graph.md) $4\to5$ is also a back [edge](../../../../../edge-of-a-graph.md), while $3\to6$ reaches an already finished [vertex](../../../../../vertex-graph-theory.md) in a different search tree.[§6.1, discovery/finish intervals and edge classification](../../../../../depth-first-search-by-jeff-erickson.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
