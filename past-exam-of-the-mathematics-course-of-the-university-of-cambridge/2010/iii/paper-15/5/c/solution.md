<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First verify the [difference of affine connections is a tensor](../../../../../../difference-of-affine-connections-is-a-tensor.md). Linearity over [smooth functions](../../../../../../smooth-function.md) in $X$ follows from the [affine connection](../../../../../../affine-connection.md) axioms. In $Y$, the two derivative terms cancel:

$$
A(X,fY)=\nabla_X(fY)-\nabla'_X(fY)=fA(X,Y).
$$

Thus $A$ is a smooth $(1,2)$-[tensor field](../../../../../../tensor-field.md), and $A_p(u,v)$ depends only on the tangent vectors $u,v$ at $p$. For any [smooth curve](../../../../../../smooth-curve.md), its two covariant accelerations satisfy

$$
D_t\dot\gamma-D'_t\dot\gamma=A(\dot\gamma,\dot\gamma).
$$

If $A(X,Y)=-A(Y,X)$, its diagonal values vanish. The two [geodesic equations](../../../../../../geodesic-equation.md) are therefore identical, and the connections have the same parametrized [geodesics](../../../../../../geodesic.md).

For necessity, the required local [geodesic](../../../../../../geodesic.md) existence theorem is this: for every smooth [affine connection](../../../../../../affine-connection.md), $p\in M$ and $v\in T_pM$, a unique [geodesic](../../../../../../geodesic.md) exists on some interval about zero with $\gamma(0)=p$ and $\dot\gamma(0)=v$. Indeed the [geodesic equation](../../../../../../geodesic-equation.md) is the smooth first-order [ordinary differential equation](../../../../../../ordinary-differential-equation.md) on position and velocity

$$
\dot x^k=v^k,\qquad \dot v^k=-\Gamma^k{}_{ij}(x)v^iv^j,
$$

so local existence and uniqueness apply. If the two connections have the same parametrized [geodesics](../../../../../../geodesic.md), apply the acceleration identity to this [geodesic](../../../../../../geodesic.md) at zero to obtain $A_p(v,v)=0$ for every $p,v$. Expanding $A_p(u+v,u+v)=0$ gives $A_p(u,v)+A_p(v,u)=0$. Therefore

$$
\boxed{\text{same parametrized geodesics}\quad\Longleftrightarrow\quad
A(X,Y)=-A(Y,X).}
$$

This is the criterion that [parametrized geodesics determine the symmetric part of an affine connection](../../../../../../parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection.md). It concerns equality with the same affine parameters. Agreement merely of unparametrized images is weaker: adding $\alpha(X)Y+\alpha(Y)X$ to a connection, for a smooth one-form $\alpha$, changes acceleration by a multiple of the velocity, which can be absorbed by reparametrization. Such a difference need not be antisymmetric.

Finally, since $\nabla'_XY=\nabla_XY-A(X,Y)$, expand the derivative of the [metric tensor](../../../../../../metric-tensor.md):

$$
(\nabla'_Xg)(Y,Z)
=X(g(Y,Z))-g(\nabla'_XY,Z)-g(Y,\nabla'_XZ)
=(\nabla_Xg)(Y,Z)+g(A(X,Y),Z)+g(Y,A(X,Z)).
$$

Under the assumed [metric compatibility](../../../../../../metric-compatibility.md) of $\nabla$, the first term is zero. Consequently

$$
\boxed{\nabla' g=0\quad\Longleftrightarrow\quad
g(A(X,Y),Z)=-g(Y,A(X,Z))\quad\text{for all }X,Y,Z.}
$$

Equivalently, for each fixed $X$, the endomorphism $A(X,\cdot)$ is skew-adjoint for the [Riemannian metric](../../../../../../riemannian-metric.md). This metric criterion does not require the two connections to have the same [geodesics](../../../../../../geodesic.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
