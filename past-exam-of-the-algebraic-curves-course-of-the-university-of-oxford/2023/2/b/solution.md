<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $F=x^3+y^3+3xz^2$, the first [partial derivatives](../../../../partial-derivative.md) are

$$
F_x=3(x^2+z^2),\qquad F_y=3y^2,\qquad F_z=6xz.
$$

Their simultaneous vanishing would force $y=0$, $xz=0$ and $x^2+z^2=0$, hence $x=y=z=0$, which is not a [projective point](../../../../projective-point.md). This also verifies that the given [plane cubic](../../../../plane-cubic.md) is nonsingular.

The [Hessian matrix](../../../../hessian-matrix.md) and its [determinant](../../../../determinant.md) are

$$
\operatorname{Hess}F=6\begin{pmatrix}x&0&z\\0&y&0\\z&0&x\end{pmatrix},
\qquad H_F=216y(x^2-z^2).
$$

Thus the [Hessian curve](../../../../hessian-curve-of-a-plane-curve.md) is the union of $y=0$, $x=z$ and $x=-z$. On $y=0$, the equation of $C$ reduces to $x(x^2+3z^2)=0$, giving

$$
\boxed{[0:0:1],\quad[\mathrm i\sqrt3:0:1],\quad[-\mathrm i\sqrt3:0:1].}
$$

On $x=z$ one must have $z\ne0$, so put $z=x=1$ and obtain $y^3=-4$. On $x=-z$ similarly put $z=1$, $x=-1$, obtaining $y^3=4$. Choose $r\in\mathbb C$ with $r^3=4$ and let $\omega=\exp(2\pi\mathrm i/3)$. The remaining points are

$$
\boxed{[1:-r\omega^j:1],\quad[-1:r\omega^j:1],\qquad j=0,1,2.}
$$

All nine listed [projective points](../../../../projective-point.md) are distinct. They exhaust the intersection with the [Hessian curve](../../../../hessian-curve-of-a-plane-curve.md), so the [Hessian criterion for a flex](../../../../hessian-criterion-for-a-flex.md) proves that these, and only these, are the [flexes](../../../../inflection-point-of-an-algebraic-plane-curve.md) in this example. There are none at infinity: $z=0$ and $H_F=0$ would force $x=y=0$ on $C$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
