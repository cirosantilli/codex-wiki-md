<h1 id="10/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For general coordinates $q=(a,b,c)$ expressed as functions of $u=(u,v,w)$, the [chain rule](../../../../../chain-rule.md) gives $dq=J\,du$, where

$$
J=\frac{\partial(a,b,c)}{\partial(u,v,w)}
=\begin{pmatrix}a_u&a_v&a_w\\b_u&b_v&b_w\\c_u&c_v&c_w\end{pmatrix}.
$$

The [Jacobian determinant](../../../../../jacobian-determinant.md) is the oriented volume scaling of this linearized map. Thus the unsigned [volume element](../../../../../volume-element.md) transforms as $da\,db\,dc=|\det J|\,du\,dv\,dw$. Where the coordinate change is invertible, the inverse [Jacobian determinant](../../../../../jacobian-determinant.md) is $1/\det J$, by the [Jacobian chain rule](../../../../../multivariable-chain-rule.md).

For [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), use $x=r\cos\phi$, $y=r\sin\phi$, and unchanged height $z$. Direct differentiation gives

$$
\frac{\partial(x,y,z)}{\partial(r,\phi,z)}
=\begin{pmatrix}\cos\phi&-r\sin\phi&0\\\sin\phi&r\cos\phi&0\\0&0&1\end{pmatrix},
$$

whose [determinant](../../../../../determinant.md) is $r$. Therefore

$$
\boxed{dV=r\,dr\,d\phi\,dz,\qquad
\det\frac{\partial(r,\phi,z)}{\partial(x,y,z)}=\frac1r\quad(r>0).}
$$

Both directions are displayed because “from Cartesian to cylindrical” can refer either to the derivative of the new coordinates or to the factor used in transforming a Cartesian volume integral. They are reciprocals; the cylindrical axis is a coordinate degeneracy.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [10](../../../10.md)
4. [2019 resit](../../../../2019-resit-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

## ← Incoming links (1)

- [Solution](../ii/solution.md)
