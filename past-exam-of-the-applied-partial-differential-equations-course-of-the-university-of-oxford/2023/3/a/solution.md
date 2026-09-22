<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Freeze the coefficients at a point. Characteristic normals $(\tau,\xi)\ne(0,0)$ satisfy the homogeneous quadratic [matrix pencil](../../../../matrix-pencil.md) equation $\det(\tau A+\xi B)=0$. In the elementary characteristic classification, two distinct real characteristic directions give a hyperbolic system, no real directions an elliptic system, and a repeated real direction the parabolic case. An identically zero determinant polynomial is a further degeneracy, not covered by that nondegenerate classification.

When $A$ is invertible, write $C=A^{-1}B$. The finite characteristic slopes solve $\det(B-\lambda A)=0$, or

$$
\lambda^2-(\operatorname{tr}C)\lambda+\det C=0.
$$

Its discriminant $(\operatorname{tr}C)^2-4\det C$ is positive, negative, or zero in the three cases above. For the well-posed first-order evolution meaning of [hyperbolicity](../../../../hyperbolicity.md), real eigenvalues must also admit a complete eigenbasis: a repeated but diagonalizable pair is non-strictly hyperbolic rather than a defective parabolic system. Distinct real roots suffice for strict hyperbolicity.

For the given [shallow water equations](../../../../shallow-water-equations.md), subtracting $u$ times mass conservation from momentum conservation and dividing by $h>0$ gives the primitive-variable system

$$
\begin{pmatrix}h\\u\end{pmatrix}_t+\begin{pmatrix}u&h\\1&u\end{pmatrix}\begin{pmatrix}h\\u\end{pmatrix}_x=0.
$$

The [characteristic polynomial](../../../../characteristic-polynomial.md) is $(u-\lambda)^2-h$, so

$$
\boxed{\lambda_-=u-\sqrt h,\qquad\lambda_+=u+\sqrt h}.
$$

They are real and distinct whenever $h>0$, proving strict [hyperbolicity](../../../../hyperbolicity.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the applied partial differential equations course of the University of Oxford](../../../split.md)
5. [Applied partial differential equations course of the University of Oxford](../../../../applied-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
