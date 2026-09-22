<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) $\sigma=-pI+2\mu e$, where $e=(\nabla u+\nabla u^T)/2$. The [Stokes equations](../../../../../stokes-equation.md) for a point [force](../../../../../force.md) on the fluid are $\nabla\cdot u=0$ and $\nabla\cdot\sigma+F\delta(x)=0$. Put $r=|x|$. Away from the origin, a harmonic vector potential proportional to $F/r$ in the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md) gives the rotationally covariant decaying solution. Specifically, take $\Phi=-F/(8\pi\mu r)$ and $\chi=0$. Differentiation yields

$$
\boxed{u_i=J_{ij}F_j,\quad J_{ij}(x)=\frac1{8\pi\mu}\left(\frac{\delta_{ij}}r+\frac{x_ix_j}{r^3}\right),\qquad p=\frac{F\cdot x}{4\pi r^3}.}
$$

This satisfies the homogeneous [Stokes equations](../../../../../stokes-equation.md) for $r>0$. Its [stress](../../../../../stress.md) is

$$
\boxed{\sigma_{ij}=K_{kij}F_k,\qquad K_{kij}(x)=-\frac{3x_kx_ix_j}{4\pi r^5}.}
$$

To verify the point-force normalization, on a sphere $r=\varepsilon$ the [traction](../../../../../traction.md) is $\sigma n=-3(F\cdot n)n/(4\pi\varepsilon^2)$. Since $\int_{S^2}n_in_j\,d\Omega=4\pi\delta_{ij}/3$, its surface integral is $-F$. Thus integrating momentum balance over the small ball gives exactly the applied [force](../../../../../force.md) $F$, fixing the normalization of the [Stokeslet](../../../../../stokeslet.md). Its radial [velocity](../../../../../velocity.md) is $(F\cdot n)/(4\pi\mu r)$, so

$$
\boxed{\int_{|x|=r}u\cdot n\,dS=\frac r{4\pi\mu}F\cdot\int_{S^2}n\,d\Omega=0.}
$$

There is no net volume or mass source at the singularity. The kernels have the parity $J(-x)=J(x)$ and $K(-x)=-K(x)$.

For two Stokes flows with the same [viscosity](../../../../../dynamic-viscosity.md) and body [forces](../../../../../force.md) $f^{(1)},f^{(2)}$, the [Lorentz reciprocal theorem](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) including body [forces](../../../../../force.md) is

$$
\boxed{\int_{\partial V}\big(u^{(1)}\cdot\sigma^{(2)}n-u^{(2)}\cdot\sigma^{(1)}n\big)dS
=\int_V\big(u^{(2)}\cdot f^{(1)}-u^{(1)}\cdot f^{(2)}\big)dV.}
$$

Indeed, apply the [divergence theorem](../../../../../divergence-theorem.md) to $u_i^{(1)}\sigma_{ij}^{(2)}-u_i^{(2)}\sigma_{ij}^{(1)}$. The cross-gradient terms cancel: [incompressibility](../../../../../incompressible-flow.md) removes each [pressure](../../../../../pressure.md) contraction and the remaining terms are both $2\mu e^{(1)}:e^{(2)}$. The two [stress](../../../../../stress.md) divergences give the body-force terms shown.

Choose flow 1 to be the desired body-force-free field and flow 2 to be a [Stokeslet](../../../../../stokeslet.md) with arbitrary [force](../../../../../force.md) vector $q$ at $y$. For $y\in V$, the body-force term is $-q\cdot u(y)$. Rearrange the reciprocal identity and use the parity of $J,K$; equality for every $q$ gives

$$
\boxed{u_i(y)=\int_{\partial V}J_{ij}(y-x)\sigma_{jk}(x)n_k\,dS
+\int_{\partial V}u_j(x)K_{ijk}(y-x)n_k\,dS.}
$$

For $y$ outside the volume there is no point [force](../../../../../force.md) in $V$, so the same two integrals sum to zero. To obtain the smooth boundary value, exclude a small hemisphere about $y$, use continuity of $u$ to replace it by $u(y)$ on that hemisphere, and take the radius to zero. A full small sphere contributes $u(y)$; a hemisphere contributes half of it. Equivalently, the local solid-angle factor is $2\pi/(4\pi)$. The result is the [boundary integral representation of Stokes flow](../../../../../boundary-integral-representation-of-stokes-flow.md) with right side $\tfrac12u(y)$ on a smooth boundary, and with the double layer interpreted by its boundary [principal value](../../../../../cauchy-principal-value.md). A nonsmooth corner would have a different solid-angle coefficient.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
