<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [linear spline](../../../../linear-spline.md) is a [continuous function](../../../../continuous-function.md) whose restriction to every [interval](../../../../interval-mathematics.md) $[x_{i-1},x_i]$ is a [polynomial](../../../../polynomial-split.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) at most one. With $h_i=x_i-x_{i-1}$ and $\ell_i=\ell(x_i)$, [linear interpolation](../../../../linear-interpolation.md) gives

$$
\ell(x)=\frac{x_i-x}{h_i}\ell_{i-1}+\frac{x-x_{i-1}}{h_i}\ell_i,
\qquad x_{i-1}\leq x\leq x_i.
$$

Integrating the two [linear polynomials](../../../../linear-polynomial.md) and adding the contributions gives

$$
\boxed{\int_{x_0}^{x_n}\ell(x)\,dx=\sum_{i=1}^n\frac{h_i}{2}\bigl(\ell_{i-1}+\ell_i\bigr).}
$$

This is the [composite trapezoidal rule](../../../../composite-trapezoidal-rule.md) applied to the nodal values, and it is exact for the [linear spline](../../../../linear-spline.md) itself, including nonuniform [spline knots](../../../../spline-knot.md).

A [cubic spline](../../../../cubic-spline.md) on this [partition of an interval](../../../../partition-of-an-interval.md) is a [function](../../../../function-split.md) $S\in C^2[x_0,x_n]$ that restricts to a [polynomial](../../../../polynomial-split.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) at most three on every [interval](../../../../interval-mathematics.md) $[x_{i-1},x_i]$. Thus its [second derivative](../../../../second-derivative.md) is continuous and piecewise of [polynomial degree](../../../../degree-of-a-polynomial.md) at most one: **$S''$ is a [linear spline](../../../../linear-spline.md) on the same [spline knots](../../../../spline-knot.md)**. Its [third derivative](../../../../third-derivative.md) is constant on each open [interval](../../../../interval-mathematics.md) and can jump across the [spline knots](../../../../spline-knot.md); its [fourth derivative](../../../../fourth-derivative.md) vanishes inside each open [interval](../../../../interval-mathematics.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
