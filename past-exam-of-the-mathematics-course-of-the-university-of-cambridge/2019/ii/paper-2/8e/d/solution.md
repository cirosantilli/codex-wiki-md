<h1 id="8e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By the multivariable [chain rule](../../../../../../chain-rule.md) and [Hamilton's equations](../../../../../../hamilton-s-equations.md),

$$
\frac{df}{dt}
=\sum_i\left(
\frac{\partial f}{\partial q_i}\dot q_i
+\frac{\partial f}{\partial p_i}\dot p_i
\right)+\frac{\partial f}{\partial t}
=\sum_i\left(
\frac{\partial f}{\partial q_i}\frac{\partial H}{\partial p_i}
-\frac{\partial f}{\partial p_i}\frac{\partial H}{\partial q_i}
\right)+\frac{\partial f}{\partial t}.
$$

The sum is the [Poisson bracket](../../../../../../poisson-bracket.md) $\{f,H\}$, giving

$$
\boxed{\frac{df}{dt}=\{f,H\}+\frac{\partial f}{\partial t}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [8E](../../8e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
