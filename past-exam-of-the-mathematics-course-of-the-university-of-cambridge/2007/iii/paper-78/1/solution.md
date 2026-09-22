<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a fixed fluid domain with prescribed [velocity](../../../../../velocity.md) on its whole boundary, the [Minimum-dissipation theorem for Stokes flow](../../../../../minimum-dissipation-theorem-for-stokes-flow.md) compares the actual incompressible [Stokes flow](../../../../../stokes-flow-split.md) $u$ with every admissible incompressible [velocity](../../../../../velocity.md) field $v$ having the same boundary values. The trial fields need not themselves satisfy the momentum equation. With $e(u)=(\nabla u+\nabla u^T)/2$ and constant [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu$, define the [viscous dissipation](../../../../../viscous-dissipation.md)

$$
\mathcal D[u]=2\mu\int e(u):e(u)\,dV.
$$

Assume no nonconservative body force, or absorb a conservative force into the [pressure](../../../../../pressure.md). Set $w=v-u$, so $\nabla\cdot w=0$ and $w=0$ on the boundary. The Stokes [stress tensor](../../../../../cauchy-stress-tensor.md) $\sigma=-pI+2\mu e(u)$ obeys $\nabla\cdot\sigma=0$. Because [pressure](../../../../../pressure.md) has zero contraction with $e(w)$,

$$
2\mu\int e(u):e(w)\,dV=\int\sigma:\nabla w\,dV=\int_{\partial V}w\cdot\sigma n\,dS-\int_Vw\cdot(\nabla\cdot\sigma)\,dV=0.
$$

Expanding the square proves

$$
\boxed{\mathcal D[v]=\mathcal D[u]+2\mu\int e(w):e(w)\,dV\geq\mathcal D[u].}
$$

Equality requires $e(w)=0$, so $w$ is a rigid motion; the homogeneous boundary values force it to vanish. The theorem concerns fixed boundary velocities, not fixed applied forces or arbitrary comparisons between different fluid domains.

For the concentric-sphere motion, seek $u=F(r)\boldsymbol\Omega\times x$. Incompressibility is automatic. The choice $F=A+B/r^3$ gives a harmonic [velocity](../../../../../velocity.md): the linear term is harmonic, and each component of $x/r^3$ is a derivative of the harmonic function $1/r$. The no-slip conditions $F(a)=1$, $F(b)=0$ give

$$
B=\frac{a^3b^3}{b^3-a^3},\qquad A=-\frac{a^3}{b^3-a^3}.
$$

Thus the [Rotational Stokes flow between concentric spheres](../../../../../rotational-stokes-flow-between-concentric-spheres.md) is

$$
\boxed{u(x)=\frac{a^3}{b^3-a^3}\left(\frac{b^3}{r^3}-1\right)\boldsymbol\Omega\times x.}
$$

It satisfies the Stokes equation with constant [pressure](../../../../../pressure.md), and the uniqueness implied by the theorem identifies it as the required flow.

In the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md), take $\Phi=-u/2$ and $\chi=0$. Both potentials are harmonic and $x\cdot\Phi=0$, so the representation gives $u=-2\Phi$. Also

$$
\nabla\cdot\Phi=-\tfrac12\{\nabla F\cdot(\boldsymbol\Omega\times x)+F\nabla\cdot(\boldsymbol\Omega\times x)\}=0,
$$

and therefore **$p=0$**, after choosing the arbitrary [pressure](../../../../../pressure.md) constant.

This [pressure](../../../../../pressure.md) conclusion also follows from symmetry and [Linearity of Stokes flow](../../../../../linearity-of-stokes-flow.md). [Pressure](../../../../../pressure.md) is a scalar linear in the axial vector $\boldsymbol\Omega$, and isotropy leaves only a possible term proportional to $\boldsymbol\Omega\cdot x$. That is a pseudoscalar, forbidden by reflection symmetry of the concentric spherical domain. Hence the [pressure](../../../../../pressure.md) perturbation vanishes. Equivalently, axisymmetry and reflection with flow reversal make the motion purely azimuthal, while its meridional momentum balance has no [pressure](../../../../../pressure.md) gradient.

