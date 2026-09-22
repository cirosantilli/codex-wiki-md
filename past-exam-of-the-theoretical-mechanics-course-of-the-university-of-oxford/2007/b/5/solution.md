<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [material volume](../../../../material-volume.md), [mass conservation](../../../../mass-conservation.md) is $d\int_{V(t)}\rho\,dV/dt=0$. The transport theorem and arbitrariness of that volume give $\boxed{\rho_t+\nabla\cdot(\rho u)=0}$. [Balance of linear momentum](../../../../balance-of-linear-momentum.md) includes the [pressure](../../../../pressure-split.md) [traction](../../../../traction.md) and [body force](../../../../body-force.md):

$$
\frac d{dt}\int_{V(t)}\rho u\,dV=-\int_{\partial V(t)}pn\,dS+\int_{V(t)}\rho g\,dV.
$$

Apply transport, the [divergence theorem](../../../../divergence-theorem.md) and the mass equation to obtain

$$
\boxed{u_t+(u\cdot\nabla)u=-\frac1\rho\nabla p+g.}
$$

For small [perturbations](../../../../perturbation.md) of the uniform resting barotropic state, write $\rho=\rho_0+\rho'$, $p=p_0+c_0^2\rho'+\cdots$. Linearized mass and momentum are

$$
\rho'_t+\rho_0\nabla\cdot u=0,\qquad
u_t=-\frac{c_0^2}{\rho_0}\nabla\rho',\qquad\boxed{c_0^2=P'(\rho_0)>0.}
$$

Taking the [curl](../../../../curl.md) shows that initially vanishing [vorticity](../../../../vorticity-split.md) remains zero, so the acoustic [velocity](../../../../velocity.md) has a potential $u=\nabla\phi$. Integrating momentum, using the [additive freedom of a velocity potential](../../../../additive-freedom-of-a-velocity-potential.md) to remove the spatially constant integration term, gives $\rho'=-(\rho_0/c_0^2)\phi_t$. Continuity now yields $\boxed{\phi_{tt}=c_0^2\nabla^2\phi}$.

For [spherical symmetry](../../../../spherical-symmetry.md), set $\phi=e^{-i\omega t}F(r)$ and $k=\omega/c_0$. The radial equation is $(r^2F')'+k^2r^2F=0$, or $(rF)''+k^2(rF)=0$. Hence

$$
\boxed{\phi=\frac{e^{-i\omega t}}r[A\cos kr+B\sin kr].}
$$

Rigid boundaries require radial [velocity](../../../../velocity.md) $F'=0$ at both radii. A form automatically satisfying the condition at $a$ is

$$
F(r)=\frac C r\left[\cos k(r-a)+\frac1{ka}\sin k(r-a)\right].
$$

At $b$, the condition $b(rF)'-(rF)=0$ becomes

$$
k(b-a)\cos k(b-a)-(1+k^2ab)\sin k(b-a)=0.
$$

Therefore the nonzero oscillatory eigenfrequencies obey

$$
\boxed{(1+k^2ab)\tan k(b-a)=k(b-a),\qquad\omega=kc_0.}
$$

The undivided [sine](../../../../sine.md)-[cosine](../../../../cosine.md) form avoids artificial issues from dividing by a [cosine](../../../../cosine.md). The formal $k=0$ root is the spatially constant zero-frequency potential [additive freedom of a velocity potential](../../../../additive-freedom-of-a-velocity-potential.md), not a propagating acoustic oscillation. This is the [radial acoustic spectrum between rigid concentric spheres](../../../../radial-acoustic-spectrum-between-rigid-concentric-spheres.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
