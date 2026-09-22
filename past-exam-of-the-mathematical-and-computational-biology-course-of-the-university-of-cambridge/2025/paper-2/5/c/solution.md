<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is an [immigration--death process](../../../../../immigration-death-process.md), equivalently an [M-M-infinity queue](../../../../../m-m-%E2%88%9E-queue.md): admission occurs at rate $\alpha$ regardless of occupancy, and each of $n$ animals is discharged independently at rate $\delta$. Its state-transition diagram through four animals is

$$
0\underset{\delta}{\overset{\alpha}{\rightleftarrows}}1\underset{2\delta}{\overset{\alpha}{\rightleftarrows}}2\underset{3\delta}{\overset{\alpha}{\rightleftarrows}}3\underset{4\delta}{\overset{\alpha}{\rightleftarrows}}4\underset{5\delta}{\overset{\alpha}{\rightleftarrows}}\cdots.
$$

Every upper arrow points right and every lower arrow points left. Thus $q_{n,n+1}=\alpha$ and $q_{n,n-1}=n\delta$ for $n\geq1$, with no discharge from zero. Four is only the limit of the requested sketch, not an absorbing state or a capacity boundary.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
