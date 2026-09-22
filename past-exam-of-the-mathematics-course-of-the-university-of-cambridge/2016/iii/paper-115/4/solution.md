<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $i:M\hookrightarrow N$ be the inclusion. The [restriction of a connection to an embedded submanifold](../../../../../restriction-of-a-connection-to-an-embedded-submanifold.md) is the [pullback connection](../../../../../pullback-connection.md) on $i^*TN=TN|_M$. Concretely, for a tangent [vector field](../../../../../vector-field.md) $X$ on $M$ and a local section $S$ of $TN|_M$, extend $S$ smoothly off $M$ and define $\nabla_XS$ by differentiating the extension in direction $di(X)$. Two extensions differ by a field whose coefficients vanish on $M$. Their derivatives along every tangent curve in $M$ vanish too, and the connection's coefficient terms are multiplied by the zero field. The answer is therefore independent of the extension. Dependence only on the value of the first argument follows from the connection's linearity over [smooth functions](../../../../../smooth-function.md).

The induced [Riemannian metric](../../../../../riemannian-metric.md) is positive definite, so the fibrewise [orthogonal projection](../../../../../orthogonal-projection.md) $\pi:TN|_M\to TM$ is smooth. For tangent fields define the [projected ambient connection](../../../../../projected-ambient-connection.md) $D_XY=\pi(\nabla_XY)$. It is real-linear and satisfies

$$
D_{fX}Y=fD_XY,\qquad
D_X(fY)=X(f)Y+fD_XY,
$$

because $\pi Y=Y$. Thus $D$ is a [Koszul connection](../../../../../affine-connection.md) on $M$.

The [Levi-Civita connection](../../../../../levi-civita-connection.md) is characterized by the [torsion-free connection](../../../../../torsion-free-connection.md) and [metric connection](../../../../../metric-connection.md) conditions

$$
\nabla_XY-\nabla_YX=[X,Y],\qquad
X\langle Y,Z\rangle=\langle\nabla_XY,Z\rangle+\langle Y,\nabla_XZ\rangle.
$$

These determine it uniquely. For the ambient [Levi-Civita connection](../../../../../levi-civita-connection.md), the [Gauss formula](../../../../../gauss-formula.md) is $\nabla_XY=D_XY+II(X,Y)$, with

$$
II(X,Y)=(I-\pi)\nabla_XY.
$$

Linearity over [smooth functions](../../../../../smooth-function.md) in $X$ is immediate. In $Y$, the additional $X(f)Y$ term is tangent and is killed by $I-\pi$. Thus [tensoriality](../../../../../tensoriality.md) makes $II$ a [bilinear map](../../../../../bilinear-map.md) $TM\times_M TM\to\nu M$ into the [normal bundle](../../../../../normal-bundle.md). Its antisymmetric part is

$$
II(X,Y)-II(Y,X)=(I-\pi)[X,Y]=0,
$$

because the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) tangent to $M$ is tangent. This proves the [symmetry of the second fundamental form](../../../../../symmetry-of-the-second-fundamental-form.md) in an arbitrary Riemannian ambient manifold.

Write the curvature operators as $R^N(v,w)y=\nabla_v\nabla_wy-\nabla_w\nabla_vy-\nabla_{[v,w]}y$ and $R^M$ with $D$ in place of $\nabla$. To match the four-slot notation in the requested identity, use

$$
R(x,y,v,w)=\langle R^N(v,w)y,x\rangle,\qquad
\overline R(x,y,v,w)=\langle R^M(v,w)y,x\rangle.
$$

This convention is stated because permuting the slots can change the displayed signs.

If $\eta$ is a normal field and $x$ is tangent, metric compatibility applied to $\langle\eta,x\rangle=0$ gives the [tangential derivative of a normal field](../../../../../tangential-derivative-of-a-normal-field.md) identity

$$
\langle\nabla_v\eta,x\rangle=-\langle\eta,II(v,x)\rangle.
$$

Using the [Gauss formula](../../../../../gauss-formula.md) and this identity,

$$
\langle\nabla_v\nabla_wy,x\rangle
=\langle D_vD_wy,x\rangle-\langle II(w,y),II(v,x)\rangle.
$$

Here the normal part of $\nabla_v(D_wy)$ pairs to zero with $x$. Interchange $v,w$ and subtract; the bracket term obeys $\langle\nabla_{[v,w]}y,x\rangle=\langle D_{[v,w]}y,x\rangle$. It follows that

$$
R(x,y,v,w)=\overline R(x,y,v,w)
-\langle II(w,y),II(v,x)\rangle+\langle II(v,y),II(w,x)\rangle.
$$

Rearranging proves the [Gauss equation in a curved ambient manifold](../../../../../gauss-equation-in-a-curved-ambient-manifold.md):

$$
\boxed{\overline R(x,y,v,w)=R(x,y,v,w)
+\langle II(v,x),II(w,y)\rangle-\langle II(v,y),II(w,x)\rangle}.
$$

All expressions are tensorial, so choosing local extensions of the four tangent vectors proves the pointwise identity at $P$. With flat Euclidean ambient space, $R^N=0$ and this reduces to the usual [Gauss equation](../../../../../gauss-equation.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
