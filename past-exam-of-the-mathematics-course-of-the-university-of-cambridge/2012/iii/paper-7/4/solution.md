<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**A kinetic model of a dilute gas.** In the [Boltzmann equation](../../../../../boltzmann-equation.md), $f(t,x,v)\geq0$ is the particle number density in [phase space](../../../../../phase-space.md), so $f\,dx\,dv$ counts particles near position $x$ and velocity $v$. For unit particle mass in three dimensions, without external forces, the nonlinear equation is

$$
\boxed{\partial_t f+v\cdot\nabla_xf=Q(f,f).}
$$

The left side is the [free transport equation](../../../../../free-transport-equation.md). The quadratic right side describes binary [elastic collisions](../../../../../elastic-collision.md) occurring locally in space. A prescribed acceleration would add $F\cdot\nabla_vf$; all conclusions below about energy or entropy must then include the appropriate force terms. Assume enough smoothness, velocity decay and finite moments to justify the calculations, and either periodic space or decay that removes spatial boundary fluxes. These are assumptions on a classical solution, not a general existence theorem.

The dilute-gas approximation neglects simultaneous many-body collisions and treats the interaction region as small relative to macroscopic spatial scales. [Molecular chaos for the Boltzmann equation](../../../../../molecular-chaos-for-the-boltzmann-equation.md) factorizes the distribution of two incoming particles as $f(v)f(v_*)$. It applies to incoming collision pairs; it does not assert that an interacting many-particle system stays exactly independent. This approximation closes the equation at the one-particle level and explains its nonlinearity.

**Collision geometry and the gain-loss operator.** Let $g=v-v_*$ and $n\in S^2$. A useful parametrization of an equal-mass [elastic collision](../../../../../elastic-collision.md) is

$$
v'=v-(g\cdot n)n,\qquad
v_*'=v_*+(g\cdot n)n.
$$

The center velocity $(v+v_*)/2$ is unchanged and the relative velocity is reflected in the plane normal to $n$. Consequently

$$
v'+v_*'=v+v_*,
\qquad |v'|^2+|v_*'|^2=|v|^2+|v_*|^2.
$$

The fixed-$n$ pre/post-collision transformation is an involutive orthogonal map of $\mathbb R^6$, so it preserves $dv\,dv_*$. Take a nonnegative collision kernel $B(g,n)$ invariant under interchange of particles and reversal of the collision; for example $B=B(|g|,|\widehat g\cdot n|)$. The [nonlinear Boltzmann collision operator](../../../../../nonlinear-boltzmann-collision-operator.md) is

$$
Q(f,f)(v)=
\int_{\mathbb R^3}\int_{S^2}
B(g,n)\bigl[f(v')f(v_*')-f(v)f(v_*)\bigr]\,dn\,dv_*.
$$

Any convention about counting $n$ and $-n$ is absorbed in $B$. For a [hard-sphere gas](../../../../../hard-sphere-gas.md), this reflection parametrization has $B=c|g\cdot n|$, with a positive constant determined by the sphere size and counting convention. [Maxwell molecule collision operators](../../../../../maxwell-molecule-collision-operator.md) instead have a collision frequency independent of $|g|$ after angular integration. A [Grad angular cutoff](../../../../../grad-angular-cutoff.md) requires a finite angular integral; singular kernels need additional cancellation analysis and cannot be handled by every elementary gain-loss argument below.

Writing $Q=Q^+-\nu_f f$, where

$$
Q^+(f,f)=\int Bf'f_*'\,dn\,dv_*,
\qquad
\nu_f(v)=\int Bf_*\,dn\,dv_*,
$$

makes the physical meaning clear: gain into velocity $v$ competes with loss out of $v$. Along a free [characteristic curve](../../../../../characteristic-curve.md), put $F(t)=f(t,x+tv,v)$. Then $F'+\nu_f(t,x+tv,v)F=Q^+(t,x+tv,v)$. The [integrating factor](../../../../../integrating-factor.md) gives

