<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the flat-surface [Boussinesq approximation](../../../../../boussinesq-approximation.md), with small thermal expansion, constant properties, negligible surface deformation, and constant surface tension. The top is impermeable and shear-free, while the solid walls are no-slip. Temperature-dependent surface tension would introduce a separate [Marangoni stress](../../../../../marangoni-effect.md), which is not included in this buoyancy-driven model. The stated time scale requires $\kappa$ to mean [thermal diffusivity](../../../../../thermal-diffusivity.md); if the material property given is a dimensional [thermal conductivity](../../../../../thermal-conductivity.md) $k$, use $\kappa=k/(\rho_0c_p)$.

Take $z$ positive downwards and define the nondimensional [streamfunction](../../../../../stream-function.md) by $u=\psi_z$, $w=-\psi_x$. [Velocity](../../../../../velocity.md) is scaled by $\kappa/L$, [streamfunction](../../../../../stream-function.md) by $\kappa$, and [temperature](../../../../../temperature.md) is measured from the cold-end surface value. Define the [Prandtl number](../../../../../prandtl-number.md) and horizontal-length [Rayleigh number](../../../../../rayleigh-number.md) by

$$
\operatorname{Pr}=\frac\nu\kappa,\qquad
\operatorname{Ra}=\frac{g\alpha_T\Delta T L^3}{\nu\kappa},
$$

where $\alpha_T$ is the [thermal expansion coefficient](../../../../../thermal-expansion-coefficient.md). Put $J(\psi,f)=\psi_zf_x-\psi_xf_z$, and let $\nabla^2=\partial_x^2+\partial_z^2$. Taking the curl of the [Boussinesq equations](../../../../../boussinesq-equations.md) eliminates [pressure](../../../../../pressure.md) and gives the full nonlinear vorticity-temperature system

$$
\boxed{\operatorname{Pr}^{-1}\left[\partial_t\nabla^2\psi+J(\psi,\nabla^2\psi)\right]
=\nabla^4\psi+\operatorname{Ra}T_x,\qquad
T_t+J(\psi,T)=\nabla^2T.}
$$

The [buoyancy](../../../../../buoyancy.md) sign follows from the downward coordinate: warmer fluid has body acceleration $-g\alpha_T\Delta T\,T\mathbf e_z$.

Choose the same [streamfunction](../../../../../stream-function.md) constant, zero, on the connected boundary. The mechanical and thermal boundary conditions are

$$
\begin{array}{c|c|c}
\text{boundary}&\text{velocity conditions}&\text{temperature condition}\\\hline
z=0&\psi=0,\quad\psi_{zz}-\psi_{xx}=0&T=x\\
z=\epsilon&\psi=0,\quad\psi_z=0&T_z=0\\
x=0,1&\psi=0,\quad\psi_x=0&T_x=0.
\end{array}
$$

The upper [stress-free boundary condition](../../../../../stress-free-boundary-condition.md) reduces to $\psi_{zz}=0$, since $\psi=0$ there already gives $\psi_{xx}=0$. An arbitrary additive constant in $T$ changes only the reference hydrostatic [pressure](../../../../../pressure.md).

In steady [infinite-Prandtl-number convection](../../../../../infinite-prandtl-number-convection.md), momentum inertia disappears but thermal advection remains:

$$
\boxed{\nabla^4\psi=-\operatorname{Ra}T_x,\qquad
J(\psi,T)=\nabla^2T.}
$$

For a shallow lake, with fixed $\operatorname{Ra}$ as $\epsilon\to0$, the leading interior [temperature](../../../../../temperature.md) is $T_0=x$. This is an outer solution: it does not satisfy the insulated sidewall derivative right at $x=0,1$. The leading global conductive solution, which resolves those end regions, is

$$
T_c(x,z)=\frac12-\frac4{\pi^2}\sum_{\substack{n\geq1\\n\ {
m odd}}}
\frac{\cos(n\pi x)}{n^2}
\frac{\cosh[n\pi(\epsilon-z)]}{\cosh(n\pi\epsilon)}.
$$

It is harmonic, has $T_c(x,0)=x$, and satisfies the insulated sides and bottom. Away from sidewall layers of horizontal width $O(\epsilon)$ it reduces to $x$ with exponentially small end corrections. These layers also turn the flow and enforce the sidewall [no-slip boundary condition](../../../../../no-slip-boundary-condition.md).

