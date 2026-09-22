<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let the basic [temperature](../../../../../temperature.md) be $\overline T=T_* -\beta z$ with $\beta>0$, the density be $\rho_0$, gravitational acceleration be $-g\widehat{\mathbf z}$, and [thermal expansion coefficient](../../../../../thermal-expansion-coefficient.md) be $a_T$. Denote [kinematic viscosity](../../../../../kinematic-viscosity.md), [thermal diffusivity](../../../../../thermal-diffusivity.md) and [magnetic diffusivity](../../../../../magnetic-diffusivity.md) by $\nu,\kappa,\eta$. Write the dimensional magnetic perturbation as $\mathbf b_d$, the [temperature](../../../../../temperature.md) perturbation as $\theta_d$, and use constant permeability $\mu_0$. Linearizing the [Boussinesq equations](../../../../../boussinesq-equations.md) and the [resistive induction equation](../../../../../resistive-induction-equation.md) about the static state gives

$$
\begin{aligned}
\partial_t\mathbf u_d&=-\rho_0^{-1}\nabla P_d+ga_T\theta_d\widehat{\mathbf z}+\frac{B_0}{\mu_0\rho_0}(\mathbf c\cdot\nabla)\mathbf b_d+\nu\nabla^2\mathbf u_d,\\
\partial_t\mathbf b_d&=B_0(\mathbf c\cdot\nabla)\mathbf u_d+\eta\nabla^2\mathbf b_d,\\
\partial_t\theta_d&=\beta u_{d,z}+\kappa\nabla^2\theta_d,\qquad \nabla\cdot\mathbf u_d=\nabla\cdot\mathbf b_d=0.
\end{aligned}
$$

The [Lorentz force](../../../../../lorentz-force.md) identity is $(\nabla\times\mathbf b_d)\times B_0\mathbf c=B_0(\mathbf c\cdot\nabla)\mathbf b_d-\nabla(B_0\mathbf c\cdot\mathbf b_d)$. Its [gradient](../../../../../gradient.md) term is absorbed into $P_d$, the perturbation [magnetohydrodynamic total pressure](../../../../../magnetohydrodynamic-total-pressure.md). The [temperature](../../../../../temperature.md) source follows from $\mathbf u_d\cdot\nabla\overline T=-\beta u_{d,z}$.

Choose any reference length $d$, since no vertical boundaries are prescribed. Scale length by $d$, time by $d^2/\kappa$, [velocity](../../../../../velocity.md) by $\kappa/d$, [temperature](../../../../../temperature.md) perturbation by $\beta d$, magnetic perturbation by $B_0$, and total [pressure](../../../../../pressure.md) by $\rho_0\nu\kappa/d^2$. The dimensionless parameters are

$$
\boxed{\sigma=\frac\nu\kappa,\quad\zeta=\frac\eta\kappa,\quad R=\frac{ga_T\beta d^4}{\nu\kappa},\quad Q=\frac{B_0^2d^2}{\mu_0\rho_0\nu\eta}.}
$$

They are the [Prandtl number](../../../../../prandtl-number.md), magnetic-to-thermal diffusivity ratio, [Rayleigh number](../../../../../rayleigh-number.md), and [Chandrasekhar number](../../../../../chandrasekhar-number.md), respectively. Division by the chosen scales gives

$$
\begin{aligned}
\sigma^{-1}\dot{\mathbf u}&=-\nabla p'+R\theta\widehat{\mathbf z}+Q\zeta(\mathbf c\cdot\nabla)\mathbf b+\nabla^2\mathbf u,\\
\dot{\mathbf b}&=(\mathbf c\cdot\nabla)\mathbf u+\zeta\nabla^2\mathbf b,\\
\dot\theta&=w+\nabla^2\theta,\qquad\nabla\cdot\mathbf u=\nabla\cdot\mathbf b=0.
\end{aligned}
$$

In particular $Q\zeta=B_0^2d^2/(\mu_0\rho_0\nu\kappa)$, so the diffusivity convention agrees with the momentum coefficient.

For a [plane wave](../../../../../plane-wave.md) put $\mathbf l=(k,0,m)$, $q=|\mathbf l|^2=k^2+m^2$, and $d_\parallel=\mathbf c\cdot\mathbf l=k\sin\alpha+m\cos\alpha$. The induction and [temperature](../../../../../temperature.md) equations imply $\widehat{\mathbf b}=id_\parallel\widehat{\mathbf u}/(s+\zeta q)$ and $\widehat\theta=\widehat w/(s+q)$. The [projection](../../../../../projection-linear-algebra.md) $P=I-\mathbf l\mathbf l^{\mathsf T}/q$ removes [pressure](../../../../../pressure.md). Because $(P\widehat{\mathbf z})_z=k^2/q$, its vertical momentum equation is

