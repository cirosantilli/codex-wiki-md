<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $e=(\nabla\mathbf u+\nabla\mathbf u^T)/2$ be the [rate-of-strain tensor](../../../../../strain-rate-tensor.md) and $\boldsymbol\sigma=-pI+2\mu e$ the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md). The [viscous dissipation](../../../../../viscous-dissipation.md) is $D[\mathbf u]=2\mu\int_V e:e\,dV$. The [Minimum-dissipation theorem for Stokes flow](../../../../../minimum-dissipation-theorem-for-stokes-flow.md) compares the [Stokes flow](../../../../../stokes-flow-split.md) with every sufficiently regular [incompressible flow](../../../../../incompressible-flow.md) in the same domain having the same prescribed boundary velocity, with no [body force](../../../../../body-force.md) or with a conservative [body force](../../../../../body-force.md) absorbed into the [fluid pressure](../../../../../fluid-pressure.md). A trial field need not satisfy the [Stokes flow](../../../../../stokes-flow-split.md) equations. Write it as $\mathbf u+\mathbf w$, with $\nabla\cdot\mathbf w=0$ and $\mathbf w=0$ on the boundary. Integration by parts, the symmetry of the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md), and $\nabla\cdot\boldsymbol\sigma=0$ give

$$
2\mu\int_V e(\mathbf u):e(\mathbf w)\,dV=\int_V\boldsymbol\sigma:\nabla\mathbf w\,dV=\int_{\partial V}\mathbf w\cdot\boldsymbol\sigma\mathbf n\,dS-\int_V\mathbf w\cdot\nabla\cdot\boldsymbol\sigma\,dV=0.
$$

Consequently **the Stokes flow minimizes dissipation**:

$$
\boxed{D[\mathbf u+\mathbf w]-D[\mathbf u]=2\mu\int_V e(\mathbf w):e(\mathbf w)\,dV\geq0.}
$$

Equality requires a [rigid body](../../../../../rigid-body-dynamics.md) motion of $\mathbf w$, which the prescribed boundary eliminates. Extending the flow inside the inserted particle as its [rigid body](../../../../../rigid-body-dynamics.md) velocity produces an admissible comparison field with zero internal [rate-of-strain tensor](../../../../../strain-rate-tensor.md); hence the [extra dissipation due to a rigid inclusion](../../../../../extra-dissipation-due-to-a-rigid-inclusion.md) is nonnegative.

Here and below $\mathbf n$ on $A$ points into the particle, so the [traction](../../../../../traction.md) $\boldsymbol\sigma\mathbf n$ represents force exerted by the particle on the fluid. Apply the [Lorentz reciprocal theorem for Stokes flow](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) in the fluid region to $\mathbf u$ and the restriction of $\mathbf u_0$. The equal outer boundary velocities yield

$$
\int_{\partial V}\mathbf V_0\cdot(\boldsymbol\sigma-\boldsymbol\sigma_0)\mathbf n\,dS=\int_A(\mathbf u\cdot\boldsymbol\sigma_0\mathbf n-\mathbf u_0\cdot\boldsymbol\sigma\mathbf n)\,dS.
$$

The boundary-work formula for [viscous dissipation](../../../../../viscous-dissipation.md) therefore gives $D'=\int_A[(\mathbf u-\mathbf u_0)\cdot\boldsymbol\sigma\mathbf n+\mathbf u\cdot\boldsymbol\sigma_0\mathbf n]dS$. The last integral is zero: $\boldsymbol\sigma_0$ is symmetric and divergence-free throughout the particle's original volume, so its total force and [torque](../../../../../torque.md) there vanish, and $\mathbf u$ on $A$ is a [rigid body](../../../../../rigid-body-dynamics.md) velocity. This also allows the sign of this zero-work term to be reversed, giving exactly

