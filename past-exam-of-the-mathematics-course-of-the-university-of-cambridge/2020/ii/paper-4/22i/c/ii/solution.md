<h1 id="22i/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The preceding estimate makes $(x_k)$ [equicontinuous](../../../../../../../equicontinuity.md), and

$$
\lVert x_k(t)-x_0\rVert\leq Mt
$$

makes it uniformly bounded. The [Arzelà-Ascoli theorem](../../../../../../../arzela-ascoli-theorem.md) therefore supplies a subsequence converging uniformly to a continuous function $x:[0,1]\to\mathbb R^n$. On every mesh interval,

$$
\lVert x_k(t)-y_k(t)\rVert\leq\frac Mk,
$$

including an endpoint by using the adjacent interval. Consequently $y_k\to x$ uniformly along the same subsequence.

All $x_k(t)$ and $y_k(t)$ lie in one compact ball. The restriction of the continuous [vector field](../../../../../../../vector-field.md) $F$ to that ball is [uniformly continuous](../../../../../../../uniform-continuity.md), so $F\circ y_k\to F\circ x$ uniformly. Passing to the limit in the defining equation gives

$$
x(t)=x_0+\int_0^tF(x(s))\,ds.
$$

The [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) now makes $x$ differentiable and yields $x'(t)=F(x(t))$. This proves the required special case of the [Peano existence theorem](../../../../../../../peano-existence-theorem.md); uniqueness need not hold because $F$ was assumed continuous but not locally [Lipschitz continuous](../../../../../../../lipschitz-continuity.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [22I](../../../22i.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
