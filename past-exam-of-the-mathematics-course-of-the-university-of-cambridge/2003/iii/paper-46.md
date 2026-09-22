# Paper 46

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper46.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper46.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [phase diagram](../../../thermodynamics.md#phase-diagram) divides a space of control parameters into equilibrium [thermodynamic phases](../../../thermodynamics.md#thermodynamic-phase), marking [phase coexistence](../../../critical-phenomenon.md#phase-coexistence) boundaries and [thermodynamic critical points](../../../critical-phenomenon.md#thermodynamic-critical-point). Its dimension counts independently variable controls, not spatial dimensions. An explicit three-dimensional example uses the controls $(r,u,h)$ of a [sextic even Landau potential](../../../critical-phenomenon.md#sextic-even-landau-potential):

$$
V(M)=\frac r2M^2+\frac u4M^4+\frac v6M^6-hM,\qquad v>0.
$$

Here $M$ is a scalar [order parameter](../../../critical-phenomenon.md#order-parameter), $h$ its [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter), and $r$ a thermal control. The [equilibrium magnetization](../../../critical-phenomenon.md#equilibrium-magnetization) minimizes $V$ globally. At $h=0$, $u>0$, the boundary $r=0$ is a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition). At $h=0$, $u<0$, the boundary $r=3u^2/(16v)$ is a [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) between $M=0$ and $M=\pm\sqrt{-3u/(4v)}$. The two boundaries meet at the **[tricritical point](../../../critical-phenomenon.md#tricritical-point) $r=u=h=0$**. A fixed strictly positive quartic coupling alone cannot produce this [tricritical point](../../../critical-phenomenon.md#tricritical-point); the stabilizing sextic term is essential when the quartic coefficient is tuned through zero.

The full [phase diagram](../../../thermodynamics.md#phase-diagram) also contains the $h=0$ [phase coexistence](../../../critical-phenomenon.md#phase-coexistence) sheet between positive and negative ordered phases. Crossing it changes the sign of $M$ discontinuously. For $u<0$, the three-phase line $r=3u^2/(16v)$ is the junction of this sheet and two [tricritical wings](../../../critical-phenomenon.md#tricritical-wing), on which two unequal same-sign [equilibrium magnetizations](../../../critical-phenomenon.md#equilibrium-magnetization) coexist at nonzero $h$. The [tricritical wing critical edges](../../../critical-phenomenon.md#tricritical-wing-critical-edge) are lines of ordinary [thermodynamic critical points](../../../critical-phenomenon.md#thermodynamic-critical-point); they terminate the first-order sheets and meet at the [tricritical point](../../../critical-phenomenon.md#tricritical-point). Away from these boundaries, varying $h$ produces a smooth crossover.

For an explicit construction of the [tricritical wings](../../../critical-phenomenon.md#tricritical-wing), write their two coexisting [order parameters](../../../critical-phenomenon.md#order-parameter) as $M_1=s-d$ and $M_2=s+d$, with $s>0$ and $0<d\leq s$. Equality of their [Landau free energies](../../../critical-phenomenon.md#landau-free-energy) and first derivatives gives

$$
u=-v\left(\frac{10}{3}s^2+2d^2\right),\qquad
r=v\left(5s^4-\frac23s^2d^2+d^4\right),\qquad
h=\frac83vs^3(s^2-d^2).
$$

Indeed, for these controls the [tricritical wing coexistence factorization](../../../critical-phenomenon.md#tricritical-wing-coexistence-factorization) is

$$
V(M)-V(M_1)=\frac v6[(M-s)^2-d^2]^2[M^2+4sM+5s^2-d^2].
$$

The last factor is $(M+2s)^2+s^2-d^2\geq0$, proving that both specified minima are global. The reflected wing has negative $h$ and negative $M$. Letting $d\to0$ gives the [tricritical wing critical edge](../../../critical-phenomenon.md#tricritical-wing-critical-edge) $u=-10vs^2/3$, $r=5vs^4$, $h=8vs^5/3$; there $V''(s)=V'''(s)=0$ and $V''''(s)=40vs^2>0$. Letting $d=s$ recovers the three-phase line. This supplies the first-order sheets and their continuous boundary curves, rather than only a zero-field section.

<a id="1/image-zero-field-section-and-three-dimensional-coexistence-wings-of-a-sextic-landau-phase-diagram"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46-phases.png)

**[Figure 1](#1/image-zero-field-section-and-three-dimensional-coexistence-wings-of-a-sextic-landau-phase-diagram). Zero-field section and three-dimensional coexistence wings of a sextic Landau phase diagram**.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [order parameter](../../../critical-phenomenon.md#order-parameter) distinguishes equilibrium [thermodynamic phases](../../../thermodynamics.md#thermodynamic-phase). For a scalar magnetic system, a slowly varying coarse-grained [scalar field](../../../quantum-field-theory.md#scalar-field) $\phi(x)$ represents local [magnetization](../../../electromagnetism.md#magnetization), and its uniform expectation $M=\langle\phi\rangle$ is the [order parameter](../../../critical-phenomenon.md#order-parameter). Under [spin inversion symmetry](../../../statistical-physics.md#spin-inversion-symmetry), $\phi\mapsto-\phi$ and $h\mapsto-h$. The disordered phase has $M=0$ at $h=0$, while a pure ordered phase has $M\ne0$. In a finite symmetric system the average still vanishes at $h=0$; [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) means taking the [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit) before $h\to0^+$ or $h\to0^-$ to select a [pure thermodynamic phase](../../../critical-phenomenon.md#pure-thermodynamic-phase).

[Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) assigns a local [free-energy functional](../../../thermodynamics.md#free-energy-functional)

$$
\mathcal F[\phi]=\int d^Dx\left[\frac\kappa2|\nabla\phi|^2+\frac r2\phi^2+\frac u4\phi^4+\frac v6\phi^6-h\phi\right],\qquad \kappa>0.
$$

[Spin inversion symmetry](../../../statistical-physics.md#spin-inversion-symmetry) forbids odd powers at zero [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter); locality and slow variation motivate the [gradient expansion](../../../critical-phenomenon.md#gradient-expansion). The [gradient energy](../../../critical-phenomenon.md#gradient-energy) penalizes interfaces and determines long-wavelength response. Integrating $e^{-\mathcal F/(k_BT)}$ over fields includes fluctuations, whereas the [Landau approximation](../../../critical-phenomenon.md#landau-approximation) replaces that integral by its stable stationary configuration. For a uniform phase this reduces to minimizing $V(M)$. If $f$ is the equilibrium [free-energy density](../../../statistical-physics.md#free-energy-density), then $M=-\partial f/\partial h$, so the [order parameter](../../../critical-phenomenon.md#order-parameter) is also the thermodynamic response to its [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The uniform stationarity equation and local stability condition are

$$
rM+uM^3+vM^5=h,\qquad V''(M)=r+3uM^2+5vM^4>0.
$$

For $u>0$, $h=0$, and small negative $r$, the stable nonzero solution satisfies $M^2=-r/u+O(r^2)$. Thus the [order parameter](../../../critical-phenomenon.md#order-parameter) vanishes continuously as $r\uparrow0$. The equilibrium [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) has leading singular contribution $f_{\min}=-r^2/(4u)$ below the transition and zero above it. Its first thermal derivative is continuous, while its second derivative has a finite jump: the [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) predicts a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition) with no [latent heat](../../../thermodynamics.md#latent-heat). The [magnetic susceptibility](../../../statistical-physics.md#magnetic-susceptibility) follows by differentiating the stationarity equation:

$$
\chi=\frac{\partial M}{\partial h}=\frac{1}{r+3uM^2+5vM^4}.
$$

It diverges on approaching the ordinary [thermodynamic critical point](../../../critical-phenomenon.md#thermodynamic-critical-point), and the quadratic [Landau scalar correlation length](../../../critical-phenomenon.md#landau-scalar-correlation-length) behaves as $\xi\sim\sqrt{\kappa/|r|}$, with a different amplitude on the two sides.

For $u<0$, a nonzero stationary point at $h=0$ has $r+uM^2+vM^4=0$. Substitution into $V(M)-V(0)$ gives $-uM^4/4-vM^6/3$. Setting this to zero yields

$$
\boxed{M_{\mathrm{coex}}^2=-\frac{3u}{4v},\qquad r_{\mathrm{coex}}=\frac{3u^2}{16v}.}
$$

The finite jump of $M$ makes this a [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition). For a thermal path $r=r(T)$ with $r'(T)\ne0$ and the other coefficients fixed, $\partial f_{\min}/\partial T=r'(T)M^2/2$ jumps, giving an entropy discontinuity and nonzero [latent heat](../../../thermodynamics.md#latent-heat). The [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) itself remains continuous. The disordered minimum loses stability at $r=0$; the two nonzero stationary solutions merge at $r=u^2/(4v)$. These [spinodal points](../../../critical-phenomenon.md#spinodal-point) bound [metastability](../../../critical-phenomenon.md#metastability), but neither replaces the equilibrium [phase coexistence](../../../critical-phenomenon.md#phase-coexistence) condition.

Writing $r=a t$ with $a>0$ near an ordinary [thermodynamic critical point](../../../critical-phenomenon.md#thermodynamic-critical-point), the zero-field equation gives $M\sim(-t)^{1/2}$. At $r=0$, small $h$ obeys $h=uM^3+O(M^5)$, hence $M\sim\operatorname{sgn}(h)|h|^{1/3}$. The ordinary [mean-field critical exponents](../../../critical-phenomenon.md#mean-field-critical-exponent) are therefore **$\beta=1/2$ and $\delta=3$**. These are [Landau theory](../../../critical-phenomenon.md#landau-theory) predictions, not dimension-independent values for an interacting theory below its [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $A(M)=V(M)+hM$ be the zero-field [constrained order-parameter free energy](../../../critical-phenomenon.md#constrained-order-parameter-free-energy). At coexistence in a [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter) $h_c$, two global minima $M_1<M_2$ obey

$$
A'(M_1)=A'(M_2)=h_c,\qquad
A(M_2)-A(M_1)=h_c(M_2-M_1).
$$

Thus the same line of slope $h_c$ is tangent to $A$ at both endpoints: the [common-tangent construction for phase coexistence](../../../critical-phenomenon.md#common-tangent-construction-for-phase-coexistence). Equivalently,

$$
\boxed{\int_{M_1}^{M_2}[A'(M)-h_c]\,dM=0.}
$$

This is the [Maxwell equal-area construction](../../../thermodynamics.md#maxwell-construction) on the equation-of-state curve $h=A'(M)$: the signed areas on either side of the horizontal coexistence line cancel. Equal slope alone finds stationary phases; the integral additionally enforces equal [free energy](../../../thermodynamics.md#thermodynamic-free-energy).

If the mean [order parameter](../../../critical-phenomenon.md#order-parameter) is constrained between the endpoints, the system can separate into two macroscopic phases. With $\lambda=(M-M_1)/(M_2-M_1)$, their bulk [free-energy density](../../../statistical-physics.md#free-energy-density) is $(1-\lambda)A(M_1)+\lambda A(M_2)$. The interface contributes subextensively in the [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit). The resulting [constrained order-parameter free energy](../../../critical-phenomenon.md#constrained-order-parameter-free-energy) is the convex envelope of $A$, with a straight coexistence segment. This explains why a nonconvex uniform [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) must be convexified when describing stable constrained equilibrium, and why a [spinodal point](../../../critical-phenomenon.md#spinodal-point) is not the [Maxwell construction](../../../thermodynamics.md#maxwell-construction) boundary.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

At the [tricritical point](../../../critical-phenomenon.md#tricritical-point), both the quadratic and quartic even coefficients vanish, while the sextic coefficient remains positive. Two even control parameters must therefore be tuned, in addition to setting the symmetry-breaking [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter) to zero. The [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition) line and [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) line meet, the coexistence [order parameter](../../../critical-phenomenon.md#order-parameter) jump shrinks to zero, and the [tricritical wings](../../../critical-phenomenon.md#tricritical-wing) end there. The balance governing the equation of state changes from quartic to sextic stabilization.

Along the tricritical thermal path $u=0$, $r=a t$, $h=0$, minimizing $V$ gives $M^4=-r/v$ on the ordered side. At $r=u=0$, the equation of state is $h=vM^5$. Consequently

$$
\boxed{\beta_{\mathrm{tri}}=\frac14,\qquad \delta_{\mathrm{tri}}=5.}
$$

These [mean-field critical exponents](../../../critical-phenomenon.md#mean-field-critical-exponent) require the tuned tricritical path; a path with fixed $u>0$ instead has the ordinary exponents derived above. The corresponding equilibrium [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) is $f_{\min}=-(-r)^{3/2}/(3\sqrt v)$ below the transition. Its first thermal derivative is continuous but its second derivative diverges, giving the tricritical [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) a heat-capacity exponent $\alpha=1/2$. Fluctuations are negligible asymptotically only above the tricritical [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) three; at three dimensions logarithmic corrections can accompany these powers.

## 2

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $\beta_T=(k_BT)^{-1}$ to distinguish inverse temperature from an [order-parameter critical exponent](../../../critical-phenomenon.md#order-parameter-critical-exponent). For the [Ising model](../../../statistical-physics.md#ising-model), define the full [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) $G(r)=\langle\sigma_0\sigma_r\rangle$ and its [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function) $G_c(r)=G(r)-M^2$ in a translation-invariant phase. Away from a [thermodynamic critical point](../../../critical-phenomenon.md#thermodynamic-critical-point), the large-distance envelope decays exponentially, possibly multiplied by a power of distance:

$$
\xi^{-1}=-\lim_{|r|\to\infty}\frac{\log|G_c(r)|}{|r|}.
$$

This defines the [correlation length](../../../critical-phenomenon.md#correlation-length) in physical distance units when the limit exists. At a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition), $\xi\to\infty$ and the critical [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function) typically has algebraic decay $G_c(r)\sim |r|^{-(D-2+\eta)}$, where $\eta$ is the [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension). Below the transition the full $G(r)$ tends to $M^2$, so the decay definition must use $G_c$.

Let $S=\sum_r\sigma_r$ and $F=-\beta_T^{-1}\log Z$ be the extensive [Helmholtz free energy](../../../thermodynamics.md#helmholtz-free-energy). Holding the field-independent constant $C$ and other physical couplings fixed,

$$
M=-\frac1N\frac{\partial F}{\partial h},\qquad
\chi=-\frac1N\frac{\partial^2F}{\partial h^2}.
$$

Because the Hamiltonian contains $-hS$, $\partial_h\log Z=\beta_T\langle S\rangle$ and $\partial_h^2\log Z=\beta_T^2(\langle S^2\rangle-\langle S\rangle^2)$. Translation invariance then proves the [correlation-function susceptibility sum rule](../../../critical-phenomenon.md#correlation-function-susceptibility-sum-rule):

$$
\boxed{\chi=\frac{\beta_T}{N}\operatorname{Var}S
=\frac{\beta_T}{N}\sum_{r,r'}\langle\sigma_r\sigma_{r'}\rangle_c
=\beta_T\sum_rG_c(r).}
$$

In the ordered zero-field phase these statements refer to a selected [pure thermodynamic phase](../../../critical-phenomenon.md#pure-thermodynamic-phase); averaging equally over opposite [magnetizations](../../../electromagnetism.md#magnetization) introduces the separate [spin-mixture contribution to zero-field susceptibility](../../../critical-phenomenon.md#spin-mixture-contribution-to-zero-field-susceptibility).

A [normalized blocking kernel](../../../critical-phenomenon.md#normalized-blocking-kernel) $K_b(\sigma',\sigma)\geq0$ satisfies $\sum_{\sigma'}K_b(\sigma',\sigma)=1$. For example, assign one block spin to each block of $b^D$ microscopic spins using majority sign, with equal probabilities for a tie. Define the blocked Hamiltonian, retaining the entire generated operator space, by

$$
\sum_\sigma K_b(\sigma',\sigma)e^{-\beta_TH(u,\sigma)}
=e^{-\beta_TH(R_bu,\sigma')-\beta_TNg_E(u)}.
$$

The field-independent contribution $Ng_E$ belongs to the identity operator. With $N'=Nb^{-D}$ and

$$
u'=R_bu,\qquad C'=b^D[C+g_E(u)],
$$

summing over $\sigma'$ proves **$Z(u,C,N)=Z(u',C',N')$** exactly. Iterating gives $N_p=Nb^{-pD}$ and the same [partition function](../../../statistical-physics.md#canonical-partition-function) with $(u_p,C_p,N_p)$. Observables at large scales are reproduced by appropriately blocked observables and sources. Truncating the generated interactions makes this an approximation; dropping the additive constant already destroys the equality of [free energies](../../../thermodynamics.md#thermodynamic-free-energy) even when normalized spin expectations remain correct.

The extensive [Helmholtz free energy](../../../thermodynamics.md#helmholtz-free-energy) is unchanged: $F(u_0,C_0,N)=F(u_p,C_p,N_p)$. In contrast, its value per site changes because the number of sites changes. Define the reduced zero-constant [free-energy density](../../../statistical-physics.md#free-energy-density) $f_0(u)=\beta_TF(u,0,N)/N$ in the [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit). The preceding equality yields

$$
f_0(u)=b^{-D}f_0(R_bu)+g_0(u),\qquad g_0(u)=\beta_Tg_E(u),
$$

and iteration proves the [additive free-energy recursion under blocking](../../../critical-phenomenon.md#additive-free-energy-recursion-under-blocking):

$$
\boxed{f_0(u_0)=b^{-pD}f_0(u_p)+\sum_{j=0}^{p-1}b^{-jD}g_0(u_j).}
$$

Equivalently $C_p=b^{pD}[C_0+\sum_{j=0}^{p-1}b^{-jD}g_E(u_j)]$. Thus the inhomogeneous source records the [identity-operator contribution to renormalization-group free energy](../../../critical-phenomenon.md#identity-operator-contribution-to-renormalization-group-free-energy) from eliminated short-distance degrees of freedom.

To express this recursion for the singular part, write $f_0=a+f_s$, where $a$ is the regular analytic background. Then the same displayed recursion holds with $f_s$ and

$$
g_s(u)=g_0(u)+b^{-D}a(R_bu)-a(u).
$$

This is the [analytic subtraction of an inhomogeneous renormalization recursion](../../../critical-phenomenon.md#analytic-subtraction-of-an-inhomogeneous-renormalization-recursion). A purely analytic source can often be absorbed into $a$, after which it does not control the leading singular powers. It is not legitimate simply to discard an analytic source in the full [free energy](../../../thermodynamics.md#thermodynamic-free-energy), where it can dominate the regular background. Moreover an analytic monomial $c\,t^m h^n$ contributes

$$
c\,t^mh^n\sum_{j=0}^{p-1}b^{j(ml_t+nl_h-D)}.
$$

If $ml_t+nl_h=D$, the sum is $p$ and hence generates a logarithm when $p\sim-\log|t|/(l_t\log b)$: a [renormalization-group free-energy resonance](../../../critical-phenomenon.md#renormalization-group-free-energy-resonance). Such a term cannot be discarded when describing that logarithmic singularity. Neglect of the inhomogeneous term in the leading power-law scaling therefore assumes that its regular part has been subtracted, that any remaining source only changes finite scaling amplitudes, and that there are no relevant resonances or marginal logarithms. Omitting an [irrelevant operator](../../../critical-phenomenon.md#irrelevant-operator) further requires absence of a [dangerously irrelevant coupling](../../../critical-phenomenon.md#dangerously-irrelevant-coupling), whose vanishing limit can make a scaling function singular.

A [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point) obeys $R_bu_*=u_*$. Linearization gives $\delta u'=A\delta u$; in [eigenvector](../../../linear-operator-theory.md#eigenvector) coordinates $w_i'=b^{l_i}w_i$. Positive $l_i$ label [relevant operators](../../../critical-phenomenon.md#relevant-operator), negative $l_i$ label [irrelevant operators](../../../critical-phenomenon.md#irrelevant-operator), and zero $l_i$ labels a [marginal operator](../../../critical-phenomenon.md#marginal-operator) requiring nonlinear analysis. The [critical surface](../../../critical-phenomenon.md#critical-surface) is the stable manifold obtained by tuning all relevant scaling fields to zero. A [repulsive renormalization-group trajectory](../../../critical-phenomenon.md#repulsive-renormalization-group-trajectory) leaves the fixed point along a relevant direction as the observation length increases. Locally a typical zero-field section has $dw/d\ell=-\omega w$, $dt/d\ell=l_tt$, $\ell=\log b$, so the critical surface $t=0$ attracts along $w$, while trajectories with either sign of $t$ depart from it. A magnetic scaling field adds another relevant direction.

<a id="2/image-renormalization-group-saddle-flow-in-a-zero-field-section-and-two-relevant-directions-transverse-to-the-critical-surface"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46-rg-flow.png)

**[Figure 2](#2/image-renormalization-group-saddle-flow-in-a-zero-field-section-and-two-relevant-directions-transverse-to-the-critical-surface). Renormalization-group saddle flow in a zero-field section and two relevant directions transverse to the critical surface**.

Under the stated homogeneous-scaling assumptions and after fixing irrelevant fields at their limiting values, two relevant scaling fields obey $t'=b^{l_t}t$, $h'=b^{l_h}h$. These fields are analytic coordinates near the [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point), proportional to the physical [reduced temperature](../../../critical-phenomenon.md#reduced-temperature) and [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter) to leading order. The singular [free-energy density](../../../statistical-physics.md#free-energy-density) consequently obeys

$$
F_s(t,h)=b^{-D}F_s(b^{l_t}t,b^{l_h}h).
$$

Here $F_s$ denotes the singular free energy per original site or unit volume, with regular dimensional factors absorbed; the extensive singular part is $NF_s$. Iterate and choose $b^p=|t|^{-1/l_t}$ to obtain the [scaling hypothesis for critical phenomena](../../../critical-phenomenon.md#scaling-hypothesis-for-critical-phenomena):

$$
\boxed{F_s(t,h)=|t|^{D/l_t}f_\pm\left(h/|t|^{l_h/l_t}\right).}
$$

The sign labels the two sides of the transition: $f_+$ describes $t>0$, the disordered side, while $f_-$ describes $t<0$, the ordered side. The two functions need not coincide; $f_-$ has the zero-field one-sided derivative appropriate to spontaneous [magnetization](../../../electromagnetism.md#magnetization). The numbers $l_t,l_h$ are scaling eigenvalues in logarithmic form: the corresponding discrete RG multipliers are $b^{l_t},b^{l_h}$.

The [correlation length](../../../critical-phenomenon.md#correlation-length) obeys $\xi(t,h)=b\,\xi(b^{l_t}t,b^{l_h}h)$. The same scale choice gives $\nu=1/l_t$. Differentiating $F_s$ once and twice with respect to the [conjugate field](../../../critical-phenomenon.md#field-conjugate-to-an-order-parameter), and twice with respect to temperature, gives

$$
\beta=\frac{D-l_h}{l_t},\qquad
\gamma=\frac{2l_h-D}{l_t},\qquad
\alpha=2-\frac D{l_t}.
$$

At $t=0$, instead choose the scale $b^p=|h|^{-1/l_h}$. Then $F_s(0,h)\sim|h|^{D/l_h}$ and $M\sim\operatorname{sgn}(h)|h|^{D/l_h-1}$, so $\delta=l_h/(D-l_h)$. Thus differentiation and scale matching establish

$$
\boxed{\beta\delta=\frac{l_h}{l_t}=\beta+\gamma,\qquad \alpha=2-D\nu.}
$$

The first is the [Widom scaling relation](../../../critical-phenomenon.md#widom-scaling-relation) and the second the [hyperscaling relation](../../../critical-phenomenon.md#hyperscaling-relation). The [hyperscaling relation](../../../critical-phenomenon.md#hyperscaling-relation) requires precisely the regular homogeneous scaling used here. Above the ordinary [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension), the quartic coupling is [dangerously irrelevant](../../../critical-phenomenon.md#dangerously-irrelevant-coupling) in the ordered phase and this derivation cannot discard it: the [mean-field critical exponents](../../../critical-phenomenon.md#mean-field-critical-exponent) $\nu=1/2$, $\alpha=0$ do not obey $\alpha=2-D\nu$ for $D>4$. At marginal dimensions logarithmic factors likewise require care beyond the displayed pure powers.

## 3

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Changing the [ultraviolet cutoff](../../../quantum-field-theory.md#ultraviolet-cutoff) changes which fluctuations remain explicit. Integrating out a shell of [Fourier modes](../../../fourier-analysis.md#fourier-mode) shifts the coefficients of all symmetry-allowed operators and a field-independent constant. Hence the cutoff-dependent coefficients are chosen so that the remaining [partition function](../../../statistical-physics.md#canonical-partition-function) and long-distance observables reproduce the same microscopic system. This is the [Wilsonian coarse-grained statistical Hamiltonian](../../../critical-phenomenon.md#wilsonian-coarse-grained-statistical-hamiltonian); retaining only the printed operators is a [local derivative expansion](../../../critical-phenomenon.md#local-derivative-expansion), not an exact closure.

In a massive symmetric phase, the quadratic long-wavelength inverse [two-point function](../../../critical-phenomenon.md#two-point-correlation-function) has the form $\alpha^{-1}p^2+m^2$. Its [Landau scalar correlation length](../../../critical-phenomenon.md#landau-scalar-correlation-length) satisfies $\xi^{-2}=\alpha m^2$ in this approximation. For [canonical normalization of a scalar gradient term](../../../critical-phenomenon.md#canonical-normalization-of-a-scalar-gradient-term), set $\phi=\sqrt\alpha\,\psi$; then the mass and quartic coefficients become $r=\alpha m^2$ and $g_c=\alpha^2g$. With this normalization the infrared mass is the inverse [correlation length](../../../critical-phenomenon.md#correlation-length), $m_R=\xi^{-1}$, within the massive quadratic or one-loop approximation. More generally the decay rate is a [pole mass](../../../perturbative-quantum-field-theory.md#pole-mass), whereas the zero-momentum inverse [magnetic susceptibility](../../../statistical-physics.md#magnetic-susceptibility) is a curvature mass; an [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) or nontrivial momentum dependence can distinguish them. In the ordered phase one must first expand about a selected stable [equilibrium magnetization](../../../critical-phenomenon.md#equilibrium-magnetization), rather than identify a negative quadratic coefficient at the unstable origin with a squared inverse [correlation length](../../../critical-phenomenon.md#correlation-length). Thus the intended mass identification includes a field normalization and a stable-phase qualification.

For [momentum-shell renormalization group](../../../critical-phenomenon.md#momentum-shell-renormalization-group), split $\phi=\phi_<+\phi_>$, retaining $|p|<\Lambda/b$ and eliminating $\Lambda/b<|p|<\Lambda$. Define

$$
e^{-H_{\mathrm{eff}}[\phi_<]}=\int\mathcal D\phi_>\,e^{-H[\phi_<+\phi_>]}.
$$

Taking a logarithm gives the [cumulant expansion of a coarse-grained free energy](../../../critical-phenomenon.md#cumulant-expansion-of-a-coarse-grained-free-energy). For a centered fast [Gaussian measure](../../../stochastic-process.md#gaussian-measure) with $G_>(0)=\langle\phi_>^2\rangle$, the first quartic cumulant is

$$
\frac g{4!}\int d^Dx\,\langle(\phi_<+\phi_>)^4\rangle_>
=\frac g{24}\int d^Dx\,[\phi_<^4+6G_>(0)\phi_<^2+3G_>(0)^2].
$$

The [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) give a mass shift $\Delta r=gG_>(0)/2$ and an identity-operator contribution, while leaving the quartic term at this order. The second cumulant produces higher interactions and a quartic correction. After the length and field rescalings $x=bx'$ and $\phi_<(x)=b^{-(D-2)/2}\phi'(x')$, the gradient coefficient remains one, and

$$
r'=b^2\left[r+\frac g2G_>(0)+O(g^2)\right],\qquad
g'=b^{4-D}g+O(g^2),\qquad v'=b^{6-2D}v+\cdots.
$$

The [one-loop shell mass renormalization in scalar quartic theory](../../../critical-phenomenon.md#one-loop-shell-mass-renormalization-in-scalar-quartic-theory) explicitly shows why the critical bare mass is shifted by fluctuations.

Assume short-range interactions, an analytic even local potential, a positive gradient coefficient, and a weak-coupling trajectory in the basin of the [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point). Above four dimensions the quartic interaction has negative [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) and its dimensionless strength decreases under coarse graining; higher local powers and higher derivative terms also decrease. After absorbing analytic short-distance shifts into the coefficients, long-wavelength fluctuations are small compared with the ordered [order parameter](../../../critical-phenomenon.md#order-parameter). The remaining coarse [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) can therefore be evaluated at its stable saddle:

$$
\mathcal F_{\mathrm L}[M]=\int d^Dx\left[\frac12(\nabla M)^2+\frac12r_R(T)M^2+\frac{g_R}{4!}M^4-hM+\cdots\right].
$$

The quartic stabilizer must still be retained for the ordered minimum even though it is [dangerously irrelevant](../../../critical-phenomenon.md#dangerously-irrelevant-coupling). Stationarity, $r_RM+g_RM^3/6=h$, gives the ordinary [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) and its [mean-field critical exponents](../../../critical-phenomenon.md#mean-field-critical-exponent). This derives the saddle approximation from decreasing fluctuation strength under the stated RG assumptions; it does not assume that every exact coarse-grained functional becomes a quartic polynomial. Below four dimensions the quartic coupling grows, long-wavelength loop corrections cease to be small, and the argument fails. At four dimensions the interaction is marginal and generates logarithmic corrections. The tuned sextic theory has the analogous boundary at three dimensions.

Use a consistent [Fourier transform](../../../analysis.md#fourier-transform) pair for the [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function):

$$
\widetilde G(p)=\int d^Dx\,e^{-ip\cdot x}G_c(x),\qquad
G_c(x)=\int\frac{d^Dp}{(2\pi)^D}e^{ip\cdot x}\widetilde G(p).
$$

The printed forward-transform expression integrates over $p$ while leaving $x$ free; that integration variable is an error. The above convention resolves it and produces the loop measure used below. At zero [magnetization](../../../electromagnetism.md#magnetization), $G_c(x)=\langle\phi(0)\phi(x)\rangle$; otherwise the disconnected product of expectations must be subtracted.

In the inverse-propagator identity used here, the truncated two-point function means the full [one-particle-irreducible two-point vertex](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-two-point-vertex), including its free quadratic part. This convention differs from using “truncated” for a connected cumulant. To derive the inverse relation, introduce $W[J]=\log Z[J]$, $\varphi=\delta W/\delta J$ and the [effective action](../../../perturbative-quantum-field-theory.md#effective-action) $\Gamma[\varphi]=\int J\varphi-W[J]$. Then $\delta\Gamma/\delta\varphi=J$ and the chain rule gives $\Gamma^{(2)}W^{(2)}=1$. Since $W^{(2)}$ is the [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function), translation invariance gives **$\widetilde\Gamma(p)=\widetilde G(p)^{-1}$**.

Now use canonically normalized coefficients, denoting the cutoff mass by $m_b^2=m^2(\Lambda,T)$ and the renormalized infrared mass by $m_R^2=m^2(0,T)$. Choose the free [propagator](../../../quantum-field-theory.md#propagator) $\widetilde G_0(p)=(p^2+m_R^2)^{-1}$ and put $\delta m^2=m_b^2-m_R^2$ in the interaction as a quadratic [counterterm](../../../perturbative-quantum-field-theory.md#counterterm). With the Euclidean [self-energy](../../../perturbative-quantum-field-theory.md#self-energy) convention in which an insertion changes the connected propagator by $-G_0\Sigma G_0$, the perturbative series begins

$$
\widetilde G=\widetilde G_0-\widetilde G_0(\delta m^2+\Sigma)\widetilde G_0+\cdots,
\qquad
\boxed{\widetilde\Gamma(p)=p^2+m_R^2+\delta m^2+\Sigma(p).}
$$

The [self-energy](../../../perturbative-quantum-field-theory.md#self-energy) sums one-particle-irreducible loop insertions; the explicit mass [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) is kept separate. Repeated insertions generate the geometric [Dyson resummation](../../../perturbative-quantum-field-theory.md#dyson-resummation), which explains why reducible chains occur in $G$ but not as independent terms in its inverse. Beyond one loop a momentum-dependent [self-energy](../../../perturbative-quantum-field-theory.md#self-energy) and [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) must also be included.

At one loop the only quartic two-point graph is the [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram). At a $g\phi^4/4!$ vertex, attaching the two labeled external fields uses $4\cdot3=12$ choices and contracts the remaining two fields together. The factor is $12/4!=1/2$. Equivalently this is the same quadratic term in the shell [cumulant expansion](../../../probability-theory.md#cumulant-expansion) above. Thus

$$
\Sigma^{(1)}(p)=\frac g2 I_D(m_R^2;\Lambda),\qquad
I_D(R;\Lambda)=\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}\frac1{k^2+R}.
$$

It is positive for $g>0$ and independent of external momentum, so there is no one-loop gradient renormalization. The condition $\widetilde\Gamma(0)=m_R^2$ implies $\delta m^2+\Sigma(0)=0$, hence

$$
\boxed{m_R^2=m_b^2+\frac g2\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}\frac1{k^2+m_R^2}+O(g^2).}
$$

The cutoff is necessary: the unregulated integral is ultraviolet divergent for $D\geq2$. Using the renormalized mass internally is a self-consistent one-loop organization, not an exact resummation of all critical fluctuations. With nonunit $\alpha$, this formula instead applies to $r=\alpha m^2$, $g_c=\alpha^2g$ after [canonical normalization of a scalar gradient term](../../../critical-phenomenon.md#canonical-normalization-of-a-scalar-gradient-term).

To test a linear thermal mass, approach the ordinary transition from the symmetric side and set $R=m_R^2>0$. For $D>2$ the massless tadpole is infrared finite. Subtract its critical value, absorb regular temperature dependence of the coupling into a nonzero thermal coefficient $A$, and write $m_b^2(T)-m_b^2(T_C)=A(T-T_C)+\cdots$. The [one-loop critical-mass subtraction](../../../critical-phenomenon.md#one-loop-critical-mass-subtraction) gives

$$
R=A(T-T_C)+\frac g2[I_D(R)-I_D(0)],\qquad
\boxed{R\left[1+\frac g2J_D(R)\right]=A(T-T_C),}
$$

where

$$
J_D(R)=\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D k^2(k^2+R)}
=c_D\int_0^\Lambda\frac{k^{D-3}}{k^2+R}\,dk,\qquad
c_D=\frac{S_{D-1}}{(2\pi)^D}.
$$

For $D>4$, $J_D(0)=c_D\Lambda^{D-4}/(D-4)$ is finite, so the bracket tends to a finite constant and $R\propto T-T_C$ is self-consistent. At $D=4$,

$$
J_4(R)=\frac{1}{16\pi^2}\log\frac{\Lambda^2+R}{R},
$$

and the growing logarithm obstructs an asymptotically constant linear coefficient at nonzero coupling. For $2<D<4$, put $k=\sqrt R\,q$ to obtain

$$
J_D(R)\sim c_D R^{(D-4)/2}\int_0^\infty\frac{q^{D-3}}{1+q^2}\,dq
=c_D R^{(D-4)/2}\frac\pi2\csc\frac{\pi(D-2)}2.
$$

The divergent bracket then invalidates the assumed linear thermal mass. The [radial critical-mass subtraction in dimensions three to five](../../../critical-phenomenon.md#radial-critical-mass-subtraction-in-dimensions-three-to-five) gives explicit checks of all three behaviors. For $D\leq2$, the massless tadpole subtraction itself is infrared divergent; that failure of the Gaussian expansion does not prove absence of an interacting transition. Therefore the ordinary **[upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) is $D_C=4$**, with the unmodified [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) asymptotically justified by this test only for $D>4$. Exponents inferred by solving the self-consistent one-loop equation below four dimensions would not be exact interacting exponents.

For a [tricritical point](../../../critical-phenomenon.md#tricritical-point) the renormalized quartic coefficient must be tuned to zero, and a positive sextic interaction stabilizes the [order parameter](../../../critical-phenomenon.md#order-parameter). The gradient term gives the [scalar field](../../../quantum-field-theory.md#scalar-field) [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) $(D-2)/2$. A coefficient of $\phi^6$ therefore has dimension $D-6(D-2)/2=6-2D$, which becomes marginal at $D=3$. This gives **$D_C^{\mathrm{tri}}=3$**. A direct [Ginzburg criterion](../../../critical-phenomenon.md#ginzburg-criterion) reaches the same result: long-wavelength variance in a [correlation volume](../../../critical-phenomenon.md#correlation-volume) is

$$
\langle(\delta M)^2\rangle_\xi\sim\int_{|k|\lesssim\xi^{-1}}\frac{d^Dk}{k^2+\xi^{-2}}
\sim\xi^{2-D}\sim |r|^{(D-2)/2},
$$

while the tricritical saddle has $M^2\sim|r|^{1/2}$. Their ratio scales as $|r|^{(D-3)/2}$, vanishing only above three dimensions. At three dimensions it is marginal; below three it grows. In contrast the ordinary saddle $M^2\sim|r|/g$ gives a ratio $g|r|^{(D-4)/2}$. Both calculations assume the thermal mass is measured relative to its shifted critical value. A sextic interaction generates quartic terms under coarse graining, so tricriticality requires tuning the renormalized quartic scaling field as well as the mass.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
