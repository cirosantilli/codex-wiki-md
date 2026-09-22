# Paper 79

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper79.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper79.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [zeroth law of turbulence](../../../turbulence.md#zeroth-law-of-turbulence) states that at fixed outer [velocity](../../../classical-mechanics.md#velocity) $u$ and [integral scale of turbulence](../../../turbulence.md#integral-scale-of-turbulence) $\ell$, the mean [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) per unit mass approaches a nonzero finite value as the [Reynolds number](../../../fluid-mechanics.md#reynolds-number) $\mathrm{Re}=u\ell/\nu$ becomes large. In an established forward [energy cascade](../../../turbulence.md#energy-cascade), this gives $\epsilon\sim C_\epsilon u^3/\ell$, with $C_\epsilon$ of order one. The small-scale [velocity gradients](../../../continuum-mechanics.md#velocity-gradient) become large enough to offset decreasing [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity); this is the [turbulent dissipation anomaly](../../../turbulence.md#turbulent-dissipation-anomaly).

At the [Kolmogorov microscales](../../../turbulence.md#kolmogorov-microscales), the local [Reynolds number](../../../fluid-mechanics.md#reynolds-number) is of order one, $v\eta/\nu\sim1$, and the [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) is $\epsilon\sim\nu(v/\eta)^2$. Solving these balances gives

$$
\boxed{\eta=(\nu^3/\epsilon)^{1/4},\qquad v=(\nu\epsilon)^{1/4}}.
$$

Substituting the outer-scale estimate, and omitting order-one constants, gives

$$
\boxed{\eta\sim\ell\,\mathrm{Re}^{-3/4},\qquad v\sim u\,\mathrm{Re}^{-1/4}}.
$$

The associated [eddy turnover time](../../../turbulence.md#eddy-turnover-time) is $\eta/v=(\nu/\epsilon)^{1/2}$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

[Local isotropy of turbulence](../../../turbulence.md#local-isotropy-of-turbulence) means that joint small-scale [velocity increment](../../../turbulence.md#velocity-increment) statistics are approximately unchanged by [rotations](../../../riemannian-geometry.md#rotation-mathematics), even when the large-scale flow is anisotropic. The [universal equilibrium range](../../../turbulence.md#equilibrium-range) contains separations much smaller than the [integral scale of turbulence](../../../turbulence.md#integral-scale-of-turbulence): their adjustment times are short compared with the outer [eddy turnover time](../../../turbulence.md#eddy-turnover-time), and their normalized statistics are assumed independent of the detailed large-scale forcing. It includes the [inertial range](../../../turbulence.md#inertial-range) and the [dissipation range](../../../turbulence.md#dissipation-range).

The [Kolmogorov first similarity hypothesis](../../../turbulence.md#kolmogorov-first-similarity-hypothesis) says that these locally isotropic statistics depend only on $r$, mean [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) $\epsilon$ and [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) $\nu$. [Dimensional analysis](../../../physics.md#dimensional-analysis) therefore expresses the second-order [longitudinal structure function](../../../turbulence.md#longitudinal-velocity-structure-function) in terms of the [Kolmogorov microscales](../../../turbulence.md#kolmogorov-microscales):

$$
\boxed{S_2(r)=\langle(\Delta v)^2\rangle=v^2F(r/\eta),\qquad r\ll\ell}.
$$

The universality of $F$ is an assumption of the theory, not a consequence of [dimensional analysis](../../../physics.md#dimensional-analysis) alone.

The [Kolmogorov second similarity hypothesis](../../../turbulence.md#kolmogorov-second-similarity-hypothesis) removes dependence on [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) when $\eta\ll r\ll\ell$. Only $\epsilon$ and $r$ remain, so the [Kolmogorov two-thirds law](../../../turbulence.md#kolmogorov-two-thirds-law) is

$$
\boxed{S_2(r)=\beta(\epsilon r)^{2/3}}.
$$

The same reasoning gives the predicted order-$P$ [longitudinal structure function](../../../turbulence.md#longitudinal-velocity-structure-function):

$$
\boxed{\langle(\Delta v)^P\rangle=\beta_P(\epsilon r)^{P/3}}.
$$

These are signed [moments](../../../probability-theory.md#moment) for integer $P$; for noninteger orders, use $\langle|\Delta v|^P\rangle$. In particular, the signed third-order coefficient is negative, $\beta_3=-4/5$, in the [Kolmogorov four-fifths law](../../../turbulence.md#kolmogorov-four-fifths-law).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

[External intermittency](../../../turbulence.md#external-intermittency) is the alternation of turbulent and non-turbulent fluid at a point as a fluctuating interface passes it. [Internal intermittency](../../../turbulence.md#internal-intermittency) in the [equilibrium range](../../../turbulence.md#equilibrium-range) instead describes uneven, bursty concentrations of small-scale [velocity gradients](../../../continuum-mechanics.md#velocity-gradient) and [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) within turbulent fluid. [Integral-scale intermittency](../../../turbulence.md#integral-scale-intermittency) is modulation of the energy-containing motions and their energy supply. It is non-universal because it retains information about forcing, boundary conditions and the history of the large-scale flow.

The [Landau intermittency counterexample](../../../turbulence.md#landau-intermittency-counterexample) challenges the unconditional universality asserted by [Kolmogorov 1941 theory](../../../turbulence.md#kolmogorov-1941-theory). Suppose turbulent populations have different conditional mean [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) rates $\epsilon_a$. Even if each obeys the same conditional scaling, averaging over populations gives

$$
S_P=\beta_Pr^{P/3}\langle\epsilon_a^{P/3}\rangle,
$$

which generally differs from $\beta_Pr^{P/3}\langle\epsilon_a\rangle^{P/3}$. Thus a coefficient normalized by the global mean depends on the large-scale intensity distribution. The third-order case escapes this particular objection because the power of $\epsilon_a$ is one.

The [Kolmogorov refined similarity hypothesis](../../../turbulence.md#kolmogorov-refined-similarity-hypothesis) replaces global mean [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) by [coarse-grained energy dissipation](../../../turbulence.md#coarse-grained-energy-dissipation) $\epsilon_{\mathrm{AV}}(r)$. It assumes that

$$
V=\frac{\Delta v}{[r\epsilon_{\mathrm{AV}}(r)]^{1/3}}
$$

has universal conditional statistics at sufficiently large local [Reynolds number](../../../fluid-mechanics.md#reynolds-number). If the conditional $P$th [moment](../../../probability-theory.md#moment) is $\beta_P$, the [law of total expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\boxed{\langle(\Delta v)^P\rangle=\beta_P\langle\epsilon_{\mathrm{AV}}(r)^{P/3}\rangle r^{P/3}}.
$$

The [refined similarity](../../../turbulence.md#kolmogorov-refined-similarity-hypothesis) hypothesis does not itself prescribe the distribution of [coarse-grained energy dissipation](../../../turbulence.md#coarse-grained-energy-dissipation). Scale dependence of those [moments](../../../probability-theory.md#moment) can change the predicted exponents. As before, noninteger orders require absolute [velocity increments](../../../turbulence.md#velocity-increment).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

A [passive scalar](../../../fluid-mechanics.md#passive-scalar) $\theta$ is transported by the [velocity field](../../../fluid-mechanics.md#velocity-field) without feeding back on it:

$$
\partial_t\theta+\mathbf u\cdot\nabla\theta=\kappa\Delta\theta.
$$

Take its mean to be zero, and define the [scalar dissipation rate](../../../fluid-mechanics.md#scalar-dissipation-rate) by the half-[scalar variance](../../../fluid-mechanics.md#scalar-variance) convention $\chi=\kappa\langle|\nabla\theta|^2\rangle$. In a statistically equilibrated [energy cascade](../../../turbulence.md#energy-cascade) of scalar fluctuations, this is also the flux of half-[scalar variance](../../../fluid-mechanics.md#scalar-variance) toward small scales.

The [Kolmogorov two-thirds law](../../../turbulence.md#kolmogorov-two-thirds-law) gives a typical [velocity increment](../../../turbulence.md#velocity-increment) $\delta u_r\sim(\epsilon r)^{1/3}$ and hence [eddy turnover time](../../../turbulence.md#eddy-turnover-time) $\tau_r\sim r/\delta u_r\sim\epsilon^{-1/3}r^{2/3}$. Assuming local scalar transfer on this same time scale, $\chi\sim\langle(\Delta\theta)^2\rangle/\tau_r$. The [Obukhov-Corrsin theory](../../../fluid-mechanics.md#obukhov-corrsin-theory) therefore gives the scalar analogue:

$$
\boxed{\langle(\Delta\theta)^2\rangle=C_\theta\chi\epsilon^{-1/3}r^{2/3}}.
$$

This applies to separations at which both direct forcing and molecular [diffusion](../../../thermodynamics.md#diffusion) are negligible and the transporting [velocity increments](../../../turbulence.md#velocity-increment) lie in the [inertial range](../../../turbulence.md#inertial-range). For very large or very small ratios $\nu/\kappa$, the scalar and velocity cutoff scales differ, so this common range must be checked. Defining $\chi$ as dissipation of the full [scalar variance](../../../fluid-mechanics.md#scalar-variance) instead simply changes the convention for $C_\theta$.

## 2

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Write $A_{ij}=\partial_j u_i$ and use [incompressibility](../../../fluid-mechanics.md#incompressible-flow), $A_{ii}=0$. The displayed vector can be expressed as

$$
D_i=A_{ij}A_{jk}u_k-\frac12u_i\operatorname{tr}(A^2).
$$

On taking its [divergence](../../../calculus.md#divergence), $\partial_iA_{ij}=0$. Commuting the remaining [partial derivatives](../../../calculus.md#partial-derivative) gives

$$
A_{ij}(\partial_iA_{jk})u_k
=u_kA_{ij}\partial_kA_{ji}
=\frac12u_k\partial_k\operatorname{tr}(A^2),
$$

which cancels the derivative of the second term of $D_i$. The derivatives falling on $u_k$ leave

$$
\boxed{\partial_iD_i=A_{ij}A_{jk}A_{ki}=\operatorname{tr}(A^3)}.
$$

In [homogeneous turbulence](../../../turbulence.md#homogeneous-turbulence), averaging commutes with differentiation and $\langle D_i\rangle$ is position independent, provided these [moments](../../../probability-theory.md#moment) exist. Consequently $\langle\operatorname{tr}(A^3)\rangle=0$.

Using the [strain-rate tensor](../../../viscous-fluid-flow.md#strain-rate-tensor) and [vorticity](../../../fluid-mechanics.md#vorticity) decomposition supplied in the question now gives the [Betchov relation](../../../turbulence.md#betchov-relation):

$$
\boxed{\langle S_{ij}S_{jk}S_{ki}\rangle=-\frac34\langle\omega_i\omega_jS_{ij}\rangle}.
$$

This uses homogeneity and [incompressibility](../../../fluid-mechanics.md#incompressible-flow); isotropy is unnecessary.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [principal strain rates](../../../viscous-fluid-flow.md#principal-strain-rates) $a,b,c$ are the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of the symmetric [strain-rate tensor](../../../viscous-fluid-flow.md#strain-rate-tensor). [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) makes its [trace](../../../linear-algebra.md#matrix-trace) zero, so $a+b+c=0$. The polynomial identity

$$
a^3+b^3+c^3-3abc
=(a+b+c)(a^2+b^2+c^2-ab-bc-ca)
$$

therefore gives $a^3+b^3+c^3=3abc$. Since the [trace](../../../linear-algebra.md#matrix-trace) of $S^3$ is the sum of the cubes of its [eigenvalues](../../../linear-operator-theory.md#eigenvalue), the [Betchov relation](../../../turbulence.md#betchov-relation) becomes

$$
3\langle abc\rangle=-\frac34\langle\omega_i\omega_jS_{ij}\rangle,
\qquad
\boxed{\langle abc\rangle=-\frac14\langle\omega_i\omega_jS_{ij}\rangle}.
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

In established three-dimensional [turbulence](../../../turbulence.md), mean [vortex stretching](../../../physics.md#vortex-stretching) is positive: $\langle\omega_i\omega_jS_{ij}\rangle>0$. The [Betchov relation](../../../turbulence.md#betchov-relation) then gives $\langle abc\rangle<0$. [Bi-axial strain](../../../viscous-fluid-flow.md#bi-axial-strain) has two positive [principal strain rates](../../../viscous-fluid-flow.md#principal-strain-rates) and one negative rate, hence $abc<0$; extension along one axis with compression along the other two instead gives $abc>0$.

Thus the cubic strain statistic favors [bi-axial strain](../../../viscous-fluid-flow.md#bi-axial-strain). Strictly, this is an amplitude-weighted preference: a negative average alone cannot prove that there are more events of one type, since a few strong events could dominate it. Positive mean [vortex stretching](../../../physics.md#vortex-stretching) is additional physical information, not a consequence of homogeneity alone.

[Bi-axial strain](../../../viscous-fluid-flow.md#bi-axial-strain) spreads a nearly incompressible material volume along two directions while thinning it along the third, favoring sheet-like concentrations of [vorticity](../../../fluid-mechanics.md#vorticity). A sheet can then become unstable and roll up into [vortex tubes](../../../fluid-mechanics.md#vortex-tube). The [Townsend-Betchov cascade cartoon](../../../turbulence.md#townsend-betchov-cascade-cartoon) uses this sequence to reconcile strain-favored sheets with the intense tubes observed at dissipative scales. Alignment of [vorticity](../../../fluid-mechanics.md#vorticity) with the [principal strain rates](../../../viscous-fluid-flow.md#principal-strain-rates) also affects the stretching; the determinant statistic does not specify the entire geometry.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For a [Burgers vortex](../../../continuum-mechanics.md#burgers-vortex), integrating the axial [vorticity](../../../fluid-mechanics.md#vorticity) gives the azimuthal [velocity](../../../classical-mechanics.md#velocity):

$$
u_\theta(r)=\frac\Gamma{2\pi r}(1-e^{-r^2/\delta^2}),\qquad \delta^2=\frac{4\nu}{\alpha}.
$$

The swirl contribution to the [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) per unit length and per unit density is

$$
\mathcal D_\theta=\nu\int_0^\infty
\left(\frac{du_\theta}{dr}-\frac{u_\theta}{r}\right)^2 2\pi r\,dr
=\nu\int_0^\infty\omega_z^2\,2\pi r\,dr.
$$

For the equality, expand the two squares using $\omega_z=u_\theta'+u_\theta/r$; their integrated difference is proportional to $[u_\theta^2]_0^\infty$, which vanishes. Substitution of the Gaussian [vorticity](../../../fluid-mechanics.md#vorticity) profile gives

$$
\mathcal D_\theta
=\frac{2\nu\Gamma^2}{\pi\delta^4}\int_0^\infty r e^{-2r^2/\delta^2}\,dr
=\frac{\nu\Gamma^2}{2\pi\delta^2}
=\boxed{\frac{\alpha\Gamma^2}{8\pi}}.
$$

This [excess dissipation of a Burgers vortex](../../../continuum-mechanics.md#excess-dissipation-of-a-burgers-vortex) is independent of [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) at fixed strain $\alpha$ and [circulation](../../../fluid-mechanics.md#circulation-physics) $\Gamma$. Multiply by the [mass density](../../../fluid-mechanics.md#density) if a dimensional power per length is wanted.

The qualification "excess" matters. The imposed uniform strain itself has [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) density $3\nu\alpha^2$ per unit mass, so its integral over an infinite cross-section diverges. One must subtract that background or restrict to a finite cross-section. In a core-sized area, its contribution is of order $\nu^2\alpha$, smaller than the swirl contribution by order $(\nu/\Gamma)^2$ as $\Gamma/\nu\to\infty$.

Meanwhile $\delta\propto\nu^{1/2}$ shrinks and the central [vorticity](../../../fluid-mechanics.md#vorticity) $\Gamma/(\pi\delta^2)$ grows. The finite dissipation becomes concentrated in a narrow tube: a useful local model of [internal intermittency](../../../turbulence.md#internal-intermittency) and the [turbulent dissipation anomaly](../../../turbulence.md#turbulent-dissipation-anomaly), though not a proof that an entire turbulent flow consists of such vortices.

## 3

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $u^2$ denote one-component [velocity](../../../classical-mechanics.md#velocity) [variance](../../../variance.md), $F=u^2f$ the [longitudinal velocity correlation](../../../turbulence.md#longitudinal-velocity-correlation), and $S_p=\langle(\Delta v)^p\rangle$ the signed [longitudinal structure functions](../../../turbulence.md#longitudinal-velocity-structure-function). Homogeneity gives $F=u^2-S_2/2$, while the third-order convention here is $u^3K=S_3/6$. Thus the [Kármán-Howarth equation](../../../turbulence.md#karman-howarth-equation) becomes

$$
\partial_tF=\frac1{r^4}\partial_r\left[r^4\left(\frac{S_3}{6}-\nu S_2'\right)\right].
$$

The mean [kinetic energy](../../../classical-mechanics.md#kinetic-energy) per unit mass is $3u^2/2$, so its decay gives $\partial_tu^2=-2\epsilon/3$. In the [universal equilibrium range](../../../turbulence.md#equilibrium-range), the small-scale variation $\partial_tS_2$ is negligible at leading order, hence $\partial_tF\simeq-2\epsilon/3$. Integrating from zero and using regularity gives

$$
r^4\left(\frac{S_3}{6}-\nu S_2'\right)
=-\frac{2\epsilon}{3}\frac{r^5}{5}.
$$

The [Kolmogorov equation for structure functions](../../../turbulence.md#kolmogorov-equation-for-structure-functions) is therefore

$$
\boxed{S_3(r)-6\nu S_2'(r)=-\frac45\epsilon r}.
$$

For finite local unsteadiness the right side has the additional term $-3r^{-4}\int_0^r s^4\partial_tS_2(s,t)\,ds$; dropping it is the local-equilibrium approximation used here.

In the [inertial range](../../../turbulence.md#inertial-range) the viscous term is also negligible, leaving the [Kolmogorov four-fifths law](../../../turbulence.md#kolmogorov-four-fifths-law), **$S_3(r)=-4\epsilon r/5$**. Its coefficient and sign follow from the exact energy balance and [Kármán-Howarth equation](../../../turbulence.md#karman-howarth-equation), rather than from dimensional similarity. It supplies a firm third-order constraint on [Kolmogorov 1941 theory](../../../turbulence.md#kolmogorov-1941-theory) and measures the forward [energy cascade](../../../turbulence.md#energy-cascade), while leaving the second- and higher-order exponents open to [internal intermittency](../../../turbulence.md#internal-intermittency) corrections.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Put $W=\langle\omega^2\rangle$, $C=\langle|\nabla\times\boldsymbol\omega|^2\rangle$ and $M=\langle G^3\rangle$, where $G=\partial_xu_x$. The small-$r$ [Taylor series](../../../calculus.md#taylor-series) give

$$
F=u^2-\frac{Wr^2}{30}+\frac{Cr^4}{840}+\cdots,\qquad S_3=Mr^3+\cdots.
$$

In the [Kármán-Howarth equation](../../../turbulence.md#karman-howarth-equation), the coefficient of $r^2$ on the left is $-\dot W/30$. On the right, the triple-correlation term contributes $7M/6$ and the viscous term contributes $\nu C/15$. Hence

$$
-\frac{\dot W}{30}=\frac76M+\frac\nu{15}C,
\qquad
\boxed{\frac12\dot W=-\frac{35}{2}\langle G^3\rangle-\nu C}.
$$

Comparing with the [mean enstrophy balance](../../../fluid-mechanics.md#mean-enstrophy-balance) identifies the mean [vortex stretching](../../../physics.md#vortex-stretching):

$$
\langle\omega_i\omega_jS_{ij}\rangle=-\frac{35}{2}\langle G^3\rangle.
$$

Also $S_2=2(u^2-F)=Wr^2/15+\cdots$, whereas differentiability gives $S_2=\langle G^2\rangle r^2+\cdots$. Thus $\langle G^2\rangle=W/15$. Homogeneity makes $\langle G\rangle=0$, so the [longitudinal velocity-gradient skewness](../../../turbulence.md#longitudinal-velocity-gradient-skewness) is $S_0=M/(W/15)^{3/2}$. Substitution gives

$$
\boxed{\langle\omega_i\omega_jS_{ij}\rangle=-\frac7{6\sqrt{15}}S_0\langle\omega^2\rangle^{3/2}}.
$$

Positive mean [vortex stretching](../../../physics.md#vortex-stretching) therefore requires negative [skewness](../../../probability-theory.md#skewness). A centered [Gaussian distribution](../../../probability-theory.md#normal-distribution) has zero third [moment](../../../probability-theory.md#moment), so the derivative statistics cannot be Gaussian. This conclusion uses the physically positive mean stretching, not homogeneity alone.

The [probability density function](../../../continuous-probability-distribution.md#probability-density-function) has mean zero but a longer or stronger negative tail, representing intermittent compression. The illustration uses a standardized [Gaussian mixture distribution](../../../probability-theory.md#gaussian-mixture-distribution) solely to sketch this sign of [skewness](../../../probability-theory.md#skewness); it is not turbulence simulation data or a fitted universal distribution.

<a id="3/ii/image-illustrative-negatively-skewed-longitudinal-velocity-gradient-density"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-79-gradient-skewness.png)

**[Figure 1](#3/ii/image-illustrative-negatively-skewed-longitudinal-velocity-gradient-density). Illustrative negatively skewed longitudinal velocity-gradient density**.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Combining the [Kolmogorov two-thirds law](../../../turbulence.md#kolmogorov-two-thirds-law) with the [Kolmogorov four-fifths law](../../../turbulence.md#kolmogorov-four-fifths-law) gives the [velocity increment](../../../turbulence.md#velocity-increment) [skewness](../../../probability-theory.md#skewness) in the [inertial range](../../../turbulence.md#inertial-range):

$$
S(r)=\frac{S_3(r)}{S_2(r)^{3/2}}
=\frac{-4\epsilon r/5}{[\beta(\epsilon r)^{2/3}]^{3/2}}
=\boxed{-\frac4{5\beta^{3/2}}}.
$$

The [constant-skewness turbulence closure](../../../turbulence.md#constant-skewness-turbulence-closure) assumes this same value throughout the [universal equilibrium range](../../../turbulence.md#equilibrium-range), including the dissipative crossover. This is an extra modeling assumption; neither similarity law establishes it near $r=0$.

Write $A=\beta(15\beta)^{1/2}$, $B=(15\beta)^{3/4}$, $S_2=Av^2h$ and $r=B\eta x$. Since $\nu=v\eta$ and $\epsilon\eta=v^3$, substituting $S_3=-4S_2^{3/2}/(5\beta^{3/2})$ into the [Kolmogorov equation for structure functions](../../../turbulence.md#kolmogorov-equation-for-structure-functions) gives

$$
\frac{6A}{B}h'+\frac{4A^{3/2}}{5\beta^{3/2}}h^{3/2}=\frac45Bx.
$$

Dividing by $2B/5$ yields the [normalized constant-skewness structure-function equation](../../../turbulence.md#normalized-constant-skewness-structure-function-equation):

$$
\boxed{\frac{dh}{dx}+2h^{3/2}=2x,\qquad h(0)=0}.
$$

At small $x$, $h\sim x^2$, recovering $S_2\sim\epsilon r^2/(15\nu)$ for differentiable [velocity increments](../../../turbulence.md#velocity-increment). At large $x$, the dominant balance gives $h\sim x^{2/3}$, recovering the assumed [Kolmogorov two-thirds law](../../../turbulence.md#kolmogorov-two-thirds-law).

This [turbulence closure](../../../turbulence.md#turbulence-closure) is inexpensive: a single [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) interpolates between the two regimes while respecting the local third-order balance. Its prescribed [skewness](../../../probability-theory.md#skewness) cannot independently predict scale-dependent derivative statistics, transient spectral evolution or [internal intermittency](../../../turbulence.md#internal-intermittency).

[EDQNM closure](../../../turbulence.md#eddy-damped-quasi-normal-markovian-closure) instead evolves the [turbulent energy spectrum](../../../turbulence.md#turbulent-energy-spectrum) through modeled [spectral triad interactions](../../../turbulence.md#spectral-triad-interaction). Its quasi-normal fourth-order approximation is supplemented by eddy damping and a Markovian treatment of correlation memory. It retains more information about scale-dependent transfer and evolving spectra, at the cost of spectral integrals and modeled damping times. It is still approximate and does not automatically describe coherent structures or [internal intermittency](../../../turbulence.md#internal-intermittency). The simple constant-skewness model is therefore useful as an equilibrium interpolation; [EDQNM closure](../../../turbulence.md#eddy-damped-quasi-normal-markovian-closure) addresses a broader spectral evolution problem.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
