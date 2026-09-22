<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the nonnegative convention for the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md). For a smooth function $f$ on a [Riemannian manifold](../../../../../riemannian-manifold.md) $(M,g)$, three intrinsic definitions are

$$
\boxed{\Delta f=d^*df=-\operatorname{div}(\operatorname{grad}f)=-\operatorname{tr}_g(\nabla df)}.
$$

Here $d$ is the [exterior derivative](../../../../../exterior-derivative.md), $d^*$ its formal $L^2$ adjoint for the Riemannian volume density, $\operatorname{grad}f$ the [Riemannian gradient](../../../../../riemannian-gradient.md), and $\nabla$ the [Levi-Civita connection](../../../../../levi-civita-connection.md). The bilinear form $\nabla df$ is the [Riemannian Hessian](../../../../../riemannian-hessian.md). The equally common nonpositive convention negates all three definitions simultaneously.

In local coordinates let $g^{ij}$ be the inverse metric [matrix](../../../../../matrix.md) and $\rho=\sqrt{\det(g_{ij})}$. By the defining relation $g(\operatorname{grad}f,V)=df(V)$,

$$
(\operatorname{grad}f)^i=g^{ij}\partial_jf.
$$

The [divergence of a Riemannian vector field](../../../../../divergence-of-a-riemannian-vector-field.md) can be defined by $\mathcal L_V(dV_g)=(\operatorname{div}V)dV_g$. Differentiating the coordinate volume density gives $\operatorname{div}V=\rho^{-1}\partial_i(\rho V^i)$. Thus the second definition becomes

$$
-\operatorname{div}(\operatorname{grad}f)
=-\frac1\rho\partial_i(\rho g^{ij}\partial_jf).
$$

For compactly supported smooth $h$, coordinate [integration by parts](../../../../../integration-by-parts.md) shows

$$
\int_M h\left[-\rho^{-1}\partial_i(\rho g^{ij}\partial_jf)\right]dV_g
=\int_M g^{ij}(\partial_i h)(\partial_jf)\,dV_g
=\langle dh,df\rangle_{L^2}
=\langle h,d^*df\rangle_{L^2}.
$$

Since this holds for every such $h$, the first and second definitions agree. This argument also works on a nonorientable [Riemannian manifold](../../../../../riemannian-manifold.md), using its volume density; no global [orientation](../../../../../orientation-of-a-simplex.md) is needed.

For the third definition,

$$
(\nabla df)_{ij}=\partial_i\partial_jf-\Gamma^k_{ij}\partial_kf.
$$

The [Christoffel symbols](../../../../../christoffel-symbol.md) satisfy $\Gamma^i_{ik}=\partial_k\log\rho$. This follows by tracing their formula and using $\partial_k\log\det g=\operatorname{tr}(g^{-1}\partial_kg)$. [Metric compatibility](../../../../../metric-compatibility.md) gives

$$
\partial_i g^{ij}+\Gamma^i_{ik}g^{kj}=-\Gamma^j_{ik}g^{ik}.
$$

Substitute both identities into the coordinate divergence expression to obtain

$$
-\rho^{-1}\partial_i(\rho g^{ij}\partial_jf)
=-g^{ij}\partial_i\partial_jf+g^{ij}\Gamma^k_{ij}\partial_kf
=-\operatorname{tr}_g(\nabla df).
$$

This proves all three definitions equivalent. In [geodesic normal coordinates](../../../../../geodesic-normal-coordinates.md) at a point $p$, the common value is $-\sum_i\partial_i^2f(p)$. Finally, on a closed manifold,

$$
\int_M f\Delta f\,dV_g=\int_M|df|_g^2\,dV_g\geq0,
$$

confirming the chosen [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) sign convention.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
