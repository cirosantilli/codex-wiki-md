# Paper 48

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_48.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_48.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Assume positive fluid density, $\rho_0>0$, and write $m=1+3w>0$. A [perfect fluid](../../../general-relativity.md#perfect-fluid) with constant [equation of state](../../../thermodynamics.md#equation-of-state) obeys the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation), giving

$$
\dot\rho+3H(\rho+P)=0,\qquad\rho=\rho_0a^{-3(1+w)}.
$$

In the stated units the [Friedmann equation](../../../cosmology.md#friedmann-equations) is $H^2=\rho/3-k/a^2+\Lambda/3$. Multiplication by $a^2/2$ yields the [Friedmann effective potential for a constant-equation-of-state fluid](../../../cosmology.md#friedmann-effective-potential-for-a-constant-equation-of-state-fluid),

$$
\boxed{\tfrac12\dot a^2+V(a)=0,\qquad V(a)=-\frac{\rho_0}{6}a^{-m}+\frac{k}{2}-\frac{\Lambda}{6}a^2}.
$$

The allowed region has $V\leq0$. The [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) is equivalently $\ddot a=-V'(a)$, including turning points by continuity. Thus a zero-energy mechanical trajectory reproduces the cosmological evolution, with $a>0$.

For $k=0$, $\Lambda<0$, the potential increases strictly from negative infinity to positive infinity. Its unique zero gives

$$
\boxed{a_{\max}=\left(\frac{\rho_0}{|\Lambda|}\right)^{1/[3(1+w)]}}.
$$

Expansion from the [Big Bang](../../../cosmology.md#big-bang) stops there, with negative acceleration, then reverses into a [Big Crunch](../../../cosmology.md#big-crunch). Both the turning point and the final singularity occur in finite [proper time](../../../special-relativity.md#proper-time): $dt=da/\sqrt{-2V}$ is integrable near a simple turning point and behaves as a constant times $a^{m/2}da$ near zero.

For $\Lambda=0$, $k=+1$, $V$ increases from negative infinity to $1/2$ and crosses zero at

$$
\boxed{a_{\max}=\left(\frac{\rho_0}{3}\right)^{1/(1+3w)}}.
$$

This is again expansion followed by finite-time recollapse. For $k=-1$, the same increasing curve has asymptote $-1/2$ and never meets zero. Expansion continues without a finite maximum; asymptotically $\dot a\to1$ and $a\sim t$, as spatial curvature dominates the diluted fluid.

For $k=0$, $\Lambda>0$, $V$ tends to negative infinity at both ends. It has a maximum at

$$
a_*^{m+2}=\frac{m\rho_0}{2\Lambda},\qquad
V(a_*)=-\frac{(m+2)\rho_0}{12}a_*^{-m}<0.
$$

There is no turning point. Expansion initially decelerates, then accelerates once $a>a_*$, and approaches [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) expansion $a\propto e^{\sqrt{\Lambda/3}\,t}$. Thus **positive flat dark-energy expansion is unbounded; negative flat dark energy and positive curvature without dark energy recollapse**.

<a id="1/a/image-zero-energy-friedmann-potentials-showing-recollapse-curvature-dominated-expansion-and-positive-cosmological-constant-expansion"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-48-friedmann-potentials.png)

**[Figure 1](#1/a/image-zero-energy-friedmann-potentials-showing-recollapse-curvature-dominated-expansion-and-positive-cosmological-constant-expansion). Zero-energy Friedmann potentials showing recollapse, curvature-dominated expansion and positive-cosmological-constant expansion**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use [conformal time](../../../cosmology.md#conformal-time), $dt=a\,d\tau$, and let primes mean $d/d\tau$. Then $a'=a\dot a$ and $a''=a\dot a^2+a^2\ddot a$. For $k=1$, $\Lambda=0$, the [Friedmann equation](../../../cosmology.md#friedmann-equations) and acceleration equation give

$$
\dot a^2=\frac{\rho_0}{3}a^{-(1+3w)}-1,\qquad
\ddot a=-\frac{\rho_0}{6}(1+3w)a^{-(2+3w)}.
$$

Substitution yields

$$
\boxed{a''+a=\frac{\rho_0}{6}(1-3w)a^{-3w}}.
$$

Use the supplied solution without deriving it. Its first maximum has sine equal to one, so its amplitude must equal the physical turnaround scale in part (a):

$$
\boxed{A=\left(\frac{\rho_0}{3}\right)^{1/(1+3w)}}.
$$

Choose the expanding branch with $B=0$ and the first zero at $\tau=0$.

For [pressureless matter](../../../cosmology.md#pressureless-matter), $w=0$, the [closed matter-dominated Friedmann solution](../../../cosmology.md#closed-matter-dominated-friedmann-solution) is

$$
\boxed{a(\tau)=A\sin^2(\tau/2)=\frac A2(1-\cos\tau),\quad
 t(\tau)=\frac A2(\tau-\sin\tau),\quad A=\rho_0/3}.
$$

The [Big Crunch](../../../cosmology.md#big-crunch) is at $\tau_c=2\pi$, or [proper time](../../../special-relativity.md#proper-time) $t_c=\pi A=\pi\rho_0/3$, measured from the [Big Bang](../../../cosmology.md#big-bang).

For radiation, $w=1/3$, the [closed radiation-dominated Friedmann solution](../../../cosmology.md#closed-radiation-dominated-friedmann-solution) is

$$
\boxed{a(\tau)=A\sin\tau,\quad t(\tau)=A(1-\cos\tau),\quad A=\sqrt{\rho_0/3}}.
$$

The [Big Crunch](../../../cosmology.md#big-crunch) is at $\tau_c=\pi$, or $t_c=2A$.

A [radial null geodesic in FLRW spacetime](../../../cosmology.md#radial-null-geodesic-in-flrw-spacetime) obeys $d\chi/d\tau=\pm1$. The spatial slice is a unit three-sphere times $a$, so a great circle has comoving circumference $2\pi$. The dust lifetime supplies conformal distance $2\pi$: **one circumference, with the return occurring only in the crunch limit**. Strictly before the singular endpoint no full return is completed. The radiation lifetime supplies conformal distance $\pi$: **the [photon](../../../quantum-mechanics.md#photon) reaches the antipode, half a great circle, in the crunch limit**. These are limiting null rays from near the initial singularity, not [photons](../../../quantum-mechanics.md#photon) at a regular event on the singular surface.

## 2

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the reaction $p+e\leftrightarrow H+\gamma$, [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) requires $\mu_p+\mu_e=\mu_H$ because thermal [photons](../../../quantum-mechanics.md#photon) have zero [chemical potential](../../../thermodynamics.md#chemical-potential). Insert the nonrelativistic [Maxwell-Boltzmann distribution](../../../statistical-physics.md#maxwell-boltzmann-distribution) number densities and use $m_H=m_p+m_e-\mathcal B$:

$$
\frac{n_en_p}{n_H}=\frac{g_eg_p}{g_H}\left(\frac{m_em_p}{m_H}\frac{T}{2\pi}\right)^{3/2}e^{-\mathcal B/T}.
$$

For ground-state [hydrogen](../../../chemistry.md#hydrogen), including its spin states, $g_e=g_p=2$, $g_H=4$; hence the degeneracy factor is one. Since $m_p/m_H\simeq1$, the right side is $(m_eT/2\pi)^{3/2}e^{-\mathcal B/T}$.

Charge neutrality gives $n_p=n_e$, while baryon conservation gives $n_b=n_p+n_H$. Consequently $n_e=n_p=X_en_b$ and $n_H=(1-X_e)n_b$. Inverting the preceding ratio and inserting the [photon number density](../../../statistical-physics.md#photon-number-density) with $n_b=\eta n_\gamma$ gives the [hydrogen-only Saha equation](../../../cosmology.md#hydrogen-only-saha-equation)

$$
\boxed{\frac{1-X_e}{X_e^2}=\frac{2\zeta(3)}{\pi^2}\eta\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{\mathcal B/T}}.
$$

Writing $y=\mathcal B/T$, its coefficient is $(2\zeta(3)/\pi^2)\eta(2\pi\mathcal B/m_e)^{3/2}\simeq3.2\times10^{-16}$, consistent with the rounded $3\times10^{-16}$. The negligible mass-ratio correction and ground-state approximation are the assumptions behind this form.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

At $X_e=1/2$, the left side of the [Saha equation](../../../cosmology.md#saha-ionization-equation) is two. With its rounded coefficient, the [recombination temperature](../../../cosmology.md#recombination-temperature) therefore satisfies

$$
2=3\times10^{-16}\frac{e^y}{y^{3/2}},\qquad
 y-\frac32\ln y=\ln\left(\frac23\times10^{16}\right)\simeq36.
$$

Neglecting the logarithmic prefactor gives $y\sim36$ and

$$
\boxed{T_{\rm rec}\sim13.6/36\ {
m eV}\sim0.4\ {
m eV}}.
$$

This is the requested rough scale. Retaining the prefactor and the unrounded logarithm gives $y\simeq42.0$ and $T_{\rm rec}\simeq0.32$ eV; the displayed $0.4$ eV is not a high-accuracy numerical root of the [Saha equation](../../../cosmology.md#saha-ionization-equation).

The small [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) means that radiation and the entropy of the free charged particles strongly favor [ionization](../../../physics.md#ionization). A low mean [photon](../../../quantum-mechanics.md#photon) energy does not eliminate the energetic tail, and ionized particles have a large phase-space advantage. The exponential binding factor must become very large before neutral atoms dominate this dilute gas. Accordingly $\mathcal B/T$ is of order forty rather than order one, so **recombination occurs well below the [hydrogen](../../../chemistry.md#hydrogen) binding energy**.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

[Photon decoupling](../../../cosmology.md#photon-decoupling) is a dynamical loss of frequent scattering, distinct from the chemical conversion of charged particles into neutral atoms. Before recombination, [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) on free [Electrons](../../../physics.md#electron) keeps [photons](../../../quantum-mechanics.md#photon) coupled to the baryon plasma. The physical scattering rate is

$$
\Gamma_\gamma=n_e\sigma_T=X_en_b\sigma_T,
$$

in units with $c=1$. Define the approximate decoupling [temperature](../../../thermodynamics.md#temperature) by

$$
\boxed{\Gamma_\gamma(T_{\rm dec})\simeq H(T_{\rm dec})}.
$$

Equivalently the [photon](../../../quantum-mechanics.md#photon) mean scattering time becomes comparable to an expansion time. A refined last-scattering definition uses the optical depth and the maximum of the visibility function; it need not coincide exactly with the local rate criterion. As $X_e$ falls, scattering becomes inefficient, ordinarily after the half-ionized recombination stage, so $T_{\rm dec}<T_{\rm rec}$.

[Residual electron freeze-out](../../../cosmology.md#residual-electron-freeze-out) concerns the remaining ionized fraction. The [Saha equation](../../../cosmology.md#saha-ionization-equation) presumes sufficiently rapid forward and reverse reactions to maintain [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium). Real recombination is slowed by radiative bottlenecks and expansion; the free-electron fraction can therefore exceed its equilibrium value. Eventually the effective recombination rate per free [Electron](../../../physics.md#electron), roughly $\alpha_{\rm eff}(T)n_e$, falls below $H$. The remaining [Electrons](../../../physics.md#electron) cannot all find and recombine with [protons](../../../physics.md#proton) within an expansion time. A small nonzero residual fraction survives while the Saha prediction decreases exponentially toward zero.

The sketch shows this lag and residual floor. Its kinetic curve and the position of the decoupling marker are schematic: the data supplied determine the equilibrium curve, but not a quantitative recombination history or an exact $T_{\rm dec}$. Determining those needs the expansion history and atomic transition rates. The horizontal axis decreases toward the right to follow cosmological cooling.

<a id="2/c/image-saha-equilibrium-and-a-schematic-delayed-recombination-curve-with-recombination-and-photon-decoupling-temperatures-marked-during-cooling"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-48-recombination-sketch.png)

**[Figure 2](#2/c/image-saha-equilibrium-and-a-schematic-delayed-recombination-curve-with-recombination-and-photon-decoupling-temperatures-marked-during-cooling). Saha equilibrium and a schematic delayed recombination curve, with recombination and photon-decoupling temperatures marked during cooling**.

## 3

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Differentiate the [linearized cosmological continuity equation](../../../linear-cosmological-density-perturbation.md#linearized-cosmological-continuity-equation), remembering the [derivative](../../../calculus.md#derivative) of $1/a$:

$$
\ddot\delta_m=\frac{H}{a}\nabla\cdot\mathbf v_m-\frac1a\nabla\cdot\dot{\mathbf v}_m.
$$

Insert the linear [cosmological Euler equation](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation) for the [peculiar velocity](../../../cosmology.md#peculiar-velocity), giving

$$
\ddot\delta_m=\frac{2H}{a}\nabla\cdot\mathbf v_m+\frac1{a^2}\nabla^2\Phi
=-2H\dot\delta_m+4\pi G\bar\rho_m\delta_m.
$$

Thus the [linear matter perturbation growth equation](../../../linear-cosmological-density-perturbation.md#linear-matter-perturbation-growth-equation) is

$$
\boxed{\ddot\delta_m+2H\dot\delta_m-4\pi G\bar\rho_m\delta_m=0}.
$$

The factor $2H$ includes one expansion term from continuity and one from momentum dilution. This equation uses sub-Hubble, pressureless linear perturbations and the stated matter-only source for the [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Change independent variable from [proper time](../../../special-relativity.md#proper-time) to the [scale factor](../../../cosmology.md#scale-factor-cosmology). Then $\dot\delta=\dot a\delta_a$ and $\ddot\delta=\dot a^2\delta_{aa}+\ddot a\delta_a$. Under [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), $\ddot a=-\dot a^2/a$ and $H^2\simeq8\pi G\bar\rho_r/3$. Since $\bar\rho_m/\bar\rho_r=a/a_{\rm eq}$, the [linear matter perturbation growth equation](../../../linear-cosmological-density-perturbation.md#linear-matter-perturbation-growth-equation) becomes

$$
\delta_{aa}+\frac1a\delta_a-\frac{3}{2aa_{\rm eq}}\delta=0.
$$

Putting $\delta=au$ gives

$$
\boxed{u_{aa}+\frac3a u_a+\frac1{a^2}\left(1-\frac32\frac a{a_{\rm eq}}\right)u=0}.
$$

This keeps the matter self-gravity term in a radiation-dominated background. It is not an exact background equation through radiation-matter equality.

At $a/a_{\rm eq}\ll1$, neglecting that small term gives $\delta_{aa}+\delta_a/a=0$. Integration yields

$$
\boxed{\delta_m=C_1+C_2\ln(a/a_*),\qquad u=[C_1+C_2\ln(a/a_*)]/a}.
$$

Thus matter has at most logarithmic growth during this leading radiation approximation, together with a constant independent mode. The constant is non-growing, not a mode that literally falls as $a^{-1}$; that power belongs to $u$ rather than $\delta_m$.

For an increasing/decreasing basis of the displayed equation with matter self-gravity retained, put $x=\sqrt{6a/a_{\rm eq}}$. Its equation becomes $x^2\delta_{xx}+x\delta_x-x^2\delta=0$. Hence

$$
\boxed{\delta_+=I_0(x),\qquad\delta_-=K_0(x)}.
$$

The [Modified Bessel function of the first kind](../../../analysis.md#modified-bessel-function-of-the-first-kind) gives $I_0(x)=1+3a/(2a_{\rm eq})+O((a/a_{\rm eq})^2)$, which increases slowly. The [Modified Bessel function of the second kind](../../../analysis.md#modified-bessel-function-of-the-second-kind) gives $K_0(x)=-\tfrac12\ln(a/a_{\rm eq})+\tfrac12\ln(2/3)-\gamma_E+O((a/a_{\rm eq})|\ln(a/a_{\rm eq})|)$, where $\gamma_E$ is [Euler's constant](../../../complex-analysis.md#euler-s-constant); this mode decreases as $a$ increases. Their leading span is precisely the constant/logarithmic pair above. Mode labels depend on the chosen basis and normalization; no rapid matter-era growth $\delta\propto a$ occurs here. Neglected background corrections can change subleading terms, so the Bessel basis should not be extrapolated through equality.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $u=\delta_m/H$. The supplied equation has integrating factor $(aH)^3$:

$$
\frac d{da}\bigl[(aH)^3u_a\bigr]=0.
$$

Consequently the [integral linear growth factor in a matter-Lambda universe](../../../linear-cosmological-density-perturbation.md#integral-linear-growth-factor-in-a-matter-lambda-universe) gives the two independent solutions

$$
\boxed{\delta_m=C_1H(a)+C_2H(a)\int_{a_i}^a\frac{d\widetilde a}{[\widetilde aH(\widetilde a)]^3}}.
$$

The first is the conventional matter-era decaying mode. A finite lower limit in the second fixes a decaying admixture; adding a multiple of $H$ can choose a pure growing normalization.

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), write $H=h\,a^{-3/2}$. The [integral](../../../calculus.md#integral) solution is

$$
H\int_{a_i}^a\frac{d\widetilde a}{(\widetilde aH)^3}
=\frac{2}{5h^2}\left(a-a_i^{5/2}a^{-3/2}\right).
$$

Removing the second term by the independent $H$ solution gives the [matter-era linear growth factor](../../../linear-cosmological-density-perturbation.md#matter-era-linear-growth-factor)

$$
\boxed{\delta_{\rm grow}\propto a,\qquad\delta_{\rm decay}\propto a^{-3/2}}.
$$

For positive [cosmological constant](../../../cosmology.md#cosmological-constant) at sufficiently late times, $H\to H_\Lambda>0$. The integrand approaches $H_\Lambda^{-3}a^{-3}$, whose tail is integrable. Therefore

$$
\boxed{\delta_{\rm grow}(a)\longrightarrow\text{a finite constant as }a\to\infty}.
$$

Its remaining approach has leading $a^{-2}$ behavior for the usual matter-plus-Lambda background. Growth of structure freezes rather than continuing as $a$. The basis function $H$ also approaches a constant; subtracting a suitable multiple of it isolates a genuinely decaying late-time solution $\propto a^{-2}$. The name “decaying mode” for $H$ refers to its matter-era behavior.

## 4

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use primes for conformal-time [derivatives](../../../calculus.md#derivative) in this question, reserving $V_{,\phi\phi}$ for a potential [derivative](../../../calculus.md#derivative). The [inflaton](../../../cosmic-inflation.md#inflaton) background obeys $(a^2\bar\phi')'+a^4V_{,\phi}=0$, so the linear variation of its action vanishes up to boundary terms. With $\delta\phi=f/a$, the [conformal-time quadratic action for an inflaton perturbation](../../../cosmic-inflation.md#conformal-time-quadratic-action-for-an-inflaton-perturbation) is initially

$$
S^{(2)}=\frac12\int d\tau\,d^3x\left[(f'-\mathcal Hf)^2-(\nabla f)^2-a^2V_{,\phi\phi}f^2\right],\qquad\mathcal H=a'/a.
$$

The cross term $-\mathcal H(f^2)'$ integrates to $\mathcal H'f^2$. Since $\mathcal H'+\mathcal H^2=a''/a$, this becomes

$$
\boxed{S^{(2)}=\frac12\int d\tau\,d^3x\left[f'^2-(\nabla f)^2+\left(\frac{a''}a-a^2V_{,\phi\phi}\right)f^2\right]}.
$$

Varying $f$ gives $f''-\nabla^2f+(a^2V_{,\phi\phi}-a''/a)f=0$. The symmetric [Fourier transform](../../../analysis.md#fourier-transform) convention used in the question turns $-\nabla^2$ into $k^2$. Dropping the small mass term under the stated [slow-roll inflation](../../../cosmic-inflation.md#slow-roll-approximation) assumption yields

$$
\boxed{f_{\mathbf k}''+\left(k^2-\frac{a''}a\right)f_{\mathbf k}=0}.
$$

For [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime), $a=-1/(H\tau)$ with $\tau<0$, so $a''/a=2/\tau^2$. The rescaled field has a canonical kinetic term; $f$ rather than $\delta\phi$ is therefore the convenient oscillator variable.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Promote the canonical field and momentum $\pi=f'$ to operators satisfying the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation), $[\hat f(\tau,\mathbf x),\hat\pi(\tau,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$. A real field has Fourier reality condition $\hat f_{\mathbf k}^\dagger=\hat f_{-\mathbf k}$. Its oscillator expansion is

$$
\boxed{\hat f_{\mathbf k}=u_k\hat a_{\mathbf k}+u_k^*\hat a_{-\mathbf k}^\dagger}.
$$

The [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) add or remove excitations in the selected mode basis, with

$$
[\hat a_{\mathbf k},\hat a_{\mathbf k'}^\dagger]=\delta^{(3)}(\mathbf k-\mathbf k'),\qquad
[\hat a_{\mathbf k},\hat a_{\mathbf k'}]=[\hat a_{\mathbf k}^\dagger,\hat a_{\mathbf k'}^\dagger]=0,\qquad
\hat a_{\mathbf k}|0\rangle=0.
$$

Canonical normalization requires the [Wronskian](../../../differential-equation.md#wronskian) $u_ku_k^{*\prime}-u_k^*u_k'=i$.

For the [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum), choose the positive-frequency short-wavelength behavior $u_k\sim e^{-ik\tau}/\sqrt{2k}$ as $k|\tau|\to\infty$. For the proposed solution, direct differentiation gives

$$
u_k'=\frac{e^{-ik\tau}}{\sqrt{2k}}\left[-ik-\frac1\tau+\frac{i}{k\tau^2}\right],\qquad
u_k''=\frac{e^{-ik\tau}}{\sqrt{2k}}\left[-k^2+\frac{ik}\tau+\frac2{\tau^2}-\frac{2i}{k\tau^3}\right].
$$

Substitution cancels every term in $u_k''+(k^2-2/\tau^2)u_k$. Its [Wronskian](../../../differential-equation.md#wronskian) is $i$, and its large-$|k\tau|$ limit is the required flat-spacetime positive-frequency mode. Thus

$$
\boxed{u_k=\frac{e^{-ik\tau}}{\sqrt{2k}}\left(1-\frac{i}{k\tau}\right)}.
$$

A term with the conjugate frequency is another allowed classical solution, but would describe a different quantum state, through a [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation). Its coefficient is set to zero by the early-time vacuum condition, not by absence of a second solution to the differential equation.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The annihilation operators kill the vacuum, and their commutator gives

$$
\langle0|\delta\hat\phi_{\mathbf k}^\dagger\delta\hat\phi_{\mathbf k'}|0\rangle
=\frac{|u_k|^2}{a^2}\delta^{(3)}(\mathbf k-\mathbf k')
=\frac{H^2}{2k^3}(1+k^2\tau^2)\delta^{(3)}(\mathbf k-\mathbf k').
$$

Therefore the [scale-invariant inflationary power spectrum](../../../cosmic-inflation.md#scale-invariant-inflationary-power-spectrum) has the superhorizon limit

$$
\boxed{\langle\delta\hat\phi_{\mathbf k}^\dagger\delta\hat\phi_{\mathbf k'}\rangle
\longrightarrow\frac{H^2}{2k^3}\delta^{(3)}(\mathbf k-\mathbf k'),\qquad
\Delta_{\delta\phi}^2=\frac{k^3}{2\pi^2}\frac{H^2}{2k^3}=\left(\frac H{2\pi}\right)^2}.
$$

The canonical mode grows as $1/|\tau|$ outside the [Hubble radius](../../../cosmology.md#hubble-radius), while the physical field perturbation $f/a$ freezes. A slowly varying $H$ produces an almost scale-invariant spectrum rather than exact scale invariance.

For a slowly rolling single field, fluctuations in the [inflaton](../../../cosmic-inflation.md#inflaton) clock become the [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation), $\mathcal R\simeq-H\delta\phi/\dot{\bar\phi}$ up to sign convention. Restoring the [reduced Planck mass](../../../physics.md#reduced-planck-mass) and using $\epsilon=\dot{\bar\phi}^{\,2}/(2M_{\rm pl}^2H^2)$ gives

$$
\boxed{\Delta_{\mathcal R}^2\simeq\frac{H^2}{8\pi^2\epsilon M_{\rm pl}^2}}.
$$

This conversion presumes nonzero background roll; a strictly constant test scalar in exact de Sitter spacetime does not by itself define a finite [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) through this formula. The curvature perturbations seed the later density fluctuations.

When metric fluctuations and their Einstein-gravity normalization are restored, the two graviton polarizations have the same massless mode equation. The usual total [primordial tensor power spectrum](../../../cosmic-inflation.md#primordial-tensor-power-spectrum) is $\Delta_t^2=2H^2/(\pi^2M_{\rm pl}^2)$, so the single-field leading ratio is $r=16\epsilon$. Tensor amplitudes therefore probe the inflationary energy scale, whereas scalar amplitudes also depend on the roll rate. These tensor statements explain the relevance of the mode result; they are not derived from a scalar action with metric perturbations omitted.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
