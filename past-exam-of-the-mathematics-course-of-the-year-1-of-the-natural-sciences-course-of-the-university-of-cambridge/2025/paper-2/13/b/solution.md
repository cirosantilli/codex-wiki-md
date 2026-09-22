<h1 id="13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [differential operator](../../../../../differential-operator.md) on the left is $(D-3)^2$, where $D=d/dt$. Its repeated [characteristic root](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) suggests writing $y=e^{3t}v$. By the [product rule](../../../../../product-rule.md),

$$
y'=e^{3t}(v'+3v),\qquad y''=e^{3t}(v''+6v'+9v),
$$

so the [ordinary differential equation](../../../../../ordinary-differential-equation.md) reduces to $v''=3(t+1)$. Two [antiderivatives](../../../../../antiderivative.md) give

$$
v'=\frac32t^2+3t+A,\qquad
v=\frac12t^3+\frac32t^2+At+B.
$$

The [boundary conditions](../../../../../boundary-condition.md) imply $v(0)=1$ and $v(1)=0$, hence $B=1$ and $A=-3$. Therefore

$$
\boxed{y(t)=e^{3t}\left(\frac12t^3+\frac32t^2-3t+1\right)}.
$$

The calculation of $v''$ verifies the [ordinary differential equation](../../../../../ordinary-differential-equation.md), and the bracket takes the values one and zero at the two endpoints. These [boundary conditions](../../../../../boundary-condition.md) determine both constants uniquely.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [13](../../13.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
