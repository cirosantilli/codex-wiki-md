<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume the level set is regular and non-null. The latter hypothesis is necessary: a [null hypersurface](../../../../../null-hypersurface.md) has a degenerate [induced metric](../../../../../induced-metric.md) and hence no ordinary intrinsic [Levi-Civita connection](../../../../../levi-civita-connection.md) determined by that metric. Normalize the [normal vector](../../../../../normal-vector.md) and define the [non-null hypersurface projection](../../../../../non-null-hypersurface-projection.md) by

$$
n_a=\frac{\partial_af}{\sqrt{|g^{bc}\partial_bf\partial_cf|}},\qquad \varepsilon=n_an^a=\pm1,\qquad P^a{}_b=\delta^a{}_b-\varepsilon n^an_b,\qquad h_{ab}=g_{ab}-\varepsilon n_an_b.
$$

Here $h$ denotes the [induced metric](../../../../../induced-metric.md) restricted to [tangent vectors](../../../../../tangent-vector.md), while its ambient extension annihilates $n$. The intrinsic [covariant derivative](../../../../../covariant-derivative.md) is $D_XY=P\nabla_XY$ for tangent [vector fields](../../../../../vector-field.md). Projection of the ambient [torsion-free connection](../../../../../torsion-free-connection.md) and [metric compatibility](../../../../../metric-compatibility.md) shows that $D$ is the [Levi-Civita connection](../../../../../levi-civita-connection.md) of $h$. Define the [extrinsic curvature](../../../../../extrinsic-curvature.md) by $K(X,Y)=g(\nabla_Xn,Y)$, or $K_{ab}=P^c{}_aP^d{}_b\nabla_cn_d$. It is symmetric: differentiating the defining function twice and projecting removes the derivative of its normalization, leaving a multiple of its symmetric [Hessian](../../../../../hessian-matrix.md). This sign convention makes the scalar [second fundamental form](../../../../../second-fundamental-form-split.md) $g(n,\nabla_XY)=-K(X,Y)$.

Let $S$ be the tangent linear map characterized by $h(SX,Y)=K(X,Y)$. Differentiating $g(n,n)=\varepsilon$ and $g(n,Y)=0$ gives the [Gauss formula](../../../../../gauss-formula.md)

$$
\nabla_Xn=SX,\qquad \nabla_XY=D_XY-\varepsilon K(X,Y)n.
$$

Fix the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,\qquad R_{abcd}=g(e_a,R(e_c,e_d)e_b).
$$

Applying the [Gauss formula](../../../../../gauss-formula.md) twice gives

$$
P\nabla_X\nabla_YZ=D_XD_YZ-\varepsilon K(Y,Z)SX.
$$

Subtracting the expression with $X,Y$ interchanged, and then subtracting the bracket derivative, proves

$$
\mathcal R(X,Y)Z=PR(X,Y)Z+\varepsilon\bigl(K(Y,Z)SX-K(X,Z)SY\bigr).
$$

Thus the [Gauss–Codazzi equations for a non-null hypersurface](../../../../../gauss-codazzi-equations-for-a-non-null-hypersurface.md) give the intrinsic [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) as

$$
\boxed{\mathcal R_{abcd}=P^e{}_aP^f{}_bP^g{}_cP^h{}_dR_{efgh}+\varepsilon(K_{ac}K_{bd}-K_{ad}K_{bc}).}
$$

All free indices here are tangent to the [hypersurface](../../../../../hypersurface.md). The normal component of the same calculation is

$$
g(n,\nabla_X\nabla_YZ)=-K(X,D_YZ)-X\bigl(K(Y,Z)\bigr).
$$

After antisymmetrizing and using $D_XY-D_YX=[X,Y]$, this yields the curved-ambient [Codazzi equation](../../../../../codazzi-equation.md)

$$
\boxed{g(n,R(X,Y)Z)=-(D_XK)(Y,Z)+(D_YK)(X,Z).}
$$

The [extrinsic curvature](../../../../../extrinsic-curvature.md) measures how tangent planes turn in the ambient manifold; the [Gauss equation](../../../../../gauss-equation.md) says that this turning contributes to intrinsic curvature even when the ambient [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) is zero.

For the quadric in [Minkowski spacetime](../../../../../minkowski-spacetime.md), write its position vector as $X^a$. On the [hypersurface](../../../../../hypersurface.md), $g(X,X)=1$ and differentiating this identity in a tangent direction gives $g(X,Y)=0$. Hence $n=X$ is a [unit normal](../../../../../unit-normal.md) and a [spacelike vector](../../../../../spacelike-vector.md), $\varepsilon=1$, and $\nabla_Yn=Y$ in flat [Cartesian coordinates](../../../../../cartesian-coordinate-system.md). Therefore $K=h$. The ambient [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) vanishes, so

$$
\boxed{\mathcal R_{abcd}=h_{ac}h_{bd}-h_{ad}h_{bc},\qquad \mathcal R_{ab}=3h_{ab},\qquad \mathcal R=12>0.}
$$

This is unit-radius [de Sitter spacetime](../../../../../de-sitter-spacetime.md). Reversing the normal changes $K$ to $-K$ but does not change this curvature. An opposite overall convention for the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) would reverse both curvature signs below.

To retain a four-dimensional [Lorentzian metric](../../../../../lorentzian-metric.md) while reversing the curvature, take a flat ambient metric with two negative directions and the quadric

$$
-dt^2-dw^2+dx^2+dy^2+dz^2,\qquad -t^2-w^2+x^2+y^2+z^2=-1.
$$

Now the position vector is a [unit normal](../../../../../unit-normal.md) with negative squared norm, so $\varepsilon=-1$ while $K=h$ remains true. The [Gauss equation](../../../../../gauss-equation.md) gives

$$
\boxed{\mathcal R_{abcd}=-(h_{ac}h_{bd}-h_{ad}h_{bc}),\qquad \mathcal R=-12.}
$$

This is unit-radius [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md). If a positive-definite [induced metric](../../../../../induced-metric.md) is acceptable, an even simpler alternative is to keep the original one-time ambient [Minkowski metric](../../../../../minkowski-metric.md) and change the quadric level to $g(X,X)=-1$. Each sheet then gives four-dimensional [hyperbolic space](../../../../../hyperbolic-space.md) with the same negative curvature, but its induced signature differs from that of [de Sitter spacetime](../../../../../de-sitter-spacetime.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
