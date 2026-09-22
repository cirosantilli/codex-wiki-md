<h1 id="11f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to $Y_1=X$ and the [indicator variable](../../../../../../indicator-variable.md) $Y_2=\mathbf1_A$. Since $\mathbf1_A^2=\mathbf1_A$, it gives

$$
\bigl(\mathbb E[X\mathbf1_A]\bigr)^2\leq\mathbb E[X^2]\,\mathbb P(A).
$$

Both sides of the [truncated first moment bound](../../../../../../truncated-first-moment-bound.md) in part (a) are nonnegative, so squaring it preserves the inequality. Combining the bounds and dividing by the positive [second moment](../../../../../../second-moment.md) proves

$$
\boxed{\mathbb P\bigl(X>\theta\mathbb E[X]\bigr)\geq(1-\theta)^2\frac{\mathbb E[X]^2}{\mathbb E[X^2]}.}
$$

This is the [Paley-Zygmund inequality](../../../../../../paley-zygmund-inequality.md). It includes $\theta=0$; at $\theta=1$ the lower bound is zero and remains valid.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
