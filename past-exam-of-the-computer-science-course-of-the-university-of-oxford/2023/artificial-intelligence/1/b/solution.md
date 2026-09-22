<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $F=|V|\le mn$. The ordered position pairs give at most $F^2$ states, or $F(F-1)$ live states after excluding capture. Thus the usual [Big O notation](../../../../../big-o-notation.md) estimate is **$O(m^2n^2)$**. An additional terminal-failure marker changes this by only one.

For $k$ distinguishable foxes, retain $(r,f_1,\ldots,f_k)$. Different foxes may share a square; none may share the rabbit's square in a live state. There are at most $F(F-1)^k$ live position tuples, giving **$O((mn)^{k+1})$**. These counts describe possible encodings; obstacles, starting positions and the fixed fox rule can make the reachable [state space](../../../../../state-space.md) much smaller.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
