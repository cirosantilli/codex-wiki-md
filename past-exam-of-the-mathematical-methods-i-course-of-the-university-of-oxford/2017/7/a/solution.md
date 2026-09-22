<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x>0$, use the [Euler differential equation](../../../../cauchy-euler-equation.md) substitution $t=\ln x$, so $x=e^t$, $xy'=\dot y$ and $x^2y''=\ddot y-\dot y$. The transformed equation is

$$
\ddot y+\dot y-2y=e^t.
$$

Its [characteristic polynomial](../../../../characteristic-polynomial.md) factors as $(r-1)(r+2)$. The forcing $e^t$ coincides with a homogeneous solution, so the [method of undetermined coefficients](../../../../method-of-undetermined-coefficients.md) requires a particular solution $y_p=At e^t$. Substitution gives $3Ae^t=e^t$, hence $A=1/3$. Transforming back,

$$
y(x)=C_1x+C_2x^{-2}+\frac{x\ln x}{3}.
$$

The conditions at $x=1$ give $C_1+C_2=0$ and $C_1-2C_2+1/3=0$, so

$$
\boxed{y(x)=\frac{x\ln x}{3}-\frac{x}{9}+\frac1{9x^2},\qquad x>0.}
$$

Differentiating confirms both initial values and the original equation. The solution interval containing $x=1$ excludes the singular point $x=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
