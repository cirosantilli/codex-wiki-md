<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Far from the inner edge of a steady [Keplerian accretion disk](../../../../../keplerian-accretion-disk.md), the inner angular-momentum flux is negligible compared with $\dot Mj$. Since $\Omega\propto R^{-3/2}$, the [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) becomes $\mathcal G=3\pi\nu\Sigma j$. The steady balance $\mathcal G\simeq\dot Mj$ therefore gives $\nu\Sigma=\dot M/(3\pi)$. With the stated [surface density of a disk](../../../../../surface-density-of-a-disk.md),

$$
\boxed{\nu=\nu_0R^2,\qquad\nu_0\Sigma_0=\frac{\dot M}{3\pi}.}
$$

Steady [conservation of mass](../../../../../mass-conservation.md) gives $\dot M=-2\pi R\Sigma v_R$, and consequently

$$
\boxed{v_R=-\frac{\dot M}{2\pi R\Sigma}=-\frac{3\nu}{2R}=-\frac32\nu_0R.}
$$

Both relations use the far-inner-edge approximation, rather than extrapolating the stress-free boundary profile to the inner edge.

For the trace [passive scalar](../../../../../passive-scalar.md), put $\sigma=\Sigma C$. Substitute this into the contaminant conservation equation and expand its advective flux:

$$
0=\partial_t(\Sigma C)+\nabla\cdot(\Sigma C u)-\nabla\cdot(k\Sigma\nabla C)
=C\{\partial_t\Sigma+\nabla\cdot(\Sigma u)\}+\Sigma\{\partial_tC+u\cdot\nabla C\}-\nabla\cdot(k\Sigma\nabla C).
$$

The braces multiplying $C$ vanish by background [conservation of mass](../../../../../mass-conservation.md). Hence the [concentration](../../../../../concentration.md) satisfies

$$
\boxed{\Sigma(C_t+u\cdot\nabla C)=\nabla\cdot(k\Sigma\nabla C).}
$$

The small contaminant fraction ensures it does not alter the ambient disk dynamics. The surface-density model already averages vertically; an axisymmetric background and ring-like injection give $C=C(R,t)$. More generally, rapid differential orbital motion winds azimuthal structure and facilitates mixing, but radial-only dependence remains a symmetry or mixing assumption, not a property of every initial injection.

For the axisymmetric [advection-diffusion equation](../../../../../advection-diffusion-equation.md), cylindrical geometry gives

$$
\Sigma(C_t+v_RC_R)=\frac1R\partial_R(Rk\Sigma C_R).
$$

Here $k=\zeta\nu$ and $k\Sigma=\zeta\nu_0\Sigma_0$ are independent of radius. Thus

$$
C_t-\frac32\nu_0RC_R=\zeta\nu_0(R^2C_{RR}+RC_R).
$$

Let $Y=\ln(R/R_*)$, with any fixed reference length $R_*$. Since $C_Y=RC_R$ and $C_{YY}=R^2C_{RR}+RC_R$, this is the [tracer diffusion in a power-law accretion disk](../../../../../tracer-diffusion-in-a-power-law-accretion-disk.md) equation

$$
\boxed{\frac1{\nu_0}C_t-\frac32C_Y=\zeta C_{YY}.}
$$

Assume $\zeta>0$, $\nu_0>0$, and write $v=3\nu_0/2$, $D=\zeta\nu_0$. The change $X=Y+vt$ turns this into the [heat equation](../../../../../heat-equation.md) $C_t=DC_{XX}$. The radial [Dirac delta function](../../../../../dirac-delta-function.md) must be transformed with its Jacobian:

$$
\delta(R-R_0)=\frac1{R_0}\delta(Y-Y_0),\qquad Y_0=\ln(R_0/R_*).
$$

Convolution with the [Gaussian heat kernel](../../../../../gaussian-heat-kernel.md) gives

$$
\boxed{C(R,t)=\frac{C_0}{R_0\sqrt{4\pi\zeta\nu_0t}}\exp\!\left[-\frac{\{\ln(R/R_0)+(3/2)\nu_0t\}^2}{4\zeta\nu_0t}\right].}
$$