$$
\left(\frac s\sigma+q+\frac{Q\zeta d_\parallel^2}{s+\zeta q}\right)\widehat w=R\frac{k^2}{q}\widehat\theta.
$$

Thus the [oblique-field plane-wave magnetoconvection](../../../../../oblique-field-plane-wave-magnetoconvection.md) [dispersion relation](../../../../../dispersion-relation.md) is

$$
\boxed{q(s+q)\left[(s/\sigma+q)(s+\zeta q)+Q\zeta d_\parallel^2\right]-Rk^2(s+\zeta q)=0.}
$$

If out-of-plane [velocity](../../../../../velocity.md) is also allowed, its decoupled magnetic branch satisfies $(s/\sigma+q)(s+\zeta q)+Q\zeta d_\parallel^2=0$; it has no buoyant driving. At stationary marginality, for $k\ne0$,

$$
\boxed{R_{mathrm{stat}}(k,m)=\frac{(k^2+m^2)^3}{k^2}+Q\frac{k^2+m^2}{k^2}(k\sin\alpha+m\cos\alpha)^2.}
$$

These are stationary thresholds; an oscillatory marginal mode, if present for particular diffusivity ratios, is a different onset calculation.

For $m=1$, write $R_{mathrm{stat}}=F(k)+QG(k)$, where $F=(1+k^2)^3/k^2$ and $G=(1+k^2)(\cos\alpha+k\sin\alpha)^2/k^2$. Direct differentiation gives $F'(k)=-2k^{-3}+6k+4k^3$, so its two minima are $\pm1/\sqrt2$, with $F=27/4$ and $F''=36$. For $Q>0$ the negative sign has the smaller magnetic penalty: at every positive $k$, $G(-k)<G(k)$ because both sine and cosine of the inclination are positive. The [wavenumber selection in oblique-field magnetoconvection](../../../../../wavenumber-selection-in-oblique-field-magnetoconvection.md) therefore starts from $a=-1/\sqrt2$. Expanding $F'(k_c)+QG'(k_c)=0$ gives $k_c=a+C_1Q+O(Q^2)$, where $C_1=-G'(a)/F''(a)$. [Taylor expansion](../../../../../taylor-expansion.md) of the value then gives

$$
\boxed{R_c=\frac{27}{4}+3Q(\cos\alpha-\sin\alpha/\sqrt2)^2+C_2Q^2+O(Q^3),\quad C_2=-\frac{G'(a)^2}{2F''(a)}.}
$$

This proves the small-field forms, including the order of the correction.

For large $Q$, $G$ is nonnegative and vanishes only at $b=-\cot\alpha$. The candidate $k=b$ has finite threshold $F(b)$, so a global minimizer must satisfy $QG(k_c)\leq F(b)$ and hence tend to $b$. Here $G''(b)=2(1+b^2)\sin^2\alpha/b^2>0$. Expanding the stationarity condition at $b$ yields

$$
\boxed{k_c=-\cot\alpha+\frac{C_3}{Q}+O(Q^{-2}),\qquad C_3=-\frac{F'(b)}{G''(b)}.}
$$

The value expansion is

$$
\boxed{R_c=\frac{\csc^6\alpha}{\cot^2\alpha}+\frac{C_4}{Q}+O(Q^{-2}),\qquad C_4=-\frac{F'(b)^2}{2G''(b)}.}
$$

The leading coefficient follows from $1+\cot^2\alpha=\csc^2\alpha$. The expansion holds at fixed $0<\alpha<\pi/2$.

Finally choose $\cot\alpha=1/\sqrt2$. Then the nonmagnetic minimizing [wavevector](../../../../../wavevector.md) also has $d_\parallel=0$, and its magnetic penalty vanishes. Since $F(k)\geq27/4$ and $QG(k)\geq0$, this is the [global minimum](../../../../../global-minimum.md) for every nonnegative field strength:

$$
\boxed{\alpha=\arctan\sqrt2,\qquad k_c=-1/\sqrt2,\qquad R_c=27/4\quad\text{for every }Q\geq0.}
$$

This [field-independent stationary threshold in oblique magnetoconvection](../../../../../field-independent-stationary-threshold-in-oblique-magnetoconvection.md) has a simple physical explanation: the disturbance is constant along the imposed field, so it does not bend field lines.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
