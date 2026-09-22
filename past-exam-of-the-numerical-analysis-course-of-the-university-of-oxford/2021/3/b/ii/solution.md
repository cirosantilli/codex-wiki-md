<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Backward Euler method](../../../../../backward-euler-method.md) uses the new point:

$$
y_{n+1}=y_n-hx_{n+1}y_{n+1}^2,
\qquad x_{n+1}=x_n+h.
$$

Writing $a=h(x_n+h)>0$ gives the [quadratic equation](../../../../../quadratic-equation.md) $ay_{n+1}^2+y_{n+1}-y_n=0$. Starting from $y_n>0$, its two [polynomial roots](../../../../../root-of-a-polynomial.md) have opposite signs. The positive root, which continues the solution as $h\to0$, is

$$
\boxed{y_{n+1}=\frac{-1+\sqrt{1+4h(x_n+h)y_n}}{2h(x_n+h)}.}
$$

The other root is negative and does not approach $y_n$ as $h\to0$. Rationalizing the numerator gives an equivalent form that avoids [cancellation error](../../../../../cancellation-error.md) when the [step size](../../../../../step-size.md) is small:

$$
\boxed{y_{n+1}=\frac{2y_n}{1+\sqrt{1+4h(x_n+h)y_n}}.}
$$

The defining [quadratic equation](../../../../../quadratic-equation.md) gives $0<y_{n+1}<y_n$ for this root, so positivity is maintained inductively from $y_0=1$. The branch choice is part of specifying the [Backward Euler method](../../../../../backward-euler-method.md) here: the algebraic update alone has two solutions.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
