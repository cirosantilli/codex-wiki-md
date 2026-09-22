<h1 id="17c/solution">Solution</h1>

↑ **Parent:** [17C](../17c.md)

Remove a small disc about $x$ and apply [Green second identity](../../../../../green-second-identity.md) to $u(x_0)$ and $G_0(x;x_0)$. Since $\nabla_{x_0}^2G_0=\delta(x_0-x)$ and $\nabla^2u=-\rho$, the shrinking inner boundary contributes $u(x)$ and gives

$$
u(x)=-\int_\Omega G_0(x;x_0)\rho(x_0)\,dx_0dy_0
+\oint_{\partial\Omega}\left(u\,\partial_nG_0-G_0\partial_nu\right)ds.
$$

For the unit disc, the [method of images](../../../../../method-of-images.md) gives the [Dirichlet Green function](../../../../../dirichlet-green-function.md)

$$
G_D(x;x_0)=\frac1{2\pi}\log\frac{|x-x_0|}{|x_0|\,|x-x_0/|x_0|^2|},
$$

which vanishes on the boundary by the hinted identity. The boundary representation with $u(1,\theta_0)=\delta(\theta_0-\alpha)$ evaluates the normal derivative of $G_D$ at $\theta_0=\alpha$, giving the [Poisson kernel](../../../../../poisson-kernel-for-the-upper-half-plane.md)

$$
\boxed{u(r,\theta)=\frac1{2\pi}\frac{1-r^2}{1+r^2-2r\cos(\theta-\alpha)}.}
$$

## ↑ Ancestors (10)

1. [17C](../17c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
