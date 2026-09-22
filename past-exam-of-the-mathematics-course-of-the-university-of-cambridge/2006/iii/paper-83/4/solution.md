<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $z>0$ measure height from the lower edge and $y>0$ distance from one face of the vertical plate. Use the steady [Boussinesq approximation](../../../../../boussinesq-approximation.md), homogeneous isotropic [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) $K$, reference fluid [mass density](../../../../../density.md) $\rho_0$, [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu$, [thermal expansion coefficient](../../../../../thermal-expansion-coefficient.md) $\alpha$, effective [thermal conductivity](../../../../../thermal-conductivity.md) $k_e$ and liquid volumetric [heat capacity](../../../../../heat-capacity.md) $C_f=\rho_0c_f$. Define $B=\rho_0g\alpha K/\mu$ and $\kappa=k_e/C_f$, consistently with the thermal convention used above. Write $\theta=T-T_a$, where $T_a$ is the uniform ambient [temperature](../../../../../temperature.md).

Interpret $F$ as uniform wall heat-flux [density](../../../../../density.md): a plate segment of height $dz$ inputs heat $F\,dz$ per unit horizontal span. The cumulative heat input up to height $z$ is therefore $Fz$. If $F$ instead denotes the sum of flux densities into two identically heated faces, replace it by $F/2$ in each face formula before summing. A specification only of total power per span, without its distribution in height, would not determine this uniformly heated-wall problem. We calculate one heated face; identical heating on both faces doubles the integrated fluxes.

Away from the leading edge, suppose the [boundary layer](../../../../../boundary-layer.md) is slender, $\delta(z)\ll z$, and porous inertia and longitudinal heat conduction are negligible. Lateral [pressure](../../../../../pressure.md) adjustment leaves the vertical [Darcy velocity](../../../../../darcy-velocity.md) proportional to [buoyancy](../../../../../buoyancy.md):

$$
w=B\theta,\qquad v_y+w_z=0,\qquad
v\theta_y+w\theta_z=\kappa\theta_{yy}.
$$

At the plate, $v=0$ and $-k_e\theta_y=F$; in the far field $w,\theta\to0$. [Darcy law](../../../../../darcy-law.md) permits tangential discharge at an impermeable plate, so imposing a further no-slip condition $w=0$ would be inappropriate in this leading porous model.

Balance $\theta\sim F\delta/k_e$, $w\sim B\theta$ and $w\theta/z\sim\kappa\theta/\delta^2$ to obtain

$$
\boxed{\delta(z)=\left(\frac{\kappa k_e z}{BF}\right)^{1/3},\quad
\theta\sim\frac{F\delta}{k_e}\propto z^{1/3},\quad w\propto z^{1/3}.}
$$

Thus the warmed layer thickens and accelerates upward. Define a [streamfunction](../../../../../stream-function.md) by $w=\psi_y$, $v=-\psi_z$ and set

$$
\eta=\frac y\delta,\qquad
\psi=\frac{\kappa z}{\delta}f(\eta),\qquad
w=\frac{\kappa z}{\delta^2}f'(\eta),\qquad
\theta=\frac{F\delta}{k_e}f'(\eta).
$$

The last two expressions agree because $\delta^3=\kappa k_e z/(BF)$. Differentiation gives $v=-(\kappa/3\delta)(2f-\eta f')$. Substituting in the thermal equation leaves the single nonlinear equation for the [uniformly heated vertical plate in a porous medium](../../../../../uniformly-heated-vertical-plate-in-a-porous-medium.md):

$$
\boxed{f'''+\frac23ff''-\frac13(f')^2=0,\qquad
f(0)=0,\quad f''(0)=-1,\quad f'(\infty)=0.}
$$

The first condition is impermeability; the second fixes the wall heat flux; the third fixes ambient [temperature](../../../../../temperature.md) and vertical [velocity](../../../../../velocity.md). Seek the positive-temperature branch with $f'\geq0$ and finite $f(\infty)$. Decay also gives $f''(\infty)=0$. The far-field transverse inflow need not vanish: $v_\infty=-(2\kappa/3\delta)f(\infty)$ supplies the increasing discharge.

An approximate solution can be obtained without a numerical shooting calculation. Integrate the [differential equation](../../../../../differential-equation-split.md) over $0<\eta<\infty$. The [boundary conditions](../../../../../boundary-condition.md) and [integration by parts](../../../../../integration-by-parts.md) give

$$
0=[f'']_0^\infty+\frac23[ff']_0^\infty-\int_0^\infty(f')^2d\eta
=1-\int_0^\infty(f')^2d\eta.
$$

Thus the exact thermal budget is $\int_0^\infty(f')^2d\eta=1$. Assume an exponential thermal shape, $f=C(1-e^{-\eta/d})$. The wall [derivative](../../../../../derivative.md) requires $C/d^2=1$, and the [integral](../../../../../integral.md) condition requires $C^2/(2d)=1$. Hence $d=2^{1/3}$, $C=2^{2/3}$ and the [integral exponential profile for porous wall convection](../../../../../integral-exponential-profile-for-porous-wall-convection.md) is

$$
\boxed{f(\eta)\simeq2^{2/3}(1-e^{-\eta/2^{1/3}}),\qquad
\theta(y,z)\simeq\frac{2^{1/3}F\delta}{k_e}e^{-y/(2^{1/3}\delta)}.}
$$

It satisfies all [boundary conditions](../../../../../boundary-condition.md), has positive decaying [temperature](../../../../../temperature.md), and matches the exact integrated heat budget. It is an [integral](../../../../../integral.md) approximation, not an exact pointwise solution of the [differential equation](../../../../../differential-equation-split.md); its mass-flux coefficient should be read accordingly.

Define the volume discharge, kinematic Darcy [momentum flux](../../../../../momentum-flux.md) and [buoyancy flux](../../../../../buoyancy-flux.md) per horizontal span by

$$
Q(z)=\int_0^\infty w\,dy,\qquad
\mathcal M(z)=\int_0^\infty w^2\,dy,\qquad
\mathcal B(z)=g\alpha\int_0^\infty w\theta\,dy.
$$

With these standard discharge conventions the [mass flux](../../../../../mass-flux.md) is $\dot m=\rho_0Q$. Their similarity expressions are

$$
Q=\frac{\kappa z}{\delta}f(\infty),\qquad
\mathcal M=\frac{\kappa^2z^2}{\delta^3}\int_0^\infty(f')^2d\eta,\qquad
\mathcal B=\frac{g\alpha}{B}\mathcal M.
$$

The [integral](../../../../../integral.md) identity evaluates two of them exactly:

$$
\boxed{\mathcal M(z)=\frac{B\kappa Fz}{k_e}=\frac{BFz}{C_f},\qquad
\mathcal B(z)=\frac{g\alpha\kappa Fz}{k_e}=\frac{g\alpha Fz}{C_f}.}
$$

Equivalently $C_f\int w\theta\,dy=Fz$: all the heat supplied below height $z$ is carried upward through that section. Although these fluxes are exact within the boundary-layer equations, porous drag means that the [momentum flux](../../../../../momentum-flux.md) itself is not conserved with height.

The approximate [mass flux](../../../../../mass-flux.md) is

$$
\boxed{\dot m(z)\simeq2^{2/3}\rho_0\frac{\kappa z}{\delta(z)}
=2^{2/3}\rho_0\kappa^{2/3}\left(\frac{BF}{k_e}\right)^{1/3}z^{2/3}.}
$$

For clarity, if “[momentum flux](../../../../../momentum-flux.md)” means actual pore-fluid momentum rather than the commonly quoted kinematic Darcy diagnostic, constant [porosity](../../../../../porosity.md) $\phi$ and pore speed $w/\phi$ give $\dot P=(\rho_0/\phi)\mathcal M$. The [mass flux](../../../../../mass-flux.md) remains $\rho_0Q$ because $w$ already denotes discharge per bulk area. Stating both prevents an implicit [porosity](../../../../../porosity.md) error. Validity also requires $\alpha\theta\ll1$ and a sufficiently slender, low-inertia porous [boundary layer](../../../../../boundary-layer.md); the approximation is not the immediate leading-edge conduction field.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
