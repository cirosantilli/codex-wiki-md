<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the classical regularity setting $u\in C^2(D)\cap C(\overline D)$, with $D$ bounded. Continuity on the [compact set](../../../../../compact-space.md) $\overline D$ guarantees existence of a minimum. The inequality $\Delta u=f\leq0$ means that $u$ is [superharmonic function](../../../../../superharmonic-function.md).

A strict inequality $\Delta u<0$ would immediately exclude an interior minimum, because its [Hessian matrix](../../../../../hessian-matrix.md) there would be positive semidefinite and have nonnegative [trace](../../../../../matrix-trace.md). To handle equality, introduce the [quadratic perturbation proof of the minimum principle](../../../../../quadratic-perturbation-proof-of-the-minimum-principle.md):

$$
u_\varepsilon(x,y)=u(x,y)-\varepsilon(x^2+y^2),\qquad
\Delta u_\varepsilon=f-4\varepsilon<0.
$$

Its minimum must lie on $\partial D$. Choose $R$ so that $x^2+y^2\leq R^2$ on $\overline D$. For any $p\in D$,

$$
u_\varepsilon(p)\geq\min_{\partial D}u_\varepsilon
\geq\min_{\partial D}u-\varepsilon R^2.
$$

Letting $\varepsilon\downarrow0$ gives $u(p)\geq\min_{\partial D}u$. Therefore

$$
\boxed{\min_{\overline D}u=\min_{\partial D}u.}
$$

This asserts that a minimum is attained on the boundary, not that it cannot also be attained inside; a constant [function](../../../../../function-split.md) attains it everywhere.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
