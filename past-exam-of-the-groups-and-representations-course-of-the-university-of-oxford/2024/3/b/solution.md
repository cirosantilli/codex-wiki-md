<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $x=(x_1,x_2,x_3)^T$, $v=(x_4,x_5,x_6)^T$ and $z=x+iv$. Here products of differentials in a [metric tensor](../../../../metric-tensor.md) are symmetric products, unlike the [wedge products](../../../../exterior-product.md) used later. Then

$$
\boxed{g=\sum_{k=1}^3 dz_k\,d\bar z_k
=\frac12\sum_{k=1}^3(dz_k\otimes d\bar z_k+d\bar z_k\otimes dz_k).}
$$

Indeed $dz_k\,d\bar z_k=dx_k^2+dx_{k+3}^2$. A transformation $z'=Uz$ preserves this [metric](../../../../metric.md) whenever $U^\dagger U=I$, because

$$
\sum_k d\bar z'_k\,dz'_k=d\bar z^T U^\dagger U\,dz=d\bar z^Tdz.
$$

Thus the entire [unitary group](../../../../unitary-group.md) $U(3)$ preserves it, including its [special unitary group](../../../../special-unitary-group.md) $SU(3)$.

To obtain a real [matrix](../../../../matrix.md) embedding, write $U=A+iB$ with $A,B$ real. Then

$$
\boxed{\rho:SU(3)\hookrightarrow SO(6),\qquad
\rho(U)=\begin{pmatrix}A&-B\\B&A\end{pmatrix}.}
$$

The [unitarity](../../../../unitary-operator.md) equations imply $A^TA+B^TB=I$ and $A^TB=B^TA$, hence $\rho(U)^T\rho(U)=I$. Multiplication of the block [matrices](../../../../matrix.md) gives $\rho(UV)=\rho(U)\rho(V)$, and the blocks recover $U$, proving injectivity. Finally

$$
\det_{\mathbb R}\rho(U)=\det_{\mathbb C}U\,\det_{\mathbb C}\bar U=|\det_{\mathbb C}U|^2=1.
$$

For this last identity, over the [complex numbers](../../../../complex-number.md) the change of [basis](../../../../basis.md) from $(x,v)$ to $(z,\bar z)$ conjugates $\rho(U)$ to $\operatorname{diag}(U,\bar U)$. This proves that the image lies in the [special orthogonal group](../../../../special-orthogonal-group.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
