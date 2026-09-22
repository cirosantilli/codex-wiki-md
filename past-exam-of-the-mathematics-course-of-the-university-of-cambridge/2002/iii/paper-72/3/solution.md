<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $Q=g^{ab}\chi_{,a}\chi_{,b}$ and $\mathcal L=p(\epsilon)+n(Q-\epsilon^2)/(2\epsilon)$. Vary $n,\epsilon,\chi$ independently, taking compactly supported variations. The multiplier variation is $\partial\mathcal L/\partial n=(Q-\epsilon^2)/(2\epsilon)=0$. With $u_a=\chi_{,a}/\epsilon$, it gives the unit [four-velocity](../../../../../four-velocity.md) condition $u^au_a=1$. The enthalpy variation is

$$
\frac{\partial\mathcal L}{\partial\epsilon}
=p'(\epsilon)-\frac{nQ}{2\epsilon^2}-\frac n2=0.
$$

Using $Q=\epsilon^2$ yields $p'(\epsilon)=n$. Finally,

$$
\delta_\chi S=\int\sqrt{-g}\,\frac n\epsilon\nabla^a\chi\,\nabla_a\delta\chi\,d^4x
=-\int\sqrt{-g}\,\nabla_a(nu^a)\delta\chi\,d^4x.
$$

The [integration by parts](../../../../../integration-by-parts.md) boundary term vanishes. Thus the three matter equations are

$$
\boxed{u^au_a=1,\qquad \frac{dp}{d\epsilon}=n,\qquad \nabla_a(nu^a)=0.}
$$

The last is [particle number conservation in a relativistic fluid](../../../../../particle-number-conservation-in-a-relativistic-fluid.md). Off shell $n,\epsilon$ are independent variational fields; on shell the thermodynamic relation ties them to the specified function $p(\epsilon)$.

For the [Hilbert stress-energy tensor](../../../../../hilbert-stress-energy-tensor.md), keep these matter fields fixed while varying the inverse metric. The volume variation is $\delta\sqrt{-g}=-\tfrac12\sqrt{-g}\,g_{ab}\delta g^{ab}$, and $\delta Q=\chi_{,a}\chi_{,b}\delta g^{ab}$. Therefore

$$
\delta_g S=\frac12\int\sqrt{-g}
\left(\frac n\epsilon\chi_{,a}\chi_{,b}-g_{ab}\mathcal L\right)\delta g^{ab}\,d^4x.
$$

On shell, $\mathcal L=p$ and $n\epsilon=\rho+p$. With signature $(+---)$,

$$
\boxed{T^{ab}=(\rho+p)u^au^b-pg^{ab}.}
$$

For variation of the covariant metric the same definition reads $\delta_gS=-\tfrac12\int\sqrt{-g}T^{ab}\delta g_{ab}\,d^4x$. In a local rest frame the tensor has entries $\operatorname{diag}(\rho,p,p,p)$, which checks both the energy density and pressure sign.

Define a derivative along the flow by $\dot F=u^a\nabla_aF$, and set $\theta=\nabla_au^a$, $a^b=u^a\nabla_au^b$. The number equation immediately gives $\dot n+n\theta=0$. The [specific enthalpy per particle](../../../../../specific-enthalpy-per-particle.md) relation and $dp=n\,d\epsilon$ give

$$
d\rho=d(n\epsilon-p)=\epsilon\,dn.
$$

Consequently the energy equation follows from the number equation: $\dot\rho=\epsilon\dot n=-(\rho+p)\theta$.

The velocity equation follows directly from the potential, rather than requiring an independent assumption about the fluid force. Since $\epsilon u_a=\nabla_a\chi$ and the connection has zero torsion, the [canonical vorticity of a relativistic fluid](../../../../../canonical-vorticity-of-a-relativistic-fluid.md) vanishes:

$$
\nabla_a(\epsilon u_b)-\nabla_b(\epsilon u_a)=0.
$$

Contract with $u^a$ and use $u^au_a=1$ and $u^a\nabla_bu_a=0$. This gives $\epsilon a_b=\nabla_b\epsilon-u_b\dot\epsilon$. Multiplication by $n$ and use of $\nabla_bp=n\nabla_b\epsilon$ produces the [relativistic Euler equation](../../../../../relativistic-euler-equation.md). The evolution system is therefore

