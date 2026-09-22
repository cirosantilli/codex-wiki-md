<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here $\alpha$ is the [thermal expansion coefficient](../../../../../../thermal-expansion-coefficient.md) and $\rho$ is the [mass density](../../../../../../density.md). Let $K=|\mathbf k|$, $h^2=K^2-k_z^2$, $q=\mathbf B\cdot\mathbf k$, and $a^2=q^2/(\mu_0\rho)$, the squared [Alfvén frequency](../../../../../../alfven-frequency.md). We initially consider a nonzero frequency. The temperature and magnetic equations for a [Fourier mode](../../../../../../fourier-mode.md) give

$$
\widehat\theta=\frac{i\beta}{\omega}\widehat w,\qquad
\widehat{\mathbf b}=-\frac{q}{\omega}\widehat{\mathbf u},\qquad
w=u_z.
$$

In particular, the minus sign in the magnetic relation follows from $-i\omega\widehat{\mathbf b}=iq\widehat{\mathbf u}$. Substitution into the [magnetohydrodynamic momentum equation](../../../../../../magnetohydrodynamic-momentum-equation.md), with $P=p/\rho$, gives

$$
-i\Delta\widehat{\mathbf u}+2\Omega\widehat{\mathbf z}\times\widehat{\mathbf u}
=-i\mathbf k\widehat P+g\alpha\widehat\theta\widehat{\mathbf z},\qquad
\Delta=\omega-\frac{a^2}{\omega}.
$$

For [incompressible flow](../../../../../../incompressible-flow.md), $\nabla\times(\widehat{\mathbf z}\times\mathbf u)=-\partial_z\mathbf u$. Taking the vertical component of the [curl](../../../../../../curl.md) eliminates [pressure](../../../../../../pressure.md) and gives, with $\widehat\zeta=(i\mathbf k\times\widehat{\mathbf u})_z$,

$$
-i\Delta\widehat\zeta-2i\Omega k_z\widehat w=0,
\qquad \Delta\widehat\zeta+2\Omega k_z\widehat w=0.
$$

Taking another [curl](../../../../../../curl.md) and its vertical component uses $\nabla\times\nabla\times\mathbf u=-\nabla^2\mathbf u$ and $(\nabla\times\nabla\times(\theta\widehat{\mathbf z}))_z=h^2\widehat\theta$. Thus

$$
-i\Delta K^2\widehat w-2i\Omega k_z\widehat\zeta=g\alpha h^2\widehat\theta,
$$

or, after eliminating temperature,

$$
\left(\Delta K^2+\frac{g\alpha\beta h^2}{\omega}\right)\widehat w+2\Omega k_z\widehat\zeta=0.
$$

The two equations for vertical velocity and vertical [vorticity](../../../../../../vorticity.md) have a nontrivial solution only when their determinant vanishes. This proves the [stratified magneto-Coriolis wave](../../../../../../stratified-magneto-coriolis-wave.md) [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{\Delta^2K^2-4\Omega^2k_z^2+
\frac{g\alpha\beta}{\omega}\Delta h^2=0,\qquad
\Delta=\omega-\frac{(\mathbf B\cdot\mathbf k)^2}{\mu_0\rho\omega}}.
$$

No division by $\Delta$ was necessary, so a possible $\Delta=0$ is retained. Division by $\omega$, however, was necessary. Stationary disturbances must be checked directly in the original equations: for example, with $q\ne0$, $\mathbf u=0$ and an appropriate solenoidal magnetic perturbation can balance temperature-induced [buoyancy](../../../../../../buoyancy.md) and [pressure](../../../../../../pressure.md). Such static balances are separate from the nonzero-frequency wave branches.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