$$
\begin{aligned}
f(t,x+tv,v)
={}&f_{\mathrm{in}}(x,v)
\exp\left[-\int_0^t\nu_f(s,x+sv,v)\,ds\right]\\
&+\int_0^t Q^+(f,f)(s,x+sv,v)
\exp\left[-\int_s^t\nu_f(r,x+rv,v)\,dr\right]ds.
\end{aligned}
$$

For finite collision integrals, this representation shows preservation of nonnegativity. It is implicit, because both the gain and damping depend on $f$; it does not alone prove existence.

**The weak collision identity and conserved quantities.** The [weak Boltzmann collision identity](../../../../../weak-boltzmann-collision-identity.md) follows from particle interchange and the measure-preserving pre/post-collision substitution: it gives, for a velocity test function $\psi$,

$$
\boxed{\int Q(f,f)\psi(v)\,dv
=\frac12\int Bff_*
[\psi(v')+\psi(v_*')-\psi(v)-\psi(v_*)]\,dv\,dv_*\,dn.}
$$

The factor $1/2$ comes from averaging the two particle labels. Equivalently the right side is

$$
\frac14\int B(f'f_*'-ff_*)
[\psi(v)+\psi(v_*)-\psi(v')-\psi(v_*')]\,dv\,dv_*\,dn.
$$

A [collision invariant](../../../../../collision-invariant.md) has zero square-bracketed change in every collision. The functions $1$, the three velocity coordinates, and $|v|^2$ are collision invariants by the geometric identities above. Hence the collision term conserves particle number, [momentum](../../../../../momentum.md) and [kinetic energy](../../../../../kinetic-energy.md) locally in position. Multiplying the full [Boltzmann equation](../../../../../boltzmann-equation.md) by these functions and integrating in velocity gives local [conservation laws](../../../../../conservation-law.md); integrating in space yields constant total mass, momentum and energy when boundary fluxes vanish.

The smooth [collision invariants](../../../../../collision-invariant.md) are exactly their linear span, provided the kernel allows all scattering directions. Here is a direct proof. If $\psi(v)+\psi(v_*)$ is unchanged by every collision, then for fixed center $c$ and relative radius $r$, the sum $\psi(c+r\omega)+\psi(c-r\omega)$ is independent of the unit vector $\omega$. Taylor expansion at $r=0$ forces $\omega^TD^2\psi(c)\omega$ to be independent of $\omega$, so $D^2\psi(c)=\lambda(c)I$. Mixed derivatives vanish. Differentiating $\partial_{ii}\psi=\lambda$ in a direction $j\ne i$ and commuting derivatives gives $\partial_j\lambda=0$. Thus $\lambda$ is constant and

$$
\boxed{\psi(v)=a+b\cdot v+c|v|^2.}
$$

This proof can be read for $C^3$ invariants; weaker regularity is handled distributionally. The multidimensional scattering hypothesis matters: in one dimension equal-mass elastic collisions only exchange the two velocities, and every function is then a collision invariant.

**Entropy dissipation and the H theorem.** Define the [Boltzmann H functional](../../../../../boltzmann-h-functional.md) $H(f)=\int f\log f\,dx\,dv$, with $0\log0=0$. The physical kinetic [entropy](../../../../../entropy.md) has the opposite sign, up to constants and the particle-number normalization. Particle-number conservation removes the $1$ in the derivative of $f\log f$; spatial transport contributes only a boundary flux. With $A=f'f_*'$ and $B_0=ff_*$, the symmetrized weak collision identity gives

$$
\boxed{\frac{dH}{dt}=-\int D(f)(x)\,dx,\qquad
D(f)=\frac14\int B(g,n)(A-B_0)\log\frac A{B_0}\,dv\,dv_*\,dn\geq0.}
$$

The sign follows from monotonicity of the logarithm: $(a-b)(\log a-\log b)\geq0$. Zeros are treated by the usual extended nonnegative limit. This is the [Boltzmann H theorem](../../../../../h-theorem.md) for the present kernel normalization, and $D$ is the [Boltzmann entropy dissipation](../../../../../boltzmann-entropy-dissipation.md).

