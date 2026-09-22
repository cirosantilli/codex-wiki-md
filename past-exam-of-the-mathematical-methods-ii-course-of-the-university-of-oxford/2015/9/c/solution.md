<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a [stationary point](../../../../stationary-point.md) of a twice continuously differentiable [function](../../../../function-split.md), write the [Hessian matrix](../../../../hessian-matrix.md) as $H=\begin{pmatrix}A&B\\B&C\end{pmatrix}$ and its [determinant](../../../../determinant.md) as $D=AC-B^2$. The quadratic term in the [Taylor expansion](../../../../taylor-expansion.md) determines the local nature whenever $H$ is nonsingular.

If $D>0$, its two [eigenvalues](../../../../eigenvalue.md) have the same sign. With $A>0$ the [quadratic form](../../../../quadratic-form-split.md) is positive definite, giving a strict local minimum; with $A<0$ it is negative definite, giving a strict local maximum. If $D<0$, the [eigenvalues](../../../../eigenvalue.md) have opposite signs and the point is a saddle, with nearby increasing and decreasing directions. Thus

$$
\boxed{D>0,\ A>0:\ \min;\qquad D>0,\ A<0:\ \max;\qquad D<0:\ \text{saddle}}.
$$

If $D=0$, the test is inconclusive. For example, $x^4+y^4$, $-x^4-y^4$ and $x^4-y^4$ all have zero [gradient](../../../../gradient.md) and zero [Hessian matrix](../../../../hessian-matrix.md) at the origin, yet give a minimum, a maximum and a saddle respectively. One must inspect higher-order terms or use another argument in such a case.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
