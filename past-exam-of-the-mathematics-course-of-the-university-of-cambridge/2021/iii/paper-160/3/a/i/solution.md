<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Trace the southeast boundary of the [hook of a Young diagram](../../../../../../../hook-of-a-young-diagram.md) based at $(i,j)$. At each horizontal boundary step record the hook length $h_{i,y}$ of the cell in row $i$ above that step. At each vertical step ending beside row $x$, record $h_{i,j}-h_{x,j}$. Starting at the northeast end and moving to the southwest end, these records increase by one from $1$ to $h_{i,j}$; horizontal and vertical steps are disjoint and account for every step. Therefore the [Hook-interval decomposition at a Young-diagram cell](../../../../../../../hook-interval-decomposition-at-a-young-diagram-cell.md) is

$$
\boxed{
\{1,\ldots,h_{i,j}\}
=\{h_{i,y}:j\leq y\leq\lambda_i\}
\sqcup
\{h_{i,j}-h_{x,j}:i<x\leq\lambda'_j\}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 160](../../../../paper-160-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
