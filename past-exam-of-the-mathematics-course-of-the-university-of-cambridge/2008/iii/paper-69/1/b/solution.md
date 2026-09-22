<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the standard uniform-density [incompressible flow](../../../../../../incompressible-flow.md) version of [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md), in which $\nabla\cdot\mathbf u=0$ and [pressure](../../../../../../pressure.md) enforces that constraint. The finite-$\gamma$ compressible adiabatic [pressure](../../../../../../pressure.md) equation is replaced by this [pressure](../../../../../../pressure.md) constraint. The consequences of retaining that cover-sheet equation literally as an additional condition are given below.

Write $F=f(R,z+v(R)t)$, $G=g(R,z-v(R)t)$, $U=F+G$ and $b=F-G$, where $b$ is the toroidal [Alfvén velocity](../../../../../../alfven-velocity.md). The azimuthal [velocity](../../../../../../velocity.md) is $U$, while the [Alfvén velocity](../../../../../../alfven-velocity.md) vector is $b\mathbf e_\phi+v\mathbf e_z$. Both solenoidal constraints hold automatically. Since there is no meridional flow, the azimuthal [magnetohydrodynamic momentum equation](../../../../../../magnetohydrodynamic-momentum-equation.md) and [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) reduce to

$$
U_t=v\,b_z,\qquad b_t=v\,U_z.
$$

Differentiating the traveling arguments verifies both equations for arbitrary smooth $f$, $g$ and $v$. In particular, no condition $v'=0$ is needed.

The remaining force balance is essential. Define the total [pressure](../../../../../../pressure.md) per unit mass, including the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md), by

$$
\Pi=\frac p\rho+\Phi+\frac12(b^2+v^2).
$$

The radial acceleration is $-U^2/R$, and magnetic curvature tension contributes $-b^2/R$. The radial and axial momentum equations are consequently

$$
\boxed{\Pi_R=\frac{U^2-b^2}{R}=\frac{4FG}{R},\qquad \Pi_z=0.}
$$

They are compatible if and only if

$$
\boxed{\partial_z(FG)=0.}
$$

This is the [pressure compatibility of nonlinear torsional Alfvén profiles](../../../../../../pressure-compatibility-of-nonlinear-torsional-alfven-profiles.md). It is also sufficient locally: when $FG$ is independent of $z$, choose

$$
\Pi(R,t)=C(t)+\int_{R_0}^R\frac{4F(R',z,t)G(R',z,t)}{R'}\,dR',\qquad
p=\rho\left[\Pi-\Phi-\frac12(b^2+v^2)\right].
$$

A stationary axisymmetric $\Phi$ satisfying the Poisson equation can be absorbed in this [pressure](../../../../../../pressure.md). Gravity need not vanish. If the axis is included, smoothness requires $U,b=O(R)$ and a regular axial field; $f,g=O(R)$ and smooth even $v$ give the usual regular extension. The [pressure](../../../../../../pressure.md) constant may be chosen to make $p$ positive on a bounded region where the other terms are bounded.

The compatible profiles have the following interpretation. At a cylinder with $v\ne0$, the variables $a=z+vt$ and $c=z-vt$ are independent as $z,t$ vary. Compatibility reads $f_a(R,a)g(R,c)+f(R,a)g_c(R,c)=0$. If both profiles are nonzero, division gives $f_a/f=-g_c/g=\kappa(R)$, independent of both traveling arguments. Therefore

$$
\boxed{f(R,a)=A(R)e^{\kappa(R)a},\qquad
 g(R,c)=C(R)e^{-\kappa(R)c}}
$$

locally on such a region. Alternatively, one profile vanishes identically and the other is unrestricted. Choosing a point where one profile is nonzero shows that a nontrivial opposite profile obeys the same linear [ordinary differential equation](../../../../../../ordinary-differential-equation.md) everywhere on a connected axial interval, so isolated zeros do not create additional overlapping branches.

If $v>0$, a pure $f$ profile travels towards negative $z$, and a pure $g$ profile towards positive $z$, each at the local [Alfvén speed](../../../../../../alfven-speed.md) $v(R)$. Their [velocity](../../../../../../velocity.md) and toroidal-field perturbations have equal magnitudes, with respectively the same or opposite signs. They are finite-amplitude [torsional Alfvén waves](../../../../../../torsional-alfven-wave.md). For a single profile, centrifugal force and magnetic curvature tension cancel, leaving spatially constant $\Pi$; [gas pressure](../../../../../../gas-pressure.md) compensates the varying [magnetic pressure](../../../../../../magnetic-pressure.md). The waveform is transported without axial steepening. Different cylinder speeds shear its phase radially, [magnetohydrodynamic phase mixing](../../../../../../magnetohydrodynamic-phase-mixing.md).

At linear order both wave families may be superposed, since their interaction product is second order in amplitude. Two arbitrary opposing profiles cannot simply be superposed at finite amplitude: their product would generate an axial variation in the radial force imbalance, incompatible with purely azimuthal [velocity](../../../../../../velocity.md). The exponential pair is a formal exception, but is unbounded in an axial direction when $\kappa\ne0$. If both profiles must be bounded on the whole axial line, $\kappa=0$, so $f=A(R)$ and $g=C(R)$ describe a steady rotating, twisted-field equilibrium. Their [pressure](../../../../../../pressure.md) gradient balances the remaining centrifugal and magnetic curvature forces. At $v=0$ there is no propagation; the condition is just $f(R,z)g(R,z)=h(R)$, giving additional steady profiles. These cases exhaust the local possibilities under the stated ansatz and domain qualifications.

There is a closure distinction in the wording. [Incompressible flow](../../../../../../incompressible-flow.md) is the formal infinite-sound-speed limit, not the simultaneous imposition of finite-$\gamma$ adiabatic compression and an independently fixed density; see [Ogilvie's discussion of simplified fluid models, section 2.8](https://arxiv.org/pdf/1604.03835). If the cover-sheet [pressure](../../../../../../pressure.md) equation is nevertheless imposed in addition, then axisymmetry and purely azimuthal motion give $p_t=0$. In addition to $(FG)_z=0$, the necessary and sufficient local [pressure](../../../../../../pressure.md)-gradient conditions, with stationary $\Phi$, are

$$
\boxed{\partial_t\partial_z(b^2)=0,\qquad
\partial_t\left[\frac12\partial_R(b^2)-\frac{4FG}{R}\right]=0.}
$$

They follow by requiring the gradients $p_z/\rho=-\Phi_z-\tfrac12(b^2)_z$ and $p_R/\rho=4FG/R-\Phi_R-\tfrac12(b^2+v^2)_R$ to be time independent; the remaining spatially uniform [pressure](../../../../../../pressure.md) variation is removed by $C(t)$.

For a single traveling profile with $v\ne0$, these extra conditions require its square to be affine in its traveling argument, $f^2=a(R)(z+vt)+b_0(R)$ or $g^2=a(R)(z-vt)+b_0(R)$, with $v(R)a(R)$ constant across a connected radial region. Smooth bounded profiles on the entire axial line then have $a=0$ and are steady. For two nonzero exponential profiles the extra conditions force $\kappa=0$. Thus arbitrary finite-amplitude traveling pulses are valid for the intended incompressible [pressure](../../../../../../pressure.md) model, but not generally for the overconstrained finite-$\gamma$ closure. The force compatibility derived above makes the distinction explicit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
