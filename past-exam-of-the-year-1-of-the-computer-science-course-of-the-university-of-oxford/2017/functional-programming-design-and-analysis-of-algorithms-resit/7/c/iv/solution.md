<h1 id="7/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**False.** Take edges $u\to a$ and $c\to u$, and let the outer DFS loop try vertices in order $a,u,c$. The first call finishes $a$ immediately. The next discovers $u$, whose only outgoing edge reaches already black $a$, so its tree contains only $u$. Finally $c$ sees already black $u$.

Vertex $u$ has both an incoming edge from $c$ and an outgoing edge to $a$, yet is the sole vertex of its DFS tree. Nonzero incoming and outgoing degrees do not require either edge to become a [tree edge in depth-first search](../../../../../../tree-edge-in-depth-first-search.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms (resit)](../../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
