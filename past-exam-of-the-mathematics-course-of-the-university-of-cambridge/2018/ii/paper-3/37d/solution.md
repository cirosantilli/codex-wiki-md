<h1 id="37d/solution">Solution</h1>

↑ **Parent:** [37D](../37d.md)

Write the [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) as $F^{\mu\nu}=\partial^\mu A^\nu-\partial^\nu A^\mu$. Substitution into the [Covariant Maxwell equation with the minus-plus-plus-plus metric](../../../../../covariant-maxwell-equation-with-the-minus-plus-plus-plus-metric.md) gives

$$
\partial_\mu\partial^\mu A^\nu-\partial^\nu(\partial_\mu A^\mu)=-\mu_0J^\nu.
$$

Choose the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\partial_\mu A^\mu=0$. Since $\partial_\mu\partial^\mu=\nabla^2-c^{-2}\partial_t^2$, the [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md) obeys

$$
\boxed{\left(\nabla^2-\frac1{c^2}\frac{\partial^2}{\partial t^2}\right)A^\mu=-\mu_0J^\mu.}
$$

Convolution with the outgoing [retarded Green function](../../../../../retarded-green-function.md) gives the [retarded electromagnetic potential](../../../../../retarded-potential.md)

$$
\boxed{A^\mu(t,\mathbf x)=\frac{\mu_0}{4\pi}
\int\frac{J^\mu(t_{\rm ret},\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x',
\qquad
t_{\rm ret}=t-\frac{|\mathbf x-\mathbf x'|}{c}.}
$$

For the point particle, $\tau_*(x)$ is its unique retarded [proper time](../../../../../proper-time.md), characterized by

$$
\boxed{R^\mu(\tau_*)R_\mu(\tau_*)=0,\qquad R^0(\tau_*)>0.}
$$

Thus $y(\tau_*)$ is where the particle's [worldline](../../../../../world-line.md) intersects the [past light cone](../../../../../past-light-cone.md) of the observation event $x$; the displayed expression is the covariant form of the [Liénard–Wiechert potentials](../../../../../lienard-wiechert-potential.md).

On the $z$-axis put $D=\sqrt{R^2+z^2}$. The [retarded time](../../../../../retarded-time.md) is $t_*=t-D/c$. For the circular orbit, the spatial velocity at that time is

$$
\mathbf v(t_*)=R\omega\bigl(-\sin(\omega t_*),\cos(\omega t_*),0\bigr).
$$

Because the displacement from the retarded source point to the observation point is orthogonal to this velocity, $|R^\nu\dot y_\nu|=\gamma cD$, while $\dot y^\mu=\gamma(c,\mathbf v)$. The factors of $\gamma$ cancel, leaving

$$
\boxed{A^\mu(t,0,0,z)=\frac{\mu_0q}{4\pi D}
\left(c,-R\omega\sin\!\left[\omega\left(t-\frac Dc\right)\right],
R\omega\cos\!\left[\omega\left(t-\frac Dc\right)\right],0\right).}
$$

## ↑ Ancestors (10)

1. [37D](../37d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
