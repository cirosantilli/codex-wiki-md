# Paper 1

↑ **Parent:** [2012](../2012.md)

Original paper: [Public original PDF, physical pages 199–202; cover on page 199 and questions on pages 200–202](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=199).

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use [thermal de Broglie wavelength](../../canonical-ensemble.md#thermal-de-broglie-wavelength) $\lambda_T=h/\sqrt{2\pi mk_BT}$ and spacing $a=n^{-1/3}$. [Degeneracy onset from thermal wavelength](../../canonical-ensemble.md#degeneracy-onset-from-thermal-wavelength) occurs at

$$
\boxed{T_\lambda=\frac{h^2n^{2/3}}{2\pi mk_B}.}
$$

The numerical factor depends on the convention for a typical [momentum](../../momentum.md), but the scale $\hbar^2n^{2/3}/(mk_B)$ does not. For [fermions](../../tensor-product-of-quantum-systems.md#fermion) the [Fermi temperature](../../quantum-ideal-gas-statistics.md#fermi-temperature) $T_F=\hbar^2(3\pi^2n)^{2/3}/(2mk_B)$ gives a comparable scale for spin degeneracy two.

Representative estimates, with the assumed [densities](../../fluid-mechanics.md#density) stated explicitly, are:

| System | Assumed [number density](../../statistical-physics.md#number-density) | Assumed particle [mass](../../classical-mechanics.md#mass) | $T_\lambda$ |
| --- | --- | --- | --- |
| [Conduction electrons](../../quantum-mechanics.md#conduction-electron) | $10^{29}\,\mathrm{m^{-3}}$ | $m_e$ | $1.2\times10^5\,\mathrm K$ |
| Dilute heavy atomic cloud | $10^{19}\,\mathrm{m^{-3}}$ | $87u$ | $1.6\times10^{-7}\,\mathrm K$ |
| [Neutrons](../../neutron.md) at nuclear-scale [density](../../fluid-mechanics.md#density) | $10^{44}\,\mathrm{m^{-3}}$ | $m_n$ | $6.5\times10^{11}\,\mathrm K$ |

Here $u$ is the atomic [mass](../../classical-mechanics.md#mass) constant. Thus the characteristic orders are **$10^5\,\mathrm K$ for [electrons](../../physics.md#electron), sub-microkelvin for a dilute heavy atomic gas, and $10^{12}\,\mathrm K$ for [neutrons](../../neutron.md)**. There is no density-independent quantum-degeneracy [temperature](../../temperature.md) for atomic gases: for example, taking $n=2.5\times10^{25}\,\mathrm{m^{-3}}$ and [mass](../../classical-mechanics.md#mass) $4u$ instead gives about $0.065\,\mathrm K$. These are illustrative input estimates, not values supplied by the paper. Denser neutron-star cores require relativistic and interaction corrections; the estimate identifies the degeneracy scale rather than a precise stellar [temperature](../../temperature.md).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Assume three-dimensional isotropic gapless excitations, zero [chemical potential](../../chemical-potential.md) and one independent branch. Momentum-state counting gives

$$
\frac{g(\epsilon)}V=\frac{1}{2\pi^2\hbar^3n}\alpha^{-3/n}\epsilon^{3/n-1}.
$$

Substituting $x=\epsilon/(k_BT)$ into the Bose [energy](../../energy.md) integral shows $U/V\propto T^{1+3/n}$ and $C/V\propto T^{3/n}$. The observed exponent therefore gives **$n=2$**.

For the [quadratic-boson heat-capacity coefficient](../../quantum-ideal-gas-statistics.md#quadratic-boson-heat-capacity-coefficient), the required Bose integral is

$$
I_{3/2}=\int_0^\infty\frac{x^{3/2}\,dx}{e^x-1}
=\Gamma(5/2)\zeta(5/2)=1.78329.
$$

The equality follows by expanding $(e^x-1)^{-1}=\sum_{r\ge1}e^{-rx}$ and integrating term by term. Hence

$$
\frac UV=\frac{I_{3/2}(k_BT)^{5/2}}{4\pi^2\hbar^3\alpha^{3/2}},\qquad
\frac CV=\frac{5I_{3/2}k_B^{5/2}}{8\pi^2\hbar^3\alpha^{3/2}}T^{3/2}.
$$

The supplied units make its $C$ a [heat capacity](../../heat.md#heat-capacity) per [volume](../../geometry-and-topology.md#volume). Equating its coefficient to $220\,\mathrm{J\,K^{-5/2}\,m^{-3}}$ gives

$$
\boxed{\alpha=4.58\times10^{27}\,\mathrm{kg^{-1}}.}
$$

Equivalently $\epsilon=p^2/(2m_*)$ has $m_*=1.09\times10^{-28}\,\mathrm{kg}$. For $q_b$ identical branches, the measured coefficient fixes $q_b/\alpha^{3/2}$, so instead $\alpha=(4.58\times10^{27}\,\mathrm{kg^{-1}})q_b^{2/3}$. The one-branch convention is necessary for the quoted numerical value. The supplied integral with $x^4$ is not the moment arising for the exponent determined here.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For either [phase](../../wave.md#phase-waves), the [entropy](../../entropy.md) differential at fixed composition is

$$
dS=\frac{C_P}{T}\,dT-\left(\frac{\partial V}{\partial T}\right)_P dP
=\frac{C_P}{T}\,dT-V\alpha_T\,dP.
$$

The pressure derivative uses the [Maxwell relation](../../thermodynamics.md#maxwell-relations) from $dG=-S\,dT+V\,dP$. Differentiating the equality of [entropies](../../entropy.md) along coexistence gives the general relation

$$
\frac{\Delta C_P}{T}\,dT=\Delta(V\alpha_T)\,dP.
$$

For a differentiable coexistence curve with pressure varying, equality of [Gibbs free energies](../../thermodynamic-potential.md#gibbs-free-energy) also implies $-\Delta S\,dT+\Delta V\,dP=0$. Since $\Delta S=0$, the two [phases](../../wave.md#phase-waves) then share $V$. Thus, with $\Delta C_P\ne0$,

$$
\boxed{\frac{dT}{dP}=\frac{TV\Delta\alpha_T}{\Delta C_P}.}
$$

This is the [Ehrenfest entropy-continuity relation](../../critical-phenomenon.md#ehrenfest-entropy-continuity-relation). [Entropy](../../entropy.md) equality alone would give $T\Delta(V\alpha_T)/\Delta C_P$ without the shared-volume condition; a constant-pressure boundary or vanishing discontinuities needs separate limiting analysis.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Landau theory](../../critical-phenomenon.md#landau-theory) expands a thermodynamic potential in an [order parameter](../../critical-phenomenon.md#order-parameter), constrained by [symmetry](../../physics.md#symmetry-physics). For a scalar with sign-reversal [symmetry](../../physics.md#symmetry-physics), a useful [free-energy density](../../statistical-physics.md#free-energy-density) is

$$
f=f_0+\frac{a(T-T_c)}2\eta^2+\frac b4\eta^4-h\eta,
\qquad a,b>0.
$$

Here $h$ is the [conjugate field](../../critical-phenomenon.md#field-conjugate-to-an-order-parameter). At $h=0$, minimizing rather than merely finding stationary points gives

$$
\boxed{\eta_{\rm eq}=0\quad(T>T_c),\qquad
\eta_{\rm eq}=\pm\sqrt{\frac{a(T_c-T)}b}\quad(T<T_c).}
$$

The symmetry-related minima represent [spontaneous symmetry breaking](../../quantum-field-theory.md#spontaneous-symmetry-breaking), as for a simple uniaxial [ferromagnet](../../electromagnetism.md#ferromagnet) with [magnetization](../../electromagnetism.md#magnetization) as [order parameter](../../critical-phenomenon.md#order-parameter). An infinitesimal field selects one sign. Above $T_c$, the susceptibility is $1/[a(T-T_c)]$; below it the stable-branch susceptibility is $1/[2a(T_c-T)]$. Minimization lowers $f$ by $-a^2(T-T_c)^2/(4b)$ below $T_c$, producing a heat-capacity [density](../../fluid-mechanics.md#density) jump $T_ca^2/(2b)$ with continuous [entropy](../../entropy.md).

<a id="2/a/image-landau-minima"></a>
![](../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1-tsp2012-landau.png)

**[Figure 1](#2/a/image-landau-minima). Landau minima**. Original normalized quartic free-energy curves above, at and below a continuous transition, with the two symmetry-related equilibrium order-parameter branches.

A negative quartic coefficient requires a stabilizing $+c\eta^6/6$ with $c>0$. It can produce a first-order transition before the quadratic coefficient changes sign: coexistence occurs at $a(T-T_c)=3b^2/(16c)$ and $\eta^2=-3b/(4c)$. Odd terms are allowed when the assumed [symmetry](../../physics.md#symmetry-physics) is absent. [Landau theory](../../critical-phenomenon.md#landau-theory) predicts mean-field exponents; spatial fluctuations can change critical behaviour, especially close to a [critical point](../../analysis.md#critical-point) in low dimensions. A [gradient](../../multivariable-calculus.md#gradient) term extends the model to nonuniform [order parameters](../../critical-phenomenon.md#order-parameter) but does not by itself supply dynamical equations.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[Brownian motion](../../brownian-motion.md) arises from many microscopic collisions. A one-dimensional Langevin description is

$$
m\dot v=-\zeta v-\kappa x+\xi(t),\qquad
\langle\xi(t)\rangle=0,\qquad
\langle\xi(t)\xi(t')\rangle=2\zeta k_BT\delta(t-t').
$$

The fluctuation-dissipation relation ties random forcing to drag, ensuring [thermal equilibrium](../../thermal-equilibrium.md). For a free particle set $\kappa=0$. With initially thermal [velocities](../../classical-mechanics.md#velocity), its mean-square displacement is

$$
\boxed{\langle[x(t)-x(0)]^2\rangle
=2D[t-\tau_v(1-e^{-t/\tau_v})],\qquad
D=\frac{k_BT}{\zeta},\quad \tau_v=\frac m\zeta.}
$$

It is ballistic, $(k_BT/m)t^2$, at short times and diffusive, $2Dt$, for $t\gg\tau_v$. In three dimensions the corresponding long-time result is $6Dt$. At diffusive times, the position propagator from a specified origin is [Gaussian](../../probability-distribution.md#normal-distribution) with [variance](../../variance.md) $2Dt$ per coordinate. A small [sphere](../../euclidean-geometry.md#sphere) in a viscous liquid supplies a physical example; in the slow unbounded-fluid limit its drag is $6\pi\eta_fa$.

For a harmonic trap, overdamped relaxation has time $\tau_\kappa=\zeta/\kappa$, equilibrium [variance](../../variance.md) $k_BT/\kappa$ and stationary [correlation](../../variance.md#pearson-correlation-coefficient)

$$
\langle x(t)x(0)\rangle=\frac{k_BT}{\kappa}e^{-|t|/\tau_\kappa}.
$$

Consequently [stationary trapped Brownian displacement](../../gaussian-process.md#stationary-trapped-brownian-displacement) obeys

$$
\boxed{\langle[x(t)-x(0)]^2\rangle=\frac{2k_BT}{\kappa}(1-e^{-t/\tau_\kappa}).}
$$

Confinement makes this displacement saturate, unlike free [diffusion](../../thermodynamics.md#diffusion). A trajectory initialized exactly at the centre instead has [variance](../../variance.md) $(k_BT/\kappa)(1-e^{-2t/\tau_\kappa})$; confusing that conditional [variance](../../variance.md) with the stationary displacement gives an erroneous factor of two. The equilibrium position distribution is proportional to $\exp[-\kappa x^2/(2k_BT)]$. More general finite confinement has a geometry-dependent equilibrium distribution and bounded displacement, not necessarily a [Gaussian](../../probability-distribution.md#normal-distribution) one.

<a id="2/b/image-free-and-trapped-brownian-motion"></a>
![](../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1-tsp2012-brownian.png)

**[Figure 2](#2/b/image-free-and-trapped-brownian-motion). Free and trapped Brownian motion**. Original analytic mean-square-displacement curves compare free overdamped diffusion, a stationary harmonic trap and a fixed-origin harmonic-trap variance. The last two have different initial ensembles.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

[Bose-Einstein condensation](../../quantum-ideal-gas-statistics.md#bose-einstein-condensation) is macroscopic occupation of a single lowest-energy one-particle state. For a homogeneous three-dimensional [ideal gas](../../ideal-gas.md) of conserved massive [bosons](../../tensor-product-of-quantum-systems.md#boson), set that [energy](../../energy.md) to zero. The excited-state population is

$$
N_{\rm ex}=\frac{V}{\lambda_T^3}g_{3/2}(z),\qquad
z=e^{\mu/(k_BT)}\le1,\qquad
\lambda_T=\sqrt{\frac{2\pi\hbar^2}{mk_BT}}.
$$

Here $g_{3/2}(z)=\sum_{r\ge1}z^r/r^{3/2}$. As $\mu\to0^-$, the [excited states](../../energy-eigenvalue.md#excited-state) can hold only $V\zeta(3/2)/\lambda_T^3$ particles. Additional particles occupy the [ground state](../../quantum-mechanics.md#ground-state). Thus

$$
\boxed{T_c=\frac{2\pi\hbar^2}{mk_B}\left[\frac{n}{\zeta(3/2)}\right]^{2/3},\qquad
\frac{N_0}{N}=1-\left(\frac T{T_c}\right)^{3/2}\quad(T<T_c).}
$$

The isolated [ground state](../../quantum-mechanics.md#ground-state) must be counted separately from the continuum [density of states](../../quantum-ideal-gas-statistics.md#density-of-states); otherwise one misses the condensate. A dilute atomic gas is a physical realization of the quantum-degeneracy regime, but trapping geometry and interactions modify the homogeneous ideal-gas formulas.[§3.5.3: saturation of excited states, separate ground-state occupation and ideal-gas condensation temperature](../../physics-bibliography.md#statistical-physics-by-david-tong)

<a id="2/c/image-ideal-bose-condensate-fraction"></a>
![](../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1-tsp2012-condensation.png)

**[Figure 3](#2/c/image-ideal-bose-condensate-fraction). Ideal Bose condensate fraction**. Original homogeneous three-dimensional ideal-gas condensate fraction and maximum thermal population, normalized to the critical temperature. No trapped-gas or experimental data are implied.

In the homogeneous [ideal gas](../../ideal-gas.md), one and two dimensions do not have finite-temperature condensation in the [thermodynamic limit](../../statistical-physics.md#thermodynamic-limit) because the low-energy population integral diverges. Finite size or a trap changes that conclusion's assumptions. Condensation and [superfluidity](../../statistical-physics.md#superfluidity) are distinct: the ideal quadratic gas has zero [Landau critical velocity](../../statistical-physics.md#landau-critical-velocity), while interactions can support a sound mode and superfluid flow. Neither zero [viscosity](../../dynamic-viscosity.md) nor phase-rigid flow follows from the occupation formula alone.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\beta=1/(k_BT)$. Each independent [fermion](../../tensor-product-of-quantum-systems.md#fermion) orbital is either empty or occupied once, so its grand partition factor is $1+e^{-\beta(\epsilon_j-\mu)}$. Multiplying factors and taking the logarithm gives

$$
\Xi=\prod_j[1+e^{-\beta(\epsilon_j-\mu)}],\qquad
\Phi=-k_BT\ln\Xi=-k_BT\int_0^\infty g(\epsilon)\ln[1+e^{-\beta(\epsilon-\mu)}]d\epsilon.
$$

Since $1-n_F=[1+e^{-\beta(\epsilon-\mu)}]^{-1}$, this is the requested form. Spin or other orbital degeneracy is already included in $g$.

For the [Fermi-window convolution of the grand potential](../../statistical-physics.md#fermi-window-convolution-of-the-grand-potential), define

$$
A(\epsilon)=\int_0^\epsilon g(t)dt,\qquad
\Phi_0(\epsilon)=-\int_0^\epsilon A(t)dt,\qquad
F(\epsilon)=k_BT\ln[1-n_F(\epsilon,\mu)].
$$

Direct differentiation gives **$F'=+n_F$**. The supplied PDF hint has the opposite sign; using that sign would contradict its grand-potential formula. Integrating twice with $A(0)=\Phi_0(0)=0$ and vanishing upper boundary terms,

$$
\Phi=\int_0^\infty A'F\,d\epsilon
=-\int_0^\infty A n_F\,d\epsilon
=\int_0^\infty\Phi'_0 n_F\,d\epsilon
=\boxed{\int_0^\infty\Phi_0(\epsilon)[-\partial_\epsilon n_F]d\epsilon.}
$$

At zero [temperature](../../temperature.md) $-\partial_\epsilon n_F\to\delta(\epsilon-\mu)$, confirming $\Phi_0(\mu)=\Phi(0,\mu)$.

Use the source's implicit unit normalization of the constant [density of states](../../quantum-ideal-gas-statistics.md#density-of-states); restoring a constant baseline $g_0$ multiplies the following potentials by $g_0$. For the sinusoidal [density of states](../../quantum-ideal-gas-statistics.md#density-of-states), direct integration gives

$$
\Phi_0(\epsilon)=-\frac{\epsilon^2}{2}
+\frac{\alpha\Delta^2}{4\pi^2}\left[\cos\left(\frac{2\pi\epsilon}{\Delta}\right)-1\right].
$$

Physical nonnegative [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) requires $|\alpha|\le1$. Write $t=k_BT$ and $y=\epsilon-\mu$. The [Fermi window](../../quantum-ideal-gas-statistics.md#fermi-window)

$$
w(y)=\frac1{4t}\operatorname{sech}^2\left(\frac y{2t}\right)
$$

is even, with full-line moments $\int w\,dy=1$, $\int yw\,dy=0$ and $\int y^2w\,dy=\pi^2t^2/3$. The last integral follows, for example, by expanding $e^x/(1+e^x)^2$ on $x>0$ into its alternating exponential series. When $t\ll\mu$, extending the lower integration limit to $-\infty$ introduces only exponentially small band-edge corrections. The supplied [Fourier transform](../../fourier-transform.md) gives

$$
\int_{-\infty}^{\infty}w(y)\cos\left[\frac{2\pi(\mu+y)}\Delta\right]dy
=\frac X{\sinh X}\cos\left(\frac{2\pi\mu}\Delta\right),\qquad
X=\frac{2\pi^2t}\Delta.
$$

The odd [sine](../../geometry-and-topology.md#sine) term vanishes. Substitution proves

$$
\boxed{\Phi(T,\mu)=\Phi_0(\mu)-\frac{\pi^2t^2}{6}
+\frac{\alpha\Delta^2}{4\pi^2}\left(\frac X{\sinh X}-1\right)
\cos\left(\frac{2\pi\mu}\Delta\right).}
$$

The [thermal damping of a sinusoidal density of states](../../quantum-ideal-gas-statistics.md#thermal-damping-of-a-sinusoidal-density-of-states) is therefore $X/\sinh X$ in the full oscillatory potential. The requested ratio instead concerns the thermal change $\Phi(T,\mu)-\Phi_0(\mu)$. Its [oscillatory thermal-change amplitude ratio](../../quantum-ideal-gas-statistics.md#oscillatory-thermal-change-amplitude-ratio) is

$$
\boxed{\mathcal R(X)=\frac{6|\alpha|}{X^2}\left(1-\frac X{\sinh X}\right).}
$$

For positive $X$ it decreases smoothly from the limit $|\alpha|$ to zero:

$$
\mathcal R=|\alpha|\left[1-\frac{7X^2}{60}+O(X^4)\right]\quad(X\ll1),\qquad
\mathcal R\sim\frac{6|\alpha|}{X^2}\quad(X\gg1).
$$

At exactly $T=0$ both thermal changes vanish; the quoted value is their limiting ratio. The [amplitude](../../wave.md#wave-amplitude) is the envelope in [chemical potential](../../chemical-potential.md). At a particular fixed $\mu$, the signed contribution ratio has $\alpha\cos(2\pi\mu/\Delta)$ in place of $|\alpha|$; at an [oscillation](../../wave.md#oscillation) [node](../../dynamical-systems.md#node-dynamical-systems) the actual oscillatory contribution is zero. The large-$X$ behaviour still requires $k_BT\ll\mu$, so the useful range is $1\ll X\ll2\pi^2\mu/\Delta$.

<a id="3/image-fermion-thermal-smoothing"></a>
![](../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1-tsp2012-fermi-window.png)

**[Figure 4](#3/image-fermion-thermal-smoothing). Fermion thermal smoothing**. Original curves distinguish exponential damping of the full oscillatory grand potential from the algebraically decreasing oscillatory-to-smooth amplitude ratio in its thermal change. The right curve is divided by the stipulated oscillation amplitude.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For two localized [energy](../../energy.md) levels $0,\delta$ with degeneracies $d_0,d_1$, let $x=\delta/(k_BT)$. Canonical equilibrium gives

$$
z=d_0+d_1e^{-x},\qquad p_1=\frac{d_1e^{-x}}z,\qquad
u=\delta p_1,\qquad s=k_B(\ln z+xp_1),\qquad
c=k_Bx^2p_1(1-p_1).
$$

Here $p_1$ is the total upper-level occupation [probability](../../probability-theory.md#probability) and $u,s,c$ are per unit. For nondegenerate levels the [entropy](../../entropy.md) rises from zero to $k_B\ln2$, while the [heat capacity](../../heat.md#heat-capacity) vanishes at both low and high [temperatures](../../temperature.md) and has a Schottky maximum near $k_BT=0.417\delta$. A [spin one-half](../../angular-momentum-operator.md#spin-one-half) in a field, or a localized defect with two configurations, supplies an example. Higher levels must be thermally inaccessible; unequal degeneracies change the populations and peak. Distinguishable localized units have total [partition function](../../canonical-ensemble.md#canonical-partition-function) $z^N$, unlike a gas of indistinguishable particles sharing just two orbitals.

For the magnetic atom, choose level labels with $E_m=-mg\mu_BB$, $m=-J,\ldots,J$. Put $x=T_B/T=g\mu_BB/(k_BT)$. Its [partition function](../../canonical-ensemble.md#canonical-partition-function) and exact [entropy of a finite magnetic multiplet](../../temperature.md#entropy-of-a-finite-magnetic-multiplet) are

$$
\boxed{Z_J(x)=\sum_{m=-J}^{J}e^{mx}
=\frac{\sinh[(2J+1)x/2]}{\sinh(x/2)},\qquad
\frac{s_J}{k_B}=\ln Z_J-x\frac{d\ln Z_J}{dx}.}
$$

The ratio form has removable limit $Z_J(0)=2J+1$. Since $s_J$ is a function of $x$ only, it depends on field and [temperature](../../temperature.md) solely through $B/T$. For fixed $J$ at small $x$, [symmetry](../../physics.md#symmetry-physics) removes the odd [powers](../../energy.md#power) and the supplied sum of $m^2$ gives

$$
Z_J=(2J+1)\left[1+\frac{J(J+1)}6x^2+O(x^4)\right],
\qquad
\boxed{s_J=k_B\left[\ln(2J+1)-\frac{J(J+1)}6\frac{T_B^2}{T^2}+O(x^4)\right].}
$$

For large $J$, the expansion requires $J|x|\ll1$, not merely $|x|\ll1$.

<a id="4/image-two-level-heat-and-magnetic-entropy"></a>
![](../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1-tsp2012-magnetic-entropy.png)

**[Figure 5](#4/image-two-level-heat-and-magnetic-entropy). Two-level heat and magnetic entropy**. Original Schottky heat-capacity curve and exact finite-spin entropies show the entropy deficit removed by isothermal magnetization. Quadratic high-temperature expansions are shown only over a limited small-field interval.

For [demagnetization with a linear-heat-capacity load](../../temperature.md#demagnetization-with-a-linear-heat-capacity-load), integrate its specified $C_L/T$:

$$
S_L(T)=S_L(0)+\frac{Mk_B}{\theta}T.
$$

Isothermal [magnetization](../../electromagnetism.md#magnetization) at $T_i$ removes spin [entropy](../../entropy.md); the bath receives the corresponding heat. During the following reversible, thermally isolated demagnetization, it is the combined [entropy](../../entropy.md) of spins and load that stays constant. At the minimum-field endpoint $B_f=0$, the ideal independent spins reach $s_{\max}=k_B\ln(2J+1)$. Therefore

$$
Ns_J(T_i,B_i)+S_L(T_i)=Nk_B\ln(2J+1)+S_L(T_{\min}),
$$



$$
\boxed{N\left[k_B\ln(2J+1)-s_J(T_i,B_i)\right]
=\frac{Mk_B}{\theta}(T_i-T_{\min}).}
$$

The bracket is the initial [magnetic entropy deficit](../../temperature.md#magnetic-entropy-deficit). The PDF's intermediate equality uses the initial [entropy](../../entropy.md) itself instead; with its preceding definition of $s$, that equality omits the maximum-entropy term. The corrected balance recovers its final [temperature](../../temperature.md) formula:

$$
\boxed{T_{\min}=T_i-\frac{N\theta J(J+1)g^2\mu_B^2B_i^2}{6Mk_B^2T_i^2}.}
$$

Without the small-field expansion, the exact independent-spin prediction is $T_i-(N\theta/M)[\ln(2J+1)-s_J(T_i,B_i)/k_B]$. As a check, zero initial field gives zero [entropy](../../entropy.md) deficit and no cooling. The incorrectly printed intermediate balance would fail this check.

The result requires the load law throughout the [temperature](../../temperature.md) interval, hence $T_i\ll\theta$; a small initial [Zeeman splitting](../../atomic-physics.md#zeeman-splitting), quantitatively $JT_{B,i}/T_i\ll1$; positive final [temperature](../../temperature.md); negligible additional [heat capacities](../../heat.md#heat-capacity) and heat leaks; thermal equilibration between subsystems; and a reversible sweep slow enough to maintain equilibrium. A negative extrapolated [temperature](../../temperature.md) is a breakdown of this approximation, not a cooling prediction. Spins alone would keep $B/T$ fixed, but the attached load changes that adiabat by transferring [entropy](../../entropy.md) to them as it cools.

Interactions invalidate the product of independent one-site [partition functions](../../canonical-ensemble.md#canonical-partition-function). The [entropy](../../entropy.md) must be computed from the many-body [energy](../../energy.md) spectrum or a justified interacting approximation. [Correlations](../../variance.md#pearson-correlation-coefficient) and possible magnetic ordering introduce an interaction scale and can remove the independent-spin [entropy](../../entropy.md) available for cooling near zero field. Internal fields and ordering commonly limit practical demagnetization. The detailed correction and any residual [entropy](../../entropy.md) depend on the interaction Hamiltonian, dimensionality and frustration; neither a universal ordering [temperature](../../temperature.md) nor a numerical final-temperature correction is specified here.

## ↑ Ancestors (11)

1. [2012](../2012.md)
2. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
3. [Thermal and Statistical Physics course of the University of Cambridge](../../university-of-cambridge.md#thermal-and-statistical-physics-course-of-the-university-of-cambridge)
4. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
