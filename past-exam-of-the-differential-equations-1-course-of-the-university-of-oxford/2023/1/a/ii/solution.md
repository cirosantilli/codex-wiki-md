<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $A(t)=\int_0^t a(s)\,ds$. Multiplying the [ordinary differential equation](../../../../../ordinary-differential-equation.md) by the [integrating factor](../../../../../integrating-factor.md) $e^{A(t)}$ and using the [product rule](../../../../../product-rule.md) gives

$$
\frac{d}{dt}\bigl(e^{A(t)}y(t)\bigr)=e^{A(t)}y(t)^2.
$$

Integration from $0$ to $t$ therefore yields the [Volterra integral equation](../../../../../volterra-integral-equation.md)

$$
\boxed{y(t)=be^{-A(t)}+\int_0^t e^{-(A(t)-A(s))}y(s)^2\,ds.}
$$

Conversely, a [continuous function](../../../../../continuous-function.md) satisfying this [integral equation](../../../../../integral-equation.md) becomes continuously differentiable after multiplication by $e^{A(t)}$, by the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md), and satisfies the original [initial value problem](../../../../../initial-value-problem.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
