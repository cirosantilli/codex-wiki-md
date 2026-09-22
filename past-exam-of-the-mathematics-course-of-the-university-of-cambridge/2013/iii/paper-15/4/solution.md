<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix the curvature convention

$$
\boxed{R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z}.
$$

To prove [tensoriality](../../../../../tensoriality.md), use $[hX,Y]=h[X,Y]-Y(h)X$ and the connection rules. The two $Y(h)\nabla_XZ$ terms cancel, giving $R(hX,Y)Z=hR(X,Y)Z$. Antisymmetry in $X,Y$ gives linearity over smooth functions in the second input. Expanding the third input gives

$$
R(X,Y)(hZ)=hR(X,Y)Z+\bigl(X(Yh)-Y(Xh)-[X,Y]h\bigr)Z=hR(X,Y)Z.
$$

It is therefore a smooth [tensor](../../../../../tensor.md) of type $(1,3)$. Lowering the output with $g$ gives the type $(0,4)$ [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) $R_4(X,Y,Z,W)=g(R(X,Y)Z,W)$.

For an independent pair $X,Y$, define [sectional curvature](../../../../../sectional-curvature.md) by

$$
K(\operatorname{span}\{X,Y\})=\frac{g(R(X,Y)Y,X)}{g(X,X)g(Y,Y)-g(X,Y)^2}.
$$

Metric compatibility gives $g(R(X,Y)Z,W)=-g(R(X,Y)W,Z)$ by applying $XY-YX-[X,Y]$ to $g(Z,W)$. Together with antisymmetry in $X,Y$, this shows that replacing the pair by $(aX+bY,cX+dY)$ multiplies both numerator and denominator by $(ad-bc)^2$. Thus the value depends only on the plane. Define [Ricci curvature](../../../../../ricci-curvature.md) by $\operatorname{Ric}(Y,Z)=\sum_i g(R(e_i,Y)Z,e_i)$ for any [orthonormal basis](../../../../../orthonormal-basis.md); a trace is independent of the [orthonormal basis](../../../../../orthonormal-basis.md).

For the [curvature of the round unit sphere](../../../../../curvature-of-the-round-unit-sphere.md), the outward unit normal is the position vector $p$. The tangential projection of ambient differentiation is [torsion-free](../../../../../torsion-free-connection.md) and has [metric compatibility](../../../../../metric-compatibility.md), so uniqueness identifies it with $\nabla$. Ambient differentiation $D$ satisfies $D_Xp=X$ and

$$
D_XY=\nabla_XY-g(X,Y)p,
$$

since differentiating $g(Y,p)=0$ gives its normal component. The ambient curvature is zero. Take tangential components of $D_XD_YZ-D_YD_XZ-D_{[X,Y]}Z=0$ to obtain

$$
\boxed{R(X,Y)Z=g(Y,Z)X-g(X,Z)Y}.
$$

Hence

$$
\boxed{R_4(X,Y,Z,W)=g(Y,Z)g(X,W)-g(X,Z)g(Y,W)}.
$$

Every two-plane has [sectional curvature](../../../../../sectional-curvature.md) one. Tracing the first formula gives $\operatorname{Ric}(Y,Z)=ng(Y,Z)-g(Y,Z)$, and consequently

$$
\boxed{\operatorname{Ric}=(n-1)g,\qquad\Lambda=n-1}.
$$

Thus the sphere is an [Einstein manifold](../../../../../einstein-manifold.md). When $n=1$ there are no tangent two-planes, the curvature [tensor](../../../../../tensor.md) is zero and the same Ricci formula gives zero. The declared slot convention fixes all signs.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