For a positive smooth $f$ and a kernel positive on all collision directions, equality $D(f)=0$ requires $f'f_*'=ff_*$ in every collision, so $\log f$ is a [collision invariant](../../../../../collision-invariant.md). Finite velocity mass then forces a negative quadratic coefficient and gives a [local Maxwellian](../../../../../local-maxwellian.md):

$$
\boxed{M_{\rho,u,\theta}(v)
=\frac{\rho}{(2\pi\theta)^{3/2}}
\exp\left(-\frac{|v-u|^2}{2\theta}\right),\quad
\rho>0,\quad\theta>0.}
$$

Here $\rho$ is number density, $u$ is mean [velocity](../../../../../velocity.md), and $\theta$ is the temperature expressed in velocity-squared units, $k_BT/m$. Completing the square proves the formula; conservation of [momentum](../../../../../momentum.md) and [kinetic energy](../../../../../kinetic-energy.md) makes $MM_*=M'M_*'$, so $Q(M,M)=0$. Vacuum is another collision equilibrium.

A [local Maxwellian](../../../../../local-maxwellian.md) annihilates the collision term at each position, but it need not solve the transport part. A spatially uniform time-independent Maxwellian is a full equilibrium on periodic space. On all of $\mathbb R^3_x$ it has infinite total mass unless it is vacuum. Spatially varying local Maxwellians must satisfy their additional transport equations; collision equilibrium alone is insufficient.

For the [spatially homogeneous Boltzmann equation](../../../../../spatially-homogeneous-boltzmann-equation.md), a Maxwellian with the same mass, mean velocity and energy is selected by these invariants. The [relative entropy](../../../../../kullback-leibler-divergence.md) $\int f\log(f/M)\,dv$ is nonnegative. Indeed, writing $f=Mr$ and using equal mass gives

$$
\int f\log(f/M)\,dv
=\int M(r\log r-r+1)\,dv\geq0.
$$

Moreover $\log M$ is a collision invariant, so the derivative of this relative entropy is $-D(f)$. Thus $M$ minimizes $H$ at fixed conserved moments. Entropy decrease and the characterization of its equality case are structural information; convergence to equilibrium or a decay rate additionally needs compactness or a quantitative coercive estimate.

**Moment equations and fluid closure.** Let

$$
\rho=\int f\,dv,\quad
\rho u=\int vf\,dv,\quad
P=\int(v-u)\otimes(v-u)f\,dv,\quad
q=\frac12\int |v-u|^2(v-u)f\,dv .
$$

The tensor $P$ is the kinetic [pressure tensor](../../../../../pressure-tensor.md) and $q$ the kinetic [heat flux](../../../../../heat-flux-density.md). Put $e=(2\rho)^{-1}\int|v-u|^2f\,dv$. The collision invariants yield

$$
\begin{aligned}
&\partial_t\rho+\nabla_x\cdot(\rho u)=0,\\
&\partial_t(\rho u)+\nabla_x\cdot(\rho u\otimes u+P)=0,\\
&\partial_t E+\nabla_x\cdot(Eu+Pu+q)=0,
\qquad E=\tfrac12\rho|u|^2+\rho e.
\end{aligned}
$$

These identities are exact whenever the moments and derivatives are justified. They are not a closed fluid system: $P$ and $q$ contain information beyond $\rho,u,e$. For a [local Maxwellian](../../../../../local-maxwellian.md), Gaussian integration gives $P=\rho\theta I$, $q=0$ and $e=3\theta/2$. Substitution gives the compressible [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) for a monatomic ideal gas, with pressure $p=\rho\theta$ and ratio of specific heats $5/3$.

