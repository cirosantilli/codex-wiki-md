<h1 id="4c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Completing the square in the [optimization constraint](../../../../../../optimization-constraint.md) gives

$$
\left(x_2-\frac32x_1\right)^2=\frac14x_1^2-1.
$$

The left side is nonnegative, so every feasible point has $x_1^2\geq4$. Equality is feasible precisely when $x_2=3x_1/2$ and $x_1=\pm2$. Thus **the global minimum is**

$$
\boxed{\min x_1^2=4,\qquad (x_1,x_2)=(2,3)\text{ or }(-2,-3).}
$$

There is **no maximum**: for every $|x_1|\geq2$, the values $x_2=3x_1/2\pm\sqrt{x_1^2/4-1}$ satisfy the [optimization constraint](../../../../../../optimization-constraint.md), allowing $x_1^2$ to be arbitrarily large. This direct argument also establishes that the two stationary points are the only [local minima](../../../../../../local-minimum.md) on the two branches of the constraint curve.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4C](../../4c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
