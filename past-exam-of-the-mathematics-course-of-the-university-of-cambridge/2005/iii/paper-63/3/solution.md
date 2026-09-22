<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Differentiate the product with the first factor close to the identity. A small displacement of its $x'$ coordinate adds to $x$; a small $y'$ displacement adds to $y$; and a small $z'$ displacement changes $(x,y,z)$ by $(-x,y,1)$ times that displacement. The infinitesimal left actions therefore give the [right-invariant vector fields](../../../../../right-invariant-vector-field.md)

$$
R_1=\partial_x,\qquad R_2=\partial_y,\qquad R_3=\partial_z-x\partial_x+y\partial_y.
$$

For right multiplication, regard $(x',y',z')$ as the fixed point and the second factor as infinitesimal. Its displacements are $(e^{-z'}\delta x,e^{z'}\delta y,\delta z)$; relabeling the coordinates of the fixed point gives the [left-invariant vector fields](../../../../../left-invariant-vector-field.md)

$$
L_1=e^{-z}\partial_x,\qquad L_2=e^z\partial_y,\qquad L_3=\partial_z.
$$

The naming distinction matters: generators of left multiplication are right invariant, whereas generators of right multiplication are left invariant.

All mixed [Lie brackets of vector fields](../../../../../lie-bracket-of-vector-fields.md) vanish. For example, $R_3(e^{-z})=-e^{-z}$ cancels $L_1(-x)=-e^{-z}$ in $[L_1,R_3]$, and $R_3(e^z)=e^z$ cancels $L_2(y)=e^z$ in $[L_2,R_3]$. The brackets with $R_1,R_2$ are zero because the coefficients of the $L_i$ have no $x$ or $y$ dependence; $[L_3,R_3]=0$ because the coefficients of $R_3$ have no $z$ dependence. Hence

$$
\boxed{[L_i,R_j]=0\quad\text{for every }i,j.}
$$

Conceptually, the corresponding flows commute because $(ag)b=a(gb)$, by associativity of the [Lie group](../../../../../lie-group.md) multiplication.

The dual [coframe](../../../../../coframe.md) is

$$
\theta^1=e^zdx,\qquad\theta^2=e^{-z}dy,\qquad\theta^3=dz,
$$

which satisfies $\theta^i(L_j)=\delta^i_j$. Under left multiplication by $(x_0,y_0,z_0)$, the transformed coordinates are $X=x_0+e^{-z_0}x$, $Y=y_0+e^{z_0}y$, $Z=z_0+z$. Therefore $e^Z dX=e^zdx$, $e^{-Z}dY=e^{-z}dy$, and $dZ=dz$. Each one-form is a [left-invariant differential form](../../../../../left-invariant-differential-form.md), so their sum of squares is the [left-invariant metric](../../../../../left-invariant-metric.md)

$$
\boxed{g=(\theta^1)^2+(\theta^2)^2+(\theta^3)^2=e^{2z}dx^2+e^{-2z}dy^2+dz^2.}
$$

This is the standard metric of the [Sol Lie group](../../../../../sol-lie-group.md). As a sign check, $[L_3,L_1]=-L_1$, $[L_3,L_2]=L_2$, while $d\theta^1=\theta^3\wedge\theta^1$ and $d\theta^2=-\theta^3\wedge\theta^2$, in agreement with the [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
