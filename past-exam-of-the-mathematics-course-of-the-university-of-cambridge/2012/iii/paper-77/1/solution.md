<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the layer depth $d$, the thermal diffusion time $d^2/\kappa$, velocity $\kappa/d$, and the imposed temperature difference $\Delta T$ as scales. Let $\theta$ be the temperature departure from the conductive profile, $\mathbf u$ the velocity, $w=\mathbf u\cdot\hat{\mathbf z}$, and let pressure absorb hydrostatic terms. The dimensionless [Boussinesq equations](../../../../../boussinesq-equations.md) for [Rayleigh-Bénard convection](../../../../../rayleigh-benard-convection.md) are

$$
\nabla\cdot\mathbf u=0,\qquad \frac1\sigma(\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u)=-\nabla p+R\theta\hat{\mathbf z}+\nabla^2\mathbf u,\qquad \partial_t\theta+\mathbf u\cdot\nabla\theta=w+\nabla^2\theta.
$$

The [Prandtl number](../../../../../prandtl-number.md) and [Rayleigh number](../../../../../rayleigh-number.md) are $\sigma=\nu/\kappa$ and $R=g\alpha_T\Delta T d^3/(\nu\kappa)$, with [kinematic viscosity](../../../../../kinematic-viscosity.md) $\nu$, [thermal diffusivity](../../../../../thermal-diffusivity.md) $\kappa$ and [coefficient of thermal expansion](../../../../../coefficient-of-thermal-expansion.md) $\alpha_T$. At $z=0,1$, the [stress-free boundary condition](../../../../../stress-free-boundary-condition.md) and [perfectly conducting thermal boundary condition](../../../../../perfectly-conducting-thermal-boundary-condition.md) give $w=0$, $\partial_z u_x=\partial_z u_y=0$, and $\theta=0$.

For the fundamental vertical [normal mode](../../../../../normal-mode.md), take $w=W\sin(\pi z)e^{i\mathbf k\cdot\mathbf x+\lambda t}$ and $\theta=\vartheta\sin(\pi z)e^{i\mathbf k\cdot\mathbf x+\lambda t}$. Here $k=|\mathbf k|>0$ is the horizontal [wavenumber](../../../../../wavenumber.md). With $s=k^2+\pi^2$, projection onto [incompressible flow](../../../../../incompressible-flow.md) eliminates pressure and gives

$$
(\lambda/\sigma+s)sW=Rk^2\vartheta,\qquad (\lambda+s)\vartheta=W.
$$

Thus the [stress-free convection growth-rate polynomial](../../../../../stress-free-convection-growth-rate-polynomial.md) is $(\lambda+\sigma s)(\lambda+s)=\sigma Rk^2/s$.

For the infinite-[Prandtl number](../../../../../prandtl-number.md) limit, the finite thermal growth rate is

$$
\boxed{\lambda_\infty(k)=\frac{Rk^2}{(k^2+\pi^2)^2}-(k^2+\pi^2).}
$$

The other, viscously damped root tends to $-\sigma s$. For $\sigma=1$, both roots are explicit:

$$
\boxed{\lambda_\pm(k)=-s\pm\sqrt{\frac{Rk^2}{s}}.}
$$

The plus root determines instability. A higher vertical harmonic replaces $\pi^2$ by $n^2\pi^2$; the fundamental is the most favorable one.

For the large-$R$ maximum in the infinite-[Prandtl number](../../../../../prandtl-number.md) limit, put $x=k^2$ and $p=\pi^2$. Differentiating gives $d\lambda_\infty/dx=R(p-x)/(p+x)^3-1$. The unique maximum for sufficiently large $R$ therefore satisfies $R(p-x)=(p+x)^3$, whence

$$
\boxed{k_{\rm max}^2=p-\frac{8p^3}{R}+O(R^{-2})\simeq\pi^2,\qquad \lambda_{\rm max}=\frac{R}{4\pi^2}-2\pi^2+O(R^{-1})\simeq\frac{R}{4\pi^2}.}
$$

This is [fastest growth in infinite-Prandtl convection](../../../../../fastest-growth-in-infinite-prandtl-convection.md). The large-$R$ expansion is taken after the infinite-[Prandtl number](../../../../../prandtl-number.md) limit; at finite $\sigma$, neglecting inertia additionally requires $|\lambda|\ll\sigma s$. It selects the fastest growing mode far above onset, rather than the neutral-curve minimum $k^2=\pi^2/2$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [Section I](../section-i.md)
3. [Paper 77](../../paper-77-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
