<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $F=x^3+y^3+13z^3-2xyz$. The [Hessian criterion for flexes of a plane cubic](../../../../../../hessian-criterion-for-flexes-of-a-plane-cubic.md) applies because the projective cubic is smooth. To check smoothness, a singular point with all coordinates nonzero would satisfy $3x^2=2yz$, $3y^2=2xz$, $39z^2=2xy$. Multiplication would force $351=8$, a contradiction. If one coordinate is zero, the three equations force all coordinates to vanish, which is not a projective point.

For completeness, the [Hessian criterion for flexes of a plane cubic](../../../../../../hessian-criterion-for-flexes-of-a-plane-cubic.md) follows locally by putting a smooth point at $(0:0:1)$ and its tangent at $y=0$. After normalization the homogeneous cubic has terms $yz^2+ax^2z+bxyz+cy^2z$ and terms cubic in $x,y$. Its tangent has contact order three precisely when $a=0$. Its [Hessian matrix](../../../../../../hessian-matrix.md) at the point has determinant $-8a$, giving exactly the same condition.

For the present cubic the Hessian determinant is

$$
\det\begin{pmatrix}
6x&-2z&-2y\\
-2z&6y&-2x\\
-2y&-2x&78z
\end{pmatrix}
=-24(x^3+y^3+13z^3)+2792xyz.
$$

On $F=0$ this is $2744xyz=8\cdot343\,xyz$. Thus the [plane cubic flexes](../../../../../../inflection-point-of-a-plane-cubic.md) are exactly the points on the cubic with $xyz=0$. Let $c=\sqrt[3]{13}$ and let $\omega$ be a primitive cube root of unity. The complete list over the [algebraic closure](../../../../../../algebraic-closure.md) is

$$
\boxed{(1:-\omega^j:0),\quad(-c\omega^j:0:1),\quad(0:-c\omega^j:1),\qquad j=0,1,2.}
$$

These nine points are distinct, and the Hessian calculation proves there are no others. They are the [flexes of a Hesse cubic](../../../../../../flexes-of-a-hesse-cubic.md). The only rational one is $O'=(1:-1:0)$: the other two points with $z=0$ require a nonrational cube root of unity, and a rational point in either remaining triple would give a rational cube root of $-13$. By prime valuations, $13$ is not a rational cube.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