$$
\boxed{\dot n=-n\theta,\qquad
\dot\rho=-(\rho+p)\theta,\qquad
\dot u^a=\frac{g^{ab}-u^au^b}{\rho+p}\nabla_bp.}
$$

It is equivalent to [stress-energy conservation](../../../../../stress-energy-conservation.md) together with number conservation, subject to the potential-flow restriction. The action describes an isentropic barotropic sector of a [perfect fluid in general relativity](../../../../../perfect-fluid-in-general-relativity.md); it does not provide general vortical or entropy-carrying fluid motions. The constraint on canonical vorticity is stronger than the Euler equation alone.

For the weak static metric, use $c=1$. To the retained order, $\sqrt{-g}=1+\phi$, $u^0=1-\phi+O(\phi^2,|\mathbf v|^2)$ and $u^i=v^i$. The correction to $u^0$ is required by normalization, even though its zeroth-order value is one. The relevant [Christoffel symbols](../../../../../christoffel-symbol.md) are

$$
\Gamma^0{}_{0i}=\Gamma^0{}_{i0}=\partial_i\phi+O(\phi\nabla\phi),\qquad
\Gamma^i{}_{00}=\partial_i\phi,
$$

with no spatial connection at this order. The cancellation $\sqrt{-g}\,u^0=1+O(\phi^2,|\mathbf v|^2)$ makes the leading number equation particularly simple:

$$
\partial_t n+\nabla\cdot(n\mathbf v)=0.
$$

The corresponding leading energy transport equation is $\partial_t\rho+\mathbf v\cdot\nabla\rho+(\rho+p)\nabla\cdot\mathbf v=0$. The spatial Euler equation contains the gravitational acceleration $-\nabla\phi$ and pressure force $-\nabla p/(\rho+p)$. In a strict first-order expansion, convective velocity acceleration and products of the small quantities are discarded.

To exhibit a fully linear system, perturb a homogeneous rest state: $n=n_0+\delta n$, $\rho=\rho_0+\delta\rho$, $p=p_0+\delta p$, and $\epsilon=\epsilon_0+\delta\epsilon$, with the perturbations, $\mathbf v$ and $\phi$ all first order. Let $w_0=\rho_0+p_0=n_0\epsilon_0$. The [weak-field slow-motion equations for a relativistic fluid](../../../../../weak-field-slow-motion-equations-for-a-relativistic-fluid.md) are

$$
\boxed{\partial_t\delta n+n_0\nabla\cdot\mathbf v=0,\qquad
\partial_t\delta\rho+w_0\nabla\cdot\mathbf v=0,\qquad
\partial_t\mathbf v=-\nabla\phi-\frac1{w_0}\nabla\delta p.}
$$

The equation of state gives $\delta\rho=\epsilon_0\delta n$ and $\delta p=n_0\delta\epsilon$. Where $p''(\epsilon_0)\ne0$, it also gives the [barotropic relativistic sound speed](../../../../../barotropic-relativistic-sound-speed.md)

$$
\delta p=c_s^2\delta\rho,\qquad
c_s^2=\left.\frac{dp}{d\rho}\right|_0
=\frac{n_0}{\epsilon_0p''(\epsilon_0)}.
$$

Without this invertibility, the primitive conservation equations remain valid and this sound-speed parametrization must not be used.

The potential furnishes a further check on the pressure and gravity signs. Write $\chi=\epsilon_0t+\delta\chi$. Its time and spatial components imply

$$
\partial_t\delta\chi=\delta\epsilon+\epsilon_0\phi,\qquad
\mathbf v=-\frac{\nabla\delta\chi}{\epsilon_0}.
$$

Their compatibility reproduces the linear Euler equation. Pressure gradients oppose gravitational acceleration, and hydrostatic balance is $\nabla\delta p=-w_0\nabla\phi$. Combining the energy and Euler equations gives the forced acoustic equation

$$
\boxed{\partial_t^2\delta\rho-c_s^2\nabla^2\delta\rho=w_0\nabla^2\phi.}
$$

For positive $c_s^2$, disturbances propagate as sound waves; the prescribed potential supplies a static forcing. A nonrelativistic equation of state gives $p\ll\rho\simeq mn$, $\epsilon\simeq m$, and reduces the inertia $\rho+p$ to mass density, recovering the ordinary linearized continuity and Euler equations. Slow velocity alone does not justify dropping $p$ from the inertia of a relativistically hot fluid. The given metric supplies an external gravitational potential; the matter action by itself supplies no Poisson equation for it.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
