# Paper 51

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_51.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_51.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use a mostly-plus target [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) metric and restore the [string tension](../../../string-theory.md#string-tension) by $T=(2\pi\alpha')^{-1}$. After [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation), the [Polyakov action](../../../string-theory.md#polyakov-action) on a [Riemann surface](../../../complex-analysis.md#riemann-surfaces) is

$$
S_E=\frac1{4\pi\alpha'}\int_\Sigma\sqrt h\,h^{\mu\nu}\partial_\mu X^a\partial_\nu X_a.
$$

The [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) integrates over embeddings and [worldsheet metrics](../../../string-theory.md#worldsheet-metric), dividing by [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformations](../../../string-theory.md#weyl-transformation). For a consistent flat [bosonic string theory](../../../string-theory.md#bosonic-string-theory), take the [critical dimension of the bosonic string](../../../string-theory.md#critical-dimension-of-string-theory) $d=26$. [Conformal gauge](../../../string-theory.md#conformal-gauge) turns the embedding fields into free scalars; its [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) is represented by the [bc system](../../../string-theory.md#bc-system). The remaining integrations are over [worldsheet moduli](../../../string-theory.md#worldsheet-moduli) and external insertion points.

A [tachyon vertex operator](../../../string-theory.md#tachyon-vertex-operator) is

$$
V_k(z,\bar z)={}:e^{ik\cdot X(z,\bar z)}:.
$$

The [worldsheet Green function](../../../string-theory.md#worldsheet-green-function) is $\langle X^a(z)X^b(w)\rangle=-(\alpha'/2)\eta^{ab}\log|z-w|^2$. The [operator product expansion](../../../string-theory.md#operator-product-expansion) with the [holomorphic stress-energy tensor](../../../string-theory.md#holomorphic-stress-energy-tensor) gives [conformal weights](../../../string-theory.md#conformal-weight) $(\alpha' k^2/4,\alpha' k^2/4)$. An [integrated string vertex operator](../../../string-theory.md#integrated-string-vertex-operator) must have weights $(1,1)$, so the [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) is $k^2=4/\alpha'$, or tachyonic [mass](../../../classical-mechanics.md#mass) parameter $m^2=-4/\alpha'$.

At lowest order in the [string coupling](../../../string-theory.md#string-coupling), the [worldsheet](../../../string-theory.md#worldsheet) is a [Riemann sphere](../../../complex-analysis.md#riemann-sphere). For four external states, three insertion points can be fixed by a [Möbius transformation](../../../group-theory.md#mobius-transformation). In the [worldsheet ghost field](../../../string-theory.md#worldsheet-ghost-field) description these three vertices carry $c\bar c$, while the fourth is integrated. The [three-point worldsheet ghost correlator](../../../string-theory.md#three-point-worldsheet-ghost-correlator) gives the squared product of the three fixed-point separations, precisely the [sphere gauge fixing for four string vertices](../../../string-theory.md#sphere-gauge-fixing-for-four-string-vertices) factor. Thus fixing three points is a gauge choice, rather than deleting three integrations without their Jacobian.

The [integral](../../../calculus.md#integral) over the constant embedding [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode) gives $(2\pi)^d\delta^{(d)}(\sum_i k_i)$. The remaining [Gaussian integral](../../../calculus.md#gaussian-integral), using [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) to remove self-contractions, gives the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor)

$$
\left\langle\prod_{i=1}^4 V_{k_i}(z_i,\bar z_i)\right\rangle
\ \propto\
\delta^{(d)}\!\left(\sum_i k_i\right)
\prod_{i<j}|z_i-z_j|^{\alpha' k_i\cdot k_j}.
$$

Set $(z_1,z_2,z_3,z_4)=(0,z,1,\infty)$; the vertex at infinity is defined with its conformal-weight factor. Let all momenta be incoming and define

$$
s=-(k_1+k_2)^2,\qquad t=-(k_2+k_3)^2,\qquad u=-(k_1+k_3)^2.
$$

The [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) and [momentum conservation](../../../classical-mechanics.md#momentum-conservation) imply $s+t+u=-16/\alpha'$. Since $\alpha'k_1\cdot k_2=-4-\alpha's/2$ and similarly for the pair $(2,3)$, the [sphere tachyon position integral](../../../string-theory.md#sphere-tachyon-position-integral) becomes

$$
\mathcal A_4^{(0)}
=\mathcal N g_s^2(2\pi)^d\delta^{(d)}\!\left(\sum_i k_i\right)
\int_{\mathbb C}d^2z\,|z|^{-4-\alpha's/2}|1-z|^{-4-\alpha't/2}.
$$

Here $\mathcal N$ depends on the normalization of external [string vertex operators](../../../string-theory.md#string-vertex-operator); it does not affect the kinematic dependence.

To evaluate the remaining [worldsheet modulus](../../../string-theory.md#worldsheet-moduli), put $a=-1-\alpha's/4$ and $b=-1-\alpha't/4$. The [complex beta integral](../../../complex-analysis.md#complex-beta-integral) is

$$
\int_{\mathbb C}d^2z\,|z|^{2a-2}|1-z|^{2b-2}
=\pi\frac{\Gamma(a)\Gamma(b)\Gamma(1-a-b)}
{\Gamma(1-a)\Gamma(1-b)\Gamma(a+b)}.
$$

For example, this identity follows by writing the two powers as Schwinger-parameter [Gamma integrals](../../../complex-analysis.md#gamma-integral), doing the two-dimensional [Gaussian integral](../../../calculus.md#gaussian-integral), and changing the two positive parameters to their sum and ratio. The [complex beta integral](../../../complex-analysis.md#complex-beta-integral) first holds for $\operatorname{Re}a,\operatorname{Re}b>0$ and $\operatorname{Re}(a+b)<1$; the scattering result is its [analytic continuation](../../../complex-analysis.md#analytic-continuation). The third gamma-function argument is $1-a-b=-1-\alpha'u/4$. Absorbing $\pi$ into $\mathcal N$, the result is the **tree-level four-tachyon amplitude**, the [Virasoro–Shapiro amplitude](../../../string-theory.md#virasoro-shapiro-amplitude):

$$
\boxed{\mathcal A_4^{(0)}
=\mathcal C g_s^2(2\pi)^d\delta^{(d)}\!\left(\sum_i k_i\right)
\prod_{q\in\{s,t,u\}}\frac{\Gamma(-1-\alpha'q/4)}{\Gamma(2+\alpha'q/4)}.}
$$

It is symmetric in the three [Mandelstam variables](../../../special-relativity.md#mandelstam-variables) and has generic poles at $q=4(N-1)/\alpha'$, matching the [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum). The formula is the leading term of [string perturbation theory](../../../string-theory.md#string-perturbation-theory). Higher orders are constructed by the same [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) prescription on higher-[genus](../../../topology.md#genus-of-a-surface) [worldsheets](../../../string-theory.md#worldsheet), with four marked points and the corresponding ghost and [worldsheet moduli](../../../string-theory.md#worldsheet-moduli) measure; genus $g$ has coupling power $g_s^{2g+2}$.

## 2

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $h_{\mu\nu}=\partial_\mu X^a\partial_\nu X_a$ be the [induced worldvolume metric](../../../string-theory.md#induced-worldvolume-metric) and write $H=\gamma^{\mu\nu}h_{\mu\nu}$. Varying the embedding in the [auxiliary-metric brane action](../../../string-theory.md#auxiliary-metric-brane-action) and integrating by parts gives

$$
\boxed{\partial_\mu\!\left(\sqrt{-\gamma}\,\gamma^{\mu\nu}\partial_\nu X^a\right)=0.}
$$

The boundary contribution, including its relative factor, is

$$
\delta I\big|_{\partial\Sigma}
=2\int_{\partial\Sigma}\sqrt{|\gamma_\partial|}\,
n_\mu\gamma^{\mu\nu}\partial_\nu X_a\,\delta X^a.
$$

At initial and final times one fixes the endpoint configurations or uses variations of compact support. At a spatial boundary, free target directions require [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) $n_\mu\gamma^{\mu\nu}\partial_\nu X^a=0$; fixed directions require [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) $\delta X^a=0$. Mixed conditions must make this boundary pairing vanish. A closed [brane](../../../string-theory.md#brane) has no spatial boundary. Since the [auxiliary worldvolume metric](../../../string-theory.md#auxiliary-worldvolume-metric) enters without [derivatives](../../../calculus.md#derivative), its variation produces no extra boundary term.

Using $\delta\sqrt{-\gamma}=-(1/2)\sqrt{-\gamma}\gamma_{\mu\nu}\delta\gamma^{\mu\nu}$, variation of the inverse [worldvolume metric](../../../string-theory.md#auxiliary-worldvolume-metric) gives

$$
\boxed{h_{\mu\nu}-\frac12\gamma_{\mu\nu}\{H-(p-1)\}=0.}
$$

Taking the trace yields $(p-1)(H-p-1)=0$. For $p\ne1$, this forces $H=p+1$, and substitution gives $\gamma_{\mu\nu}=h_{\mu\nu}$. For a nondegenerate timelike embedding, eliminating the [auxiliary worldvolume metric](../../../string-theory.md#auxiliary-worldvolume-metric) therefore gives twice the [worldvolume](../../../string-theory.md#worldvolume) area, with the overall physical [brane tension](../../../string-theory.md#brane-tension) supplied by the action normalization.

For $p=1$, the traced metric equation is an identity, and the remaining equation only says $h_{\mu\nu}=(H/2)\gamma_{\mu\nu}$. It fixes the [worldsheet metric](../../../string-theory.md#worldsheet-metric) up to a [Weyl transformation](../../../string-theory.md#weyl-transformation), rather than determining it uniquely. Indeed $\sqrt{-\gamma}\gamma^{\mu\nu}$ is Weyl invariant precisely in two [worldvolume](../../../string-theory.md#worldvolume) dimensions, and the constant term vanishes precisely at $p=1$. This is the [Weyl-invariance exception for the string among branes](../../../string-theory.md#weyl-invariance-exception-for-the-string-among-branes). In a nondegenerate interior it gives the familiar [classical equivalence of Polyakov and Nambu–Goto actions](../../../string-theory.md#classical-equivalence-of-polyakov-and-nambu-goto-actions); degeneracies at a free string endpoint must be treated through the original equations.

For the [open string](../../../string-theory.md#open-string), choose [conformal gauge](../../../string-theory.md#conformal-gauge) $\gamma_{\mu\nu}=\operatorname{diag}(-1,1)$ on $0\leq\sigma\leq\pi$. The embedding equation is the [wave equation](../../../wave-equation.md), and NN means $\partial_\sigma X^a=0$ at both spatial endpoints. For these operator formulas restore the conventional overall normalization $S=-TI/2$, with $T=(2\pi\alpha\prime)^{-1}$; the overall factor does not change the preceding classical equations. Its [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) is

$$
X^a=x^a+2\alpha'p^a\tau+
i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^a}{n}e^{-in\tau}\cos(n\sigma),
\qquad \alpha_0^a=\sqrt{2\alpha'}p^a.
$$

Reality requires $(\alpha_n^a)^\dagger=\alpha_{-n}^a$. [Canonical quantization](../../../quantum-mechanics.md#canonical-quantization) gives

$$
[x^a,p^b]=i\eta^{ab},\qquad
[\alpha_m^a,\alpha_n^b]=m\eta^{ab}\delta_{m+n,0}.
$$

The metric equation is the vanishing of the [worldsheet stress tensor](../../../string-theory.md#worldsheet-stress-energy-tensor): $(\partial_\tau X+\partial_\sigma X)^2=(\partial_\tau X-\partial_\sigma X)^2=0$. The two endpoint-compatible mode expansions contain the same [string oscillator](../../../string-theory.md#string-oscillator) family. Their quadratic coefficients are the classical [Virasoro constraints](../../../string-theory.md#virasoro-constraint).

For the operators, use [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) with positive-index [string oscillators](../../../string-theory.md#string-oscillator) as annihilators:

$$
L_m=\frac12\sum_{n\in\mathbb Z}:\alpha_{m-n}\cdot\alpha_n:,
\qquad
L_0=\alpha'p^2+\sum_{n>0}\alpha_{-n}\cdot\alpha_n.
$$

Thus $(\partial_\tau X\pm\partial_\sigma X)^2$ has modes $4\alpha'L_m$ before the quantum ordering correction. The [physical-state Virasoro conditions for an open string](../../../string-theory.md#physical-state-virasoro-conditions-for-an-open-string) are

$$
\boxed{L_m|\Phi\rangle=0\quad(m>0),\qquad
(L_0-a)|\Phi\rangle=0.}
$$

One imposes only the positive modes on kets, with the adjoint conditions on bras, as in [Gupta-Bleuler quantization](../../../relativistic-quantum-field.md#gupta-bleuler-formalism). Requiring every positive and negative mode to annihilate the same state would conflict with the [Virasoro central extension](../../../string-theory.md#virasoro-central-extension). The intercept $a$ is the zero-mode ordering constant. The standard critical [bosonic string theory](../../../string-theory.md#bosonic-string-theory) has $d=26$ and $a=1$; in [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory) the transverse [zero-point energy](../../../quantum-mechanics.md#zero-point-energy) gives $a=(d-2)/24$, while full anomaly-free Lorentz or [BRST quantization](../../../relativistic-quantum-field.md#brst-quantization) fixes the critical values. The mass constraint is then $\alpha'M^2=N-a$, with $N=\sum_{n>0}\alpha_{-n}\cdot\alpha_n$.

To compute the [Virasoro algebra](../../../string-theory.md#virasoro-algebra), commute a quadratic generator with one [string oscillator](../../../string-theory.md#string-oscillator):

$$
[L_m,\alpha_n^a]=-n\alpha_{m+n}^a,\qquad [L_m,x^a]=-i\sqrt{2\alpha'}\alpha_m^a.
$$

These identities and the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) imply that $[L_m,L_n]-(m-n)L_{m+n}$ commutes with every [string oscillator](../../../string-theory.md#string-oscillator) and with the center-of-mass coordinates and momenta. Mode number permits a scalar term only for $m+n=0$. Its coefficient follows from the formal zero-momentum [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum), on which $L_0=0$. For $m>0$,

$$
L_{-m}|0\rangle=\frac12\sum_{r=1}^{m-1}
\alpha_{-r}\cdot\alpha_{-(m-r)}|0\rangle.
$$

The two possible [string oscillator](../../../string-theory.md#string-oscillator) contractions give

$$
\langle0|L_mL_{-m}|0\rangle
=\frac d2\sum_{r=1}^{m-1}r(m-r)
=\frac d{12}(m^3-m).
$$

The timelike target coordinate still contributes one to this [central charge](../../../string-theory.md#central-charge): its two metric signs cancel in $\eta_{ab}\eta^{ab}=d$. Consequently

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}
+\frac d{12}m(m^2-1)\delta_{m+n,0}.}
$$

This is the [free-boson Virasoro central term](../../../string-theory.md#free-boson-virasoro-central-term). It vanishes for the three global conformal modes $m=0,\pm1$.

To keep the intercept convention separate, define $\mathcal L_m=L_m-a\delta_{m,0}$. The [Virasoro zero-mode shift](../../../string-theory.md#virasoro-zero-mode-shift) changes the displayed central term to

$$
[\mathcal L_m,\mathcal L_n]=(m-n)\mathcal L_{m+n}
+\left\{\frac d{12}m(m^2-1)+2am\right\}\delta_{m+n,0}.
$$

The matter [central charge](../../../string-theory.md#central-charge) here is $d$, not $d-2$. Covariant [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field) contribute $-26$; their inclusion cancels the anomaly at $d=26$, while the intercept is handled by the appropriate zero-mode and physical-state convention.

## 3

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) equals its transform under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), so its spinor components are not independent of their conjugates. In a real two-dimensional [gamma matrix](../../../algebra.md#gamma-matrices) representation it can be taken real, with anticommuting [Grassmann variables](../../../linear-algebra.md#grassmann-variable) as components. Each target index labels a separate [worldsheet Majorana fermion](../../../string-theory.md#worldsheet-majorana-fermion); it is not itself a target-space spinor.

Use worldsheet signature $(-,+)$ and the real [gamma matrices](../../../algebra.md#gamma-matrices)

$$
\gamma^0=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad
\gamma^1=\begin{pmatrix}0&1\\1&0\end{pmatrix},
\qquad
\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}.
$$

Take $\bar\psi=\psi^TC$ with $C=\gamma^0$. Define the [chirality](../../../relativistic-quantum-field.md#chirality-physics) matrix with the chosen worldsheet orientation by

$$
\gamma_*=-\gamma^0\gamma^1=\begin{pmatrix}1&0\\0&-1\end{pmatrix},
\qquad P_\pm=\frac{1\pm\gamma_*}{2}.
$$

It squares to one and anticommutes with each [gamma matrix](../../../algebra.md#gamma-matrices). [Chirality](../../../relativistic-quantum-field.md#chirality-physics) is its eigenvalue, selected by the [chiral projectors](../../../relativistic-quantum-field.md#chiral-projector). Its overall sign is conventional.

Writing $\psi=(\psi_+,\psi_-)^T$, the fermion [equation of motion](../../../classical-mechanics.md#equation-of-motion) $\gamma^\mu\partial_\mu\psi=0$ becomes

$$
(\partial_\tau+\partial_\sigma)\psi_+=0,\qquad
(\partial_\tau-\partial_\sigma)\psi_-=0.
$$

Hence

$$
\boxed{\psi_+=F(\tau-\sigma)\text{ is right-moving},\qquad
\psi_-=G(\tau+\sigma)\text{ is left-moving}.}
$$

The first profile travels toward increasing $\sigma$, and the second toward decreasing $\sigma$. Thus the choice of [chirality](../../../relativistic-quantum-field.md#chirality-physics) orientation realizes the requested [worldsheet chirality and propagation direction](../../../string-theory.md#worldsheet-chirality-and-propagation-direction) correspondence; reversing the orientation interchanges the labels.

For the rigid [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry) variation, let $\epsilon$ be a constant Grassmann-odd [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor). With the displayed conventions,

$$
\delta\bar\psi^a=-\bar\epsilon\gamma^\mu\partial_\mu X^a.
$$

The minus sign follows from $(\gamma^\mu)^TC=-C\gamma^\mu$. A second identity from the [Majorana Grassmann bilinear interchange](../../../relativistic-quantum-field.md#majorana-grassmann-bilinear-interchange) is $\bar\chi\gamma^\nu\gamma^\mu\epsilon=\bar\epsilon\gamma^\mu\gamma^\nu\chi$. Keeping these Grassmann signs is essential.

The bosonic kinetic variation is $2i\partial_\mu X_a\,\bar\epsilon\,\partial^\mu\psi^a$. The two fermionic kinetic variations, using the two identities above, give the full result

$$
\begin{aligned}
\delta\mathcal L={}&
2i\partial_\mu X_a\,\bar\epsilon\,\partial^\mu\psi^a
-i\bar\epsilon\gamma^\mu\gamma^\nu\partial_\mu X_a\,\partial_\nu\psi^a
+i\bar\epsilon\psi_a\,\partial_\mu\partial^\mu X^a\\
={}&\partial_\nu\!\left(i\bar\epsilon\gamma^\nu\gamma^\mu
\psi_a\,\partial_\mu X^a\right).
\end{aligned}
$$

For the second equality use $\gamma^\nu\gamma^\mu=2\eta^{\mu\nu}-\gamma^\mu\gamma^\nu$ and symmetry of the second embedding [derivative](../../../calculus.md#derivative). No field equation has been used. Thus the **variation is an off-shell total [derivative](../../../calculus.md#derivative)**:

$$
\boxed{\delta I=\int_{\partial\Sigma}d\Sigma_\nu\,
i\bar\epsilon\gamma^\nu\gamma^\mu\psi_a\partial_\mu X^a.}
$$

This is the [rigid worldsheet supersymmetry boundary term](../../../string-theory.md#rigid-worldsheet-supersymmetry-boundary-term). It vanishes when the boundary flux vanishes, for example on a closed worldsheet with compatible fields and variations. On a spatial circle, a constant supersymmetry parameter must also respect the chosen [spin structure](../../../riemannian-geometry.md#spin-structure). Periodic fermions allow this rigid transformation; antiperiodic fermions and a constant parameter would give an antiperiodic $\delta X$ and fail to preserve a periodic bosonic embedding. The local action identity remains valid, but global symmetry requires compatible boundary data. This is the [spin-structure obstruction to constant worldsheet supersymmetry](../../../string-theory.md#spin-structure-obstruction-to-constant-worldsheet-supersymmetry).

For the spectrum, assume the usual critical [RNS string](../../../string-theory.md#spinning-string), physical-state constraints, a nonzero null target momentum, and the supersymmetric [GSO projection](../../../string-theory.md#gso-projection). Analyze just one chiral sector. Its matter [central charge](../../../string-theory.md#central-charge) is $d+d/2$; the [bc system](../../../string-theory.md#bc-system) and [superconformal ghosts](../../../string-theory.md#superconformal-ghost) contribute $-26+11$. Therefore $3d/2-15=0$ gives the [critical dimension of the RNS superstring](../../../string-theory.md#critical-dimension-of-the-rns-superstring) $d=10$. [Light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory) leaves eight transverse bosonic and eight transverse fermionic [string oscillator](../../../string-theory.md#string-oscillator) directions.

In the [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector), the normal-ordering intercept is $a_{\rm NS}=1/2$. The massless level is $N=1/2$ and has states

$$
b_{-1/2}^{\,i}|0;k\rangle_{\rm NS},\qquad i=1,\ldots,8.
$$

The [GSO projection](../../../string-theory.md#gso-projection) retains these eight transverse vector polarizations while removing the tachyonic ground state. They are spacetime [bosons](../../../quantum-mechanics.md#boson), although the creating [string oscillator](../../../string-theory.md#string-oscillator) is a worldsheet fermion. In covariant language transversality and the longitudinal null-state quotient leave $10-2=8$ polarizations.

In the [Ramond sector](../../../string-theory.md#ramond-sector), bosonic and fermionic [zero-point energies](../../../quantum-mechanics.md#zero-point-energy) cancel, so $a_{\rm R}=0$ and the ground states are massless. The eight transverse fermion zero modes obey

$$
\{d_0^i,d_0^j\}=\delta^{ij},\qquad
\Gamma^i=\sqrt2d_0^i,\qquad
\{\Gamma^i,\Gamma^j\}=2\delta^{ij}.
$$

This [Ramond zero-mode Clifford algebra](../../../string-theory.md#ramond-zero-mode-clifford-algebra) acts on a sixteen-dimensional ground-state space. Its two [chirality](../../../relativistic-quantum-field.md#chirality-physics) subspaces each have dimension eight. The [GSO projection](../../../string-theory.md#gso-projection) keeps one, an $8_s$ or $8_c$ spinor of $\operatorname{SO}(8)$, the rotation subgroup of the massless [little group](../../../special-relativity.md#little-group). These are spacetime [fermions](../../../quantum-mechanics.md#fermion). Equivalently a ten-dimensional [Majorana-Weyl spinor](../../../relativistic-quantum-field.md#majorana-weyl-spinor) has sixteen real components before the massless [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) reduces the physical polarization count to eight.

Consequently the [massless chiral RNS spectrum after GSO projection](../../../string-theory.md#massless-chiral-rns-spectrum-after-gso-projection) satisfies

$$
\boxed{N_{\rm bosonic}=8=N_{\rm fermionic}.}
$$

The [GSO projection](../../../string-theory.md#gso-projection) is essential: without it, the transverse [Ramond sector](../../../string-theory.md#ramond-sector) would retain both eight-dimensional spinor chiralities. These are counts for one chiral sector, not the tensor-product counts of the full closed-string spectrum.

## 4

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The ungauge-fixed [Polyakov action](../../../string-theory.md#polyakov-action) has [worldsheet diffeomorphism](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformation](../../../string-theory.md#weyl-transformation) symmetries. They must survive quantization so that [conformal gauge](../../../string-theory.md#conformal-gauge) remains a valid gauge choice. In a curved target, the [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model) has a field-dependent coupling $g_{ab}(X)$. Its [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) is controlled by the renormalization of this coupling, the [sigma-model beta function](../../../string-theory.md#sigma-model-beta-function).

Restore the Euclidean normalization $(4\pi\alpha')^{-1}\int g_{ab}(X)\partial X^a\partial X^b$. Use a covariant [background field expansion of a string sigma model](../../../string-theory.md#background-field-expansion-of-a-string-sigma-model), with geodesic fluctuations about a slowly varying embedding. The quadratic fluctuation operator contains the target [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) coupled to two background embedding [derivatives](../../../calculus.md#derivative). The ultraviolet coincident propagator is $\langle\xi^a\xi^b\rangle_{\rm UV}=\alpha\prime g^{ab}\log(\Lambda/\mu)$: the kinetic operator supplies $2\pi\alpha\prime$, and the two-dimensional momentum [integral](../../../calculus.md#integral) supplies $(2\pi)^{-1}\log(\Lambda/\mu)$. Contracting the curvature vertex with this propagator gives a logarithmic metric counterterm proportional to $\alpha\prime R_{ab}$. The resulting one-loop metric counterterm gives

$$
\beta^g_{ab}=\alpha'R_{ab}+O(\alpha'^2).
$$

The trace of the [worldsheet stress tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) contains this coefficient multiplying $\partial X^a\partial X^b$, together with the curvature anomaly controlled by total [central charge](../../../string-theory.md#central-charge). Thus, with zero antisymmetric background, constant [dilaton](../../../string-theory.md#dilaton), and the critical matter/ghost system,

$$
\boxed{R_{ab}=0\quad\text{at leading order in }\alpha'.}
$$

The central-charge condition also requires $d=26$ if there is no extra internal conformal theory. This is a leading-order equation: higher-curvature terms enter the beta function at higher orders in $\alpha'$, so a Ricci-flat metric alone is not a general all-orders quantum consistency criterion.

To derive the local [T-duality](../../../string-theory.md#t-duality), work where the spacelike [Killing vector](../../../general-relativity.md#killing-vector-field) has nonzero norm $V>0$. Use dimensionless coordinates and $\alpha'=1$ units for the duality formulas. The isometry makes the action depend on $z$ only through its [derivatives](../../../calculus.md#derivative). Replace those [derivatives](../../../calculus.md#derivative) by an independent [worldsheet](../../../string-theory.md#worldsheet) one-form $A_\mu$, and enforce its flatness with a [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $\widetilde z$. With $\eta_{\mu\nu}=\operatorname{diag}(-1,1)$ and $\epsilon^{\tau\sigma}=1$, the relevant [first-order worldsheet duality action](../../../string-theory.md#first-order-action-for-abelian-worldsheet-duality) is

$$
I_1=\int d^2\xi\left[
\frac12g_{IJ}(X)\partial_\mu X^I\partial^\mu X^J
+\frac12V(X)A_\mu A^\mu
+\widetilde z\,\epsilon^{\mu\nu}\partial_\mu A_\nu
\right].
$$

Varying $\widetilde z$ sets $dA=0$. Locally $A=dz$, recovering the original theory. For the other elimination, integrate the multiplier term by parts. Varying $A_\nu$ gives $VA^\nu=\epsilon^{\mu\nu}\partial_\mu\widetilde z$, or

$$
A_\tau=V^{-1}\partial_\sigma\widetilde z,\qquad
A_\sigma=V^{-1}\partial_\tau\widetilde z.
$$

Substituting into the entire [first-order worldsheet duality action](../../../string-theory.md#first-order-action-for-abelian-worldsheet-duality), including the multiplier term, gives

$$
\widetilde I=\frac12\int d^2\xi\left[
g_{IJ}\partial_\mu X^I\partial^\mu X^J
+V^{-1}\partial_\mu\widetilde z\,\partial^\mu\widetilde z
\right].
$$

The multiplier contribution is necessary for the sign of the dual kinetic term. This is the [first-order action for Abelian worldsheet duality](../../../string-theory.md#first-order-action-for-abelian-worldsheet-duality), with [Buscher rules](../../../string-theory.md#buscher-rules)

$$
\boxed{\widetilde g_{zz}=V^{-1},\qquad
\widetilde g_{zI}=0,\qquad \widetilde g_{IJ}=g_{IJ},\qquad \widetilde B=0.}
$$

The coordinate map is $\partial_\tau\widetilde z=V\partial_\sigma z$, $\partial_\sigma\widetilde z=V\partial_\tau z$. The original $z$ equation is precisely the integrability condition for $\widetilde z$; conversely the original identity $d(dz)=0$ becomes the dual equation. Thus this transformation exchanges an [equation of motion](../../../classical-mechanics.md#equation-of-motion) with the [Bianchi identity for an Abelian p-form](../../../relativistic-quantum-field.md#bianchi-identity-for-an-abelian-p-form). It reverses one chiral [derivative](../../../calculus.md#derivative) and preserves the other.

For full closed-string equivalence, the local derivation must include the global data. For a free compact circle isometry, the period of $\widetilde z$ and the allowed gauge-field holonomies are chosen so that the [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) exchanges [momentum and winding modes](../../../string-theory.md#momentum-and-winding-modes). A circle of radius $R$ becomes a circle of radius $\alpha'/R$ when dimensions are restored. A spacelike Killing field alone does not fix these periods or ensure a free global circle action; the [global qualifications of Abelian T-duality](../../../string-theory.md#global-qualifications-of-abelian-t-duality) are additional to the local field transformation.

At the quantum level integrating out $A_\mu$ also gives a regulated [functional determinant](../../../quantum-field-theory.md#functional-determinant). The [Buscher dilaton shift](../../../string-theory.md#buscher-dilaton-shift) is

$$
\boxed{\widetilde\Phi=\Phi-\frac12\log V=-\frac12\log V,}
$$

in the stated units and conventional Euclidean dilaton normalization. It generates the [dilaton](../../../string-theory.md#dilaton) curvature coupling even though the original [dilaton](../../../string-theory.md#dilaton) vanished. The dilaton curvature coupling is defined before fixing [conformal gauge](../../../string-theory.md#conformal-gauge); its metric variation improves the [worldsheet stress tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) even when the reference worldsheet is flat. As a normalization check, $e^{-2\widetilde\Phi}\sqrt{|\widetilde g|}=e^{-2\Phi}\sqrt{|g|}$ for this block-diagonal background. The local dual metric by itself is therefore only part of the equivalent quantum background.

With a nonconstant [dilaton](../../../string-theory.md#dilaton) and no antisymmetric field, the [leading metric-dilaton Weyl condition](../../../string-theory.md#leading-metric-dilaton-weyl-condition) is

$$
\boxed{\widetilde R_{ab}
+2\widetilde\nabla_a\widetilde\nabla_b\widetilde\Phi=0,}
$$

together with the scalar dilaton anomaly condition. It does not demand $\widetilde R_{ab}=0$ separately. The new [Ricci tensor](../../../general-relativity.md#ricci-tensor) can be nonzero while the Hessian of the shifted [dilaton](../../../string-theory.md#dilaton) compensates it.

For a direct example, take flat polar coordinates away from the origin, with $ds^2=dr^2+r^2dz^2$ and flat spectator directions. The [polar-coordinate T-dual background](../../../string-theory.md#polar-coordinate-t-dual-background) is

$$
d\widetilde s^2=dr^2+r^{-2}d\widetilde z^2,\qquad \widetilde\Phi=-\log r.
$$

Here

$$
\widetilde R_{rr}=-\frac2{r^2},\qquad
\widetilde R_{\widetilde z\widetilde z}=-\frac2{r^4},\qquad
\widetilde\nabla_r\widetilde\nabla_r\widetilde\Phi=\frac1{r^2},\qquad
\widetilde\nabla_{\widetilde z}\widetilde\nabla_{\widetilde z}\widetilde\Phi=\frac1{r^4}.
$$

Both metric equations vanish. In critical dimension the scalar equation also holds: $4|\widetilde\nabla\widetilde\Phi|^2-4\widetilde\Box\widetilde\Phi-\widetilde R=4/r^2-8/r^2+4/r^2=0$. The example is local on $r>0$; the circle degenerates at the excluded origin.

**Nonzero dual Ricci curvature is consistent because quantum T-duality transforms the dilaton as well as the metric.** The displayed curvature equations and classical [Buscher rules](../../../string-theory.md#buscher-rules) are interpreted at their stated leading [derivative](../../../calculus.md#derivative) order; higher-order renormalized descriptions require the corresponding corrections and field-redefinition conventions. A constant $V$ is a special case in which the dual metric may also remain Ricci-flat.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
