<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For body-force-free Stokes fields with the same [viscosity](../../../../../dynamic-viscosity.md),

$$
\boxed{\int_{\partial V}u^{(1)}\cdot\sigma^{(2)}n\,dS
=\int_{\partial V}u^{(2)}\cdot\sigma^{(1)}n\,dS.}
$$

To prove this [Lorentz reciprocal theorem](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md), integrate the divergence of the difference of the two cross-work fluxes. Both [stress](../../../../../stress.md) divergences are zero; [incompressibility](../../../../../incompressible-flow.md) and symmetry of the Newtonian [stress](../../../../../stress.md) reduce each cross-gradient contraction to $2\mu e^{(1)}:e^{(2)}$. These are equal, so the divergence integrates to zero. The argument applies to an exterior domain by first cutting it off and taking the outer radius to infinity; the decaying [velocity](../../../../../velocity.md) and [stress](../../../../../stress.md) make the outer boundary contribution vanish.

Define the generalized [force](../../../../../force.md) as [force](../../../../../force.md) and [torque](../../../../../torque.md) exerted by the rigid body on the fluid. With a resting far field and [no-slip boundary conditions](../../../../../no-slip-boundary-condition.md), $u=U+\Omega\times x$ on the body, and linearity gives

$$
\binom{F}{G}=\mathsf R\binom{U}{\Omega}.
$$

For two such motions the reciprocal theorem becomes

$$
U^{(1)}\cdot F^{(2)}+\Omega^{(1)}\cdot G^{(2)}
=U^{(2)}\cdot F^{(1)}+\Omega^{(2)}\cdot G^{(1)}.
$$

Since the six-component velocities can be chosen independently, $\boxed{\mathsf R=\mathsf R^T}$. The ordinary work identity gives

$$
\boxed{U\cdot F+\Omega\cdot G=2\mu\int_{V_{\rm fluid}}e:e\,dV>0}
$$

for every nonzero rigid-body motion. If the integral were zero, $e=0$ would make the connected exterior flow an infinitesimal rigid motion. Its decay at infinity requires that motion to be zero, which is incompatible with a nonzero no-slip body [velocity](../../../../../velocity.md). Thus $\mathsf R$ is positive definite. Fluid-on-body [forces](../../../../../force.md) have the opposite sign; their map is $-\mathsf R$, not a positive-definite resistance [matrix](../../../../../matrix.md).

Write $s_\phi=\sin\phi$ and $c_\phi=\cos\phi$. The helix has $|dX/d\theta|=b\sqrt{1+\tan^2\phi}=b\sec\phi$, so

$$
\boxed{ds=b\sec\phi\,d\theta,\qquad L=N\pi b\sec\phi.}
$$

Its unit tangent is $X'=c_\phi e_\theta+s_\phi e_z$, where $e_\theta=(-\sin\theta,\cos\theta,0)$. The given [slender-body force density](../../../../../slender-body-force-density.md) is the [force](../../../../../force.md) per arc length exerted on the fluid. For pure axial translation, $V=Ue_z$, it gives

$$
f_z=CU(1-s_\phi^2/2),\qquad f_\theta=-CU s_\phi c_\phi/2.
$$

For pure rotation, $V=b\Omega e_\theta$, it gives

$$
f_z=-Cb\Omega s_\phi c_\phi/2,\qquad f_\theta=Cb\Omega(1-c_\phi^2/2).
$$

The axial [torque](../../../../../torque.md) per unit arc length is $bf_\theta$. Integrating along the wire gives the [axial resistance matrix of a slender helix](../../../../../axial-resistance-matrix-of-a-slender-helix.md)

$$
\boxed{\binom{F_z}{G_z}=\begin{pmatrix}\mathcal A&\mathcal B\\\mathcal B&\mathcal D\end{pmatrix}\binom{U}{\Omega},}
$$



$$
\boxed{\mathcal A=\frac{CL}{2}(1+c_\phi^2),\qquad
\mathcal B=-\frac{CLb}{2}s_\phi c_\phi,\qquad
\mathcal D=\frac{CLb^2}{2}(1+s_\phi^2).}
$$

Thus translation gives $(F_z,G_z)=(\mathcal A U,\mathcal B U)$, and rotation gives $(\mathcal B\Omega,\mathcal D\Omega)$. These are the requested axial components; the axial swimmer approximation does not require proving statements about the other components. The equality of the two off-diagonal coefficients checks reciprocity, and

$$
\mathcal A\mathcal D-\mathcal B^2=\frac{C^2L^2b^2}{2}>0.
$$

For the organism, retain the specified entrainment approximation: the head moves with the local large-scale fluid translation, and its angular [velocity](../../../../../velocity.md) $\Omega-\omega$ differs from the local fluid rotation $\Omega$ by $-\omega$. Put $D_0=8\pi\mu a^3$. Its [torque](../../../../../torque.md) on the fluid is therefore $-D_0\omega$, and its [force](../../../../../force.md) is neglected. Neutral buoyancy and absence of external [torque](../../../../../torque.md) give

$$
\mathcal A U+\mathcal B\Omega=0,\qquad \mathcal B U+\mathcal D\Omega=D_0\omega.
$$

Solving,

$$
U=-\frac{\mathcal B D_0\omega}{\mathcal A\mathcal D-\mathcal B^2}
=\frac{D_0\omega s_\phi c_\phi}{CLb}
=\boxed{\frac{\omega a^3|\log\epsilon|\sin2\phi}{bL}}.
$$

This is the [entrained-head approximation for a helical microswimmer](../../../../../entrained-head-approximation-for-a-helical-microswimmer.md), which differs from treating the head as an isolated sphere in otherwise stationary fluid. The flagellum's angular speed is also $\Omega=D_0\omega(1+c_\phi^2)/(CLb^2)$.

At fixed $b,L,a,\omega,\epsilon$, the speed is maximal at $\phi=\pi/4$ and tends to zero at either limiting pitch. At fixed other parameters it decreases as $1/L$: the longer flagellum has more resistance at the fixed [torque](../../../../../torque.md) supplied in this model. Holding the number of turns fixed instead would make $L$ change with pitch, so that is a different comparison.

The motor exerts equal and opposite [torques](../../../../../torque.md) of magnitude $D_0\omega$ on flagellum and head, whose relative angular speed is $\omega$. Therefore its rate of working is

$$
\boxed{\mathcal P=D_0\omega^2=8\pi\mu a^3\omega^2.}
$$

Equivalently, the work delivered to the fluid is $G_{\rm flag}\Omega+G_{\rm head}(\Omega-\omega)=D_0\omega\Omega-D_0\omega(\Omega-\omega)$. Translation contributes no net work because the total [force](../../../../../force.md) vanishes. This explains the independence from $U$ and $\Omega$, without assigning an isolated-fluid drag law to the entrained head.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
