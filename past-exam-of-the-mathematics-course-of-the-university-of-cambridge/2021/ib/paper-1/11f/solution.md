<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

For an oriented [smooth surface](../../../../../smooth-surface.md) $S$, the [Gauss map](../../../../../gauss-map.md) sends $p$ to the chosen unit [normal vector](../../../../../normal-vector.md) $N(p)\in S^2$. Since $|N|^2=1$, differentiation shows that $DN_p(X)$ is perpendicular to $N(p)$ and hence lies in $T_pS$.

In a local parametrization $\phi(u,v)$ with $n=N\circ\phi$, differentiating

$$
n\mathbin{\cdot}\phi_u=n\mathbin{\cdot}\phi_v=0
$$

gives

$$
n_u\mathbin{\cdot}\phi_v=-n\mathbin{\cdot}\phi_{uv}
=n_v\mathbin{\cdot}\phi_u.
$$

Thus the bilinear form $(X,Y)\mapsto DN_p(X)\mathbin{\cdot}Y$ is symmetric, so $DN_p$ is [self-adjoint](../../../../../self-adjoint-operator.md). The [Gaussian curvature](../../../../../gaussian-curvature.md) is

$$
\kappa=\det(DN_p).
$$

Writing the coefficients of the [first fundamental form](../../../../../first-fundamental-form.md) as

$$
E=\phi_u^2,\qquad F=\phi_u\mathbin{\cdot}\phi_v,\qquad G=\phi_v^2
$$

and those of the [second fundamental form](../../../../../second-fundamental-form-split.md) as

$$
e=n\mathbin{\cdot}\phi_{uu},\qquad
f=n\mathbin{\cdot}\phi_{uv},\qquad
g=n\mathbin{\cdot}\phi_{vv},
$$

one obtains

$$
\boxed{\kappa=\frac{eg-f^2}{EG-F^2}}.
$$

At an [umbilic point](../../../../../umbilical-point.md), the self-adjoint map $DN_p$ has a repeated eigenvalue, so it is a scalar map. If every point is umbilic, there is a function $\lambda$ with

$$
n_u=\lambda\phi_u,\qquad n_v=\lambda\phi_v.
$$

Equality of mixed partial derivatives gives

$$
\lambda_v\phi_u=\lambda_u\phi_v.
$$

The two tangent vectors are linearly independent, hence $\lambda_u=\lambda_v=0$. Since $\mathbb R^2$ is connected, $\lambda$ is constant.

If $\lambda=0$, then $n$ is constant and

$$
\partial_u(n\mathbin{\cdot}\phi)
=\partial_v(n\mathbin{\cdot}\phi)=0,
$$

so $S$ lies in a plane. If $\lambda\ne0$, then

$$
\partial_u(n-\lambda\phi)
=\partial_v(n-\lambda\phi)=0.
$$

Thus $n-\lambda\phi=c$ is constant, and

$$
\left|\phi+\frac c\lambda\right|
=\frac{|n|}{|\lambda|}
=\frac1{|\lambda|}.
$$

**Therefore $S$ lies in a sphere of radius $1/|\lambda|$. This proves that the surface is part of a plane or part of a sphere.**

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
