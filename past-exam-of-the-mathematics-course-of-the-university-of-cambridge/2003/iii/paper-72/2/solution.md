<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

After removing the hydrostatic background pressure, the two-dimensional ideal [Boussinesq equations](../../../../../boussinesq-equations.md) are

$$
u_t+uu_x+wu_z=-p_x,\qquad
w_t+uw_x+ww_z=-p_z+\sigma,\qquad u_x+w_z=0,
$$

with the [buoyancy](../../../../../buoyancy.md) equation $\sigma_t+u\sigma_x+w\sigma_z+N^2(z)w=0$. The last equation follows by materially advecting total buoyancy $B_0(z)+\sigma$ with $B_0'(z)=N^2(z)$. Take the [streamfunction](../../../../../stream-function.md) convention

$$
u=\psi_z,\qquad w=-\psi_x,
$$

so the $y$-component of [vorticity](../../../../../vorticity.md) is $q=u_z-w_x=\nabla^2\psi$. Taking $\partial_z$ of horizontal momentum minus $\partial_x$ of vertical momentum cancels pressure. [Incompressibility](../../../../../incompressible-flow.md) combines the remaining nonlinear terms into advection of $q$, giving $q_t+uq_x+wq_z=-\sigma_x$. Hence the full equations are

$$
\boxed{\nabla^2\psi_t+\sigma_x=\psi_x(\nabla^2\psi)_z-\psi_z(\nabla^2\psi)_x,}
$$



$$
\boxed{\sigma_t+\psi_z\sigma_x-\psi_x\sigma_z-N^2(z)\psi_x=0.}
$$

There is no vortex stretching in this genuinely two-dimensional velocity field.

Write $\psi=\psi_0(z)+\phi$, with $\psi_0'=\overline u=U(z)$ and background buoyancy anomaly zero. The [Linearized Boussinesq equations](../../../../../linearized-boussinesq-equations.md) become

$$
(\partial_t+U\partial_x)\nabla^2\phi-U''\phi_x+\sigma_x=0,\qquad
(\partial_t+U\partial_x)\sigma-N^2\phi_x=0.
$$

For a stationary disturbance $\phi=\widehat\psi(z)e^{ikx}$ with real $k\ne0$ and $U>0$, the second equation gives $\widehat\sigma=(N^2/U)\widehat\psi$. The first therefore reduces to the stationary [Taylor–Goldstein equation](../../../../../taylor-goldstein-equation.md)

$$
\boxed{\widehat\psi''+m^2(z)\widehat\psi=0,\qquad
m^2(z)=\frac{N^2}{U^2}-\frac{U''}{U}-k^2.}
$$

The restriction $k\ne0$ is used when cancelling $ik$; a purely horizontally uniform alteration of the background is not this wave problem.

For the [exponential-profile stationary stratified waves](../../../../../exponential-profile-stationary-stratified-waves.md), define

$$
C=\frac{N_0^2}{U_0^2}-M^2,\qquad s=C-k^2.
$$

Since $U''/U=M^2$ and $N/U=N_0/U_0$, all coefficients are constant. The complete vertical solution set is

$$
\boxed{\widehat\psi(z)=
\begin{cases}
A\cos(\sqrt s\,z)+B\sin(\sqrt s\,z),&s>0,\\
A+Bz,&s=0,\\
Ae^{\sqrt{-s}\,z}+Be^{-\sqrt{-s}\,z},&s<0.
\end{cases}}
$$

Shifting the origin of $z$ simply changes the two constants. Vertical oscillation requires $N_0/U_0>\sqrt{M^2+k^2}$; equality gives an affine structure; below that value the structure is evanescent or growing, with admissibility determined by the physical boundaries.

The [Rayleigh quotient with one Neumann endpoint](../../../../../rayleigh-quotient-with-one-neumann-endpoint.md) must retain its upper boundary term. On a finite interval with $D=z_2-z_1>0$, choose a nonzero real vertical structure, so the denominator is strictly positive. Multiplication of the differential equation by $\widehat\psi$ and [integration by parts](../../../../../integration-by-parts.md) gives

$$
\mathcal R=\frac{\int_{z_1}^{z_2}(C\widehat\psi^2-\widehat\psi'^2)\,dz}
{\int_{z_1}^{z_2}\widehat\psi^2\,dz}
=k^2-\frac{[\widehat\psi\widehat\psi']_{z_1}^{z_2}}
{\int_{z_1}^{z_2}\widehat\psi^2\,dz}.
$$

With only $\widehat\psi'(z_1)=0$, it equals $k^2$ precisely when $\widehat\psi(z_2)\widehat\psi'(z_2)=0$. A lower [Neumann boundary condition](../../../../../neumann-boundary-condition.md) alone does not ensure this.

For $s>0$, the lower condition selects $\widehat\psi=A\cos[\sqrt s(z-z_1)]$. Equality of the quotient requires $\sqrt sD=n\pi/2$ for a positive integer $n$: even $n$ gives an upper Neumann condition, odd $n$ an upper [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md). Thus

$$
k^2=C-\frac{n^2\pi^2}{4D^2}>0,
$$

which additionally restricts $N_0^2/U_0^2>M^2+n^2\pi^2/(4D^2)$. If $s=0$, the lower condition leaves a constant structure; it has quotient $C=k^2$, possible for a genuine wave only when $C>0$. If $s<0$, the lower condition leaves $A\cosh[\sqrt{-s}(z-z_1)]$, whose upper product is positive and whose quotient is strictly less than $k^2$. On an infinite interval, none of these nonzero lower-Neumann structures is square-integrable, so the displayed ratio of integrals is not a defined finite-integral quotient there. Ratios of truncated integrals would be a different limiting prescription.

For every mode above, including the affine and exponential cases, the disturbance satisfies

$$
\boxed{\nabla^2\phi=-C\phi=\left(M^2-\frac{N_0^2}{U_0^2}\right)\phi.}
$$

This statement concerns the disturbance, not the sum with the background [streamfunction](../../../../../stream-function.md); the latter generally has a different Laplacian eigenvalue. Its buoyancy polarization is

$$
\boxed{\sigma=\alpha(z)\phi,\qquad \alpha(z)=\frac{N_0^2}{U_0}e^{Mz}.}
$$

Thus no nonzero mode has a constant buoyancy-to-streamfunction ratio when $M\ne0$.

The [nonlinear exactness test for a stratified streamfunction mode](../../../../../nonlinear-exactness-test-for-a-stratified-streamfunction-mode.md) now distinguishes the two equations. The disturbance's vorticity self-advection vanishes because its Laplacian is proportional to itself. But its buoyancy self-advection is

$$
\phi_z\sigma_x-\phi_x\sigma_z=-\alpha'(z)\phi\phi_x=-M\alpha(z)\phi\phi_x.
$$

For a nonzero real sinusoidal disturbance and $M>0$, this is a nonzero second harmonic somewhere. Consequently **none of the nontrivial modes with the stipulated positive $M$ is by itself an exact finite-amplitude solution of both nonlinear equations**. Additional harmonics or mean corrections would be needed. In the limiting case $M=0$, $U,N,\alpha$ are constant; both self-interactions vanish, and these same single-wavenumber structures, or their superpositions with the same $C$, do solve the full ideal equations wherever their boundary conditions are admissible.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