$$
\boxed{D'=\int_A(\mathbf u\cdot\boldsymbol\sigma-\mathbf u_0\cdot\boldsymbol\sigma-\mathbf u\cdot\boldsymbol\sigma_0)\cdot\mathbf n\,dS.}
$$

With the particle's centre as origin, define $\mathbf F=\int_A\boldsymbol\sigma\mathbf n\,dS$, $\mathbf G=\int_A\mathbf x\times(\boldsymbol\sigma\mathbf n)\,dS$ and the [particle stresslet tensor](../../../../../particle-stresslet-tensor.md) $S=-\tfrac12\int_A[\mathbf x(\boldsymbol\sigma\mathbf n)+(\boldsymbol\sigma\mathbf n)\mathbf x]dS$. Contracting the linear background velocity with the [traction](../../../../../traction.md) gives

$$
\boxed{D'=\mathbf F\cdot(\mathbf U-\mathbf U_0)+\mathbf G\cdot(\boldsymbol\Omega-\boldsymbol\Omega_0)+S:E_0.}
$$

The background [rate-of-strain tensor](../../../../../strain-rate-tensor.md) $E_0$ is symmetric and trace-free; the trace of this unprojected [particle stresslet tensor](../../../../../particle-stresslet-tensor.md) does not affect the contraction.

For the [straight-rod resistance in a linear flow](../../../../../straight-rod-resistance-in-a-linear-flow.md), write $\Delta\mathbf U=\mathbf U-\mathbf U_0$, $\Delta\boldsymbol\Omega=\boldsymbol\Omega-\boldsymbol\Omega_0$, $M=I-\mathbf p\mathbf p/2$, and $\mathbf X=s\mathbf p$, $-L\leq s\leq L$. The [slender-body force density](../../../../../slender-body-force-density.md) becomes $\mathbf f=C M[\Delta\mathbf U+s(\Delta\boldsymbol\Omega\times\mathbf p-E_0\mathbf p)]$. The integrals of $s$ and $s^2$ are $0$ and $2L^3/3$, respectively, so

$$
\boxed{\mathbf F=2CLM\Delta\mathbf U,\qquad\mathbf G=\frac{2CL^3}{3}\left[(I-\mathbf p\mathbf p)\Delta\boldsymbol\Omega-\mathbf p\times E_0\mathbf p\right].}
$$

For a [force-free](../../../../../force-free.md), [torque-free](../../../../../torque-free.md) rod, $\Delta\mathbf U=0$ and the perpendicular component of $\Delta\boldsymbol\Omega$ is $\mathbf p\times E_0\mathbf p$. Axial spin is not determined by this leading, zero-thickness [slender-body theory](../../../../../slender-body-theory.md); it has no effect on $\mathbf p$. Put $a_p=\mathbf p\cdot E_0\mathbf p$. The vector identity $(\mathbf p\times E_0\mathbf p)\times\mathbf p=E_0\mathbf p-a_p\mathbf p$ gives

$$
\boxed{\mathbf f=-\frac C2s a_p\mathbf p,\qquad\dot{\mathbf p}=\boldsymbol\Omega_0\times\mathbf p+E_0\mathbf p-a_p\mathbf p.}
$$

The [force-free straight-rod orientation equation](../../../../../force-free-straight-rod-orientation-equation.md) combines the background rotation with the part of strain that turns the rod; removing $a_p\mathbf p$ preserves its unit length. A [rigid body](../../../../../rigid-body-dynamics.md) cannot undergo the axial extension or compression imposed by $a_p$, so opposite axial forces resist that deformation. No leading [slender-body force density](../../../../../slender-body-force-density.md) is needed when $a_p=0$, even though the rod may rotate. Its [particle stresslet tensor](../../../../../particle-stresslet-tensor.md) and [viscous dissipation](../../../../../viscous-dissipation.md) are

$$
\boxed{S=\frac{CL^3}{3}a_p\mathbf p\mathbf p,\qquad D'=\frac{CL^3}{3}a_p^2.}
$$

In the [simple shear flow](../../../../../simple-shear-flow.md), $\boldsymbol\Omega_0=-\gamma\mathbf e_z/2$, $(E_0)_{xy}=(E_0)_{yx}=\gamma/2$ and $a_p=\gamma\cos\theta\sin\theta$. Thus the [rod excess dissipation in shear](../../../../../rod-excess-dissipation-in-shear.md) is

$$
\boxed{D'(\theta)=\frac{CL^3\gamma^2}{12}\sin^2(2\theta),\qquad\dot\theta=-\gamma\sin^2\theta.}
$$

The maxima at $\theta=\pi/4,3\pi/4$ correspond to strongest axial extension and compression. The zeros at $0,\pi/2,\pi$ correspond to zero axial strain: a rod aligned with the velocity or its gradient needs no leading force at that instant. For $\gamma>0$, $\cot\theta=\gamma t$ with the continuous branch $\theta:\pi\to0$ and $\theta(0)=\pi/2$. Reversing the [shear flow](../../../../../shear-flow.md) reverses the traversal. Substitution gives

$$
D'(t)=\frac{CL^3\gamma^2}{3}\frac{(\gamma t)^2}{[1+(\gamma t)^2]^2},\qquad\boxed{\int_{-\infty}^{\infty}D'(t)\,dt=\frac{\pi CL^3|\gamma|}{6}.}
$$

The $t^{-2}$ tails make the total finite; the instantaneous zero at $t=0$ lies between two maxima.

<a id="1/image-rod-excess-dissipation-versus-orientation-and-time-in-simple-shear"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-329-rod-dissipation.png)

**[Figure 1](#1/image-rod-excess-dissipation-versus-orientation-and-time-in-simple-shear). Rod excess dissipation versus orientation and time in simple shear**.

For a [dilute rod suspension](../../../../../dilute-rod-suspension.md), the added bulk stress is the number density times the orientation average of the [particle stresslet tensor](../../../../../particle-stresslet-tensor.md). In this ideal infinitely slender, non-interacting model, rods approach alignment with the [shear flow](../../../../../shear-flow.md) and their excess [viscous dissipation](../../../../../viscous-dissipation.md) decays. A real finite-aspect-ratio rod continues to tumble; rotational diffusion and interactions also maintain a spread of orientations. One therefore expects increased effective [viscosity](../../../../../dynamic-viscosity.md), with alignment offering a mechanism for reduced excess [viscosity](../../../../../dynamic-viscosity.md) at strong [shear flow](../../../../../shear-flow.md). This is a qualitative expectation, not a claim that a finite rod suspension has zero steady excess stress.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
