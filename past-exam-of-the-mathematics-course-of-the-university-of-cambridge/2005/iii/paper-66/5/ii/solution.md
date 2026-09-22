<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Evaluate all quantities at $(u_0,v_0)$ and assume a [regular surface](../../../../../../smooth-surface.md) point, $S_u\times S_v\ne0$. The [tangent plane](../../../../../../tangent-plane.md) passes through $S_0=S(u_0,v_0)$ and is spanned by $S_u,S_v$. Thus

$$
\boxed{x=S_0+\alpha S_u+\beta S_v,\qquad (S_u\times S_v)\cdot(x-S_0)=0.}
$$

Choose the [unit normal](../../../../../../unit-normal.md) $n=(S_u\times S_v)/\|S_u\times S_v\|$. The [first fundamental form](../../../../../../first-fundamental-form.md) has coefficients

$$
E=S_u\cdot S_u,\qquad F=S_u\cdot S_v,\qquad G=S_v\cdot S_v,
$$

while the [second fundamental form](../../../../../../second-fundamental-form-split.md) has coefficients

$$
e=n\cdot S_{uu},\qquad f=n\cdot S_{uv},\qquad g=n\cdot S_{vv}.
$$

To derive the [curvature](../../../../../../curvature.md) formula, differentiate $n\cdot S_u=n\cdot S_v=0$. This gives $-n_u\cdot S_u=e$, $-n_u\cdot S_v=f$, $-n_v\cdot S_u=f$ and $-n_v\cdot S_v=g$. Therefore the [shape operator](../../../../../../shape-operator.md) $-dn$, expressed in the tangent basis, is

$$
\begin{pmatrix}E&F\\F&G\end{pmatrix}^{-1}\begin{pmatrix}e&f\\f&g\end{pmatrix}.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are the [principal curvatures](../../../../../../principal-curvature.md). Their product, the [Gaussian curvature](../../../../../../gaussian-curvature.md), is its [determinant](../../../../../../determinant.md):

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}.}
$$

Regularity ensures $EG-F^2=\|S_u\times S_v\|^2>0$. Reversing $n$ changes the signs of $e,f,g$ and both [principal curvatures](../../../../../../principal-curvature.md) but leaves $K$ unchanged. At a singular parameter point this quotient and the cross-product [normal vector](../../../../../../normal-vector.md) are undefined; an alternative regular chart or separate geometric analysis is required.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