Let $v=\boldsymbol\Omega\times x$ in the following stress calculation. The symmetric [velocity](../../../../../velocity.md) gradient is

$$
e_{ij}=\frac{F'(r)}{2r}(x_jv_i+x_iv_j),\qquad F'=-\frac{3B}{r^4}.
$$

The full [stress tensor](../../../../../cauchy-stress-tensor.md), in the zero-[pressure](../../../../../pressure.md) gauge, is therefore

$$
\boxed{\sigma_{ij}=-\frac{3\mu B}{r^5}(x_jv_i+x_iv_j).}
$$

For $n=x/r$, the traction on a radial surface is $\sigma n=-3\mu B(\boldsymbol\Omega\times n)/r^3$. This completely specifies the stress field; with the polar axis along $\boldsymbol\Omega$, its only nonzero spherical shear component is $\sigma_{r\phi}=-3\mu B\Omega\sin\theta/r^3$.

The fluid couple on the inner sphere is the integral of $x\times\sigma n$ with the normal pointing from the solid into the fluid. Using $\int n_i n_j\,d\omega=(4\pi/3)\delta_{ij}$,

$$
\int_{r=a}x\times\sigma n\,dS=-3\mu B\int\{\boldsymbol\Omega-n(n\cdot\boldsymbol\Omega)\}\,d\omega=-8\pi\mu B\boldsymbol\Omega.
$$

Hence the sustaining applied [Torque in rotational Stokes flow between concentric spheres](../../../../../torque-in-rotational-stokes-flow-between-concentric-spheres.md) is

$$
\boxed{\boldsymbol G=\frac{8\pi\mu a^3b^3}{b^3-a^3}\boldsymbol\Omega.}
$$

For $a\ll b$, it approaches the isolated [rotating sphere in Stokes flow](../../../../../rotating-sphere-in-stokes-flow.md) result $8\pi\mu a^3\boldsymbol\Omega$. For a narrow gap $d=b-a\ll a$, it becomes $8\pi\mu a^4\boldsymbol\Omega/(3d)$: the divergent resistance is that of a thin Couette shear layer, with speed scale $a\Omega$ and gradient scale $a\Omega/d$.

Now add the force-free, couple-free rigid particles and denote the resulting [velocity](../../../../../velocity.md) by $u_p$. Extend $u_p$ through each particle as its rigid translational and rotational [velocity](../../../../../velocity.md). No slip makes this extension continuous across every particle surface; it is incompressible and has zero [rate-of-strain tensor](../../../../../strain-rate-tensor.md) inside each particle. It therefore gives an admissible trial [velocity](../../../../../velocity.md) in the original particle-free annulus, with exactly the same sphere boundary velocities. Its full-annulus dissipation is the actual fluid dissipation $\mathcal D_p$, since the added interior integrals are zero. The [Minimum-dissipation theorem for Stokes flow](../../../../../minimum-dissipation-theorem-for-stokes-flow.md) consequently gives $\mathcal D_p\geq\mathcal D_0$.

The boundary-work identity follows by integrating $\nabla\cdot(\sigma u)$: dissipation equals the mechanical power supplied at all rigid boundaries. The outer sphere is stationary; the inner sphere has no translation, so any force needed to hold its centre does no work; and each added particle contributes zero power because its net force and couple are zero. Thus $\mathcal D_p=\boldsymbol G_p\cdot\boldsymbol\Omega$, while $\mathcal D_0=\boldsymbol G_0\cdot\boldsymbol\Omega$. Therefore

$$
\boxed{(\boldsymbol G_p-\boldsymbol G_0)\cdot\boldsymbol\Omega\geq0.}
$$

For $\boldsymbol\Omega\ne0$ and at least one particle of positive volume in the open annulus, the inequality is strict. Equality would make the extended [velocity](../../../../../velocity.md) identical to the particle-free solution, yet that solution has nonzero strain on every open region away from the rotation axis and cannot be rigid throughout any particle interior. Hence **the applied couple component along the imposed angular [velocity](../../../../../velocity.md) increases**. This is the fixed-[velocity](../../../../../velocity.md) [extra dissipation due to a rigid inclusion](../../../../../extra-dissipation-due-to-a-rigid-inclusion.md) argument; it does not assert an increase in every transverse torque component.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
