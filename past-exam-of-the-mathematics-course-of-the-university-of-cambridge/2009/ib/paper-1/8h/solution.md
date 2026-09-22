<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

The point $(x_1,x_2,x_3)=(4,2,2)$ is nonnegative and makes all three inequalities equalities, with objective value $20$. To certify global optimality, combine the first upper bound with coefficient $1/2$, the second with coefficient one, and the lower bound with coefficient $-3/2$:

$$
\begin{aligned}
3x_1+2x_2+2x_3&=\tfrac12(7x_1+3x_2+5x_3)+(x_1+2x_2+x_3)-\tfrac32(x_1+x_2+x_3)\\
&\le\tfrac12\cdot44+10-\tfrac32\cdot8=20.
\end{aligned}
$$

This is a [weak duality](../../../../../weak-duality.md) certificate for the [linear program](../../../../../linear-programming.md). The feasible point attains the bound, so **the optimal solution is $(4,2,2)$ and the maximum is $20$**. Equality forces each of the three constraints to be active; their simultaneous equations have this unique solution.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
