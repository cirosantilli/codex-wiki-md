<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the steady slender-plume model implicit in the requested height-only similarity. Put $\theta=T-T_0$ and introduce permeability $K$, [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu=\rho_0\nu$, fluid heat capacity per volume $C_h=\rho_0c_p$, and effective transverse [thermal diffusivity](../../../../../thermal-diffusivity.md) $\kappa$. These material constants are needed to give dimensional fluxes. Take $u,w$ to be [Darcy velocities](../../../../../darcy-velocity.md), so the thermal transport coefficient for the steady equation is $\kappa=k_e/C_h$ when $k_e$ is the effective conductivity of the saturated medium.

The [Darcy law](../../../../../darcy-law.md) with gravity is

$$
u=-\frac K\mu p_x,\qquad w=-\frac K\mu(p_z+\rho g).
$$

The ambient is hydrostatic with $p_{a,z}=-\rho_0g$. A slender plume's pressure correction has vertical gradient smaller than the buoyancy term by the squared width-to-height ratio. Indeed, [incompressibility](../../../../../incompressible-flow.md) gives $u/w$ of order width/height, and the horizontal Darcy relation makes the pressure correction of order $\mu w\,\text{width}^2/(K\,\text{height})$. Its vertical derivative has the additional inverse-height factor. Thus the leading vertical Darcy balance is

$$
\boxed{w=\beta\theta,\qquad \beta=\frac{\rho_0g\alpha K}{\mu}=\frac{Kg\alpha}{\nu}.}
$$

The proportionality is to temperature excess $T-T_0$, not absolute $T$; the velocity vanishes in the unheated ambient. This is the local buoyancy/drag balance of a [porous thermal plume](../../../../../porous-thermal-plume.md), rather than a free-fluid inertial momentum balance.

The governing [continuity equation](../../../../../continuity-equation.md) and steady [advection-diffusion equation](../../../../../advection-diffusion-equation.md), with axial conduction neglected in the slender high-[Rayleigh number](../../../../../rayleigh-number.md) limit, are

$$
u_x+w_z=0,\qquad u\theta_x+w\theta_z=\kappa\theta_{xx},\qquad w=\beta\theta.
$$

Choose the [streamfunction](../../../../../stream-function.md) convention $u=-\psi_z$, $w=\psi_x$. It enforces continuity identically and gives

$$
\boxed{\theta=\frac{\psi_x}\beta,\qquad
\kappa\psi_{xxx}+\psi_z\psi_{xx}-\psi_x\psi_{xz}=0.}
$$

A change to the opposite streamfunction convention changes the sign of $\psi$, not the physical velocity or temperature.

The upward convected excess [heat flux](../../../../../heat-flux-density.md) per unit source length is

$$
\boxed{F_h=C_h\int_{-\infty}^{\infty}w\theta\,dx.}
$$

This is the quantity denoted $F$ in this question; it differs from Question 2's buoyancy-flux symbol. In conservative form the heat equation is $\partial_x(u\theta)+\partial_z(w\theta)=\kappa\theta_{xx}$. Integrate across the plume:

$$
\frac1{C_h}\frac{dF_h}{dz}=[\kappa\theta_x-u\theta]_{-\infty}^{\infty}=0.
$$

The temperature anomaly and its derivative vanish far from the plume; lateral entrainment brings in ambient-temperature fluid and thus no excess heat. There is no heat source or sink above the line source. Transverse conduction redistributes this heat without removing its total, while axial conduction is negligible in the stated approximation. In an unsteady plume a heat-storage term would have to be retained, so the convective flux alone would not in general be independent of height.

Let $\mathcal J=\beta F_h/C_h=\int w^2dx>0$. It is constant because $w=\beta\theta$. To obtain similarity exponents without guessing a profile, write the width as $\delta\propto z^a$ and central velocity as $W\propto z^b$. The fixed heat flux requires $W^2\delta$ constant, hence $2b+a=0$. Balancing vertical advection, including its continuity-required horizontal component, against transverse conduction gives $W\delta^2\propto\kappa z$, hence $b+2a=1$. Thus $a=2/3$ and $b=-1/3$, and the streamfunction scale $W\delta$ is proportional to $z^{1/3}$. A suitable **similarity form** is

$$
\boxed{\eta=\frac{x}{Bz^{2/3}},\qquad
\psi=Az^{1/3}f(\eta),\qquad
\theta=\frac A{\beta B}z^{-1/3}f'(\eta).}
$$

The [volume flux](../../../../../volumetric-flow-rate.md) per unit span is $Q=\psi(+\infty)-\psi(-\infty)$ and therefore grows as $z^{1/3}$; it tends to zero at the ideal source. Thus the zero-source-volume requirement fixes the absence of an additive source-length scale, not a finite temperature at the singular point.

Substitution into the streamfunction equation gives

$$
f'''+\frac{AB}{3\kappa}[ff''+(f')^2]=0.
$$

Choose the scale normalization $AB=6\kappa$ and $f(+\infty)=1$. Reflection symmetry makes $f$ odd, so the relevant conditions are $f(0)=0$, $f''(0)=0$, $f'(\infty)=0$, with finite $f(\infty)$; the heat input fixes the remaining dimensional scale. The **nonlinear similarity equation** becomes

$$
\boxed{f'''+2[ff''+(f')^2]=0.}
$$

Integrate once. Since $f',f''\to0$ in the ambient, the integration constant is zero, giving $f''+2ff'=0$. A second integration gives $f'+f^2=C$; the normalized far limit fixes $C=1$. Separation with $f(0)=0$ now yields the **complete positive-plume profile**

$$
\boxed{f(\eta)=\tanh\eta,\qquad f'(\eta)=\operatorname{sech}^2\eta.}
$$

It satisfies the symmetry and decay conditions; the solution of the first-order initial-value equation is unique. The physical heat strength is determined using $\int_{-\infty}^{\infty}\operatorname{sech}^4\eta\,d\eta=4/3$, obtained by substituting $t=\tanh\eta$:

$$
\mathcal J=\frac{A^2}B\frac43=\frac{48\kappa^2}{B^3},\qquad
B=\left(\frac{48\kappa^2}{\mathcal J}\right)^{1/3},\qquad A=\frac{6\kappa}B.
$$

Equivalently, define

$$
b(z)=\left(\frac{48\kappa^2z^2}{\mathcal J}\right)^{1/3},\qquad
W(z)=\left(\frac{3\mathcal J^2}{32\kappa z}\right)^{1/3}.
$$

The [hyperbolic-secant porous plume profile](../../../../../hyperbolic-secant-porous-plume-profile.md) and its velocity field are then

$$
\boxed{\begin{aligned}
\psi(x,z)&=Wb\tanh(x/b),\\
w(x,z)&=W\operatorname{sech}^2(x/b),\\
T(x,z)&=T_0+\frac W\beta\operatorname{sech}^2(x/b),\\
u(x,z)&=\frac{Wb}{3z}\left[2\frac xb\operatorname{sech}^2(x/b)-\tanh(x/b)\right].
\end{aligned}}
$$

In particular $Wb^2=6\kappa z$. The far horizontal velocities are inward, $u(\pm\infty,z)=\mp Wb/(3z)$, supplying the entrained ambient volume. They are consistent with $Q'=2Wb/(3z)$.

Finally use specific Darcy-flux moments, per unit source length, for the requested flux relationships. The [volume flux](../../../../../volumetric-flow-rate.md), kinematic [momentum flux](../../../../../momentum-flux.md) and [buoyancy flux](../../../../../buoyancy-flux.md) are

$$
\boxed{\begin{aligned}
Q(z)&=\int w\,dx=2Wb=(36\kappa\mathcal Jz)^{1/3},\\
M(z)&=\int w^2dx=\frac43W^2b=\mathcal J=\frac{\beta F_h}{C_h},\\
F_b(z)&=\int g\alpha\theta\,w\,dx
=\frac{g\alpha}{\beta}\mathcal J=\frac{g\alpha F_h}{C_h}.
\end{aligned}}
$$

Thus the physical [mass flux](../../../../../mass-flux.md) is $\rho_0Q(z)$, and the conventional density-weighted Darcy second moment is $\rho_0M$. If intrinsic pore-velocity momentum flux is required instead, a uniform porosity $\varphi$ gives $\rho_0M/\varphi$; keeping this convention distinct does not change the displayed Darcy moments. These are the [conserved momentum flux of a porous thermal plume](../../../../../conserved-momentum-flux-of-a-porous-thermal-plume.md) relationships. Constancy of $M$ follows here from proportionality of temperature and velocity plus heat conservation, not from ignoring the drag on the solid matrix in a total momentum balance.

The ideal source has zero limiting volume flux but divergent central speed and temperature. Consequently the [Boussinesq approximation](../../../../../boussinesq-approximation.md) and slender-plume limit describe the region outside a finite source, where $|\alpha\theta|\ll1$ and $b/z\ll1$. Indeed $Wz/\kappa=6(z/b)^2\gg1$ is the local high-Rayleigh condition. These limits improve downstream; they do not make the singular similarity field a literal finite-temperature solution at $x=z=0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 84](../../paper-84-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
