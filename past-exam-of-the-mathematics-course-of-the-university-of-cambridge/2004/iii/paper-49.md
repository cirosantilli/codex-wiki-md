# Paper 49

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper49.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper49.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use a mostly-plus target [metric tensor](../../../general-relativity.md#metric-tensor) and the standard [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) convention $\alpha_0^\mu=\sqrt{2\alpha'}p^\mu$. The [integer string oscillator level](../../../string-theory.md#integer-string-oscillator-level) is $N=\sum_{n\ge1}\alpha_{-n}\cdot\alpha_n$, whose [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are nonnegative integers. Then $L_0=N+\alpha'p^2$, so the [string mass-shell condition](../../../string-theory.md#string-mass-shell-condition) gives

$$
\boxed{M^2=-p^2=\frac{N-1}{\alpha'}.}
$$

The ground state is a [tachyon](../../../physics.md#tachyon), and the level-one state is massless. The [physical string state](../../../string-theory.md#physical-string-state) conditions in [old covariant string quantization](../../../string-theory.md#old-covariant-string-quantization) are

$$
(L_0-1)|\psi\rangle=0,\qquad L_m|\psi\rangle=0\quad(m>0).
$$

Only the positive-mode [Virasoro constraints](../../../string-theory.md#virasoro-constraint) annihilate a ket; their negative-mode partners annihilate the corresponding bra. Imposing both signs on every ket would contradict the nonzero [Virasoro central extension](../../../string-theory.md#virasoro-central-extension).

The [central charge](../../../string-theory.md#central-charge) comes from [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) the quadratic oscillator expressions. Classically their [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) have no central term. Quantum mechanically, moving [annihilation operators](../../../quantum-mechanics.md#annihilation-operator) through [creation operators](../../../quantum-mechanics.md#creation-operator) produces double contractions. From the oscillator [commutator](../../../lie-algebra.md#commutator) one obtains $[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu$, which gives the noncentral part $(m-n)L_{m+n}$.

The coefficient is fixed by the [free-boson Virasoro central term](../../../string-theory.md#free-boson-virasoro-central-term). On a formal zero-momentum vacuum, for $m>0$,

$$
L_{-m}|0\rangle=\frac12\sum_{r=1}^{m-1}\alpha_{-(m-r)}\cdot\alpha_{-r}|0\rangle.
$$

The two contraction pairings give

$$
\langle0|L_mL_{-m}|0\rangle=\frac D2\sum_{r=1}^{m-1}r(m-r)=\frac D{12}m(m^2-1).
$$

Here $\eta_{\mu\nu}\eta^{\mu\nu}=D$; the time coordinate contributes one, just as each spatial coordinate does. Comparing with the [Virasoro algebra](../../../string-theory.md#virasoro-algebra) proves

$$
\boxed{c_{\rm matter}=D.}
$$

This counts covariant target coordinates. It is distinct from the $D-2$ physical transverse polarizations. Including the [central charge of reparameterization ghosts](../../../string-theory.md#central-charge-of-reparameterization-ghosts) gives $c_{\rm total}=D-26$; cancellation of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) gives the usual [critical dimension of the bosonic string](../../../string-theory.md#critical-dimension-of-string-theory) $D=26$.

A general level-one state is

$$
|\epsilon;k\rangle=\epsilon_\mu\alpha_{-1}^\mu|0;k\rangle.
$$

The zero-mode constraint requires $k^2=0$. Since $[L_1,\alpha_{-1}^\mu]=\alpha_0^\mu$, the remaining nontrivial positive-mode constraint is $k\cdot\epsilon=0$; all $L_m$ with $m\ge2$ act trivially at this level. Thus the [polarization vector](../../../relativistic-quantum-field.md#polarization-vector) is transverse to a nonzero null momentum.

There is also a [null string state](../../../string-theory.md#null-string-state) $L_{-1}|0;k\rangle=\sqrt{2\alpha'}\,k\cdot\alpha_{-1}|0;k\rangle$. It is physical when $k^2=0$ and orthogonal to every physical polarization. The [null-state quotient of a string](../../../string-theory.md#null-state-quotient-of-a-string) therefore identifies

$$
\epsilon\sim\epsilon+\lambda k.
$$

Choose $k=(E,E,0,\ldots,0)$. Transversality sets $\epsilon^1=\epsilon^0$, and the null-state identification removes this common component. The remaining $D-2$ spatial components have positive norm. Hence **the physical level-one states form a massless vector with $D-2$ polarizations**, or 24 at the critical dimension. The removed component is gauge redundancy. States violating the constraints, including independent timelike negative-norm polarizations, are unphysical; physical null states are removed by the quotient rather than counted as additional particles.

## 2

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [string sigma model in a spacetime metric](../../../string-theory.md#string-sigma-model-in-a-spacetime-metric) is the [Polyakov action](../../../string-theory.md#polyakov-action)

$$
S=-\frac T2\int d\tau d\sigma\,\sqrt{-h}\,h^{ab}g_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu,\qquad T=\frac1{2\pi\alpha'}.
$$

Take [conformal gauge](../../../string-theory.md#conformal-gauge) $h_{ab}=\operatorname{diag}(-1,1)$, and choose spatial period $2\pi$ for the [closed string](../../../string-theory.md#closed-string). Substitution of the plane-wave metric gives

$$
S=\frac T2\int d\tau d\sigma\,\left[-2\dot X^+\dot X^-+2X'^+X'^--m^2X^IX^I((\dot X^+)^2-(X'^+)^2)+\dot X^I\dot X^I-X'^IX'^I\right].
$$

The stipulated [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory) $X^+=\tau$ sets $\dot X^+=1$ and $X'^+=0$. Its longitudinal term $-T\int\dot X^-$ is a total time derivative. The transverse [string sigma model in an isotropic plane wave](../../../string-theory.md#string-sigma-model-in-an-isotropic-plane-wave) is therefore

$$
\boxed{S_\perp=\frac T2\int d\tau d\sigma\,\left[\dot X^I\dot X^I-X'^IX'^I-m^2X^IX^I\right],\qquad I=2,\ldots,25.}
$$

The resulting [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) are the massive [wave equations](../../../wave-equation.md)

$$
\boxed{\ddot X^I-X''^I+m^2X^I=0.}
$$

These conventions fix the mass term directly from $X^+=\tau$. More generally $X^+=\kappa\tau$ would replace $m$ by $|m\kappa|$, with $p^+=2\pi T\kappa$ for this spatial period.

Use the real orthonormal [Fourier basis](../../../fourier-series.md#fourier-basis)

$$
f_0(\sigma)=\frac1{\sqrt{2\pi}},\qquad f_{n,c}(\sigma)=\frac{\cos n\sigma}{\sqrt\pi},\qquad f_{n,s}(\sigma)=\frac{\sin n\sigma}{\sqrt\pi},\quad n\ge1.
$$

For the [plane-wave string mode frequencies](../../../string-theory.md#plane-wave-string-mode-frequency), let $\omega_0=|m|$ and $\omega_{n,c}=\omega_{n,s}=\sqrt{n^2+m^2}$. The complete real mode expansion for nonzero frequencies is

$$
\boxed{X^I(\tau,\sigma)=\sum_{a\in\{0,(n,c),(n,s)\}}f_a(\sigma)\left[A_a^I\cos(\omega_a\tau)+B_a^I\sin(\omega_a\tau)\right].}
$$

Every term obeys the [wave equation](../../../wave-equation.md) and is periodic. Orthonormality and completeness let its coefficients match arbitrary appropriate initial position and velocity data. For $m=0$, replace the zero-mode bracket by $q_0^I(0)+\tau p_0^I/T$; the zero mode becomes a free particle rather than an oscillator.

The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) density is $\Pi_I=T\dot X^I$. The transverse [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is

$$
H_\perp=\int_0^{2\pi}d\sigma\left[\frac{\Pi_I\Pi_I}{2T}+\frac T2(X'^IX'^I+m^2X^IX^I)\right].
$$

Write $X^I=\sum_aq_a^If_a$ and $p_a^I=T\dot q_a^I$. Since $\int f_af_b=\delta_{ab}$ and $\int f'_af'_b=n_a^2\delta_{ab}$, substitution gives the [plane-wave string mode Hamiltonian](../../../string-theory.md#plane-wave-string-mode-hamiltonian)

$$
\boxed{H_\perp=\sum_{I,a}\left[\frac{(p_a^I)^2}{2T}+\frac T2\omega_a^2(q_a^I)^2\right]=\frac T2\sum_{I,a}\omega_a^2\left[(A_a^I)^2+(B_a^I)^2\right].}
$$

This is a collection of independent [harmonic oscillators](../../../classical-mechanics.md#simple-harmonic-motion). The last equality follows by substituting the sine-and-cosine time dependence; each oscillator energy is constant.

For canonical quantization of each nonzero-frequency mode, put

$$
q_a^I(\tau)=\frac{a_a^Ie^{-i\omega_a\tau}+a_a^{I\dagger}e^{i\omega_a\tau}}{\sqrt{2T\omega_a}},\qquad[a_a^I,a_b^{J\dagger}]=\delta^{IJ}\delta_{ab}.
$$

Then $H_\perp=\sum_{I,a}\omega_a(a_a^{I\dagger}a_a^I+1/2)$. Opposite travelling-wave oscillator combinations give the equivalent form

$$
H_\perp=|m|\sum_I N_0^I+\sum_{n\ge1,I}\sqrt{n^2+m^2}(N_n^I+\widetilde N_n^I)+E_0,
$$

For $m\ne0$, the formal [zero-point energy](../../../quantum-mechanics.md#zero-point-energy) is $E_0=\tfrac{24}2[|m|+2\sum_{n\ge1}\sqrt{n^2+m^2}]$. At $m=0$, replace the zero-mode occupation term by $\sum_I(p_0^I)^2/(2T)$. The zero-point expression is divergent and needs a regulator or a specified [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) convention; no mass-independent intercept has been assumed.

The remaining [Virasoro constraints](../../../string-theory.md#virasoro-constraint) determine the longitudinal coordinate:

$$
X'^-=\dot X^IX'^I,\qquad\dot X^-=\tfrac12(\dot X^I\dot X^I+X'^IX'^I-m^2X^IX^I).
$$

Periodicity of $X^-$ imposes $\int_0^{2\pi}\Pi_I X'^I\,d\sigma=0$, the [closed-string level matching](../../../string-theory.md#closed-string-level-matching) condition. Labelling the travelling oscillators by their opposite worldsheet momenta gives $\sum_{n\ge1,I}n(N_n^I-\widetilde N_n^I)=0$. The light-cone energy $p^-=-p_+$ equals $T\int(\dot X^-+m^2X^IX^I)\,d\sigma=H_\perp$, consistent with the positive mass term in the Hamiltonian.

This is the classical reduction in the specified background. As a full quantum background with constant [dilaton](../../../string-theory.md#dilaton) and no [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), this metric has $R_{++}=24m^2$ and fails the lowest-order [sigma-model beta function](../../../string-theory.md#sigma-model-beta-function) equation when $m\ne0$; additional background fields would be required for quantum [Weyl invariance](../../../string-theory.md#weyl-transformation).

## 3

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use Euclidean [worldsheet](../../../string-theory.md#worldsheet) conventions with $\epsilon^{12}=1$. Including a target metric, a [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) $B_{\mu\nu}$ and the [dilaton](../../../string-theory.md#dilaton) $\Phi$ gives

$$
\begin{aligned}
S_E={}&\frac1{4\pi\alpha'}\int_\Sigma d^2\sigma\,\sqrt h\,h^{ab}g_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu\\
&+\frac{i}{4\pi\alpha'}\int_\Sigma d^2\sigma\,\epsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu+\frac1{4\pi}\int_\Sigma d^2\sigma\,\sqrt h\,\Phi(X)R^{(2)}.
\end{aligned}
$$

The imaginary coefficient of the antisymmetric term comes from Euclidean continuation; the Lorentzian action has the corresponding real coupling. For constant $\Phi_0$, the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives $S_\Phi=\Phi_0\chi(\Sigma)$, with [Euler characteristic](../../../homology.md#euler-characteristic) $\chi=2-2g$ on a connected closed oriented surface. Thus [dilaton Euler-characteristic weighting](../../../string-theory.md#dilaton-euler-characteristic-weighting) gives

$$
e^{-S_\Phi}=(e^{\Phi_0})^{2g-2}=g_s^{2g-2},\qquad\boxed{g_s=e^{\Phi_0}.}
$$

Adding one handle multiplies a contribution by $g_s^2$, identifying $g_s$ as the [string coupling](../../../string-theory.md#string-coupling). With canonically normalized external closed-string states, $n$ vertices add $g_s^n$, giving the [string genus expansion](../../../string-theory.md#string-genus-expansion) $g_s^{2g-2+n}$.

Before gauge fixing, the [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) for inserted [string vertex operators](../../../string-theory.md#string-vertex-operator) is schematically

$$
\mathcal A_n=\sum_g\int\frac{\mathcal Dh\,\mathcal DX}{\operatorname{Vol}(\mathrm{Diff}\times\mathrm{Weyl})}\,e^{-S_E[X,h]}\prod_{r=1}^n\int_\Sigma d^2z_r\,V_r(z_r).
$$

The quotient removes descriptions related by [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformations](../../../string-theory.md#weyl-transformation). Gauge fixing has a nontrivial Jacobian, the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant). Anticommuting vector ghosts $c^a$ and symmetric trace-free antighosts $b_{ab}$ exponentiate this determinant as a local [worldsheet ghost action](../../../string-theory.md#worldsheet-ghost-action). These [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field) implement the gauge quotient; they are not additional spacetime particles. Their zero modes must be treated separately rather than included in an invertible determinant.

Three kinds of geometry enter the scattering calculation. The [worldsheet moduli](../../../string-theory.md#worldsheet-moduli) describe genuinely different conformal shapes that remain after local gauge fixing. Each such shape must be integrated over. The [mapping class group](../../../topology.md#mapping-class-group) consists of orientation-preserving diffeomorphisms modulo those continuously deformable to the identity; it identifies different markings of the same conformal surface, so only one representative of each class is counted. The [worldsheet conformal Killing group](../../../string-theory.md#worldsheet-conformal-killing-group) is the continuous residual conformal symmetry of a chosen surface. It moves insertion positions without changing the geometry and must be divided out, usually by fixing enough vertex positions.

For a torus, write $z\sim z+1\sim z+\tau$, with $\operatorname{Im}\tau>0$. Its shape modulus is $\tau$, its [mapping class group](../../../topology.md#mapping-class-group) acts through the [modular group](../../../modular-function.md#modular-group), and its connected [worldsheet conformal Killing group](../../../string-theory.md#worldsheet-conformal-killing-group) acts by translations. Thus the shape integral runs over the [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group), while one insertion position can be fixed by translation. On the sphere, three positions can instead be fixed by [Möbius transformations](../../../group-theory.md#mobius-transformation); for [genus](../../../topology.md#genus-of-a-surface) at least two the continuous conformal Killing group is trivial.

<a id="3/image-one-representative-of-each-torus-conformal-shape-in-the-modular-fundamental-domain"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-49-modular-domain.png)

**[Figure 1](#3/image-one-representative-of-each-torus-conformal-shape-in-the-modular-fundamental-domain). One representative of each torus conformal shape in the modular fundamental domain**.

Now use the half-normalized [worldsheet diffeomorphism ghost operator](../../../string-theory.md#worldsheet-diffeomorphism-ghost-operator) in the question. A vector field $v^a$ can preserve the representative metric after a compensating [Weyl transformation](../../../string-theory.md#weyl-transformation) precisely when $P_1v=0$. The trace of the metric variation sets $\delta\omega=\tfrac12\nabla_av^a$, leaving the [Conformal Killing equation](../../../general-relativity.md#conformal-killing-equation)

$$
\boxed{\nabla_av_b+\nabla_bv_a-h_{ab}\nabla_cv^c=0.}
$$

The kernel of this operator gives the infinitesimal [worldsheet conformal Killing group](../../../string-theory.md#worldsheet-conformal-killing-group).

For a surviving [infinitesimal worldsheet modulus](../../../string-theory.md#infinitesimal-worldsheet-modulus), choose its metric variation $t_{ab}$ orthogonal to all gauge variations. Orthogonality to [Weyl transformations](../../../string-theory.md#weyl-transformation) requires $h^{ab}t_{ab}=0$. On the closed surface, the [formal adjoint of the worldsheet conformal Killing operator](../../../string-theory.md#formal-adjoint-of-the-worldsheet-conformal-killing-operator) follows by [integration by parts](../../../calculus.md#integration-by-parts):

$$
\int\sqrt h\,t^{ab}(P_1v)_{ab}=-\int\sqrt h\,(\nabla_at^{ab})v_b.
$$

Orthogonality to every diffeomorphism variation is therefore the adjoint-kernel condition, giving

$$
\boxed{h^{ab}t_{ab}=0,\qquad\nabla^at_{ab}=0.}
$$

In a local conformal coordinate these imply $\partial_{\bar z}t_{zz}=0$ and its conjugate: the moduli variations are represented by [holomorphic quadratic differentials](../../../complex-geometry.md#holomorphic-quadratic-differential). Multiplying the definition of $P_1$ by two changes its adjoint by two but changes neither kernel.

For four [tachyon vertex operators](../../../string-theory.md#tachyon-vertex-operator) on the torus, there is one complex shape modulus, four complex insertion positions and one complex translation to remove. The [worldsheet integration count after conformal gauge fixing](../../../string-theory.md#worldsheet-integration-count-after-conformal-gauge-fixing) is therefore

$$
\boxed{1+4-1=4\text{ complex integrations}=8\text{ real integrations}.}
$$

Fix the fourth insertion at $z_4=0$. A schematic gauge-fixed expression is

$$
\mathcal A_{1,4}=g_s^4\int_{\mathcal F}d\mu(\tau)\int_{T_\tau^3}\prod_{r=1}^3d^2z_r\,\left\langle(b,\mu_\tau)(\bar b,\bar\mu_\tau)c\bar cV_4(0)\prod_{r=1}^3V_r(z_r)\right\rangle.
$$

Here the antighost pair supplies the modulus measure, and the ghost pair at the fixed vertex absorbs the translation zero modes. The three unfixed positions and $\tau$ are the four complex integrations. The [punctured Riemann surface moduli dimension](../../../geometry-and-topology.md#punctured-riemann-surface-moduli-dimension) gives the same result, $3g-3+n=4$. Target-spacetime zero-mode integrals producing [momentum conservation](../../../classical-mechanics.md#momentum-conservation) are separate from this requested count of worldsheet integrations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
