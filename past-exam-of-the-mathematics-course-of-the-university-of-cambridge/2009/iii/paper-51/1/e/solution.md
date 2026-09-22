<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A classical query with known answer bit $z$ reveals exactly the one bit $f(x,y)$, since it returns $z\oplus f(x,y)$. For the four promised [Boolean functions](../../../../../../boolean-function.md), the value table is

$$
\begin{array}{c|cccc}
(x,y)&1&y&x&x\oplus y\\\hline
00&1&0&0&0\\
01&1&1&0&1\\
10&1&0&1&1\\
11&1&1&1&0
\end{array}
$$

Every possible first query splits the four alternatives into one class of size one and another of size three. On the branch with three remaining alternatives, a second binary answer can separate at most two classes. At least two alternatives therefore still agree on that branch, regardless of how the second query was chosen adaptively. This [decision tree](../../../../../../decision-tree.md) argument proves that a procedure guaranteed to identify every alternative needs at least three queries in the worst case.

For sufficiency, query $00,01,10$. The three-bit answer strings for $1,y,x,x\oplus y$ are respectively $111,010,001,011$, which are all distinct. Hence **the exact classical worst-case query requirement is three**. Some individual branches can terminate sooner; the lower bound does not assert that every oracle requires three queries.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
