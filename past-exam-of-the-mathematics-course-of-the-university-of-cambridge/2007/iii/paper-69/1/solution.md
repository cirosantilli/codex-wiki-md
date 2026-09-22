<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [integral of motion](../../../../../integral-of-motion.md) is a function of [phase space](../../../../../phase-space.md) that is constant along a trajectory. Put $\phi=-\psi+\mathrm{constant}$, so the stellar acceleration is $\dot{\mathbf v}=\nabla\psi$. In a time-independent spherical [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md),

$$
\frac{dE}{dt}=\nabla\psi\cdot\mathbf v-\mathbf v\cdot\dot{\mathbf v}=0,\qquad
\frac{d\mathbf L}{dt}=\mathbf v\times\mathbf v+\mathbf r\times\nabla\psi=0.
$$

The second equality uses the radial direction of $\nabla\psi$. Thus both the binding energy and the full [specific angular momentum](../../../../../specific-angular-momentum.md) vector are [integrals of motion](../../../../../integral-of-motion.md).

The [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) is

$$
\partial_t f+\mathbf v\cdot\nabla_{\mathbf x}f+\nabla\psi\cdot\nabla_{\mathbf v}f=0.
$$

For a stationary [galactic distribution function](../../../../../galactic-distribution-function.md), this says $df/dt=0$ on every characteristic, so $f$ is constant on each stellar orbit. Locally choose a complete set of orbit labels $I_j$, themselves [integrals of motion](../../../../../integral-of-motion.md); constancy along the characteristic means $f=F(I_1,\ldots,I_s)$. Conversely, for any such differentiable $F$, the chain rule gives $df/dt=\sum_jF_{,j}\dot I_j=0$. This proves [Jeans theorem](../../../../../jeans-theorem.md) in its orbit-invariance form. It does not claim that just two particular integrals classify every orbit in an arbitrary potential. For the specified spherical model, $F(E,L)$ is a rotationally invariant stationary choice.

For the velocity integration, write $v_r=v\cos\eta$, $v_\perp=v\sin\eta$, $L=rv\sin\eta$, and set $k=r/r_a$. At fixed position the velocity-dependent factor is

$$
\exp\!\left[-\frac{v^2}{2\sigma^2}(1+k^2\sin^2\eta)\right],\qquad
 d^3v=v^2\sin\eta\,dv\,d\eta\,d\chi.
$$

Use $\int_0^\infty v^2e^{-Av^2/(2\sigma^2)}dv=\sqrt{\pi/2}\,\sigma^3A^{-3/2}$ and integrate over $\chi$. The [mass density](../../../../../density.md) is

$$
\rho(r)=\frac{\rho_1e^{\psi(r)/\sigma^2}}2\int_0^\pi\frac{\sin\eta\,d\eta}{(1+k^2\sin^2\eta)^{3/2}}
=\frac{\rho_1e^{\psi(r)/\sigma^2}}{1+r^2/r_a^2}.
$$

Since $\rho_c=\rho(0)=\rho_1e^{\psi(0)/\sigma^2}$,

$$
\boxed{\rho(r)=\frac{\rho_c}{1+r^2/r_a^2}\exp\!\left[\frac{\psi(r)-\psi(0)}{\sigma^2}\right].}
$$

These integrals use the stated untruncated [galactic distribution function](../../../../../galactic-distribution-function.md) over all velocities; an additional escape-energy cutoff would change the result.

In local orthogonal velocity components the same exponent is $-[v_r^2+(1+k^2)(v_\theta^2+v_\phi^2)]/(2\sigma^2)$. Each component is a centred [Gaussian distribution](../../../../../normal-distribution.md). The one-dimensional identity $\int v^2e^{-Av^2/(2\sigma^2)}dv/\int e^{-Av^2/(2\sigma^2)}dv=\sigma^2/A$ yields