This connection is naturally organized by the [Knudsen number](../../../../../knudsen-number.md) $\varepsilon$, the ratio of the [mean free path](../../../../../mean-free-path.md) to a macroscopic length. In an appropriate fluid scaling the equation reads $\partial_tf+v\cdot\nabla_xf=\varepsilon^{-1}Q(f,f)$. Formally, as $\varepsilon\to0$, the dominant collision term imposes $Q(f,f)=0$, hence local Maxwellian form, and the conserved moments evolve by the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md). The first correction to a local Maxwellian produces viscous stress and thermal conduction, leading to [Navier-Stokes equations](../../../../../navier-stokes-equation.md) with a thermal equation. This is a formal [hydrodynamic limit of the Boltzmann equation](../../../../../hydrodynamic-limit-of-the-boltzmann-equation.md); a rigorous limit requires estimates, preparation of data and treatment of boundaries, and is not justified merely by inserting $\varepsilon=0$.

**Linearization and its dissipative structure.** Around a fixed positive Maxwellian $M$, write $f=M(1+h)$. The linearized collision operator on the relative perturbation is

$$
\mathcal Lh(v)=\int B(g,n)M(v_*)
[h(v')+h(v_*')-h(v)-h(v_*)]\,dv_*\,dn .
$$

This follows by expanding the two quadratic products to first order and using $MM_*=M'M_*'$. In the weighted [Hilbert space](../../../../../hilbert-space-split.md) with inner product $\langle h,k\rangle_M=\int Mhk\,dv$, collision symmetrization gives

$$
\boxed{-\langle h,\mathcal Lh\rangle_M
=\frac14\int B(g,n)MM_*
[h'+h_*'-h-h_*]^2\,dv\,dv_*\,dn\geq0.}
$$

This [dissipation form of the linearized Boltzmann operator](../../../../../dissipation-form-of-the-linearized-boltzmann-operator.md) and its corresponding polarized identity prove symmetry on a common domain where the integrals converge. Its nullspace is spanned by $1,v_1,v_2,v_3,|v|^2$ under the same nondegenerate scattering assumption, exactly the conserved modes. For unbounded collision frequencies, the domain and closed realization must be specified before calling the operator self-adjoint. A [spectral gap](../../../../../spectral-gap.md) on the orthogonal complement is an additional theorem depending on the collision kernel; it does not follow just from the displayed nonnegative quadratic form.

**Analytic scope and irreversibility.** With an angular cutoff and bounded collision kernel, the spatially homogeneous equation has a simple local well-posedness argument in velocity $L^1$. The pre/post-collision substitution gives $\|Q(f,g)\|_1\leq C\|f\|_1\|g\|_1$, so the quadratic map is locally Lipschitz. The [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) applied to the integral equation gives a local unique solution; gain-loss iteration preserves positivity. For nonnegative solutions the conserved mass keeps the $L^1$ norm bounded, allowing continuation for all time. This bounded-kernel homogeneous argument is a precise special case, not a proof of global classical well-posedness for arbitrary inhomogeneous hard-sphere data.

More difficult collision kernels and spatial dependence require different solution frameworks. One should distinguish classical solutions, weak solutions and renormalized solutions rather than infer smoothness from conservation and entropy alone. For instance, a [renormalized Boltzmann solution](../../../../../renormalized-boltzmann-solution.md) uses nonlinear bounded transforms $\beta(f)$ to make sense of collision and transport terms when their raw integrability is insufficient. No general smooth global existence conclusion for unrestricted large inhomogeneous data follows from the elementary calculations above.

Microscopic [elastic collision](../../../../../elastic-collision.md) dynamics are reversible, while the [Boltzmann H theorem](../../../../../h-theorem.md) selects a direction of increasing entropy. The step that introduces this direction is the incoming-pair factorization: time reversal creates correlations in incoming pairs that the same factorization discards. The [Boltzmann-Grad limit](../../../../../boltzmann-grad-limit.md) gives a route from a dilute many-particle gas to a kinetic equation by letting particle size shrink while keeping a finite mean free path. Propagation of an appropriate chaos hypothesis and control of recollisions are substantive parts of that limit; the collision geometry alone is not a derivation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
