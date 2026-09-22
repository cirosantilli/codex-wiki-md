<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

The [characteristic polynomial](../../../../../characteristic-polynomial.md) of the homogeneous [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) is

$$
r^2-2r-3=(r-3)(r+1),
$$

so its [complementary solution](../../../../../homogeneous-solution.md) is $Ae^{3x}+Be^{-x}$. Because the forcing contains the resonant factor $e^{-x}$, set $y=e^{-x}v$. Substitution gives

$$
y''-2y'-3y=e^{-x}(v''-4v')=-16xe^{-x}.
$$

Writing $w=v'$, a polynomial particular solution of $w'-4w=-16x$ is $w=4x+1$, and hence $v=2x^2+x$. Thus

$$
y=Ae^{3x}+(B+2x^2+x)e^{-x}.
$$

Boundedness as $x\to\infty$ forces $A=0$, while the [initial condition](../../../../../initial-condition.md) $y(0)=1$ gives $B=1$. Therefore

$$
\boxed{y(x)=(2x^2+x+1)e^{-x}}.
$$

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
