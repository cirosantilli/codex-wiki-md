<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every dyadic partition is among the finite partitions on the right-hand side, so the displayed supremum is at least $\lVert f\rVert$. For the converse, the claim is immediate if $\lVert f\rVert=\infty$. If it is finite, apply part (a) to every interval of an arbitrary partition $0\leq t_0<\cdots<t_n=1$:

$$
|f(t_k)-f(t_{k-1})|
\leq\lVert f_{t_k}\rVert-\lVert f_{t_{k-1}}\rVert.
$$

Summing telescopes and gives

$$
\sum_{k=1}^n|f(t_k)-f(t_{k-1})|
\leq\lVert f_1\rVert-\lVert f_{t_0}\rVert
\leq\lVert f\rVert.
$$

Taking the supremum proves that the dyadic definition equals the usual [total variation of a function](../../../../../../total-variation-of-a-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
