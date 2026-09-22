<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Integrate the [ordinary differential equation](../../../../ordinary-differential-equation.md) across one step, using the [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md):

$$
y(x_{n+1})-y(x_n)=\int_{x_n}^{x_n+h}f(x,y(x))\,dx.
$$

The [midpoint quadrature rule](../../../../midpoint-quadrature-rule.md) approximates the integral by $h f(x_n+h/2,y(x_n+h/2))$. Approximate the unknown midpoint state by the midpoint value of [linear interpolation](../../../../linear-interpolation.md) between the endpoint states:

$$
y(x_n+h/2)\approx\frac{y_n+y_{n+1}}2.
$$

Combining these approximations gives the [implicit midpoint rule](../../../../implicit-midpoint-rule.md)

$$
\boxed{y_{n+1}=y_n+h f\left(x_n+\frac h2,\frac{y_n+y_{n+1}}2\right),
\qquad y_0=\alpha.}
$$

It is an [implicit time-stepping method](../../../../implicit-time-stepping-method.md) because its new state occurs inside the evaluation of $f$. An equivalent derivation uses a straight-line approximation on the step and imposes the [ordinary differential equation](../../../../ordinary-differential-equation.md) at its midpoint, a one-stage [collocation method](../../../../collocation-method.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
