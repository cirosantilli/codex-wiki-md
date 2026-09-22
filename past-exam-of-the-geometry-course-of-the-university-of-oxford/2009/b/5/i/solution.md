<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [inflection point of an algebraic plane curve](../../../../../inflection-point-of-an-algebraic-plane-curve.md) is a smooth point where the tangent has [intersection multiplicity](../../../../../intersection-multiplicity.md) at least three. For a homogeneous defining polynomial $P$ of degree $d$, its [Hessian curve](../../../../../hessian-curve-of-a-plane-curve.md) is defined by the determinant of the matrix of second partial derivatives, of degree $3(d-2)$. In characteristic zero, the smooth inflection points are exactly the smooth points of $C\cap\operatorname{Hess}(C)$.

For a local verification, move a smooth point to $[0:0:1]$ and its tangent to $y=0$, and scale so $P(x,y,1)=y+ax^2+bxy+cy^2+\cdots$. The tangent contact is at least three exactly when $a=0$. The homogeneous Euler identities give the Hessian matrix at that point as $\begin{pmatrix}2a&b&0\\b&2c&d-1\\0&d-1&0\end{pmatrix}$, whose determinant is $-2a(d-1)^2$. This proves the criterion for $d>1$.

For the given cubic, the singularity equations are $x^2+\lambda yz=y^2+\lambda xz=z^2+\lambda xy=0$. No coordinate can vanish at a projective solution, since that would force all three to vanish. Multiplying the equations therefore gives $1=(-\lambda)^3$, so singularity requires $\lambda^3=-1$. Conversely, under that condition the point $[1:1:-1/\lambda]$ satisfies all three equations, and the Euler identity places it on the cubic. Thus

$$
\boxed{C\text{ is nonsingular}\iff\lambda^3\ne-1.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the geometry course of the University of Oxford](../../../../split.md)
6. [Geometry course of the University of Oxford](../../../../../geometry-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
