# Paper 43

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_43.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_43.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [Scalar potential](#2/scalar-potential)
    - [Solution](#2/scalar-potential/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Fix the [Minkowski metric](../../../special-relativity.md#minkowski-metric) convention $\eta=\operatorname{diag}(1,-1,-1,-1)$ and the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) $\epsilon_{123}=1$. The antisymmetry of the [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra) generators gives $M_{i0}=-K_i$ and the inverse relation $M_{ij}=\epsilon_{ijk}J_k$. Inserting one temporal index in each generator immediately yields

$$
[K_i,K_j]=-i\eta_{00}M_{ij}=-i\epsilon_{ijk}J_k.
$$

Two [Lorentz boosts](../../../special-relativity.md#lorentz-boost) therefore generate a rotation through their [commutator](../../../lie-algebra.md#commutator); the minus sign distinguishes this algebra from the rotation algebra in four-dimensional Euclidean space.

For a spatial generator and a boost, the same [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra) gives

$$
[M_{ab},M_{0j}]=i(\delta_{aj}K_b-\delta_{bj}K_a).
$$

Contracting with $\epsilon_{iab}/2$ gives

$$
[J_i,K_j]=\frac i2\epsilon_{iab}(\delta_{aj}K_b-\delta_{bj}K_a)
=i\epsilon_{ijk}K_k.
$$

Thus the three [Lorentz boosts](../../../special-relativity.md#lorentz-boost) transform as a spatial vector under rotations.

Finally, the all-spatial bracket becomes

$$
[M_{ab},M_{cd}]
=i(-\delta_{bc}M_{ad}-\delta_{ad}M_{bc}+\delta_{bd}M_{ac}+\delta_{ac}M_{bd}).
$$

Use $M_{ab}=\epsilon_{abr}J_r$ in the double contraction with $\epsilon_{iab}\epsilon_{jcd}/4$. The epsilon contraction identity reduces it to $[J_i,J_j]=i\epsilon_{ijk}J_k$. One can check the sign directly: $J_1=M_{23}$ and $J_2=M_{31}$ give $[J_1,J_2]=iM_{12}=iJ_3$; cyclic permutations give the other nonzero brackets. The requested coefficients are

$$
\boxed{(A_1,B_1)=(-1,0),\qquad(A_2,B_2)=(0,1),\qquad(A_3,B_3)=(1,0).}
$$

These are [rotation and boost commutators with a fixed metric signature](../../../semisimple-lie-algebra.md#rotation-and-boost-commutators-with-a-fixed-metric-signature). The PDF does not explicitly specify the signature. Keeping its generator convention but choosing $\eta=\operatorname{diag}(-1,1,1,1)$ reverses every displayed algebra coefficient: the pairs become $(1,0),(0,-1),(-1,0)$. More generally, if $s=\eta_{00}=\pm1$, the three nonzero coefficients are $A_1=-s$, $B_2=s$ and $A_3=s$. Specifying the [Minkowski metric](../../../special-relativity.md#minkowski-metric) is therefore necessary to make the numerical signs unambiguous.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [hierarchy problem](../../../standard-model.md#hierarchy-problem) begins with a large separation of scales: the weak scale is much smaller than possible unification or gravitational scales. A fundamental [scalar mass](../../../quantum-field-theory.md#scalar-mass) is especially sensitive to a much heavier scale. In an effective description with ultraviolet cutoff $\Lambda$, one schematically finds

$$
m_H^2=m_{H,\mathrm{bare}}^2+\delta m_H^2,\qquad
\delta m_H^2\sim\frac{c}{16\pi^2}\Lambda^2.
$$

The coefficient $c$ contains gauge, scalar and [Yukawa couplings](../../../standard-model.md#yukawa-interaction), with different signs for bosonic and fermionic loops. The explicit quadratic cutoff dependence is regulator-dependent, but a heavy physical particle coupled to the Higgs produces a threshold correction of order its mass squared. That heavy-threshold sensitivity is the physical difficulty.

The [technical hierarchy problem](../../../standard-model.md#technical-hierarchy-problem) asks whether a small scale, once chosen, remains stable under such [radiative corrections](../../../perturbative-quantum-field-theory.md#radiative-correction). Maintaining $m_H^2\ll\Lambda^2$ by cancelling unrelated bare and loop contributions, and readjusting the cancellation at successive orders, is the [naturalness](../../../standard-model.md#naturalness-physics) concern. It is different from explaining why the small scale was chosen in the first place. [Supersymmetry](../../../supersymmetry.md) primarily supplies protection against the technical instability; a complete explanation of the origin of supersymmetry-breaking scales needs additional dynamics.

The relevant comparison of mass types is:

- For a [gauge boson](../../../relativistic-quantum-field.md#gauge-boson), an explicit Proca mass term is forbidden by an unbroken [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance). This is [gauge protection of a vector mass](../../../standard-model.md#gauge-protection-of-a-vector-mass). In a Higgs phase, a vector mass is of order $gv$, but the stability of $v$ then depends on the [scalar mass](../../../quantum-field-theory.md#scalar-mass) that determines the symmetry-breaking scale. Gauge invariance does not, by itself, solve that scalar problem.
- A chiral [fermion](../../../quantum-mechanics.md#fermion) mass is protected because setting it to zero restores an appropriate chiral symmetry. Perturbative corrections cannot generate a symmetry-forbidden mass; schematically $\delta m_f\propto m_f\log\Lambda$. In the [Standard Model](../../../standard-model.md), chiral gauge quantum numbers prohibit a bare fermion mass, and the [Higgs mechanism](../../../standard-model.md#higgs-mechanism) permits masses through [Yukawa couplings](../../../standard-model.md#yukawa-interaction). This is [chiral protection of a fermion mass](../../../standard-model.md#chiral-protection-of-a-fermion-mass), rather than an additive correction of order $\Lambda$.
- A [squark](../../../supersymmetry.md#squark) or [slepton](../../../supersymmetry.md#slepton) is a scalar. Its bilinear $\widetilde f^\dagger\widetilde f$ is allowed by gauge symmetries and by the ordinary chiral phase symmetry of its fermion partner. Consequently, without [supersymmetry](../../../supersymmetry.md), those symmetries do not protect a small [scalar mass](../../../quantum-field-theory.md#scalar-mass) against corrections of order $\Lambda^2$.

In exact [supersymmetry](../../../supersymmetry.md), each [supermultiplet](../../../supersymmetry.md#supermultiplet) has matched bosonic and fermionic degrees of freedom, with their interaction strengths related. Opposite loop signs then give [supersymmetric cancellation of quadratic divergences](../../../supersymmetry.md#supersymmetric-cancellation-of-quadratic-divergences). This is not just equality of state counts: the [supersymmetric relation between quartic and Yukawa couplings](../../../supersymmetry.md#supersymmetric-relation-between-quartic-and-yukawa-couplings) is also essential. A schematic paired-loop contribution has the high-momentum form

$$
\delta m_H^2\propto |y|^2\int^{\Lambda}\frac{d^4p_E}{(2\pi)^4}
\left[\frac1{p_E^2+m_B^2}-\frac1{p_E^2+m_F^2}\right].
$$

For equal partner masses the displayed contributions cancel. With a small splitting, the difference falls as $(m_F^2-m_B^2)/p_E^4$, so the remaining ultraviolet sensitivity is logarithmic, proportional to the splitting rather than to $\Lambda^2$.

Realistic partners need not have exactly equal masses. [Soft supersymmetry breaking](../../../supersymmetry.md#soft-supersymmetry-breaking) permits scalar squared masses, gaugino masses and suitable trilinear interactions without restoring the unwanted quadratic sensitivity. Typically,

$$
\delta m_H^2\sim\frac{|y|^2}{16\pi^2}m_{\mathrm{soft}}^2
\log\frac{\Lambda}{m_{\mathrm{soft}}},
$$

up to coefficients and threshold details. Squarks and sleptons can therefore be heavier than their chiral fermion partners while the scalar sector remains stable against the much larger ultraviolet scale. Nevertheless, very large soft masses, particularly in the Higgs-coupled sector, leave large finite or logarithmic corrections and require tuning. This [soft scalar-mass sensitivity](../../../supersymmetry.md#soft-scalar-mass-sensitivity) remains after the quadratic divergence has cancelled. **Supersymmetry solves the quadratic radiative instability when breaking is suitably soft; it does not make arbitrarily heavy superpartners natural or explain the entire hierarchy by itself.**

## 2

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the usual normalization of the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra), with $\sigma^\mu=(\mathbf1,\boldsymbol\sigma)$ and $\bar Q_{\dot\alpha}=Q_\alpha^\dagger$ under the corresponding index convention:

$$
\boxed{\{Q_\alpha,\bar Q_{\dot\beta}\}
=2\sigma^\mu_{\alpha\dot\beta}P_\mu.}
$$

The [supercharges](../../../supersymmetry.md#supersymmetry-generator) are odd operators: they turn bosonic states into fermionic states and vice versa. If $\Pi=(-1)^F$ is [fermion parity](../../../topological-quantum-matter.md#fermion-parity), this statement is $\Pi Q_\alpha\Pi^{-1}=-Q_\alpha$, so

$$
\boxed{\{(-1)^F,Q_\alpha\}=0.}
$$

The same relation holds for the conjugate [supercharges](../../../supersymmetry.md#supersymmetry-generator).

For a finite-dimensional physical [supermultiplet](../../../supersymmetry.md#supermultiplet) at fixed four-momentum with energy $E>0$, let $n_B,n_F$ count physical bosonic and fermionic states. Cyclicity of the ordinary trace and the parity anticommutation imply

$$
\operatorname{Tr}\bigl(\Pi\{Q_\alpha,Q_\alpha^\dagger\}\bigr)=0:
\quad
\operatorname{Tr}(\Pi Q_\alpha^\dagger Q_\alpha)
=\operatorname{Tr}(Q_\alpha\Pi Q_\alpha^\dagger)
=-\operatorname{Tr}(\Pi Q_\alpha Q_\alpha^\dagger).
$$

Summing over the two spinor indices gives

$$
0=4E\operatorname{Tr}\Pi=4E(n_B-n_F),
\qquad\boxed{n_B=n_F.}
$$

This [supertrace pairing at positive energy](../../../supersymmetry.md#supertrace-pairing-at-positive-energy) proves [boson-fermion degeneracy in a supermultiplet](../../../supersymmetry.md#boson-fermion-degeneracy-in-a-supermultiplet) for massive as well as massless positive-energy representations. It counts on-shell polarizations, not merely the names of fields. The requirement $E>0$ matters: a zero-energy [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) can be a bosonic singlet without a paired fermionic vacuum.

If supersymmetry-breaking operators are explicitly added to the [Lagrangian](../../../calculus-of-variations.md#lagrangian), the original [supercharges](../../../supersymmetry.md#supersymmetry-generator) generally no longer commute with the full Hamiltonian. They are not conserved symmetries generating finite fixed-energy physical [supermultiplets](../../../supersymmetry.md#supermultiplet); their original anticommutator does not equal the full translation generator with the breaking terms included. Thus the step replacing the parity-weighted anticommutator by $4E\Pi$ on a closed physical representation fails. The odd parity relation alone does not force energy degeneracy or an equal number of physical states at each mass.

This is [explicit versus spontaneous supersymmetry breaking](../../../supersymmetry.md#explicit-versus-spontaneous-supersymmetry-breaking). In spontaneous breaking the action still has conserved [supercharges](../../../supersymmetry.md#supersymmetry-generator), but the vacuum is not annihilated by them. Acting on particle excitations about that vacuum involves the broken-vacuum/Goldstino sector, so an ordinary finite particle multiplet above an invariant vacuum is no longer the correct pairing argument. The vacuum-energy statements below refer to an exact globally supersymmetric Hamiltonian, including the spontaneously broken case; they are not positivity claims for an arbitrary explicitly broken Hamiltonian.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Sum the diagonal spinor entries of the [supercharge](../../../supersymmetry.md#supersymmetry-generator) anticommutator. Since $\operatorname{tr}\sigma^i=0$ and $\operatorname{tr}\sigma^0=2$, the Hamiltonian is

$$
H=\frac14\sum_{\alpha=1}^2\{Q_\alpha,Q_\alpha^\dagger\}.
$$

For a normalized vacuum, [energy positivity in global supersymmetry](../../../supersymmetry.md#energy-positivity-in-global-supersymmetry) follows from

$$
\boxed{E_{\mathrm{vac}}=\frac14\sum_\alpha
\left(\|Q_\alpha|\mathrm{vac}\rangle\|^2+
\|Q_\alpha^\dagger|\mathrm{vac}\rangle\|^2\right)\geq0.}
$$

In the unbroken case, all [supercharges](../../../supersymmetry.md#supersymmetry-generator) annihilate the vacuum, giving **$E_{\mathrm{vac}}=0$**. Conversely, zero energy forces each nonnegative norm to vanish, so the vacuum is supersymmetric. The algebra fixes the additive zero of energy here. For an infinite homogeneous vacuum, use a finite-volume regulator and interpret the result as its [vacuum energy](../../../perturbative-quantum-field-theory.md#vacuum-energy) density.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For spontaneous breaking of exact global [supersymmetry](../../../supersymmetry.md), at least one [supercharge](../../../supersymmetry.md#supersymmetry-generator) does not annihilate the vacuum. Its norm in the preceding expression is positive, hence

$$
\boxed{E_{\mathrm{vac}}>0\quad\text{for a spontaneously broken global supersymmetric vacuum}.}
$$

With canonical [kinetic terms](../../../quantum-field-theory.md#kinetic-term), this is also seen in the nonnegative [scalar potential](#2/scalar-potential), $V=\sum_i|F_i|^2+\tfrac12\sum_aD_a^2$: nonzero auxiliary expectation values signal breaking and positive energy density. The associated massless fermion is the [Goldstino](../../../supersymmetry.md#goldstino).

If “broken” instead means arbitrary explicit breaking by added operators, the exact [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) no longer fixes the full Hamiltonian, and the positive-norm argument does not constrain its vacuum energy. One can, for example, shift that explicitly broken Hamiltonian by a constant. The strict positivity conclusion therefore uses spontaneous breaking of an otherwise exact global theory, not a blanket assertion about all breaking terms. It also is not a statement about [supergravity](../../../supersymmetry.md#supergravity), whose scalar potential contains additional terms.

<h3 id="2/scalar-potential">Scalar potential</h3>

↑ **Parent:** [2](#2)

<h4 id="2/scalar-potential/solution">Solution</h4>

↑ **Parent:** [Scalar potential](#2/scalar-potential)

Take canonical charged [chiral superfield](../../../supersymmetry.md#chiral-superfield) kinetic terms, gauge coupling $e>0$, and no [Fayet–Iliopoulos term](../../../supersymmetry.md#fayet-iliopoulos-term), since none is specified. Elimination of the three complex [auxiliary fields](../../../supersymmetry.md#auxiliary-field) gives

$$
F_+^*=-\lambda\varphi_0\varphi_-,\qquad
F_0^*=-\lambda\varphi_+\varphi_-,\qquad
F_-^*=-\lambda\varphi_+\varphi_0.
$$

The Abelian gauge [auxiliary field](../../../supersymmetry.md#auxiliary-field) obeys $D=-e(|\varphi_+|^2-|\varphi_-|^2)$ in this normalization. Thus the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) and the gauge [D-term](../../../supersymmetry.md#d-term) give

$$
\boxed{V=|\lambda|^2\left(|\varphi_0|^2|\varphi_-|^2
+|\varphi_+|^2|\varphi_-|^2+|\varphi_+|^2|\varphi_0|^2\right)
+\frac{e^2}{2}\left(|\varphi_+|^2-|\varphi_-|^2\right)^2.}
$$

All terms are nonnegative. The normalization of $e$ can be changed together with the vector-field normalization, but the relative charges and the zero-potential conditions cannot. A noncanonical [Kähler potential](../../../supersymmetry.md#kahler-potential) would change the inverse-metric factors in the F-term potential; adding a [Fayet–Iliopoulos term](../../../supersymmetry.md#fayet-iliopoulos-term) would shift $D$ and define a different model. Neither is silently introduced here.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For nonzero $\lambda$, zero potential requires both [F-flatness](../../../supersymmetry.md#f-flatness) and [D-flatness](../../../supersymmetry.md#d-flatness):

$$
\varphi_+\varphi_-=0,\quad\varphi_0\varphi_-=0,\quad
\varphi_0\varphi_+=0,\qquad |\varphi_+|=|\varphi_-|.
$$

The product condition and equality of charged magnitudes together force $\varphi_+=\varphi_-=0$. There is no condition on the neutral scalar. Consequently the global minima form

$$
\boxed{\varphi_+=\varphi_-=0,\qquad\varphi_0=v\in\mathbb C,\qquad V_{\min}=0.}
$$

Only the neutral field can acquire a [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value). It does not give the gauge vector a mass: its scalar [kinetic term](../../../quantum-field-theory.md#kinetic-term) has no charged covariant derivative. Hence **the gauged $U(1)$ remains unbroken in every global minimum for $\lambda\ne0$**. This is a [neutral flat direction with oppositely charged chiral fields](../../../supersymmetry.md#neutral-flat-direction-with-oppositely-charged-chiral-fields); a continuous vacuum family is not automatically gauge-symmetry breaking.

The exceptional uncoupled case $\lambda=0$ should be separated. Then only [D-flatness](../../../supersymmetry.md#d-flatness) remains, allowing $|\varphi_+|=|\varphi_-|=r$ and arbitrary $\varphi_0$. For $r>0$, the charged expectations Higgs the $U(1)$; for $r=0$ it remains unbroken. The usual interacting answer assumes $\lambda\ne0$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Every global minimum found for nonzero $\lambda$ has $F_+=F_0=F_-=D=0$. By [energy positivity in global supersymmetry](../../../supersymmetry.md#energy-positivity-in-global-supersymmetry), its zero energy means all [supercharges](../../../supersymmetry.md#supersymmetry-generator) annihilate it. Therefore

$$
\boxed{\text{Supersymmetry is unbroken throughout the vacuum family}.}
$$

The arbitrary neutral expectation $v$ is a supersymmetric modulus; the nonzero derivatives that would break [supersymmetry](../../../supersymmetry.md) vanish even though $v$ itself need not vanish. In the exceptional $\lambda=0$ case, every [D-flatness](../../../supersymmetry.md#d-flatness) minimum likewise has zero F- and D-auxiliaries, so [supersymmetry](../../../supersymmetry.md) remains unbroken even on the gauge-Higgsed branch. The [supersymmetric Higgs mechanism](../../../supersymmetry.md#supersymmetric-higgs-mechanism) permits internal gauge breaking without supersymmetry breaking. No extra constant or linear superpotential term is needed to find a zero-energy vacuum in this model.

## 3

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

**Chirality and the component expansion.** A [chiral superfield](../../../supersymmetry.md#chiral-superfield) is constrained by

$$
\bar D_{\dot\alpha}\Phi=0.
$$

Use [left Grassmann derivatives](../../../linear-algebra.md#left-grassmann-derivative). The sign from differentiating an odd factor matters:

$$
\bar\partial_{\dot\alpha}(\theta\sigma^\mu\bar\theta)
=-(\theta\sigma^\mu)_{\dot\alpha},\qquad
\bar D_{\dot\alpha}y^\mu=0.
$$

For a general [superfield](../../../supersymmetry.md#superfield) written in coordinates $(y,\theta,\bar\theta)$, the odd chain rule consequently turns the given [superspace covariant derivative](../../../supersymmetry.md#supersymmetric-covariant-derivative) into

$$
\bar D_{\dot\alpha}=-\bar\partial_{\dot\alpha}\big|_y.
$$

The chirality constraint removes the explicit $\bar\theta$ dependence at fixed $y$. There are only two components of $\theta$, and their [Grassmann algebra](../../../linear-algebra.md#grassmann-algebra) allows at most a quadratic monomial. Its finite [chiral-superfield component expansion](../../../supersymmetry.md#chiral-superfield-component-expansion) is therefore

$$
\boxed{\Phi(y,\theta)=\varphi(y)+\sqrt2\theta\psi(y)+\theta^2F_{\mathrm{aux}}(y).}
$$

Here $\varphi$ is a [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field), $\psi$ a [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor), and $F_{\mathrm{aux}}$ a complex [auxiliary field](../../../supersymmetry.md#auxiliary-field); the last label avoids confusing it with the effective superpotential later. The factor $\sqrt2$ is the standard canonical component normalization. In ordinary coordinates the same statement is

$$
\Phi(x,\theta,\bar\theta)=
\exp\left(i\theta\sigma^\mu\bar\theta\,\partial_\mu\right)
\left[\varphi(x)+\sqrt2\theta\psi(x)+\theta^2F_{\mathrm{aux}}(x)\right].
$$

This translation exponential terminates because its shift is nilpotent; it displays the full component dependence without an unstated convention for the barred spinor square.

A [superspace covariant derivative](../../../supersymmetry.md#supersymmetric-covariant-derivative) obeys the graded product rule. Since an ordinary scalar [chiral superfield](../../../supersymmetry.md#chiral-superfield) is even, $\bar D(\Phi^n)=n\Phi^{n-1}\bar D\Phi=0$. Linear combinations prove the polynomial claim. More generally, a nonsingular [holomorphic function](../../../complex-analysis.md#holomorphic-function) of chiral fields is chiral; inserting conjugate fields generally spoils this [holomorphic closure of chiral superfields](../../../supersymmetry.md#holomorphic-closure-of-chiral-superfields).

**The superspace action.** For a real [Kähler potential](../../../supersymmetry.md#kahler-potential) and a [holomorphic superpotential](../../../supersymmetry.md#superpotential), the global chiral-field action has [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density)

$$
\boxed{\mathcal L=\int d^2\theta\,d^2\bar\theta\,
K(\Phi^\dagger,\Phi)
+\left[\int d^2\theta\,W(\Phi)+\mathrm{h.c.}\right].}
$$

Full [superspace integration](../../../supersymmetry.md#superspace-integration) gives a [D-term](../../../supersymmetry.md#d-term), and chiral [superspace integration](../../../supersymmetry.md#superspace-integration) an [F-term](../../../supersymmetry.md#f-term). The action is real, and its supersymmetry variations are spacetime total derivatives. For one field, positive $K_{\varphi\bar\varphi}$ and algebraic elimination give $V=K^{\varphi\bar\varphi}|W_\varphi|^2$. The [Wess–Zumino model](../../../supersymmetry.md#wess-zumino-model) uses the canonical choice $K=\Phi^\dagger\Phi$ at tree level.

**Scalar potential and the vertex.** In canonical normalization, the auxiliary part of the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) is

$$
\mathcal L_{\mathrm{aux}}=|F_{\mathrm{aux}}|^2+
(F_{\mathrm{aux}}W_\varphi+\mathrm{h.c.}),\qquad
F_{\mathrm{aux}}=-\overline{W_\varphi}.
$$

Substitution leaves $\mathcal L_{\mathrm{aux}}=-|W_\varphi|^2$. Differentiating the given quadratic-plus-cubic [superpotential](../../../supersymmetry.md#superpotential) therefore gives the tree-level [effective potential](../../../physics.md#effective-potential)

$$
\boxed{V_{\mathrm{tree}}=|m\varphi+g\varphi^2|^2
=|m|^2|\varphi|^2+m^*g\varphi^*\varphi^2
+mg^*\varphi\varphi^{*2}+|g|^2|\varphi|^4.}
$$

This applies for complex $m,g$. In terms of canonically normalized real fields $\varphi=(A+iB)/\sqrt2$, phases may be chosen to make $m,g$ real, in which case

$$
V_{\mathrm{tree}}=\frac{m^2}{2}(A^2+B^2)
+\frac{mg}{\sqrt2}A(A^2+B^2)
+\frac{g^2}{4}(A^2+B^2)^2.
$$

The complex-field quartic interaction is $\mathcal L_{\mathrm{int}}=-|g|^2\varphi^{*2}\varphi^2$. There are two identical external legs of each field type. Differentiating with respect to those four fields, or counting the Wick attachments to the vertex, produces the factor $2!2!$:

$$
\boxed{\text{two }\varphi\text{ and two }\varphi^*\text{ legs}:
\quad -i\,2!2!|g|^2=-4i|g|^2.}
$$

The local [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram) for this [quartic complex-scalar vertex in the Wess–Zumino model](../../../supersymmetry.md#quartic-complex-scalar-vertex-in-the-wess-zumino-model) is<a id="3/image-quartic-complex-scalar-wess-zumino-vertex-with-two-legs-of-each-field-type-and-its-factorial-normalized-feynman-rule"></a>


![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-43-quartic.png)

**[Figure 1](#3/image-quartic-complex-scalar-wess-zumino-vertex-with-two-legs-of-each-field-type-and-its-factorial-normalized-feynman-rule). Quartic complex-scalar Wess–Zumino vertex with two legs of each field type and its factorial-normalized Feynman rule**.

If real-field [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) are preferred, the $AAAA$ and $BBBB$ vertices are $-6i|g|^2$, while the $AABB$ vertex is $-2i|g|^2$. These are the same interaction in a different component basis. They should not be confused with a convention that absorbs $2!2!$ into the coefficient of the complex quartic term.

**Spurion symmetries.** Treat $m,g$ as chiral [spurions](../../../supersymmetry.md#spurion). An ordinary $U(1)$ acts on $\Phi,m,g$ with charges $(1,-2,-3)$ and leaves $\theta$ neutral. An [R-symmetry](../../../supersymmetry.md#r-symmetry) gives $\theta$ charge one and $\Phi,m,g$ charges $(1,0,-1)$. Thus

| Quantity | Ordinary $U(1)$ | $U(1)_R$ | Mass dimension |
| --- | --- | --- | --- |
| $\Phi$ | 1 | 1 | 1 |
| $m$ | $-2$ | 0 | 1 |
| $g$ | $-3$ | $-1$ | 0 |
| $\theta$ | 0 | 1 | $-1/2$ |
| $W$ | 0 | 2 | 3 |

Each superpotential term has ordinary charge zero and [R-charge](../../../supersymmetry.md#r-charge) two; the chiral integration measure has [R-charge](../../../supersymmetry.md#r-charge) minus two. In particular $m$ is neutral under the specified [R-symmetry](../../../supersymmetry.md#r-symmetry). These are formal transformations of fields and parameters together, not two exact symmetries of a theory with arbitrary fixed nontransforming numerical couplings. This [Wess–Zumino spurion charge assignment](../../../supersymmetry.md#wess-zumino-spurion-charge-assignment) is useful because it constrains possible quantum terms.

**The general holomorphic form.** Let $\mathcal F(\Phi,m,g)$ denote the local effective [superpotential](../../../supersymmetry.md#superpotential), reserving $F_{\mathrm{aux}}$ for the auxiliary component. The [holomorphy argument for superpotential non-renormalization](../../../supersymmetry.md#holomorphy-argument-for-superpotential-non-renormalization) permits dependence on the chiral [spurions](../../../supersymmetry.md#spurion), not on their conjugates. The dimensionless combination $z=g\Phi/m$ is neutral under both formal symmetries, whereas $m\Phi^2$ has the required dimension and charges. Hence, for $m\ne0$, their most general allowed form is

$$
\boxed{\mathcal F(\Phi,m,g)=m\Phi^2 f\left(\frac{g\Phi}{m}\right),}
$$

with a holomorphic function $f$ before perturbative regularity and matching conditions are imposed. Equivalently, a monomial $m^a g^b\Phi^c$ must obey

$$
-2a-3b+c=0,\qquad -b+c=2,\qquad a+c=3.
$$

Solving gives $a=1-b$, $c=b+2$. Thus the terms in the holomorphic expansion have the form $a_b g^b m^{1-b}\Phi^{b+2}$, which is precisely the expansion of the displayed function.

**What is and is not renormalized.** Apply the [non-renormalization theorem](../../../supersymmetry.md#non-renormalization-theorem) to a local [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) retaining the elementary field and a nonzero infrared cutoff. Perturbative coefficients are regular as $g\to0$ and $m\to0$: no massless infrared modes have been integrated all the way to zero momentum. Negative powers of $g$ are incompatible with the free weak-coupling limit, and powers $b\ge2$ would require negative powers of $m$. Only the quadratic and cubic structures survive this regularity test. Their coefficients cannot acquire a loop correction here: a quadratic term with no $g$ is the free-theory mass term, while a cubic term only linear in $g$ is already the tree interaction. A loop renormalizing that cubic term requires additional interaction insertions. Such a dependence is excluded by the holomorphic charge constraints; dependence on $g^*$ cannot repair it in a [superpotential](../../../supersymmetry.md#superpotential). Matching to the specified tree action fixes

$$
f(z)=\frac12+\frac13z,\qquad
\boxed{\mathcal F_{\mathrm{pert}}=\frac12m\Phi^2+\frac13g\Phi^3.}
$$

The $m=0$ limit is taken in the final polynomial, not by evaluating the intermediate ratio $g\Phi/m$. **The holomorphic Wilsonian superpotential and its parameters $m,g$ receive no independent perturbative vertex renormalization.** Symmetries alone would only give the arbitrary function $f$; regularity and the free/tree matching are necessary to reach the stronger conclusion.

The [Kähler potential](../../../supersymmetry.md#kahler-potential) is not protected by that theorem. In particular a corrected [kinetic term](../../../quantum-field-theory.md#kinetic-term) $Z(\mu)\Phi^\dagger\Phi$ leads to [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization). Writing $\Phi_c=Z^{1/2}\Phi$ in canonical normalization gives

$$
\boxed{m_c(\mu)=\frac{m}{Z(\mu)},\qquad
 g_c(\mu)=\frac{g}{Z(\mu)^{3/2}}.}
$$

These [holomorphic and canonically normalized superpotential couplings](../../../supersymmetry.md#holomorphic-and-canonically-normalized-superpotential-couplings) distinguish the two senses of “renormalized”: the physical/canonically normalized parameters can run, entirely through the common field normalization, even when the holomorphic coefficients do not. The scalar effective potential can consequently receive quantum corrections through the [Kähler potential](../../../supersymmetry.md#kahler-potential). Nor does the local perturbative statement automatically apply to infrared-singular one-particle-irreducible actions or to integrating out whole massive fields. **Non-renormalization protects the local holomorphic F-term, not the complete quantum action or every physically normalized mass and coupling.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
