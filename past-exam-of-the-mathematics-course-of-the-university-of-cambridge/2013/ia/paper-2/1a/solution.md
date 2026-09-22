<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

The [characteristic polynomial](../../../../../characteristic-polynomial.md) factors as $(r-2)(r+1)$, so the [complementary solution](../../../../../homogeneous-solution.md) is $Ae^{2t}+Be^{-t}$. Each exponential forcing resonates with a homogeneous mode; the [method of undetermined coefficients](../../../../../method-of-undetermined-coefficients.md) therefore uses $te^{2t}$ and $te^{-t}$. Substitution gives the [particular solution](../../../../../particular-solution.md) $te^{2t}-te^{-t}-3t$. Thus

$$
y=(A+t)e^{2t}+(B-t)e^{-t}-3t.
$$

The [initial conditions](../../../../../initial-condition.md) give $A+B=0$ and $2A-B-3=0$. Hence

$$
\boxed{y(t)=(t+1)e^{2t}-(t+1)e^{-t}-3t}.
$$

The factors of $t$ in the [particular solution](../../../../../particular-solution.md) are essential: an unmodified exponential trial lies in the [kernel](../../../../../kernel-of-a-linear-map.md) of the differential operator.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
