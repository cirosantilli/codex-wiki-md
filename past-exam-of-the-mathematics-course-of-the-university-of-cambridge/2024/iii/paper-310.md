# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_310.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a component with $P=w\rho$ and constant $w$, the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) becomes

$$
\frac{\dot\rho}{\rho}=-3(1+w)\frac{\dot a}{a}.
$$

Integration gives the [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling)

$$
\boxed{\rho_i(a)=\rho_{i,0}a^{-3(1+w_i)}
=\rho_{i,0}(1+z)^{3(1+w_i)}}.
$$

Define the present [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) by

$$
\boxed{\Omega_{i,0}=\frac{\rho_{i,0}}{\rho_{\rm crit,0}},
\qquad \rho_{\rm crit,0}=\frac{3H_0^2}{8\pi G}}.
$$

Substitution into the spatially flat [Friedmann equation](../../../cosmology.md#friedmann-equations) gives the [Hubble parameter for constant-equation-of-state components](../../../cosmology.md#hubble-parameter-for-constant-equation-of-state-components)

$$
\boxed{H(z)=H_0\left[
\sum_i\Omega_{i,0}(1+z)^{3(1+w_i)}
\right]^{1/2}}.
$$

Spatial flatness is what allows the expression to contain only the listed density components, with $\sum_i\Omega_{i,0}=1$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For [dynamical dark energy](../../../cosmology.md#dynamical-dark-energy), use $dz/dt=-(1+z)H$ in the continuity equation to obtain

$$
\frac{d\log\rho_{\rm DE}}{dz}
=\frac{3[1+w(z)]}{1+z}.
$$

Therefore the [variable dark-energy equation of state](../../../cosmology.md#variable-dark-energy-equation-of-state) gives

$$
\rho_{\rm DE}(z)=\rho_{{\rm DE},0}(1+z)^3
\exp\left[3\int_0^z\frac{w(z')}{1+z'}\,dz'\right].
$$

Combining this with $\rho_m=\rho_{m,0}(1+z)^3$ in the [Friedmann equation](../../../cosmology.md#friedmann-equations) yields

$$
\boxed{H(z)=H_0\left\{
\Omega_{m,0}(1+z)^3
+\Omega_{{\rm DE},0}(1+z)^3
\exp\left[\int_0^z\frac{3w(z')}{X(z')}\,dz'\right]
\right\}^{1/2}},
$$

where

$$
\boxed{X(z)=1+z}.
$$

This is the [Hubble parameter for matter and dynamical dark energy](../../../cosmology.md#hubble-parameter-for-matter-and-dynamical-dark-energy).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The flux relation is $F=L/(4\pi d_L^2)$ with [luminosity distance](../../../cosmology.md#luminosity-distance) $d_L=(1+z)\chi(z)$. In a spatially flat universe,

$$
\chi(z)=c\int_0^z\frac{dz'}{H(z')},
\qquad
d_L(z)=(1+z)c\int_0^z\frac{dz'}{H(z')}.
$$

Thus [Type Ia supernova cosmology](../../../cosmology.md#type-ia-supernova-cosmology) measures the distance-redshift curve. Equation (2) makes $H(z)$ depend on an integral of $w(z)$, while $d_L$ introduces a second integral. Fitting predicted distances to many supernova fluxes over a range of redshifts therefore constrains parameters or bins describing $w(z)$, although these integrations smooth fine redshift structure.

The common luminosity $L$ need not be known to constrain the shape of $w(z)$. An unknown $L$ multiplies every inferred distance by the same factor and is degenerate with the overall scale $H_0^{-1}$, or equivalently with the supernova absolute magnitude. Relative distances at different redshifts still determine the shape of the expansion history. An external calibration is needed to determine the absolute distance scale.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

All galaxies in the population share the same formation time $t_f$, so the difference between their stellar ages equals the difference between their cosmic emission times. The [redshift-time relation](../../../cosmology.md#redshift-time-relation) gives

$$
\frac{dz}{dt}=-(1+z)H(z).
$$

For a close pair with $|\Delta z|\ll1$,

$$
\boxed{\Delta t\simeq-\frac{\Delta z}{(1+z)H(z)}},
\qquad
\boxed{H(z)\simeq-\frac1{1+z}\frac{\Delta z}{\Delta t}}.
$$

A [cosmic chronometer](../../../cosmology.md#cosmic-chronometer) measurement therefore reconstructs $H(z)$ directly from differential galaxy ages. Inserting those values into the matter-plus-dark-energy Friedmann expression constrains $w(z)$.

Supernova distances integrate $1/H(z)$, while $H(z)$ already contains an integral of $w(z)$. Cosmic chronometers avoid the distance integral, so rapid oscillations in $w(z)$ suffer one fewer smoothing operation and can leave a more visible signal.

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Before electron-positron annihilation, photons, electrons, and positrons share one temperature. Their effective entropy degrees of freedom are

$$
g_{*s}^{\rm before}=2+\frac78(2+2)=\frac{11}{2}.
$$

The neutrinos have already undergone [thermal decoupling in cosmology](../../../cosmology.md#thermal-decoupling-in-cosmology), so $T_\nu a$ remains constant and they receive none of the electron-positron entropy. In the still-coupled electromagnetic plasma, [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) gives

$$
\frac{11}{2}T_{\rm before}^3a_{\rm before}^3
=2T_\gamma^3a^3.
$$

The decoupled neutrino temperature at the same later time is $T_\nu=T_{\rm before}a_{\rm before}/a$. Dividing the two relations gives the [Cosmic neutrino background](../../../cosmology.md#cosmic-neutrino-background) temperature

$$
\boxed{\frac{T_\nu}{T_\gamma}=\left(\frac4{11}\right)^{1/3}}.
$$

This instantaneous-decoupling calculation neglects the small reheating correction from non-instantaneous neutrino decoupling.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Photons are [bosons](../../../quantum-mechanics.md#boson) with two polarizations and temperature $T$, so $\rho_\gamma=(\pi^2/30)2T^4$. Each relativistic neutrino species includes a neutrino and antineutrino helicity state, is fermionic, and has temperature $T_\nu=(4/11)^{1/3}T$. Consequently

$$
\rho_\nu=\frac{\pi^2}{30}
\frac78\,2N_{\rm eff}T_\nu^4.
$$

Adding the two contributions gives the defining expression for the [effective number of neutrino species](../../../cosmology.md#effective-number-of-neutrino-species):

$$
\boxed{\rho_r=\frac{\pi^2}{30}\left[
2+\frac78\times2\times
\left(\frac4{11}\right)^{4/3}N_{\rm eff}
\right]T^4}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

After the real scalar decouples at $T_d$, its temperature redshifts as $a^{-1}$. The other particles continue sharing entropy. Just before standard-neutrino decoupling their entropy degrees of freedom are

$$
g_{*s}(T_{\nu,\rm dec})=2+\frac78(4+6)=\frac{43}{4}.
$$

The [temperature of a decoupled relativistic relic](../../../cosmology.md#temperature-of-a-decoupled-relativistic-relic) therefore obeys

$$
\frac{T_s}{T_\nu}
=\left[\frac{43/4}{g_{*s}(T_d)}\right]^{1/3}.
$$

A real scalar has one bosonic degree of freedom, whereas one effective neutrino species has energy weight $(7/8)\times2=7/4$. Hence the [contribution of a decoupled real scalar to Neff](../../../cosmology.md#contribution-of-a-decoupled-real-scalar-to-neff) is

$$
\boxed{\Delta N_{\rm eff}
=\frac47\left[\frac{43}{4g_{*s}(T_d)}\right]^{4/3}}.
$$

Here $g_{*s}(T_d)$ counts the other particles still coupled to the thermal bath, as specified in the question.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The measurement cannot definitively exclude the model. If only Standard Model particles supplied entropy at scalar decoupling, the largest available value $g_{*s}=106.75$ would give

$$
\Delta N_{\rm eff}
=\frac47\left(\frac{43}{4\times106.75}\right)^{4/3}
\simeq0.027,
$$

which a $0.1\%$ measurement around the Standard Model value would clearly detect.

In the proposed model, however, the many additional relativistic species are also in equilibrium when the scalar decouples. They increase $g_{*s}(T_d)$, and their later disappearance transfers entropy to the coupled bath but not to the scalar. Since $\Delta N_{\rm eff}\propto g_{*s}(T_d)^{-4/3}$, a sufficiently large hidden particle content can dilute the scalar signal below any stated finite precision; a value above roughly $g_{*s}(T_d)\sim550$ already pushes it below about $0.003$. The null measurement constrains the combination of decoupling time and total entropy degrees of freedom, but does not rule out the entire new-physics model.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

During matter domination, pressureless matter has $\bar P_m=\delta P_m=0$. On subhorizon scales the time derivative of the [Newtonian gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge) potential is negligible, so the continuity and Euler equations reduce to

$$
\delta_m'=-\nabla\mathbin\cdot\mathbf v,
\qquad
\mathbf v'+\mathcal H\mathbf v=-\nabla\Phi.
$$

Taking the divergence of the second equation, differentiating the first, and using the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) gives

$$
\delta_m''+\mathcal H\delta_m'
-4\pi Ga^2\bar\rho_m\delta_m=0.
$$

Since $d/d\tau=a,d/dt$, one has

$$
\delta_m'=a\dot\delta_m,
\qquad
\delta_m''=a^2(\ddot\delta_m+H\dot\delta_m),
\qquad
\mathcal H=aH.
$$

Division by $a^2$ yields the standard [linear cosmological density perturbation](../../../linear-cosmological-density-perturbation.md) equation

$$
\boxed{\ddot\delta_m+2H\dot\delta_m
-4\pi G\bar\rho_m\delta_m=0}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

During matter domination, $a\propto t^{2/3}$ and $4\pi G\bar\rho_m=2/(3t^2)$. Trying $\delta_m\propto t^p$ gives

$$
p(p-1)+\frac43p-\frac23=0,
$$

whose roots are $p=2/3$ and $p=-1$. Thus the [cosmic-time matter density modes](../../../linear-cosmological-density-perturbation.md#cosmic-time-matter-density-modes) are

$$
\boxed{\delta_m=C_+a+C_-a^{-3/2}}.
$$

During asymptotic [cosmological constant energy](../../../cosmology.md#cosmological-constant) domination, $H$ is constant and $\bar\rho_m$ is negligible, so

$$
\ddot\delta_m+2H\dot\delta_m=0.
$$

The [matter density modes during cosmological-constant domination](../../../linear-cosmological-density-perturbation.md#matter-density-modes-during-cosmological-constant-domination) are therefore

$$
\boxed{\delta_m=C_1+C_2e^{-2Ht}=C_1+C_2a^{-2}}.
$$

The growing matter-era solution freezes to a constant.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use $d/dt=aH,d/da$. Then

$$
\dot\delta_m=aH\frac{d\delta_m}{da},
$$



$$
\ddot\delta_m=a^2H^2\frac{d^2\delta_m}{da^2}
+aH(H+aH')\frac{d\delta_m}{da},
$$

where now $H'=dH/da$. Also

$$
4\pi G\bar\rho_m
=\frac32\Omega_{m,0}H_0^2a^{-3}.
$$

Substitution into part (a) and division by $a^2H^2$ gives the [matter growth equation as a function of scale factor](../../../linear-cosmological-density-perturbation.md#matter-growth-equation-as-a-function-of-scale-factor)

$$
\boxed{
\frac{d^2\delta_m}{da^2}
+\left(\frac{d\log H}{da}+\frac3a\right)
\frac{d\delta_m}{da}
-\frac{3\Omega_{m,0}H_0^2}{2a^5H^2}\delta_m=0}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For matter plus a cosmological constant,

$$
H^2=H_0^2(\Omega_{m,0}a^{-3}+\Omega_{\Lambda,0}).
$$

Set $\delta_m=Hu$. Substitution into the equation from part (c) makes the coefficient of $u$ vanish by the Friedmann relation and leaves

$$
u''+\left(3\frac{H'}H+\frac3a\right)u'=0,
$$

or

$$
\frac d{da}(a^3H^3u')=0.
$$

Therefore the two independent modes can be written

$$
\delta_m=C_1H(a)+C_2H(a)
\int^a\frac{da'}{a'^3H(a')^3}.
$$

The first is the decaying mode. Normalizing the second to $D_+(a)\sim a$ at early times gives the [integral linear growth factor in a matter-Lambda universe](../../../linear-cosmological-density-perturbation.md#integral-linear-growth-factor-in-a-matter-lambda-universe)

$$
\boxed{D_+(a)=\frac52\Omega_{m,0}H_0^2H(a)
\int_0^a\frac{da'}{a'^3H(a')^3}}.
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

**Yes.** A perturbation of amplitude $A$ at CMB decoupling must grow by at least $A^{-1}$ before becoming nonlinear. During matter domination $\delta_m\propto a$, but once $\rho_\Lambda$ dominates, the [suppression of matter growth by smooth accelerated expansion](../../../linear-cosmological-density-perturbation.md#suppression-of-matter-growth-by-smooth-accelerated-expansion) makes the growth approach a finite limit. Increasing $\rho_\Lambda$ moves this freeze-out to an earlier scale factor and eventually prevents $\delta_m$ from reaching unity.

For an order-of-magnitude bound, matter growth would reach unity at

$$
a_{\rm coll}\sim\frac{a_{\rm dec}}A.
$$

Requiring matter still to dominate then gives the [galaxy-formation bound on the cosmological constant](../../../linear-cosmological-density-perturbation.md#galaxy-formation-bound-on-the-cosmological-constant)

$$
\boxed{\rho_\Lambda\lesssim\rho_m(a_{\rm coll})
\sim A^3\rho_m(a_{\rm dec})}.
$$

The exact upper limit follows by imposing $A D_+(\infty)/D_+(a_{\rm dec})\gtrsim1$ with the integral growth factor and an appropriate nonlinear-collapse threshold.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) obey the canonical bosonic commutation relations

$$
\boxed{[\hat a_{\mathbf k},\hat a^\dagger_{\mathbf k'}]
=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k')},
$$



$$
\boxed{[\hat a_{\mathbf k},\hat a_{\mathbf k'}]
=[\hat a^\dagger_{\mathbf k},\hat a^\dagger_{\mathbf k'}]=0},
\qquad \hat a_{\mathbf k}|0\rangle=0.
$$

Since $\delta\phi=\hat f/a$, the vacuum [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) is

$$
\langle0|\delta\phi(\tau,\mathbf x)
\delta\phi(\tau,\mathbf x+\mathbf r)|0\rangle
=\frac1{a^2}\int\frac{d^3k}{(2\pi)^3}|f_k(\tau)|^2e^{-i\mathbf k\cdot\mathbf r}.
$$

For

$$
f_k=\frac{e^{-ik\tau}}{\sqrt{2k}}
\left(1-\frac{i}{k\tau}\right),
$$

one has $|f_k|^2=(1+1/(k^2\tau^2))/(2k)$. Comparison with the definition of the dimensionless [power spectrum](../../../probability-and-statistics.md#power-spectrum) gives

$$
\Delta_{\delta\phi}^2
=\frac{k^3}{2\pi^2a^2}|f_k|^2
=\frac{H^2}{4\pi^2}(1+k^2\tau^2),
$$

where $a=-1/(H\tau)$. On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), $k\ll aH$ or $|k\tau|\ll1$, and therefore

$$
\boxed{\Delta_{\delta\phi}^2=\left(\frac{H}{2\pi}\right)^2}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The right-hand side of the [slow-roll curvature power spectrum](../../../cosmic-inflation.md#slow-roll-curvature-power-spectrum) must be evaluated separately for each mode at [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $k=aH$. Taking logarithms gives

$$
\log\Delta_{\mathcal R}^2=2\log H-\log\epsilon+\text{constant}.
$$

For $N=\log a$,

$$
\frac{d\log H}{dN}=-\epsilon,
\qquad
\frac{d\log\epsilon}{dN}=\eta,
\qquad
\frac{d\log k}{dN}=1-\epsilon.
$$

Hence

$$
n_s-1
=\frac{-2\epsilon-\eta}{1-\epsilon}
=\boxed{-2\epsilon-\eta+O(\epsilon^2,\epsilon\eta)}.
$$

This is the [scalar spectral index in Hubble slow-roll parameters](../../../cosmic-inflation.md#scalar-spectral-index-in-hubble-slow-roll-parameters).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

At horizon exit, the [primordial tensor power spectrum](../../../cosmic-inflation.md#primordial-tensor-power-spectrum) is proportional to $H^2$. Therefore

$$
n_T=\frac{d\log\Delta_t^2}{d\log k}
=\frac{-2\epsilon}{1-\epsilon}
=-2\epsilon+O(\epsilon^2).
$$

Thus

$$
\boxed{C=2}.
$$

The ratio of the stated tensor and scalar spectra is

$$
r=\frac{8M_{\rm Pl}^{-2}(H/2\pi)^2}
{(2\epsilon M_{\rm Pl}^2)^{-1}(H/2\pi)^2}
=16\epsilon.
$$

Eliminating $\epsilon$ gives the [single-field inflation consistency relation](../../../cosmic-inflation.md#single-field-inflation-consistency-relation)

$$
\boxed{r=-8n_T}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For a canonical scalar field with positive kinetic energy, the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
\dot H=-\frac{\dot\phi^2}{2M_{\rm Pl}^2}\leq0,
$$

so the [first Hubble slow-roll parameter](../../../cosmic-inflation.md#first-hubble-slow-roll-parameter) satisfies $\epsilon\geq0$. The tensor tilt is consequently

$$
n_T=-2\epsilon\leq0.
$$

A [blue primordial spectrum](../../../cosmic-inflation.md#blue-primordial-spectrum) of tensor modes cannot arise in standard canonical single-field slow-roll inflation; it requires changing assumptions, such as the matter content, kinetic structure, initial state, or gravitational dynamics.

The scalar tilt instead obeys

$$
n_s-1=-2\epsilon-\eta.
$$

It can be positive in a standard single-field model if $\eta<-2\epsilon$, meaning that $\epsilon$ decreases sufficiently rapidly with the number of e-folds. Equivalently, in potential slow-roll parameters the first-order condition is $2\eta_V>6\epsilon_V$. Thus a blue scalar spectrum is allowed by the framework, although it is not produced by every slowly rolling potential.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
