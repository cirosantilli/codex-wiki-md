<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Because the wavelength is much smaller than the shelf thickness, the [ice-shelf corrugation relaxation](../../../../../ice-shelf-corrugation-relaxation.md) may be treated as [Stokes flow](../../../../../stokes-flow-split.md) in the half-space $z>0$, with the mean ice-ocean boundary at $z=0$. Let

$$
\eta=\widehat\eta e^{ikx+\sigma t},
\qquad
\mathbf u=\nabla\times(\psi\widehat{\mathbf y}),
$$

so $u=-\psi_z$ and $w=\psi_x$. Taking the curl of the Stokes equation gives the [biharmonic stream function for planar Stokes flow](../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) equation $\nabla^4\psi=0$. Decay as $z\to\infty$ removes the growing modes, leaving

$$
\boxed{\psi=(A+Bz)e^{-kz}e^{ikx+\sigma t}.}
$$

Thus

$$
u=(kA-B+kBz)e^{-kz}e^{ikx+\sigma t},
\qquad
w=ik(A+Bz)e^{-kz}e^{ikx+\sigma t},
$$

and the perturbation pressure obtained from the Stokes equation is

$$
\boxed{p'=2i\mu kB e^{-kz}e^{ikx+\sigma t}.}
$$

The linearized zero-[shear stress](../../../../../shear-stress.md) condition at $z=0$ is

$$
\mu(u_z+w_x)=2\mu k(B-kA)e^{ikx+\sigma t}=0,
$$

so $B=kA$. The water is hydrostatic, and displacement of the density interface gives the normal-stress condition

$$
-p'+2\mu w_z=(\rho_w-\rho)g\eta.
$$

After $B=kA$, one has $w_z(0)=0$, so

$$
-2i\mu k^2A=(\rho_w-\rho)g\widehat\eta.
$$

The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) $\eta_t=w(0)$ gives $\sigma\widehat\eta=ikA$. Eliminating $A$ yields

$$
\boxed{\sigma=-\frac{(\rho_w-\rho)g}{2\mu k}<0.}
$$

Hence a corrugation of wavelength $\lambda=2\pi/k$ decays on the timescale

$$
\boxed{\tau(\lambda)=\frac1{|\sigma|}
=\frac{4\pi\mu}{(\rho_w-\rho)g\lambda}.}
$$

Hydrostatic buoyancy supplies the restoring stress, while viscous deformation over depth $O(k^{-1})$ supplies the resistance. Shorter wavelengths deform a shallower but more strongly sheared layer and therefore have a longer decay time in this gravity-only model. As ice is advected away from the grounding line, long corrugations should disappear first, leaving progressively shorter-wavelength structure farther downstream.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
