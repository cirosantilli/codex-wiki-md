<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The [nullclines](../../../../../nullcline.md) are $y=\mu x$ and $y=x^2/[\nu(1+x^2)]$. At a nonzero [fixed point](../../../../../fixed-point.md), cancellation of $x$ yields $\mu\nu=x/(1+x^2)$. The latter function attains its maximum $1/2$ at $x=1$. Hence

$$
\boxed{\mu_c=\frac1{2\nu},\qquad
O=(0,0),\quad P_\pm=(x_\pm,\mu x_\pm),\quad
x_\pm=\frac{1\pm\sqrt{1-4\mu^2\nu^2}}{2\mu\nu}.}
$$

For $0<\mu<\mu_c$, $x_-<1<x_+$ and $x_-x_+=1$.

The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}-\mu&1\\2x/(1+x^2)^2&-\nu\end{pmatrix}.
$$

At $O$ the distinct [eigenvalues](../../../../../eigenvalue.md) are $-\mu,-\nu$, so the origin is a [stable node](../../../../../stable-node.md). At a nonzero [fixed point](../../../../../fixed-point.md) its [trace](../../../../../matrix-trace.md) is $-(\mu+\nu)<0$ and

$$
\det J=\mu\nu\frac{x^2-1}{1+x^2}.
$$

The discriminant is $(\mu-\nu)^2+8x/(1+x^2)^2>0$. Thus **$P_-$ is a saddle and $P_+$ is a [stable node](../../../../../stable-node.md)**, never a focus.

<a id="7d/image-nullclines-and-bistable-phase-portrait-with-saddle-manifolds"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1-bistable-flow.png)

**[Figure 1](#7d/image-nullclines-and-bistable-phase-portrait-with-saddle-manifolds). Nullclines and bistable phase portrait with saddle manifolds**.

Above the straight [nullcline](../../../../../nullcline.md) $\dot x>0$; below it $\dot x<0$. Below the curved [nullcline](../../../../../nullcline.md) $\dot y>0$; above it $\dot y<0$. At the saddle, an [eigenvector](../../../../../eigenvector.md) can be chosen as $(1,\mu+\lambda)$: the stable [eigenvalue](../../../../../eigenvalue.md) gives negative slope, and the unstable [eigenvalue](../../../../../eigenvalue.md) gives positive slope. The [stable manifold](../../../../../stable-manifold.md) is the basin boundary. The two branches of the [unstable manifold](../../../../../unstable-manifold.md) lead respectively to the origin and the positive [stable node](../../../../../stable-node.md), as illustrated for representative parameters.

The nonnegative quadrant is forward invariant. Since $\dot y\leq1-\nu y$, $y$ stays bounded, and then $\dot x=-\mu x+y$ also bounds $x$. Moreover the divergence is the negative constant $-(\mu+\nu)$, excluding periodic or homoclinic loops by the [Bendixson-Dulac criterion](../../../../../bendixson-dulac-theorem.md). The [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) then leaves convergence to a [fixed point](../../../../../fixed-point.md). Initial data on the saddle's [stable manifold](../../../../../stable-manifold.md) approach the saddle; data in the two open basins approach **extinction at $O$ or persistence at $P_+$**, respectively.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