In the shallow interior the dominant momentum derivatives are vertical, so $\psi_{0,zzzz}=-\operatorname{Ra}$. Integrating with the surface and bottom conditions gives the [shallow horizontal convection with an insulated bottom](../../../../../shallow-horizontal-convection-with-an-insulated-bottom.md) solution, with $y=z/\epsilon$:

$$
\boxed{T_0=x,\qquad
\psi_0=-\frac{\operatorname{Ra}\epsilon^4}{48}y(1-y)^2(2y+1),\qquad
u_0=-\frac{\operatorname{Ra}\epsilon^3}{48}(8y^3-9y^2+1),\quad w_0=0.}
$$

Surface flow is toward the colder end, with a deeper return flow. The depth-integrated [volume flux](../../../../../volumetric-flow-rate.md) is zero because $\psi_0(\epsilon)=\psi_0(0)=0$. The bulk expressions apply away from the turning regions, not unchanged on the vertical walls. A useful small-advection condition in the end layers is $\operatorname{Ra}\epsilon^4\ll1$, automatic for fixed Rayleigh number in the stated thin limit.

The [heat flux](../../../../../heat-flux-density.md) in these units is $\mathbf q=(uT-T_x,wT-T_z)$. For the leading bulk [temperature](../../../../../temperature.md), the horizontal transport through a vertical section per unit out-of-plane width is

$$
\mathcal H_x=\int_0^\epsilon(u_0T_0-T_{0,x})\,dz
=x[\psi_0(\epsilon)-\psi_0(0)]-\epsilon,
\qquad\boxed{\mathcal H_x=-\epsilon.}
$$

Thus leading advective horizontal transport vanishes: both layers have the same [temperature](../../../../../temperature.md) at a given $x$, and their opposing volume fluxes cancel. The leading conductive transport is from the hot end toward the cold end. In dimensional form it is $-\rho_0c_p\kappa\Delta T\epsilon=-k\Delta T\epsilon$ per unit width. Heat enters through the warmer portion of the maintained upper surface and leaves through its colder portion, with the conductive end adjustments particularly important near the two insulated sidewalls. It cannot enter through the insulated sides or bottom.

For the [advection correction in shallow horizontal convection](../../../../../advection-correction-in-shallow-horizontal-convection.md), set $T=x+\Theta(z)$ in the bulk. Since $w_0=0$ and $T_x=1$, the steady [heat equation](../../../../../heat-equation.md) gives $\Theta_{zz}=u_0=\psi_{0,z}$. The conditions $\Theta(0)=0$ and $\Theta_z(\epsilon)=0$ imply $\Theta_z=\psi_0$ and hence

$$
\boxed{\Theta(z)=-\frac{\operatorname{Ra}\epsilon^5}{48}
\left(\frac25y^5-\frac34y^4+\frac12y^2\right).}
$$

For example the bottom bulk [temperature](../../../../../temperature.md) is $T(x,\epsilon)=x-\operatorname{Ra}\epsilon^5/320$. The correction makes the returning deeper fluid slightly colder. Its horizontal advective heat transport is

$$
\int_0^\epsilon u_0\Theta\,dz
=\int_0^\epsilon\psi_{0,z}\Theta\,dz
=-\int_0^\epsilon\psi_0^2dz
=-\frac{19\operatorname{Ra}^2\epsilon^9}{1451520}.
$$

Thus the transport including this bulk correction is $\boxed{\mathcal H_x=-\epsilon-19\operatorname{Ra}^2\epsilon^9/1451520}$, both terms directed toward the colder end.

Vertical transport must distinguish local flux from net transport. In the leading interior $w_0=T_{0,z}=0$, whereas the [temperature](../../../../../temperature.md) correction gives a local downward conductive flux $q_z=-\Theta_z=-\psi_0>0$. The end circulation gives an upward advective transport: with impermeable sidewalls and $T_0\simeq x$, integration by parts gives $\int_0^1wT_0dx=-\int_0^1x\psi_x\,dx=\int_0^1\psi\,dx\simeq\psi_0(z)<0$. It compensates that downward conduction. More generally, steady heat conservation and insulated sides give $d[\int_0^1q_zdx]/dz=0$, and the insulated impermeable bottom sets the constant to zero. Therefore

$$
\boxed{\int_0^1q_z(x,z)dx=0\quad\text{at every depth}.}
$$

There is no net vertical heat transport through the lake, despite its local recirculating [heat flux](../../../../../heat-flux-density.md) and its nonzero horizontal heat transport.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
