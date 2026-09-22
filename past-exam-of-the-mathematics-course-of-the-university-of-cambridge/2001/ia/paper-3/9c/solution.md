<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

At a [critical point](../../../../../critical-point.md) $x_0$ of a twice continuously differentiable real function, the [Taylor expansion](../../../../../taylor-expansion.md) is

$$
f(x_0+h)=f(x_0)+\frac12h^THh+o(|h|^2),\qquad H=\nabla^2f(x_0).
$$

The [Hessian matrix](../../../../../hessian-matrix.md) is real symmetric, so an orthogonal eigenbasis diagonalizes its [quadratic form](../../../../../quadratic-form.md). If every [eigenvalue](../../../../../eigenvalue.md) is positive, that form is bounded below by a positive multiple of $|h|^2$, which dominates the remainder and gives a strict [local minimum](../../../../../local-minimum.md). If every [eigenvalue](../../../../../eigenvalue.md) is negative, the same argument gives a strict [local maximum](../../../../../local-maximum.md). If both signs occur, displacement along the corresponding eigenvectors produces values above and below $f(x_0)$, so the point is a [saddle point of a scalar function](../../../../../saddle-point-of-a-scalar-function.md). These exhaust a nonsingular [Hessian matrix](../../../../../hessian-matrix.md).

A singular [Hessian matrix](../../../../../hessian-matrix.md) does not always make the classification impossible: nonzero [eigenvalues](../../../../../eigenvalue.md) of both signs still give a saddle. If the [Hessian matrix](../../../../../hessian-matrix.md) is positive or negative semidefinite, higher-order terms in its null directions must be examined. For example, $x^2+y^4$ and $x^2-y^4$ have the same [Hessian matrix](../../../../../hessian-matrix.md) $\operatorname{diag}(2,0)$ at zero, but the first has a strict minimum and the second a saddle. The function $x^2$ has a non-strict minimum along a whole line.

For the given polynomial,

$$
f_x=2x(\alpha-3y+4x^2),\qquad f_y=2y-3x^2.
$$

A stationary point has $y=3x^2/2$ and then $x(2\alpha-x^2)=0$. Hence the origin is always critical, and two additional points exist exactly for $\alpha>0$:

$$
\boxed{(x,y)=(\pm\sqrt{2\alpha},3\alpha).}
$$

The [Hessian matrix](../../../../../hessian-matrix.md) is

$$
H=\begin{pmatrix}2\alpha-6y+24x^2&-6x\\-6x&2\end{pmatrix}.
$$

At the origin it is $\operatorname{diag}(2\alpha,2)$, giving a strict [local minimum](../../../../../local-minimum.md) for $\alpha>0$ and a saddle for $\alpha<0$. At either extra [critical point](../../../../../critical-point.md) it has [determinant](../../../../../determinant.md) $64\alpha-36(2\alpha)=-8\alpha<0$, so both extra points are saddles.

At $\alpha=0$, complete the square:

$$
f(x,y)=\left(y-\frac32x^2\right)^2-\frac14x^4.
$$

Along $x=0$ it is positive away from zero, whereas along $y=3x^2/2$ it is negative away from zero. Thus the origin remains a degenerate saddle despite its nonnegative [Hessian matrix](../../../../../hessian-matrix.md). This is the [parabolic quartic critical-point classification](../../../../../parabolic-quartic-critical-point-classification.md). The complete result is

$$
\boxed{\begin{array}{c|c}
\alpha<0&(0,0)\text{ is the only critical point, a saddle}\\
\alpha=0&(0,0)\text{ is the only critical point, a degenerate saddle}\\
\alpha>0&(0,0)\text{ is a strict local minimum; }(\pm\sqrt{2\alpha},3\alpha)\text{ are saddles}.
\end{array}}
$$

For $\alpha>0$ the [local minimum](../../../../../local-minimum.md) is not global, since along the same parabola $f=\alpha x^2-x^4/4\to-\infty$.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
