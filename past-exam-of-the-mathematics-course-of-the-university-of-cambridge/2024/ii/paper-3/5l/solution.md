<h1 id="5l/solution">Solution</h1>

↑ **Parent:** [5L](../5l.md)

In a linear model containing an intercept, the normal equations make the residual [vector](../../../../../vector.md) $e$ orthogonal to every design column. In particular $e\perp\mathbf1$, so

$$
\sum_{i=1}^{50}e_i=\mathbf1^Te=0
$$

up to floating-point rounding.

The second design [matrix](../../../../../matrix.md) has $49$ random Gaussian columns plus the intercept, hence is a random $50\times50$ [matrix](../../../../../matrix.md). It has full rank with probability one because the [determinant](../../../../../determinant.md) vanishes only on a measure-zero algebraic set. Its column space is then all of $\mathbb R^{50}$, so the fitted [vector](../../../../../vector.md) equals $Y$, the residual sum of squares is zero, and $R^2=1$.

## ↑ Ancestors (10)

1. [5L](../5l.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
