<h1 id="17j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $S\subseteq X$, count with reciprocal degrees. On every edge $xy$, $d(x)\ge d(y)$, so

$$
|S|=\sum_{x\in S}\sum_{y\sim x}\frac1{d(x)}
\le\sum_{y\in N(S)}\sum_{\substack{x\in S\\x\sim y}}\frac1{d(y)}
\le|N(S)|.
$$

Hall's condition holds, so [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) supplies the matching.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17J](../../17j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
