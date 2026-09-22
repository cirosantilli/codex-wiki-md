<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce a second multiplier $b$ and use

$$
\mathcal L=-\sum_i x_i\log x_i-\lambda\left(\sum_i x_i-1\right)
-b\left(\sum_i x_i y_i-Y\right).
$$

The stationary equations become $-\log x_i-1-\lambda-by_i=0$. Writing $a=e^{-1-\lambda}>0$ gives

$$
\boxed{x_i=ae^{-by_i}}.
$$

The two constraints determine the constants through

$$
\boxed{a\sum_{i=1}^n e^{-by_i}=1,\qquad
a\sum_{i=1}^n y_i e^{-by_i}=Y}.
$$

Equivalently, $a=1/Z(b)$ with $Z(b)=\sum_i e^{-by_i}$, and $-d\log Z/db=Y$. This is the [maximum entropy distribution with a prescribed finite mean](../../../../../maximum-entropy-distribution-with-a-prescribed-finite-mean.md).

For nonconstant $y_i$, a strictly positive solution exists exactly when $\min_i y_i<Y<\max_i y_i$. The mean's [derivative](../../../../../derivative.md) with respect to $b$ is $-\operatorname{Var}_b(y)<0$, so $b$ is unique in that case. At either extreme mean no strictly positive solution exists. If all $y_i=y_0$, feasibility requires $Y=y_0$ and the extra [constraint](../../../../../constraint-mechanics.md) is redundant: $x_i=1/n$, while $a,b$ are not separately identifiable. The negative entropy Hessian ensures that any feasible interior [stationary point](../../../../../stationary-point.md) is the unique constrained maximum.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
