<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use material coordinates $X$ and write the placement as $y=X+u$. The [strain energy density](../../../../../strain-energy-density.md) $W$ in the printed convention is per unit reference mass. It is convenient to use the conventional [first Piola-Kirchhoff stress tensor](../../../../../first-piola-kirchhoff-stress-tensor.md) $P=s^{\mathsf T}$, so

$$
\mathcal W=\rho_0W,\qquad P_{ij}=\frac{\partial\mathcal W}{\partial A_{ij}}.
$$

Assume the undeformed reference state is stress-free. With $H=A-I$ and [infinitesimal strain tensor](../../../../../infinitesimal-strain-tensor.md) $e=(H+H^{\mathsf T})/2$, [material isotropy](../../../../../material-isotropy.md) and [material frame indifference](../../../../../material-frame-indifference.md) give the quadratic expansion

$$
\mathcal W(I+H)=\mathcal W(I)+\frac{\lambda}{2}(\operatorname{tr}e)^2+\mu\,e:e+O(|H|^3).
$$

Consequently the [Lamé parameters from hyperelastic energy Hessian](../../../../../lame-parameters-from-hyperelastic-energy-hessian.md) are

$$
\boxed{\lambda=\rho_0W_{A_{11}A_{22}}(I),\qquad
\mu=\rho_0W_{A_{12}A_{12}}(I),\qquad
\lambda+2\mu=\rho_0W_{A_{11}A_{11}}(I).}
$$

Indeed, differentiating the quadratic expression twice gives

$$
\rho_0W_{A_{ij}A_{k\ell}}(I)
=\lambda\delta_{ij}\delta_{k\ell}
+\mu(\delta_{ik}\delta_{j\ell}+\delta_{i\ell}\delta_{jk}),
$$

the [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md) of [linear elasticity](../../../../../linear-elasticity.md). A prestressed reference state requires the corresponding initial-stress corrections; the displayed formula concerns the natural state.

For a plane [elastic wave](../../../../../elastic-wave.md), $u=u(X_1,t)$, put $r=e_1+u_{,X_1}$ and $\Psi(r)=W([r,e_2,e_3])$. Balance of momentum without [body force](../../../../../body-force.md) becomes

$$
\boxed{u_{i,tt}=\partial_{X_1}\Psi_{r_i}(r),\qquad
r_t=v_{,X_1},\quad v_t=C(r)r_{,X_1},\quad
v=u_t,\ C=D^2\Psi.}
$$

This is a material-coordinate equation: the reference density cancels between inertia and [nominal stress](../../../../../nominal-stress-tensor.md). If $C a_\alpha=c_\alpha^2a_\alpha$, the first-order system has [characteristic speeds](../../../../../characteristic-speed.md) $\pm c_\alpha$ and right [eigenvectors](../../../../../eigenvector.md) $(a_\alpha,\mp c_\alpha a_\alpha)$. Along a [characteristic curve](../../../../../characteristic-curve.md) with $dX_1/dt=s=\pm c_\alpha$, its differential compatibility relation is

$$
a_\alpha\cdot dv-s\,a_\alpha\cdot dr=0.
$$

This follows by multiplying the system by the left [eigenvector](../../../../../eigenvector.md) $(-s a_\alpha^{\mathsf T},a_\alpha^{\mathsf T})$. It does not assert the existence of globally integrable [Riemann invariants](../../../../../riemann-invariant.md) for an arbitrary three-component constitutive law.

There is a necessary qualification to the finite-amplitude transverse request. Set $u=(0,w,0)$ and $q=w_{,X_1}$, so $r=(1,q,0)$. The longitudinal momentum equation requires

$$
0=\partial_{X_1}\Psi_{r_1}(1,q,0).
$$

Thus arbitrary nonuniform pure transverse profiles are possible only if the [compatibility condition for pure nonlinear transverse waves](../../../../../compatibility-condition-for-pure-nonlinear-transverse-waves.md) holds:

$$
\boxed{\Psi_{r_1}(1,q,0)\ \text{is independent of }q,\quad
\Psi_{r_1r_2}(1,q,0)=0.}
$$

The third component vanishes by the reflection symmetry implied by [isotropy](../../../../../isotropy.md) and objectivity. The shear equation then closes:

