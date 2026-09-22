# Paper 55

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper55.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper55.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For null [four-momentum](../../../special-relativity.md#four-momentum), $\{Q^I,\bar Q^J\}=2\delta^{IJ}\sigma\cdot p$ has rank one in its spinor indices. Positivity makes the null combinations act trivially; the remaining $N$ normalized pairs obey $\{a_I,a_J^\dagger\}=\delta_{IJ}$. Acting with distinct lowering operators on a highest-[helicity](../../../special-relativity.md#helicity) state gives the [helicity spectrum of a massless supermultiplet](../../../supersymmetry.md#helicity-spectrum-of-a-massless-supermultiplet):

$$
\lambda_k=h-\frac{k}{2},\qquad n_k=\binom Nk\quad(0\leq k\leq N),\qquad
\boxed{\sum_k n_k=2^N.}
$$

A [CPT completion of a supermultiplet](../../../supersymmetry.md#cpt-completion-of-a-supermultiplet) adds the opposite [helicities](../../../special-relativity.md#helicity) if needed. Interpreting the physical spin bounds as $|\lambda|\leq s$, the width $N/2$ fits inside $[-s,s]$ only if $N\leq4s$. A literal one-sided bound on helicity without [CPT](../../../quantum-field-theory.md#cpt-symmetry) would not give this maximum. The maximal spectra are

$$
\begin{array}{c|rrrrr}
N=4:\ \lambda&1&1/2&0&-1/2&-1\\
\text{multiplicity}&1&4&6&4&1
\end{array}
$$

and

$$
\begin{array}{c|rrrrrrrrr}
N=8:\ \lambda&2&3/2&1&1/2&0&-1/2&-1&-3/2&-2\\
\text{multiplicity}&1&8&28&56&70&56&28&8&1.
\end{array}
$$

Thus **the maxima are (N=4) for spin at most one and (N=8) for spin at most two**, with 16 and 256 states. [Dimensional reduction](../../../physics.md#dimensional-reduction) of [ten-dimensional super Yang-Mills theory](../../../supersymmetry.md#ten-dimensional-super-yang-mills-theory) on a six-torus gives the first: the vector yields one four-dimensional vector and six [real scalar fields](../../../scalar-field-theory.md#real-scalar-field), and its [Majorana-Weyl spinor](../../../relativistic-quantum-field.md#majorana-weyl-spinor) yields four [Weyl spinors](../../../relativistic-quantum-field.md#weyl-spinor). Reducing [eleven-dimensional supergravity](../../../supersymmetry.md#eleven-dimensional-supergravity) on a seven-torus gives the second: metric components supply one [graviton](../../../quantum-theory.md#graviton), seven vectors and 28 scalars; the three-form supplies 21 vectors, 35 scalars and seven dualized two-form scalars; the [gravitino](../../../supersymmetry.md#gravitino) supplies eight [gravitini](../../../supersymmetry.md#gravitino) and 56 spin-half fields. These total 28 vectors and 70 scalars, with 128 [boson](../../../quantum-mechanics.md#boson) and 128 [fermion](../../../quantum-mechanics.md#fermion) states.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[R-parity](../../../supersymmetry.md#r-parity) is the multiplicative $\mathbb Z_2$ quantum number

$$
\boxed{R_p=(-1)^{3(B-L)+2s},}
$$

where $B,L,s$ are [baryon number](../../../standard-model.md#baryon-number), [lepton number](../../../standard-model.md#lepton-number) and spin. Ordinary [Standard Model](../../../standard-model.md) particles have $R_p=+1$ and their superpartners have $R_p=-1$. Gauge invariance alone allows [MSSM](../../../supersymmetry.md#minimal-supersymmetric-standard-model) [superpotential](../../../supersymmetry.md#superpotential) terms $LLE^c$, $LQD^c$, $U^cD^cD^c$ and $LH_u$. Simultaneous baryon- and lepton-number violation can induce rapid [proton decay](../../../standard-model.md#proton-decay). Exact [R-parity](../../../supersymmetry.md#r-parity) forbids these renormalizable terms, since the associated [matter parity](../../../supersymmetry.md#matter-parity) is odd; it does not forbid every higher-dimensional proton-decay operator, for example $QQQL$.

Two consequences are **superpartner production in pairs from ordinary-particle initial states** and **stability of the lightest supersymmetric particle**: a single parity-odd particle cannot decay only into parity-even particles. Cascades therefore end in the [lightest supersymmetric particle](../../../supersymmetry.md#lightest-supersymmetric-particle); if it is neutral and weakly interacting, it produces missing-energy signatures.

A continuous [R-symmetry](../../../supersymmetry.md#r-symmetry) rotates $\theta$ and the [supercharges](../../../supersymmetry.md#supersymmetry-generator). With $R(\theta)=1$, the [superpotential](../../../supersymmetry.md#superpotential) has [R-charge](../../../supersymmetry.md#r-charge) two and the fermion in a [chiral superfield](../../../supersymmetry.md#chiral-superfield) has one less charge than its scalar. [R-parity](../../../supersymmetry.md#r-parity) is only a discrete restriction, represented by combining [matter parity](../../../supersymmetry.md#matter-parity) with $\theta\mapsto-\theta$, and need not preserve a full continuous [R-symmetry](../../../supersymmetry.md#r-symmetry). For example, a [gaugino](../../../supersymmetry.md#gaugino) [Majorana mass term](../../../relativistic-quantum-field.md#majorana-mass-term) violates an unbroken continuous [R-symmetry](../../../supersymmetry.md#r-symmetry) but preserves [R-parity](../../../supersymmetry.md#r-parity). Thus proton protection by parity and continuous R-charge selection rules are distinct requirements.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

In conventional [Kaluza-Klein theory](../../../physics.md#kaluza-klein-theory), bulk fields have a [Kaluza-Klein tower](../../../physics.md#kaluza-klein-tower) with masses of order $1/R$. If ordinary matter propagates in the extra dimension, the absence of accessible excited modes requires a small $R$: a TeV compactification scale corresponds to roughly $10^{-19}$ m; Planck-scale compactification would be much smaller, of order the [Planck length](../../../physics.md#planck-length). This is a scale estimate, not a universal radius limit independent of the fields and spectrum.

An unwarped [brane-world scenario](../../../physics.md#brane-world-scenario) localizes ordinary fields on a [brane](../../../string-theory.md#brane) while gravity explores a large compact bulk. The volume relation

$$
M_4^2=M_*^{n+2}V_n
$$

makes gravity weak without a fundamental Planck-scale cutoff. In the original [large-extra-dimension model](https://arxiv.org/abs/hep-ph/9803315), $M_*\sim\mathrm{TeV}$ permits approximately millimetre/submillimetre dimensions for $n=2$; more dimensions are smaller. Ordinary-field KK bounds no longer limit these gravity-only radii, although gravitational and other constraints do. This replaces the large fundamental scale hierarchy by a large compact volume needing stabilization.

A warped [brane-world scenario](../../../physics.md#brane-world-scenario) instead uses a position-dependent metric factor. In the two-brane [Randall–Sundrum model](../../../physics.md#randall-sundrum-model), $m_{\rm IR}=e^{-kL}m_0$, so $kL\sim35$ generates a weak scale from a Planck-sized input without a millimetre proper separation; for $k$ of Planck order, $L$ is tens of inverse-Planck lengths. The [single-brane version](https://arxiv.org/abs/hep-th/9906064) even allows infinite proper size through [gravity localization in a noncompact warped dimension](../../../physics.md#gravity-localization-in-a-noncompact-warped-dimension); it is not by itself the two-brane redshift hierarchy construction. Thus **warped proper size can be unbounded**, while finite hierarchy models need specified warping and [radius stabilization](../../../physics.md#radius-stabilization).

[Supersymmetry](../../../supersymmetry.md) addresses the [hierarchy problem](../../../standard-model.md#hierarchy-problem) differently: boson/fermion cancellations protect scalar masses against quadratic sensitivity to high scales, with residual corrections controlled by [soft supersymmetry breaking](../../../supersymmetry.md#soft-supersymmetry-breaking). It stabilizes a chosen hierarchy rather than explaining its initial size. Volume dilution and the [warped redshift mechanism](https://arxiv.org/abs/hep-ph/9905221) explain scale separation geometrically; neither automatically determines its moduli or removes all tuning.

## 2

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [chiral superfield](../../../supersymmetry.md#chiral-superfield) of [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) one, a [renormalizable quantum field theory](../../../perturbative-quantum-field-theory.md#renormalizable-quantum-field-theory) has a quadratic [Kähler potential](../../../supersymmetry.md#kahler-potential) and a [superpotential](../../../supersymmetry.md#superpotential) of degree at most three. Before canonical normalization one may write

$$
K=Z\Phi^\dagger\Phi+[k_1\Phi+k_2\Phi^2+\mathrm{h.c.}]+k_0,\qquad Z>0,
$$

with real $k_0$, and

$$
W=w_0+\ell\Phi+\frac m2\Phi^2+\frac g3\Phi^3.
$$

The purely holomorphic terms in $K$, their conjugates and its constant have vanishing full [superspace integration](../../../supersymmetry.md#superspace-integration); they are [Kähler transformations](../../../supersymmetry.md#kahler-transformation) of the global theory. Rescaling the [chiral superfield](../../../supersymmetry.md#chiral-superfield) sets $Z=1$, so the physically general kinetic choice is $K=\Phi^\dagger\Phi$ up to these terms. The [constant superpotential in global supersymmetry](../../../supersymmetry.md#constant-superpotential-in-global-supersymmetry) also has no component effect. The dimensions of $\ell,m,g$ are respectively two, one and zero.

To eliminate the linear term, translate the complex [chiral superfield](../../../supersymmetry.md#chiral-superfield) as $\Phi=\Phi'+s$. The shifted linear coefficient is

$$
W'(s)=\ell+ms+gs^2.
$$

If $g\ne0$, this quadratic has a root over the complex numbers; if $g=0$ but $m\ne0$, take $s=-\ell/m$. The resulting linear term vanishes and the new quadratic coefficient is $m+2gs$. The canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) changes only by holomorphic, antiholomorphic and constant terms, which do not change the global kinetic action. This is the [superpotential critical-point shift](../../../supersymmetry.md#superpotential-critical-point-shift).

**The claim needs an exception:** if $m=g=0$ but $\ell\ne0$, the [superpotential](../../../supersymmetry.md#superpotential) is purely linear and no invertible translation can remove it. More generally an invertible regular field redefinition cannot turn a nowhere-zero derivative into a critical point. The theory with $W=\ell\Phi$ has $F=-\bar\ell$, a constant positive [scalar potential](../../../quantum-field-theory.md#scalar-potential) $|\ell|^2$, and [flat F-term breaking with a linear superpotential](../../../supersymmetry.md#flat-f-term-breaking-with-a-linear-superpotential). Below, $m$ and $g$ denote the quadratic/cubic coefficients after the valid shift, as intended by the question.

Expand $\Phi=\phi+\sqrt2\theta\psi+\theta^2F$ in chiral coordinates. The highest component of $W(\Phi)$ is $W'(\phi)F-\tfrac12W''(\phi)\psi\psi$, while the full-superspace kinetic term contains $F^*F$. Thus the [auxiliary field](../../../supersymmetry.md#auxiliary-field) part of the component [Lagrangian](../../../calculus-of-variations.md#lagrangian) is

$$
\mathcal L_F=F^*F+(m\phi+g\phi^2)F
+(\bar m\bar\phi+\bar g\bar\phi^2)F^*.
$$

Varying $F$ and $F^*$ independently gives

$$
F^*=-(m\phi+g\phi^2),\qquad F=-(\bar m\bar\phi+\bar g\bar\phi^2).
$$

Substitution gives $\mathcal L_F=-|m\phi+g\phi^2|^2$, and hence the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential)

$$
\boxed{V(\phi)=|m\phi+g\phi^2|^2.}
$$

It is nonnegative and vanishes at $\phi=0$, and also at $\phi=-m/g$ when $g\ne0$. These are [supersymmetric vacua](../../../supersymmetry.md#supersymmetric-vacuum), since the [auxiliary field](../../../supersymmetry.md#auxiliary-field) vanishes. Thus **the quadratic/cubic model does not spontaneously break supersymmetry**. If $m=0$ but $g\ne0$, zero is the sole critical point; if both vanish, every $\phi$ is a zero-energy vacuum. Nonzero $m,g$ give the usual two vacua, coinciding when $m=0$.

For the loop argument, promote the coefficients to background chiral [spurions](../../../supersymmetry.md#spurion). One convenient pair of independent formal $U(1)$ charge assignments is

$$
\begin{array}{c|rrrr|r}
&\Phi&m&g&\theta&W\\\hline
U(1)&1&-2&-3&0&0\\
U(1)_R&2&-2&-4&1&2
\end{array}.
$$

Both symmetries act nontrivially on all three of $\Phi,m,g$; the second is an [R-symmetry](../../../supersymmetry.md#r-symmetry). The [superspace integration](../../../supersymmetry.md#superspace-integration) measure $d^2\theta$ has [R-charge](../../../supersymmetry.md#r-charge) $-2$, so both tree monomials give invariant actions. These are spurionic selection rules, not necessarily actual symmetries after fixing numerical couplings. The R-row is an ordinary-charge redefinition of the usual [Wess–Zumino spurion charge assignment](../../../supersymmetry.md#wess-zumino-spurion-charge-assignment).

A local Wilsonian [superpotential](../../../supersymmetry.md#superpotential) is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) of the chiral fields and chiral [spurions](../../../supersymmetry.md#spurion). The ratio $z=g\Phi/m$ is neutral under both charge assignments and has dimension zero, whereas $m\Phi^2$ has exactly the charges and dimension of $W$. The general symmetry-allowed form, on a patch with $m\ne0$ and up to a physically irrelevant global constant, is therefore

$$
\boxed{W_{\mathrm{eff}}=m\Phi^2 f\left(\frac{g\Phi}{m}\right),}
$$

with $f$ holomorphic where that description is regular. Symmetry by itself does not determine $f$.

For a regular perturbative local [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) retaining the same elementary field and an infrared cutoff, expand $f(z)=\sum_n c_nz^n$. Its term of order $n$ is $c_n g^n m^{1-n}\Phi^{n+2}$. Negative $n$ are singular in $g$, while $n\geq2$ are singular in $m$; these are excluded by perturbative holomorphic regularity at the free-coupling limits. Thus only the quadratic and cubic terms survive. Their regular holomorphic coefficients cannot acquire coupling-dependent invariant corrections. At $g=0$ the quadratic theory is Gaussian, fixing $c_0=1/2$ exactly. A contribution linear in $g$ to the cubic vertex has only one cubic interaction: three external lines exhaust that vertex, leaving no contraction to form a loop. Thus $c_1=1/3$ as well in the present normalization. This supplies the [holomorphy argument for superpotential non-renormalization](../../../supersymmetry.md#holomorphy-argument-for-superpotential-non-renormalization) rather than concluding non-renormalization from symmetry alone.

The [Kähler potential](../../../supersymmetry.md#kahler-potential) can still undergo [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization). If its quadratic coefficient becomes $Z$, canonical normalization gives $m_c=m/Z$ and $g_c=g/Z^{3/2}$, so physical masses and interactions can run despite [superpotential non-renormalization](../../../supersymmetry.md#non-renormalization-theorem). More generally a positive nonsingular effective [Kähler metric](../../../complex-geometry.md#kahler-metric) replaces $V$ by $K^{\phi\bar\phi}|W'(\phi)|^2$ and does not remove its zero-energy critical points. Infrared-singular nonlocal one-particle-irreducible terms and eliminating the entire massive field are outside this Wilsonian statement.

## 3

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use a flat five-dimensional metric of signature $(+----)$ and a circle coordinate $y\sim y+2\pi r$. Start with the canonically normalized [Maxwell action](../../../electromagnetism.md#maxwell-action)

$$
S_5=-\frac14\int d^4x\int_0^{2\pi r}dy\,F_{MN}F^{MN},
\qquad F_{MN}=\partial_M A_N-\partial_N A_M.
$$

Expand the real [Maxwell field](../../../electromagnetism.md#electromagnetic-field) in a [Fourier series](../../../fourier-series.md):

$$
A_M(x,y)=\frac1{\sqrt{2\pi r}}\sum_{n\in\mathbb Z}A_M^{(n)}(x)e^{iny/r},
\qquad A_M^{(-n)}=(A_M^{(n)})^*.
$$

The circle integral makes different modes orthogonal. Writing $a^{(n)}=A_5^{(n)}$ and $k_n=n/r$, the resulting four-dimensional [action](../../../classical-mechanics.md#action) is

$$
S_4=\int d^4x\sum_n\left[-\frac14F_{\mu\nu}^{(n)}F^{\mu\nu(-n)}
+\frac12(\partial_\mu a^{(n)}-ik_nA_\mu^{(n)})
(\partial^\mu a^{(-n)}+ik_nA^{\mu(-n)})\right].
$$

The scalar sign is positive because the fifth direction is spacelike in the chosen mostly-minus metric. This expression follows directly by separating the $\mu\nu$ and the two identical $\mu5$ contributions in $F_{MN}F^{MN}$.

A five-dimensional [gauge transformation](../../../electromagnetism.md#gauge-transformation) $A_M\mapsto A_M+\partial_M\Lambda$ acts on its modes by

$$
\delta A_\mu^{(n)}=\partial_\mu\Lambda^{(n)},\qquad
\delta a^{(n)}=ik_n\Lambda^{(n)}.
$$

For $n\ne0$, define the gauge-invariant vector

$$
B_\mu^{(n)}=A_\mu^{(n)}-\frac1{ik_n}\partial_\mu a^{(n)}.
$$

Then $F_{\mu5}^{(n)}=-ik_nB_\mu^{(n)}$, so its term is a [Proca field](../../../electromagnetism.md#proca-field) mass term $+\tfrac12k_n^2B_\mu^{(n)}B^{\mu(-n)}$. Equivalently, a periodic mode-dependent [gauge transformation](../../../electromagnetism.md#gauge-transformation) sets $a^{(n)}=0$. The nonzero modes are massive vectors whose longitudinal polarization is supplied by $a^{(n)}$ through the [Stueckelberg mechanism](../../../relativistic-quantum-field.md#stueckelberg-mechanism):

$$
\boxed{m_n=\frac{|n|}{r}\quad(n\ne0).}
$$

For each positive $n$ there is one complex vector, equivalently the two real sine/cosine vectors, each with three physical polarizations. The negative mode is its conjugate, not another independent complex field. This is the infinite [Kaluza-Klein tower](../../../physics.md#kaluza-klein-tower) of the [Maxwell reduction on a circle](../../../physics.md#maxwell-reduction-on-a-circle).

At $n=0$, $\delta a^{(0)}=0$ under periodic infinitesimal gauge transformations. The zero modes are a massless vector with two polarizations and a real massless scalar with one. The scalar is the circle component, or [Wilson line](../../../relativistic-quantum-field.md#wilson-line) degree of freedom; a generic constant value cannot be removed by a periodic gauge parameter. Both have $m_0=0$. At energies $E\ll1/r$, the free theory's [low-energy effective action](../../../quantum-field-theory.md#low-energy-effective-action) is therefore

$$
\boxed{S_{\mathrm{low}}=\int d^4x\left[-\frac14F_{\mu\nu}^{(0)}F^{\mu\nu(0)}
+\frac12\partial_\mu a^{(0)}\partial^\mu a^{(0)}\right].}
$$

There is no scalar potential in this free Maxwell theory. If the original action instead has coefficient $1/g_5^2$ and unrescaled constant zero-mode fields are used, integrating the circle gives $g_4^2=g_5^2/(2\pi r)$; canonical field rescaling recovers the normalization displayed above.

For the gravitational part, allow a circle radius field $R(x)$ with vacuum value $r$, and use a dimensionless angle $\chi\sim\chi+2\pi$ in the [Kaluza-Klein theory](../../../physics.md#kaluza-klein-theory) ansatz

$$
ds_5^2=g_{\mu\nu}(x)dx^\mu dx^\nu
-R(x)^2\bigl[d\chi+\kappa A_\mu(x)dx^\mu\bigr]^2.
$$

The vector comes from off-diagonal metric components; $R$ is the [radion](../../../physics.md#radion). Perform the coordinate transformation $\chi'=\chi-\kappa\lambda(x)$, leaving $x$ unchanged. Since $d\chi=d\chi'+\kappa\partial_\mu\lambda\,dx^\mu$, the metric has the same form with

$$
\boxed{A_\mu'=A_\mu+\partial_\mu\lambda,\qquad R'=R,\qquad g_{\mu\nu}'=g_{\mu\nu}.}
$$

Thus a higher-dimensional [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) becomes an Abelian [gauge transformation](../../../electromagnetism.md#gauge-transformation) in the reduced theory. Changing the sign convention for the internal coordinate shift reverses the displayed sign without changing its content.

More generally, continuous internal isometries give lower-dimensional [gauge symmetries](../../../relativistic-quantum-field.md#gauge-invariance), with vector fields from metric components along the corresponding [Killing vector fields](../../../general-relativity.md#killing-vector-field). The circle translation group gives $U(1)$. A scalar mode $\psi_n(x)e^{in\chi}$ transforms as $\psi_n'=e^{in\kappa\lambda}\psi_n$, so $D_\mu\psi_n=(\partial_\mu-in\kappa A_\mu)\psi_n$ transforms covariantly. This derives [Kaluza-Klein charge quantization](../../../physics.md#kaluza-klein-charge-quantization) in the chosen vector normalization. The metric vector is a graviphoton; if a five-dimensional Maxwell field is present as well, its zero-mode photon is a separate field originating from that Maxwell gauge symmetry.

## 4

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Take canonical kinetic terms, gauge coupling $g>0$, and a nonzero charge $q$. Define $e=gq$ and choose the convention in which the [Fayet–Iliopoulos term](../../../supersymmetry.md#fayet-iliopoulos-term) contributes $\xi D$ to the [Lagrangian](../../../calculus-of-variations.md#lagrangian). With one charged [chiral superfield](../../../supersymmetry.md#chiral-superfield), gauge invariance permits no nonconstant polynomial [superpotential](../../../supersymmetry.md#superpotential); an irrelevant global constant gives $F=0$. The real [auxiliary field](../../../supersymmetry.md#auxiliary-field) part is

$$
\mathcal L_D=\frac12D^2+D(\xi+e|\phi|^2).
$$

Its equation of motion is $D=-(\xi+e|\phi|^2)$. Eliminating it gives the [D-term scalar potential](../../../supersymmetry.md#d-term-scalar-potential)

$$
\boxed{V_D=\frac12(\xi+e|\phi|^2)^2.}
$$

The [gaugino](../../../supersymmetry.md#gaugino) transformation has the form $\delta\lambda=i\epsilon D+$ a field-strength term, with a convention-dependent overall phase. In a translationally invariant vacuum with zero field strength, a nonzero $\langle D\rangle$ therefore gives an inhomogeneous shift of $\lambda$: no nonzero [supersymmetry](../../../supersymmetry.md) parameter leaves the vacuum invariant. The massless [Goldstino](../../../supersymmetry.md#goldstino) is consequently the [gaugino](../../../supersymmetry.md#gaugino), not the matter fermion, since $F=0$.

Minimize the potential over $u=|\phi|^2\geq0$. If $q\xi<0$, the allowed value $u=-\xi/e$ sets $D=0$, so [supersymmetry](../../../supersymmetry.md) is unbroken while the internal gauge symmetry is Higgsed. If $\xi=0$, the origin also has $D=0$. For the broken branch, $q\xi>0$ and the formal zero of $D$ would require negative $u$. The actual minimum is

$$
\boxed{\langle\phi\rangle=0,\qquad\langle D\rangle=-\xi,
\qquad V_{\min}=\frac12\xi^2>0,
\qquad q\xi>0.}
$$

This is [single charged-field D-term breaking](../../../supersymmetry.md#single-charged-field-d-term-breaking). Nonzero FI parameter alone does not force breaking if a scalar can cancel it. The degenerate case $q=0$ is different: any $\xi\ne0$ breaks [supersymmetry](../../../supersymmetry.md) in the vector sector while the neutral scalar remains flat; the sign test above assumes an actually charged field.

Expand around the broken vacuum:

$$
V_D=\frac12\xi^2+e\xi|\phi|^2+\frac12e^2|\phi|^4.
$$

For $\phi=(\phi_R+i\phi_I)/\sqrt2$, both canonically normalized real scalars have squared mass $e\xi=gq\xi>0$. The matter [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) has no [superpotential](../../../supersymmetry.md#superpotential) mass. The gauge boson remains massless because $\langle\phi\rangle=0$. The gauge Yukawa coupling, proportional to $\phi^*\lambda\psi$, gives no fermion mixing or mass at this vacuum, so the [gaugino](../../../supersymmetry.md#gaugino) is also massless. The tree-level spectrum is therefore

$$
\begin{array}{c|c}
\text{field}&\text{squared mass}\\\hline
\phi_R,\phi_I&gq\xi\\
\psi&0\\
A_\mu&0\\
\lambda\ \text{(Goldstino)}&0
\end{array}
$$

and the chiral-multiplet splitting is

$$
\boxed{m_{\mathrm{scalar}}^2-m_{\mathrm{fermion}}^2=gq\xi,\qquad
m_{\mathrm{scalar}}=\sqrt{gq\xi}.}
$$

The vector and its [gaugino](../../../supersymmetry.md#gaugino) happen to remain degenerate at zero mass even though [supersymmetry](../../../supersymmetry.md) is broken. If the sign convention for the FI contribution is reversed, the sign criterion changes accordingly; the invariant condition is that the scalar condensate cannot cancel the auxiliary source. This is the classical toy-model spectrum; a quantum completion of the single charged-fermion theory also has to cancel its [gauge anomalies](../../../relativistic-quantum-field.md#gauge-anomaly).

## 5

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Set $x=T+\bar T>0$, the domain in which the [Kähler potential](../../../supersymmetry.md#kahler-potential) is defined, and use Planck units. The nonzero entries of the [Kähler metric](../../../complex-geometry.md#kahler-metric) and its inverse are

$$
K_{T\bar T}=\frac3{x^2},\qquad K_{C\bar C}=1,
\qquad K^{T\bar T}=\frac{x^2}{3},\qquad K^{C\bar C}=1.
$$

The [Kähler covariant derivatives of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) are

$$
D_TW=-\frac3x(C^3+B),\qquad
D_CW=3C^2+\bar C(C^3+B).
$$

Denote $W=C^3+B$ and $S=3C^2+\bar C W$. The [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) is

$$
V=e^K\left(K^{T\bar T}|D_TW|^2+|D_CW|^2-3|W|^2\right).
$$

Here the $T$ contribution is exactly $3|W|^2$, cancelling the negative term. This is the [no-scale supergravity](../../../supersymmetry.md#no-scale-supergravity) identity, giving

$$
\boxed{V(T,C)=\frac{e^{|C|^2}}{x^3}\left|3C^2+\bar C(C^3+B)\right|^2\geq0.}
$$

The cancellation is important: replacing the covariant derivatives by ordinary derivatives would miss both the matter dependence and the possibility of zero [vacuum energy](../../../perturbative-quantum-field-theory.md#vacuum-energy) with [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking).

In the convention $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$, the chiral [supergravity auxiliary fields](../../../supersymmetry.md#supergravity-auxiliary-field) are

$$
\boxed{F^T=e^{K/2}x\overline W
=\frac{e^{|C|^2/2}}{\sqrt x}(\bar C^3+\bar B),}
$$



$$
\boxed{F^C=-e^{K/2}\overline S
=-\frac{e^{|C|^2/2}}{x^{3/2}}
\left[3\bar C^2+C(\bar C^3+\bar B)\right].}
$$

An overall auxiliary phase or sign convention does not change their vanishing conditions. These are upper-index fields, including the inverse [Kähler metric](../../../complex-geometry.md#kahler-metric), rather than just the covariant derivatives.

Since $V$ is nonnegative and vanishes at $C=0$, its minimum energy is

$$
\boxed{V_{\min}=0.}
$$

There are additional minima that should not be discarded by examining only real $C$. For $C=\rho e^{i\alpha}\ne0$, the condition $S=0$ becomes

$$
B=-\rho(3+\rho^2)e^{3i\alpha}.
$$

If $B\ne0$, the magnitude equation

$$
\rho^3+3\rho=|B|
$$

has exactly one positive root: its left side is strictly increasing from zero to infinity. There are three phases, differing by $2\pi/3$, determined by $e^{3i\alpha}=-B/|B|$. Thus for nonzero $B$ the finite zero-energy matter vacua consist of $C=0$ and these three nonzero phase-related values, each with arbitrary $T$ in the allowed half-plane. At a nonzero matter vacuum,

$$
W=C^3+B=-3\rho e^{3i\alpha}\ne0.
$$

At $C=0$, $W=B$.

For $B\ne0$, every such minimum has $F^C=0$ but $F^T\ne0$, so **supersymmetry is spontaneously broken despite zero vacuum energy**. Indeed no finite point anywhere is fully supersymmetric: $D_TW=0$ would force $W=0$, after which $D_CW=3C^2=0$ forces $C=0$ and then $B=0$. This proves breaking for the specified nonzero-constant case without relying just on the positivity of the potential.

**For the allowed exceptional value (B=0), the requested breaking statement is false.** Then $S=C^2(3+|C|^2)$ vanishes only at $C=0$, where $W=F^T=F^C=0$. Every finite allowed $T$ gives an unbroken [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) with zero energy. This is an explicit counterexample to unqualified breaking for an arbitrary complex $B$.

Both real components of $T$ are [flat directions of a scalar potential](../../../quantum-field-theory.md#flat-direction-of-a-scalar-potential) along every minimum: the imaginary component never appears in $V$, and when $S=0$ the entire $x$ dependence is multiplied by zero. The matter vacua are isolated in the $C$ plane; there is no continuous matter vacuum direction. At $B=0$ the potential begins quartically in $C$, so zero quadratic mass is not a flat vacuum manifold. Away from $S=0$, the real $T$ direction instead has $V\propto x^{-3}$ and a decompactification-type runaway towards zero as $x\to\infty$, not a further finite positive-energy minimum.

The [gravitino mass from a superpotential](../../../supersymmetry.md#gravitino-mass-from-a-superpotential) is

$$
\boxed{m_{3/2}=e^{K/2}|W|
=\frac{e^{|C|^2/2}|C^3+B|}{x^{3/2}}.}
$$

At the $C=0$ branch it is $|B|/x^{3/2}$; at each nonzero branch it is $3\rho e^{\rho^2/2}/x^{3/2}$. Its value is not fixed because the $T$ modulus is flat. For $B=0$ it vanishes at the supersymmetric minimum. For nonzero $B$, the [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism) absorbs the [Goldstino](../../../supersymmetry.md#goldstino) associated with $F^T$ into the massive [gravitino](../../../supersymmetry.md#gravitino). The zero-energy relation is explicitly satisfied:

$$
K_{T\bar T}|F^T|^2=3e^K|W|^2=3m_{3/2}^2,
$$

which balances the auxiliary contribution against the gravitational negative term.

## 6

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Work with metric $\eta=\operatorname{diag}(1,-1,-1,-1)$, $\sigma^\mu=(I,\boldsymbol\sigma)$ and $\bar\sigma^\mu=(I,-\boldsymbol\sigma)$, where $\boldsymbol\sigma$ are the [Pauli matrices](../../../algebra.md#pauli-matrices). The [supercharges](../../../supersymmetry.md#supersymmetry-generator) of [four-dimensional N=1 supersymmetry](../../../supersymmetry.md#four-dimensional-n-1-supersymmetry) form one [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) $Q_\alpha$ and its conjugate $\bar Q_{\dot\alpha}$. Dotted and undotted indices cannot be interchanged; the conjugate charge in the printed mixed relation has a dotted index.

A direct derivation starts from [superspace](../../../supersymmetry.md#superspace) coordinates $x^\mu,\theta^\alpha,\bar\theta^{\dot\alpha}$, with the four odd coordinates generating a [Grassmann algebra](../../../linear-algebra.md#grassmann-algebra). Use left [Grassmann derivatives](../../../linear-algebra.md#grassmann-derivative), so

$$
\partial_\alpha(\theta^\gamma f)=\delta_\alpha^\gamma f-\theta^\gamma\partial_\alpha f,
\qquad
\bar\partial_{\dot\beta}(\bar\theta^{\dot\gamma}f)
=\delta_{\dot\beta}^{\dot\gamma}f-\bar\theta^{\dot\gamma}\bar\partial_{\dot\beta}f.
$$

Odd derivatives anticommute with one another, and multiplication by distinct odd coordinates also anticommutes. The operators specified by the question can be written

$$
\mathcal P_\mu=-i\partial_\mu,\qquad
\mathcal Q_\alpha=-i\partial_\alpha
-\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,
\qquad
\bar{\mathcal Q}_{\dot\beta}=i\bar\partial_{\dot\beta}
+\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu.
$$

Their coefficients do not depend on $x$, hence $[\mathcal Q_\alpha,\mathcal P_\mu]=[\bar{\mathcal Q}_{\dot\alpha},\mathcal P_\mu]=0$. Within $\{\mathcal Q_\alpha,\mathcal Q_\beta\}$, the two odd derivative terms anticommute; the derivatives of the barred-coordinate coefficients vanish; and the two barred-coordinate multiplication terms cancel because the coordinates anticommute while the spacetime derivatives commute. Thus

$$
\{\mathcal Q_\alpha,\mathcal Q_\beta\}=0,
\qquad
\{\bar{\mathcal Q}_{\dot\alpha},\bar{\mathcal Q}_{\dot\beta}\}=0.
$$

This realizes the minimal algebra with no extra tensorial charges.

For the mixed [anticommutator](../../../vector-space.md#anticommutator), split each operator into its odd derivative and odd-coordinate parts. The derivative/derivative anticommutator is zero. The coordinate/coordinate terms also cancel, since $\theta\bar\theta=-\bar\theta\theta$. The two remaining pieces are

$$
\{-i\partial_\alpha,\ \theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu\}
=-i\sigma^\mu_{\alpha\dot\beta}\partial_\mu,
$$



$$
\{-\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,
\ i\bar\partial_{\dot\beta}\}
=-i\sigma^\mu_{\alpha\dot\beta}\partial_\mu.
$$

Adding gives the [superspace differential realization of N=1 supercharges](../../../supersymmetry.md#superspace-differential-realization-of-n-1-supercharges):

$$
\boxed{\{\mathcal Q_\alpha,\bar{\mathcal Q}_{\dot\beta}\}
=-2i\sigma^\mu_{\alpha\dot\beta}\partial_\mu
=2\sigma^\mu_{\alpha\dot\beta}\mathcal P_\mu.}
$$

In particular the differentiated-coordinate contributions have the same sign, not opposite signs. The graded product rule is the essential step; treating these as ordinary commuting-coordinate derivatives would give an incorrect algebra.

To obtain the Lorentz part, let $x$ transform as a four-vector and $\theta,\bar\theta$ in conjugate spinor representations. Define

$$
\Sigma^{\mu\nu}=\frac14(\sigma^\mu\bar\sigma^\nu-\sigma^\nu\bar\sigma^\mu),
\qquad
\bar\Sigma^{\mu\nu}=\frac14(\bar\sigma^\mu\sigma^\nu-\bar\sigma^\nu\sigma^\mu).
$$

The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives the intertwining identity

$$
\Sigma^{\mu\nu}\sigma^\rho-\sigma^\rho\bar\Sigma^{\mu\nu}
=\eta^{\nu\rho}\sigma^\mu-\eta^{\mu\rho}\sigma^\nu.
$$

It shows that the two terms in $\mathcal Q_\alpha$ transform together as a covariant [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor): the coordinate derivative transforms in the dual spinor representation, while the barred-coordinate/spacetime-derivative term transforms in that same representation through this identity. Infinitesimally, with $U=\exp[-\tfrac i2\omega_{\mu\nu}M^{\mu\nu}]$, its transformation is $UQ_\alpha U^{-1}=Q_\alpha-\tfrac12\omega_{\mu\nu}(\Sigma^{\mu\nu})_\alpha{}^\beta Q_\beta$. Comparing with the first-order expansion of $U$ gives

$$
[Q_\alpha,M^{\mu\nu}]=i(\Sigma^{\mu\nu})_\alpha{}^\beta Q_\beta.
$$

If the paper's spin matrix is denoted $\sigma^{\mu\nu}=i\Sigma^{\mu\nu}$, this is exactly its first displayed relation. Defining that spin matrix without the factor $i$ instead requires an explicit $i$ in the commutator; this is a generator convention, not a different algebra. The conjugate relation follows by Hermitian conjugation.

Combining the Lorentz transformation with the differential computations gives the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) in the question's notation:

$$
\boxed{[Q_\alpha,M^{\mu\nu}]=(\sigma^{\mu\nu})_\alpha{}^\beta Q_\beta,\quad
[Q_\alpha,P^\mu]=0,\quad\{Q_\alpha,Q_\beta\}=0,\quad
\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu.}
$$

The even generators retain the ordinary [Poincare algebra](../../../special-relativity.md#poincare-algebra). As a closure check, the even superspace variation $\delta=i(\epsilon\mathcal Q-\bar\epsilon\bar{\mathcal Q})$ gives $\delta\theta=\epsilon$, $\delta\bar\theta=\bar\epsilon$ and $\delta x^\mu=i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta$. Two such variations commute to a translation by $2i(\epsilon_1\sigma^\mu\bar\epsilon_2-\epsilon_2\sigma^\mu\bar\epsilon_1)$, with zero commutator on the odd coordinates, reproducing the same normalization and showing why the anticommutator produces momentum.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
