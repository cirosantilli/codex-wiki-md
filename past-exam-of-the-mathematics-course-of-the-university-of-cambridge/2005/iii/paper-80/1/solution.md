<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Equations and conventions.** Let $\rho_0$ be a constant reference [density](../../../../../density.md) and define total [buoyancy](../../../../../buoyancy.md) acceleration by $\sigma=-g(\rho-\rho_0)/\rho_0$. With reduced [pressure](../../../../../pressure.md) $\Pi=p/\rho_0+gz$, the nonrotating ideal [Boussinesq equations](../../../../../boussinesq-equations.md) are

$$
\frac{D\mathbf u}{Dt}=-\nabla\Pi+\sigma\widehat{\mathbf z},\qquad
\nabla\cdot\mathbf u=0,\qquad\frac{D\sigma}{Dt}=0,
\qquad\frac D{Dt}=\partial_t+\mathbf u\cdot\nabla.
$$

[Density](../../../../../density.md) departures are small compared with $\rho_0$, so they can be neglected in inertia and mass continuity but retained in the gravitational force. The reference stratification must also change [density](../../../../../density.md) only weakly over the depth of interest. [incompressible flow](../../../../../incompressible-flow.md) is already assumed; the [Boussinesq approximation](../../../../../boussinesq-approximation.md) additionally restricts the size of the [density](../../../../../density.md) variations, rather than following automatically from [incompressible flow](../../../../../incompressible-flow.md). An ideal fluid here has neither viscosity nor [buoyancy](../../../../../buoyancy.md) diffusion.

A stationary reference profile $\bar\sigma(z)$ has [buoyancy frequency](../../../../../buoyancy-frequency.md)

$$
N^2(z)=\bar\sigma_z=-\frac g{\rho_0}\bar\rho_z.
$$

Stable stratification has $N^2>0$: an upward-displaced parcel retains its old [buoyancy](../../../../../buoyancy.md) and has negative [buoyancy](../../../../../buoyancy.md) relative to its new surroundings.

**[Vorticity](../../../../../vorticity.md) equation and linearization.** For motion in the $(x,z)$ plane, choose the [streamfunction](../../../../../stream-function.md) by $u=\psi_z$, $w=-\psi_x$. The $y$-component of [vorticity](../../../../../vorticity.md) is then $u_z-w_x=\nabla^2\psi$, where $\nabla^2=\partial_x^2+\partial_z^2$. Taking the $y$-component of the curl of momentum gives

$$
\partial_t\nabla^2\psi+\sigma_x
=(\psi_x\partial_z-\psi_z\partial_x)\nabla^2\psi.
$$

The minus sign in the [buoyancy](../../../../../buoyancy.md) curl follows from $(\nabla\times\sigma\widehat z)_y=-\sigma_x$.

Write $\psi=\bar\psi(z)+\psi'$ with $\bar\psi_z=\bar u(z)$ and $\sigma=\bar\sigma(z)+\sigma'$. The linear [material derivative](../../../../../material-derivative.md) is $D_t=\partial_t+\bar u\partial_x$. The perturbation equations are

$$
D_t\nabla^2\psi'-\bar u_{zz}\psi'_x+\sigma'_x=0,\qquad
D_t\sigma'-N^2\psi'_x=0.
$$

The shear-curvature term arises because $w'$ advects the basic [vorticity](../../../../../vorticity.md) $\bar u_z$. Apply $D_t$ to the first equation and use the second; $D_t$ commutes with $\partial_x$ and does not differentiate the height-only coefficients. Therefore

