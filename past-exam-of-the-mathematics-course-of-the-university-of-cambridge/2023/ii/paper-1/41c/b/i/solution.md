<h1 id="41c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first stage is

$$
(I-\mu A_y)\mathbf u^{n+1/2}=\mathbf u^n.
$$

Because $A_y=I\otimes T$, this consists of $m$ independent tridiagonal systems of dimension $m$. The [Thomas algorithm](../../../../../../../tridiagonal-matrix-algorithm.md) solves each in $O(m)$ operations, for a total of $O(m^2)$.

The second stage,

$$
\mathbf u^{n+1}=(I+\mu A_x)\mathbf u^{n+1/2},
$$

is multiplication by a matrix with only $O(m^2)$ nonzero entries, so it also costs $O(m^2)$. Hence one complete step uses at most

$$
\boxed{O(m^2)}
$$

arithmetic operations.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [41C](../../../41c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
