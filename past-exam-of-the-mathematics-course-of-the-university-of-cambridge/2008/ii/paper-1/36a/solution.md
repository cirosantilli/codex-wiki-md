<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

Let $e_{ij}=(\partial_i u_j+\partial_j u_i)/2$ be the [rate-of-strain tensor](../../../../../strain-rate-tensor.md). A [Newtonian fluid](../../../../../newtonian-fluid.md) has a linear isotropic constitutive law for its viscous [stress tensor](../../../../../cauchy-stress-tensor.md). To determine its form, diagonalize the symmetric tensor $e$. Rotations by $\pi$ about its principal axes leave $e$ fixed, forcing its stress response to be diagonal as well. Linearity and symmetry under permutations of the axes force each diagonal entry to be $\lambda\operatorname{tr}e+2\mu e_{ii}$, with the same constants for each axis. Rotating back gives $\tau_{ij}=\lambda e_{kk}\delta_{ij}+2\mu e_{ij}$. Since [incompressibility](../../../../../incompressible-flow.md) means $e_{kk}=0$, adding the arbitrary isotropic pressure gives

$$
\boxed{\sigma_{ij}=-p\delta_{ij}+2\mu e_{ij}.}
$$

At a material interface between ordinary viscous fluids without interfacial slip, velocity is continuous, and its normal component equals the interface's normal speed. Tangential traction is continuous when [surface tension](../../../../../surface-tension.md) is constant. Normal traction has the curvature-dependent [surface tension](../../../../../surface-tension.md) jump; in a convention defining signed curvature $\kappa$ by the balance, $(\sigma_+-\sigma_-)n=\gamma\kappa n$. With no [surface tension](../../../../../surface-tension.md), the full traction is continuous. At rigid stationary walls the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) imposes zero velocity.

Put $G=-dp/dx>0$ and seek $u=u_\pm(y)e_x$. The convective acceleration vanishes, and the [Navier-Stokes equations](../../../../../navier-stokes-equation.md) reduce to $\mu_\pm u_\pm''=-G$, with $p=p_0-Gx$. [continuity](../../../../../continuous-function.md) of velocity and tangential traction at $y=0$ gives a common interface velocity $U_0$ and a common shear integration constant $C$:

$$
u_\pm(y)=U_0+\frac C{\mu_\pm}y-\frac G{2\mu_\pm}y^2.
$$

Imposing $u_-(-a)=u_+(a)=0$ gives

$$
\boxed{U_0=\frac{Ga^2}{\mu_++\mu_-},\qquad C=\frac{Ga(\mu_--\mu_+)}{2(\mu_++\mu_-)}.}
$$

The velocity has no normal component, so the flat interface remains stationary, and its normal stresses match because pressure is common. These expressions give the [two-layer plane Poiseuille flow with unequal viscosities](../../../../../two-layer-plane-poiseuille-flow-with-unequal-viscosities.md).

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