$$
\boxed{D_t^2\nabla^2\psi'-\bar u_{zz}D_t\psi'_x+N^2\psi'_{xx}=0.}
$$

For a stationary nonzero horizontal [wavenumber](../../../../../wavenumber.md) $k$, the [buoyancy](../../../../../buoyancy.md) equation gives $\widehat\sigma=N^2\widehat\psi/\bar u$. Substitution into the [vorticity](../../../../../vorticity.md) equation gives

$$
\boxed{\widehat\psi_{zz}+m^2(z)\widehat\psi=0,\qquad
m^2=\frac{N^2}{\bar u^2}-\frac{\bar u_{zz}}{\bar u}-k^2=\ell^2-k^2.}
$$

Here $\ell^2$ is the [Scorer parameter](../../../../../scorer-parameter.md). Where $m^2>0$, the vertical structure is oscillatory; where $m^2<0$, it is evanescent. A rigid flat lower boundary gives $\widehat\psi(0)=0$ for $k\ne0$. In an upper evanescent region the growing solution is excluded by boundedness. When propagation persists to infinity, an appropriate [radiation condition](../../../../../radiation-condition.md) distinguishes outgoing from incoming energy for a forced problem.

If $\bar u=U_0+Sz$ with $S>0$, its curvature term vanishes. Bounded $N^2$ implies $\ell^2=N^2/\bar u^2\to0$ aloft. Thus every fixed nonzero $k$ eventually lies in an evanescent region. If stratification is sufficiently strong near the bottom, a lower oscillatory region is separated from the upper evanescent region by a [turning level of a stationary internal wave](../../../../../turning-level-of-a-stationary-internal-wave.md). Waves reflect at that level and at the rigid lower boundary, giving vertically trapped modes for the horizontal wavenumbers that satisfy both conditions. In a slowly varying example the phase condition is approximately $\int_0^{z_t}m\,dz=(n-1/4)\pi$, from a lower node and the turning-point connection; the key point is trapping by the decrease in the [Scorer parameter](../../../../../scorer-parameter.md), not a physical lid.

**Rigid channel modes.** With constant $U=\bar u>0$ and $N$, the vertical nodes require $m_n=n\pi/H$, $n=1,2,\ldots$. Stationarity then requires

$$
k_n^2=\frac{N^2}{U^2}-\frac{n^2\pi^2}{H^2}.
$$

The specified strict interval admits positive $k_n^2$ for exactly $n=1,2$. Choosing $k_1,k_2>0$, every real superposition of these nonzero-wavenumber modes is

$$
\boxed{\psi'=\operatorname{Re}\left[C_1\sin\frac{\pi z}{H}e^{ik_1x}+C_2\sin\frac{2\pi z}{H}e^{ik_2x}\right],\qquad
\sigma'=\frac{N^2}{U}\psi'.}
$$

The two independent complex constants encode the amplitudes and horizontal phases; negative wavenumbers are supplied by complex conjugation, not additional independent constants.

**Exact finite amplitude.** Put $\lambda=N^2/U^2$. Both modes and every superposition satisfy $\nabla^2\psi'=-\lambda\psi'$. For the total [streamfunction](../../../../../stream-function.md) $\Psi=Uz+\psi'$, the total [buoyancy](../../../../../buoyancy.md) is $\sigma=N^2z+(N^2/U)\psi'=(N^2/U)\Psi$. A stationary velocity $(\Psi_z,-\Psi_x)$ is tangent to its [streamfunction](../../../../../stream-function.md) contours, so $D\sigma/Dt=0$ exactly. Moreover the nonlinear self-advection of $\nabla^2\psi'$ vanishes because it is proportional to $\psi'$ itself. The remaining [vorticity](../../../../../vorticity.md) equation is

$$
U\partial_x(-\lambda\psi')=-\partial_x[(N^2/U)\psi'],
$$

which is an identity. Both rigid boundaries remain impermeable, and the curl-free residual in momentum determines a [pressure](../../../../../pressure.md). Thus **the displayed two-mode family consists of exact finite-amplitude Boussinesq solutions**, with no small-amplitude restriction on the constants in these equations. Very large amplitudes can overturn the stratification or leave the physical Boussinesq regime; exact existence does not establish stability.

The two-constant statement concerns wave disturbances with $k\ne0$. If $k=0$ is literally included, arbitrary stationary horizontal shear adjustments $\psi'=F(z)$ and height-only [buoyancy](../../../../../buoyancy.md) changes are also possible. They are changes of the basic state and are not constrained by the wave equation obtained after division by $k$. Excluding that mean-flow sector is necessary for the intended count.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
