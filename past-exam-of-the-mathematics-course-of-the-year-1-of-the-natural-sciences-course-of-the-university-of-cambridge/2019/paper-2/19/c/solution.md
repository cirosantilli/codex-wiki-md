<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because all variables are positive, the product constraint is equivalent to $\sum_i\ln x_i=\ln a$. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations for

$$
\mathcal L=\sum_{i=1}^n x_i-\lambda\left(\sum_{i=1}^n\ln x_i-\ln a\right)
$$

are $1-\lambda/x_i=0$. Thus every $x_i$ equals $\lambda$, and the constraint requires $\lambda=a^{1/n}$. The candidate [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) is therefore

$$
\boxed{\min\sum_{i=1}^n x_i=na^{1/n},\qquad x_1=\cdots=x_n=a^{1/n}}.
$$

For a global justification, put $y_i=\ln x_i$. The objective becomes the strictly [convex function](../../../../../convex-function.md) $\sum_i e^{y_i}$ on the affine constraint $\sum_i y_i=\ln a$. A stationary point of this restricted [convex function](../../../../../convex-function.md) is its unique global [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md), establishing the claim without presupposing the desired inequality.

Finally take $a=\prod_i x_i$ and divide the minimum bound by $n$. This is the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md):

$$
\boxed{\frac1n\sum_{i=1}^n x_i\geq\left(\prod_{i=1}^n x_i\right)^{1/n}},
$$

with equality exactly when all the positive variables are equal.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
