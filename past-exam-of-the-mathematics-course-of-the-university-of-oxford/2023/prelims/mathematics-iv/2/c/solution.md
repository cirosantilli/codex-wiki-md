<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $N=(n_1,n_2,n_3)$. Restriction to the [plane](../../../../../../plane.md) $z=0$ gives

$$
M_{11}x^2+(M_{12}+M_{21})xy+M_{22}y^2+n_1x+n_2y+k=0.
$$

This is an equation of [degree](../../../../../../degree-of-a-polynomial.md) at most two in two [Cartesian coordinates](../../../../../../cartesian-coordinate-system.md), the general algebraic form of a [conic](../../../../../../conic-section.md), with possible [degenerate conics](../../../../../../degenerate-conic.md) and an [empty set](../../../../../../empty-set.md) of real points. No [determinant](../../../../../../determinant.md) hypothesis is needed for this substitution.

For an arbitrary [plane](../../../../../../plane.md), choose a point $\mathbf x_0$ and an [orthonormal basis](../../../../../../orthonormal-basis.md) $\mathbf e,\mathbf f$ of its direction [linear subspace](../../../../../../vector-subspace.md). Put $B=(\mathbf e\ \mathbf f)$ and $\mathbf x=\mathbf x_0+B\boldsymbol\xi$, where $\boldsymbol\xi=(s,t)^T$. With $S=(M+M^T)/2$, the [symmetric part of a matrix](../../../../../../symmetric-part-of-a-matrix.md), the restricted equation is

$$
\boxed{\boldsymbol\xi^TB^TSB\boldsymbol\xi+(2\mathbf x_0^TSB+NB)\boldsymbol\xi+\mathbf x_0^TS\mathbf x_0+N\mathbf x_0+k=0.}
$$

This proves the plane-section result whenever “[conic](../../../../../../conic-section.md)” allows the appropriate degeneracies. A [rigid motion](../../../../../../rigid-transformation.md) taking the chosen [plane](../../../../../../plane.md) to $z=0$ gives the same argument.

**The source's assumption $\det M\ne0$ does not guarantee a nondegenerate [conic](../../../../../../conic-section.md).** Even with $M=I$ and $f=x^2+y^2+z^2-1$, the section $z=1$ is a single [point](../../../../../../point-geometry.md), and $z=2$ has no real points. With the nonsingular [symmetric matrix](../../../../../../symmetric-matrix.md) giving $f=2xz+y^2$, the section $z=0$ is the repeated [straight line](../../../../../../straight-line.md) $y=0$.

There is a further literal omission: the source does not assume $M$ is symmetric. For

$$
M=\begin{pmatrix}0&1&1\\-1&0&1\\1&-1&0\end{pmatrix},\qquad N=0,\qquad k=0,
$$

one has $\det M=2$ but $f=2xz$. Thus the section $z=0$ is the entire [plane](../../../../../../plane.md), rather than a [conic](../../../../../../conic-section.md). Only $S$ controls the [quadratic form](../../../../../../quadratic-form-split.md); invertibility of an arbitrary $M$ cannot remove this exception. If the intended hypothesis is that $M$ is symmetric and nonsingular, the quadratic restriction to a [plane](../../../../../../plane.md) cannot vanish identically: otherwise $B^TMB=0$, so $M$ would map a two-dimensional [linear subspace](../../../../../../vector-subspace.md) injectively into its one-dimensional [orthogonal complement](../../../../../../orthogonal-complement.md), which is impossible. Degenerate and empty sections still remain possible.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