This full-line logarithmic solution extends the far-edge power-law model to $0<R<\infty$. An actual finite inner boundary would require its own boundary condition and modified kernel.

The fraction must be computed with the contaminant mass measure, rather than with $C\,dR$. Indeed

$$
dM_c=2\pi R\sigma\,dR=2\pi\Sigma_0 C\,\frac{dR}R=2\pi\Sigma_0 C\,dY.
$$

The total contaminant mass is the conserved quantity $M_c=2\pi\Sigma_0 C_0/R_0$. Its normalized logarithmic radius is therefore a [normal distribution](../../../../../normal-distribution.md) with mean $Y_0-vt$ and [variance](../../../../../variance-split.md) $2Dt$. Integrating this tail gives, for $r>0$,

$$
\boxed{F(r,t)=\frac12\operatorname{erfc}\!\left(\frac{\ln r+(3/2)\nu_0t}{\sqrt{4\zeta\nu_0t}}\right).}
$$

The [complementary error function](../../../../../complementary-error-function.md) accounts for the one-time mass fraction outside the specified radius.

For an outward target $r_1>1$, put $\ell=\ln r_1>0$. Since $\operatorname{erfc}$ is decreasing, maximize $F$ by minimizing $z(t)=(\ell+vt)/\sqrt{4Dt}$. Its derivative has the sign of $vt-\ell$, so the unique maximum occurs at $t_* =\ell/v=2\ln r_1/(3\nu_0)$. At this time $z(t_*)=\sqrt{v\ell/D}$. Thus the printed expression is correctly derived as the **maximum instantaneous exterior fraction**:

$$
\boxed{\max_{t>0}F(r_1,t)=\frac12\operatorname{erfc}\!\left(\sqrt{\frac{3\ln r_1}{2\zeta}}\right),\qquad r_1>1.}
$$

It is not, however, the probability of ever reaching the radius. A tracer can pass through the target and later return; its history is not counted by a one-time exterior fraction. The underlying logarithmic [diffusion process](../../../../../markov-diffusion.md) is

$$
Y_t-Y_0=-vt+\sqrt{2D}\,B_t,
$$

where $B_t$ is standard [Brownian motion](../../../../../brownian-motion-split.md). To compute its actual [hitting probability](../../../../../hitting-probability.md), first put absorbing levels at $-A$ and $\ell$ relative to $Y_0$. Conditioning on the first small time step gives the backward equation $Dh''-vh'=0$ for the probability of reaching the upper level first, with $h(-A)=0$, $h(\ell)=1$. Solving gives

$$
h(y)=\frac{e^{vy/D}-e^{-vA/D}}{e^{v\ell/D}-e^{-vA/D}},\qquad
h(0)=\frac{1-e^{-vA/D}}{e^{v\ell/D}-e^{-vA/D}}.
$$

Letting the lower level tend to $-\infty$ exhausts all finite-time upward-hitting paths. Therefore the correct eventual probability in this idealized model is

$$
\boxed{P_{\mathrm{hit}}(r_1)=e^{-v\ell/D}=r_1^{-3/(2\zeta)},\qquad r_1>1.}
$$

For example, if $\ln r_1=2\zeta/3$, the maximum exterior fraction is $\tfrac12\operatorname{erfc}(1)\simeq0.07865$, whereas the actual [hitting probability](../../../../../hitting-probability.md) is $e^{-1}\simeq0.36788$. This is an explicit counterexample to the last inference in the question and an instance of [maximum occupation is not a hitting probability](../../../../../maximum-occupation-is-not-a-hitting-probability.md).

For $r_1=1$, the target is the initial radius and the hitting probability is one, while $\sup_{t>0}F(1,t)=1/2$ with no attained maximum. For $0<r_1<1$, the inward drift ensures eventual hitting with probability one, and $\sup_{t>0}F(r_1,t)=1$ as $t\downarrow0$. The square-root expression involving $\ln r_1$ is therefore only meaningful for the outward-target case, and even there it describes occupancy rather than first passage.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