$$
\boxed{\langle v_r^2\rangle=\sigma^2,\qquad
\langle v_\theta^2\rangle=\langle v_\phi^2\rangle=\frac{\sigma^2r_a^2}{r_a^2+r^2}.}
$$

In particular the [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) is $\beta_{\mathrm{an}}=1-(\sigma_\theta^2+\sigma_\phi^2)/(2\sigma_r^2)=r^2/(r_a^2+r^2)$. This is [Gaussian angular-momentum suppression in a stellar distribution](../../../../../gaussian-angular-momentum-suppression-in-a-stellar-distribution.md).

The radial laws also require self-consistency through the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md):

$$
\frac1{r^2}(r^2\psi')'=-4\pi G\rho,\qquad v_c^2=-r\psi'=\frac{GM(<r)}r.
$$

For $r\ll r_a$, outside a sufficiently small core, the model is almost isotropic and isothermal. Seek its scale-free envelope with $\rho=A/r^2$. Its distribution-density relation gives $\psi'=-2\sigma^2/r$, and the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) gives $A=\sigma^2/(2\pi G)$. Thus the intended intermediate [singular isothermal sphere](../../../../../singular-isothermal-sphere.md) behaviour is

$$
\boxed{\rho\simeq\frac{\sigma^2}{2\pi Gr^2},\qquad v_c^2\simeq2\sigma^2
\quad (r_c\ll r\ll r_a),}
$$

where a core scale is $r_c=\sigma/\sqrt{4\pi G\rho_c}$.

**The stated $r^{-2}$ law cannot be the actual central limit of a regular finite-density model.** For finite $\rho_c$ and $\psi(0)$, regularity and the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) instead give

$$
\psi(r)-\psi(0)=-\frac{2\pi G\rho_c}{3}r^2+O(r^4),\qquad
\rho(r)=\rho_c\left[1-\left(\frac1{r_a^2}+\frac{2\pi G\rho_c}{3\sigma^2}\right)r^2+O(r^4)\right],
$$

and $v_c^2=(4\pi G\rho_c/3)r^2+O(r^4)$. A broad intermediate $r^{-2}$ region exists only if $r_c\ll r_a$; the radius $r_a$ alone does not ensure it.

For the outer [radially anisotropic isothermal halo asymptotics](../../../../../radially-anisotropic-isothermal-halo-asymptotics.md), put $s=\log(r/r_a)$, $y=[\psi(r)-\psi(0)]/\sigma^2$ and $\lambda=4\pi G\rho_c r_a^2/\sigma^2$. At $r\gg r_a$ the density relation and Poisson equation become

$$
y_{ss}+y_s\simeq-\lambda e^y.
$$

The slow outer balance is $y_s\sim-\lambda e^y$, so $d(e^{-y})/ds\sim\lambda$, giving $e^y\sim1/(\lambda s)$. Its consistency check is $y\sim-\log(\lambda s)$, for which $y_{ss}/y_s\sim-1/s\to0$. Therefore

$$
\boxed{\rho(r)\sim\frac{\sigma^2}{4\pi Gr^2\log(r/r_*)},\qquad
 v_c^2(r)\sim\frac{\sigma^2}{\log(r/r_*)}.}
$$

The reference radius $r_*$ changes only subleading logarithmic terms. The [circular speed](../../../../../circular-speed.md) falls as $(\log r)^{-1/2}$, rather than remaining exactly flat.

Physically, the model has an almost isotropic central region and, if the scales separate, a flat-rotation isothermal envelope. Beyond $r_a$, suppression of large [specific angular momentum](../../../../../specific-angular-momentum.md) leaves predominantly radial orbits: radial [velocity dispersion](../../../../../velocity-dispersion.md) remains $\sigma$, while transverse dispersion falls as $r^{-1}$. The outer density acquires a logarithmic suppression and the [galaxy rotation curve](../../../../../galaxy-rotation-curve.md) declines slowly. The enclosed mass still grows approximately as $r/\log r$, so this untruncated model has infinite total mass.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
