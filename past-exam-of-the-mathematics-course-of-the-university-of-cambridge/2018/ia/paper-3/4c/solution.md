<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

For a scalar $\phi$, the displayed basis identities give

$$
\nabla\phi=\mathbf e_r\phi_r+\mathbf e_\theta\frac1r\phi_\theta.
$$

Taking the [divergence](../../../../../divergence.md) and differentiating the basis vectors yields the [Laplacian in polar coordinates](../../../../../laplacian-in-polar-coordinates.md)

$$
\boxed{\nabla^2\phi=\frac1r\frac{\partial}{\partial r}\left(r\frac{\partial\phi}{\partial r}\right)+\frac1{r^2}\frac{\partial^2\phi}{\partial\theta^2}}.
$$

Consequently,

$$
\nabla^2\!\left(\alpha r^\beta\cos(\gamma\theta)\right)
=\boxed{\alpha(\beta^2-\gamma^2)r^{\beta-2}\cos(\gamma\theta)}.
$$

The regular harmonic mode with angular dependence $\cos2\theta$ is $Cr^2\cos2\theta$. Its radial derivative at $r=a$ is $2Ca\cos2\theta$, so $C=1/(2a)$. A constant is invisible to the [Neumann boundary condition](../../../../../neumann-boundary-condition.md), giving

$$
\boxed{\phi(r,\theta)=\frac{r^2}{2a}\cos2\theta+C_0.}
$$

If two solutions existed, their difference $u$ would satisfy $\nabla^2u=0$ and $\partial_nu=0$. [Green's first identity](../../../../../green-s-first-identity.md) gives $\int_D|\nabla u|^2=\int_{\partial D}u\,\partial_nu-\int_Du\nabla^2u=0$, so $\nabla u=0$ and $u$ is constant. Thus these are all the solutions.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
