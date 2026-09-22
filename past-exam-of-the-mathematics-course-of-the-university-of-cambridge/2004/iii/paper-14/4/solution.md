<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [geodesic](../../../../../geodesic.md) is an affinely parametrized [curve](../../../../../curve.md) satisfying $\nabla_{\dot\gamma}\dot\gamma=0$ for the [Levi-Civita connection](../../../../../levi-civita-connection.md) of the [Riemannian metric](../../../../../riemannian-metric.md). In coordinates, write $\nabla_{\partial_i}\partial_j=\Gamma^k_{ij}\partial_k$. For a [vector field](../../../../../vector-field.md) $V(t)=V^k(t)\partial_k$ along the [curve](../../../../../curve.md),

$$
\left(\nabla_{\dot\gamma}V\right)^k=\frac{dV^k}{dt}+\Gamma^k_{ij}(\gamma(t))\dot\gamma^iV^j.
$$

Putting $V=\dot\gamma$ gives the [geodesic equation](../../../../../geodesic-equation.md)

$$
\boxed{\ddot\gamma^k+\Gamma^k_{ij}(\gamma)\dot\gamma^i\dot\gamma^j=0.}
$$

This is a smooth second-order ordinary differential system, so the [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) gives local existence and uniqueness for prescribed position and velocity.

To prove [local extension of geodesic velocity](../../../../../local-extension-of-geodesic-velocity.md), first suppose $\dot\gamma(0)=0$. The constant [curve](../../../../../curve.md) through $\gamma(0)$ solves this initial value problem, so uniqueness makes $\gamma$ constant locally. The zero [vector field](../../../../../vector-field.md) is the desired extension.

Otherwise choose a chart about $\gamma(0)$ in which the first component of the coordinate velocity is nonzero. Write the coordinate [curve](../../../../../curve.md) as $c(t)\in\mathbb R^n$ and define

$$
\Psi(t,z_2,\ldots,z_n)=c(t)+\sum_{j=2}^nz_je_j.
$$

At $(0,0)$ its derivative has columns $c'(0),e_2,\ldots,e_n$ and is invertible, because the first component of $c'(0)$ is nonzero. The [inverse function theorem](../../../../../inverse-function-theorem.md) therefore supplies coordinates $(t,z_2,\ldots,z_n)$ on an open neighbourhood after shrinking the parameter interval to $|t|<\delta$. Along the [curve](../../../../../curve.md) these coordinates are $(t,0,\ldots,0)$. The smooth coordinate field $\partial/\partial t$, pushed back through $\Psi$ and the original chart, agrees with $\dot\gamma(t)$. This proves the extension without assuming that a long [geodesic](../../../../../geodesic.md) has no self-intersections.

By [metric compatibility](../../../../../metric-compatibility.md), differentiation along the [curve](../../../../../curve.md) gives

$$
\frac d{dt}g(\dot\gamma,\dot\gamma)
=2g(\nabla_{\dot\gamma}\dot\gamma,\dot\gamma)=0.
$$

The local extension above permits the ordinary vector-field version of the metric identity to be used along the arc, or the same identity follows directly from the coordinate derivative. Hence **an affinely parametrized [geodesic](../../../../../geodesic.md) has constant speed**, including the zero-speed case.

Now let $S^n$ be the unit [sphere](../../../../../sphere.md) in $\mathbb R^{n+1}$. Its induced Levi-Civita derivative is the tangential projection of the ordinary ambient derivative: projection preserves the metric identity, and the commuting ambient coordinate derivatives give zero torsion. By uniqueness of the [Levi-Civita connection](../../../../../levi-civita-connection.md), proved in Question 5, this is the induced connection.

Thus a [curve](../../../../../curve.md) on the [sphere](../../../../../sphere.md) is a [geodesic](../../../../../geodesic.md) exactly when its ambient acceleration has no tangential component. The normal space is spanned by $\gamma$, so $\gamma''=a(t)\gamma$. Differentiating $\gamma\cdot\gamma=1$ twice gives $\gamma\cdot\gamma'=0$ and

$$
a(t)=\gamma\cdot\gamma''=-|\gamma'|^2=-c^2,
$$

where $c\geq0$ is the constant speed. Therefore $\gamma''+c^2\gamma=0$. With initial data $\gamma(0)=p$ and $\gamma'(0)=v$, all solutions are

$$
\boxed{\gamma(t)=p\cos(ct)+\frac vc\sin(ct),\quad
|p|=1,\quad p\cdot v=0,\quad |v|=c>0,}
$$

and, when $v=0$, $\boxed{\gamma(t)=p}$. The [orthogonality](../../../../../orthogonal-vectors.md) and length conditions show directly that the displayed [curve](../../../../../curve.md) remains on the [sphere](../../../../../sphere.md), and its acceleration is $-c^2\gamma$, so it is indeed a [geodesic](../../../../../geodesic.md). The nonconstant [geodesics](../../../../../geodesic.md) are the [great circles](../../../../../great-circle.md) traversed at any constant speed; arbitrary parameter intervals give their restrictions, and shifting the initial parameter simply shifts the formula. There are no other [geodesics](../../../../../geodesic.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