$$
\rho_0 w_{tt}=\partial_{X_1}\tau(q),\qquad
\tau(q)=\frac{d}{dq}\mathcal W([e_1+qe_2,e_2,e_3]),\qquad
c(q)^2=\frac{\tau'(q)}{\rho_0}>0.
$$

General compressible [hyperelastic material](../../../../../hyperelastic-material.md) assumptions alone do not imply the required compatibility. For a concrete counterexample, take the [Saint Venant–Kirchhoff hyperelastic energy](../../../../../saint-venant-kirchhoff-hyperelastic-energy.md)

$$
\mathcal W=\frac{\lambda}{2}(\operatorname{tr}E)^2+\mu\operatorname{tr}(E^2),
\qquad E=\frac{A^{\mathsf T}A-I}{2},\qquad \lambda,\mu>0.
$$

For $A=[(a,q,0)^{\mathsf T},e_2,e_3]$, this becomes

$$
\mathcal W(a,q)=\frac{\lambda+2\mu}{8}(a^2+q^2-1)^2+\frac{\mu q^2}{2}.
$$

At $a=1$, $P_{11}=(\lambda+2\mu)q^2/2$. A varying shear therefore produces a longitudinal force $(\lambda+2\mu)q q_{,X_1}$ and cannot preserve $u_1=0$. Infinitesimal transverse waves do exist, because this coupling is second order, but a general pure finite-amplitude transverse wave does not.

The [compatible nonlinear shear energy](../../../../../compatible-nonlinear-shear-energy.md) class is nonempty and can be genuinely nonlinear. Define $J=\det A$, $S=\operatorname{tr}(A^{\mathsf T}A)-2J$, and, for $h\ge0$, take

$$
\mathcal W=\frac{\mu}{2}(S-1)+\frac h4(S-1)^2+
\frac{\lambda+\mu}{2}(J-1)^2.
$$

This is objective and [isotropic](../../../../../isotropy.md). Near $A=I$, $S-1=2\operatorname{tr}(e^2)-(\operatorname{tr}e)^2+O(|H|^3)$, so it has the specified [Lamé parameters](../../../../../lame-parameter.md). On the plane deformation above, $S-1=(a-1)^2+q^2$ and $J=a$. Hence $P_{11}=0$ at $a=1$, while

$$
\tau(q)=\mu q+hq^3,\qquad c(q)=\sqrt{\frac{\mu+3hq^2}{\rho_0}}.
$$

For positive $\lambda,\mu$, the relevant incremental plane moduli are positive. This supplies an explicit stable pure transverse family and, when $h>0$, amplitude-dependent [wave speed](../../../../../wave-speed.md).

For any compatible family, let

$$
H(q)=\int_0^q c(z)\,dz,\qquad v=w_t.
$$

The equations $q_t=v_{,X_1}$ and $v_t=c(q)^2q_{,X_1}$ give the [Riemann invariants](../../../../../riemann-invariant.md)

$$
(\partial_t-c\partial_{X_1})(v+H)=0,\qquad
(\partial_t+c\partial_{X_1})(v-H)=0.
$$

Consider the initially undisturbed half-space $X_1>0$. A right-going [simple wave](../../../../../simple-wave.md) has the incoming invariant $v+H=0$, so $v=-H(q)$. Denote the prescribed boundary [nominal stress](../../../../../nominal-stress-tensor.md) by $T(t)=P_{21}(0,t)=\tau(q_b(t))$. The physical boundary [traction](../../../../../traction.md), whose outward normal is $-e_1$, is $-T(t)e_2$. Invert the monotone law $\tau$ to obtain $q_b$. The wave state emitted at boundary time $s$ is transported along

$$
\boxed{X_1=c(q_b(s))(t-s),\quad q(X_1,t)=q_b(s),\quad v(X_1,t)=-H(q_b(s)).}
$$

Ahead of the leading front $X_1=c(0)t$ the state is zero. Before [characteristic crossing](../../../../../characteristic-crossing.md), these equations determine the unique emission time $s$ for each disturbed point. The displacement itself is also determined, rather than just its derivatives:

$$
w(0,s)=-\int_0^s H(q_b(\zeta))\,d\zeta,\qquad
w(X_1,t)=w(0,s)+\{c(q_b(s))q_b(s)-H(q_b(s))\}(t-s).
$$

Differentiating the implicit emission relation verifies $w_{,X_1}=q_b(s)$ and $w_t=-H(q_b(s))$, so this is the complete pre-shock [simple wave](../../../../../simple-wave.md) solution.

Write $c_b(s)=c(q_b(s))$. The boundary-generated [characteristic curves](../../../../../characteristic-curve.md) lose invertibility when

$$
\partial_s X_1=\dot c_b(s)(t-s)-c_b(s)=0.
$$

Thus the [characteristic crossing in a boundary-generated elastic simple wave](../../../../../characteristic-crossing-in-a-boundary-generated-elastic-simple-wave.md) criterion is

$$
\boxed{\dot c_b(s)>0,\qquad
t_{\rm sh}=\inf_{\dot c_b>0}\left(s+\frac{c_b}{\dot c_b}\right),\qquad
X_{\rm sh}(s)=\frac{c_b^2}{\dot c_b}.}
$$

Here $\dot c_b=c'(q_b)T'/(\rho_0c_b^2)$. A smoothly increasing boundary [stress](../../../../../stress.md) therefore steepens into a [shock wave](../../../../../shock-wave.md) only when later states travel faster: $c'(q_b)T'>0$. Increasing [stress](../../../../../stress.md) alone is insufficient. For the compatible example with $h>0$ and $q_b>0$, $c'(q_b)=3hq_b/(\rho_0c_b)>0$, so a nonzero increasing ramp produces finite-time crossing. For $h=0$ all rays are parallel and no such shock forms. This criterion locates the first gradient singularity; subsequent discontinuous evolution additionally requires the jump conditions and an admissibility condition.

For a general vector [simple wave](../../../../../simple-wave.md), replace the pure-shear line by an integral curve

$$
\frac{dr}{da}=a_\alpha(r),\qquad
\frac{dv}{da}=-c_\alpha(r)a_\alpha(r).
$$

Substitution gives $a_t+c_\alpha(a)a_{,X_1}=0$, with the same emission construction and crossing criterion. Boundary [tractions](../../../../../traction.md) must lie on this one-family curve. Generic finite-amplitude quasi-transverse waves may contain longitudinal displacement; arbitrary vector boundary forcing need not generate a single [simple wave](../../../../../simple-wave.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
