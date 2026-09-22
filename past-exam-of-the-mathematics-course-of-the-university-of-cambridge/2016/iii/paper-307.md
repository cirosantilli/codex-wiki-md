# Paper 307

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_307.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_307.pdf)

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
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Choose a null [four-momentum](../../../special-relativity.md#four-momentum) with $E>0$ and orient the third axis so that $2\sigma^\mu p_\mu=\operatorname{diag}(4E,0)$. The [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) gives

$$
\{Q_1^A,(Q_1^B)^\dagger\}=4E\delta^{AB},\qquad
\{Q_2^A,(Q_2^B)^\dagger\}=0.
$$

For every state $|v\rangle$ in a [unitary representation](../../../representation-theory.md#unitary-representation), the second [anticommutator](../../../vector-space.md#anticommutator) is the sum $\|Q_2^A v\|^2+\|(Q_2^A)^\dagger v\|^2$. Thus both operators act trivially. A [central charge in supersymmetry](../../../supersymmetry.md#central-charge-in-supersymmetry) also vanishes in this [massless supermultiplet](../../../supersymmetry.md#massless-supermultiplet): its mixed-spinor [anticommutator](../../../vector-space.md#anticommutator) contains the now-trivial $Q_2$. The remaining $\mathcal N$ pairs, normalized by $2\sqrt E$, satisfy the [canonical anticommutation relations](../../../quantum-mechanics.md#canonical-anticommutation-relations)

$$
\{a_A,a_B^\dagger\}=\delta_{AB},\qquad
\{a_A,a_B\}=\{a_A^\dagger,a_B^\dagger\}=0.
$$

Label a [Clifford vacuum](../../../quantum-mechanics.md#clifford-vacuum) by its highest [helicity](../../../special-relativity.md#helicity) $\lambda$ and choose the lowering convention $[J_3,a_A^\dagger]=-a_A^\dagger/2$. Acting with distinct [fermionic creation operators](../../../relativistic-quantum-field.md#fermionic-creation-operator) produces the [fermionic Fock space](../../../quantum-mechanics.md#fermionic-fock-space)

$$
a_{A_1}^\dagger\cdots a_{A_k}^\dagger|p,\lambda\rangle,
\qquad
\boxed{h_k=\lambda-\frac{k}{2},\quad n_k=\binom{\mathcal N}{k},\quad k=0,\ldots,\mathcal N}.
$$

This proves the [helicity spectrum of a massless supermultiplet](../../../supersymmetry.md#helicity-spectrum-of-a-massless-supermultiplet) and the $2^{\mathcal N}$ state count. If the internal charges or [helicities](../../../special-relativity.md#helicity) do not already make the spectrum invariant under the [CPT theorem](../../../quantum-field-theory.md#cpt-theorem), add its conjugate using the [CPT completion of a supermultiplet](../../../supersymmetry.md#cpt-completion-of-a-supermultiplet).

The [spin bound for massless supermultiplets](../../../supersymmetry.md#spin-bound-for-massless-supermultiplets) follows directly from the width $\mathcal N/2$ of this [helicity](../../../special-relativity.md#helicity) interval. Requiring $|h|\le1$ gives **$\mathcal N\le4$**, achieved by the [four-dimensional N=4 super Yang-Mills theory](../../../supersymmetry.md#four-dimensional-n-4-super-yang-mills-theory) [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) with multiplicities $1,4,6,4,1$ at [helicities](../../../special-relativity.md#helicity) $1,1/2,0,-1/2,-1$. These [helicity](../../../special-relativity.md#helicity) bounds are necessary spin restrictions for the usual interacting [renormalizable quantum field theory](../../../perturbative-quantum-field-theory.md#renormalizable-quantum-field-theory); they do not by themselves establish renormalizability for an arbitrary action. Requiring $|h|\le2$ gives **$\mathcal N\le8$**. The [four-dimensional N=8 supergravity](../../../supersymmetry.md#four-dimensional-n-8-supergravity) [supergravity multiplet](../../../supersymmetry.md#supergravity-multiplet) attains this bound with highest [helicity](../../../special-relativity.md#helicity) $2$ and multiplicities $1,8,28,56,70,56,28,8,1$. There is one $+2$ state and one $-2$ state, the two polarizations of a single [graviton](../../../quantum-theory.md#graviton).

The stronger restriction relevant to matter is the [chirality constraint on extended supersymmetry](../../../supersymmetry.md#chirality-constraint-on-extended-supersymmetry). An $\mathcal N=1$ [chiral superfield](../../../supersymmetry.md#chiral-superfield) can contain a left-handed [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) in a complex [gauge group representation](../../../relativistic-quantum-field.md#gauge-group-representation) $R$. By contrast, a full $\mathcal N=2$ [hypermultiplet](../../../supersymmetry.md#hypermultiplet) consists of $\mathcal N=1$ matter in $R\oplus\overline R$, and the [gauginos](../../../supersymmetry.md#gaugino) of a [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) are in the real adjoint [group representation](../../../representation-theory.md#group-representation). Higher unbroken [extended supersymmetry](../../../supersymmetry.md#extended-supersymmetry) retains this pairing. A [pseudoreal representation](../../../representation-theory.md#pseudoreal-representation) may allow a half-[hypermultiplet](../../../supersymmetry.md#hypermultiplet), but it does not yield net chirality in a genuinely complex [gauge group representation](../../../relativistic-quantum-field.md#gauge-group-representation). Consequently the [chiral gauge spectrum](../../../relativistic-quantum-field.md#chiral-gauge-spectrum) of the [Standard Model](../../../standard-model.md) permits **at most unbroken $\mathcal N=1$ supersymmetry** in its four-dimensional low-energy matter sector.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

On shell, a massless $\mathcal N=1$ [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) contains a [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) with two transverse polarizations and a [gaugino](../../../supersymmetry.md#gaugino) with two fermionic states. A [chiral superfield](../../../supersymmetry.md#chiral-superfield) contains a [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field), hence two real bosonic states, and a [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) with two fermionic states. Their total is $4$ bosonic and $4$ fermionic states.

Suppose charged [scalar fields](../../../quantum-field-theory.md#scalar-field) acquire [vacuum expectation values](../../../quantum-field-theory.md#vacuum-expectation-value) at a [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum), where [F-flatness](../../../supersymmetry.md#f-flatness) and [D-flatness](../../../supersymmetry.md#d-flatness) hold. For each broken generator of the [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance), the [supersymmetric Higgs mechanism](../../../supersymmetry.md#supersymmetric-higgs-mechanism) combines one massless [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) and one [chiral superfield](../../../supersymmetry.md#chiral-superfield) into a [massive N=1 vector multiplet](../../../supersymmetry.md#massive-n-1-vector-multiplet). The [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) absorbs one real [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson), acquiring its third polarization. The other real [scalar field](../../../quantum-field-theory.md#scalar-field) remains physical. The [gaugino](../../../supersymmetry.md#gaugino) and the relevant [higgsino](../../../supersymmetry.md#higgsino) mix into the four fermionic states. Thus the spin content is

$$
\boxed{(1,\tfrac12,\tfrac12,0),\qquad n_B=3+1=4,quad n_F=2+2=4}.
$$

Unbroken [supersymmetry](../../../supersymmetry.md) gives all these states the same mass through [supersymmetric mass degeneracy](../../../supersymmetry.md#supersymmetric-mass-degeneracy). Remaining massive [chiral superfields](../../../supersymmetry.md#chiral-superfield) instead have spin content $(1/2,0,0)$, with two fermionic and two bosonic states of a common mass. The [auxiliary fields](../../../supersymmetry.md#auxiliary-field) ensure matching off shell but are not additional propagating particles in these counts.

The [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism) occurs when local [supersymmetry](../../../supersymmetry.md) is spontaneously broken in [supergravity](../../../supersymmetry.md#supergravity). Its spin-$3/2$ gauge field, the [gravitino](../../../supersymmetry.md#gravitino), absorbs the spin-$1/2$ [goldstino](../../../supersymmetry.md#goldstino):

$$
\boxed{2\text{ massless gravitino states}+2\text{ goldstino states}
\longrightarrow4\text{ massive gravitino states}}.
$$

The extra states have [helicities](../../../special-relativity.md#helicity) $\pm1/2$, supplementing $\pm3/2$. The ordinary [supersymmetric Higgs mechanism](../../../supersymmetry.md#supersymmetric-higgs-mechanism) can preserve [supersymmetry](../../../supersymmetry.md) while breaking the internal [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance); the [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism) breaks the local [supersymmetry](../../../supersymmetry.md) itself. Spontaneously broken global [supersymmetry](../../../supersymmetry.md) leaves a physical massless [goldstino](../../../supersymmetry.md#goldstino), because there is no dynamical [gravitino](../../../supersymmetry.md#gravitino) to absorb it.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Take a canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) $K=\Phi^\dagger\Phi$ and the [Wess–Zumino model](../../../supersymmetry.md#wess-zumino-model) [superpotential](../../../supersymmetry.md#superpotential)

$$
W(\Phi)=\frac m2\Phi^2+\frac g3\Phi^3.
$$

The [F-term](../../../supersymmetry.md#f-term) component gives

$$
\mathcal L_F=F^*F+F W'(\phi)+F^*\overline{W'(\phi)}
-\frac12 W''(\phi)\psi\psi-\frac12\overline{W''(\phi)}\bar\psi\bar\psi.
$$

Eliminating the [auxiliary field](../../../supersymmetry.md#auxiliary-field) by $F=-\overline{W'(\phi)}$ gives the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) $V=|W'(\phi)|^2$. Consequently

$$
V=|m\phi+g\phi^2|^2
=|m|^2|\phi|^2+m\bar g\phi\bar\phi^2+\bar m g\bar\phi\phi^2
+\boxed{|g|^2|\phi|^4},
\qquad
\mathcal L_{\mathrm{Yukawa}}=-\frac12m\psi\psi-\boxed{g\phi\psi\psi}+\mathrm{h.c.}
$$

This is the [supersymmetric relation between quartic and Yukawa couplings](../../../supersymmetry.md#supersymmetric-relation-between-quartic-and-yukawa-couplings): there is one holomorphic parameter $g$, with the quartic coefficient $|g|^2$ and the [Yukawa coupling](../../../standard-model.md#yukawa-interaction) $g$ in the displayed normalization. For real $g$ the quartic coefficient is the $g^2$ of the question. They cannot be varied independently while retaining this canonical [supersymmetry](../../../supersymmetry.md).

The relation produces the [supersymmetric cancellation of quadratic divergences](../../../supersymmetry.md#supersymmetric-cancellation-of-quadratic-divergences). Bosonic and fermionic [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram) correcting a [scalar mass](../../../quantum-field-theory.md#scalar-mass) have equal ultraviolet quadratic coefficients and opposite signs, so the mass is not driven directly to the ultraviolet cutoff scale. In a theory with [soft supersymmetry breaking](../../../supersymmetry.md#soft-supersymmetry-breaking), residual corrections instead have the schematic size

$$
\delta m_H^2\sim\frac{|g|^2}{16\pi^2}m_{\mathrm{soft}}^2
\log\frac{\Lambda}{m_{\mathrm{soft}}},
$$

with coefficients and logarithms depending on the spectrum. Thus superpartner masses near the electroweak scale can stabilize the [Higgs boson](../../../standard-model.md#higgs-boson) mass against a much larger cutoff, addressing the radiative part of the [hierarchy problem](../../../standard-model.md#hierarchy-problem). Heavy [sparticles](../../../supersymmetry.md#sparticle) leave a corresponding residual sensitivity; the cancellation does not by itself explain every mass scale.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

In the conventions $\{Q_\alpha,Q_\beta^\dagger\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu$, the trace over the two spinor components of the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) gives

$$
\boxed{H=\frac14\sum_{\alpha=1}^2\{Q_\alpha,Q_\alpha^\dagger\}}.
$$

Hence, on a normalized state in the domain of the [supercharges](../../../supersymmetry.md#supersymmetry-generator),

$$
\langle v|H|v\rangle
=\frac14\sum_{\alpha=1}^2\left(\|Q_\alpha v\|^2+\|Q_\alpha^\dagger v\|^2\right)\ge0.
$$

This proves [energy positivity in global supersymmetry](../../../supersymmetry.md#energy-positivity-in-global-supersymmetry). The zero of energy is fixed by the algebra; adding an arbitrary constant to $H$ while keeping that algebra unchanged is not allowed.

For a finite-dimensional [supermultiplet](../../../supersymmetry.md#supermultiplet) at fixed positive energy and [four-momentum](../../../special-relativity.md#four-momentum), choose a nonzero component $q$ with $\{q,q^\dagger\}=cI$, $c>0$, and $q^2=0$. The Hermitian odd operator

$$
A=\frac{q+q^\dagger}{\sqrt c}
\quad\text{satisfies}\quad A^2=I,
\qquad A(-1)^F=-(-1)^F A.
$$

It is therefore an invertible map from the even [fermion parity](../../../topological-quantum-matter.md#fermion-parity) subspace to the odd subspace and conversely. This proves [boson-fermion degeneracy in a supermultiplet](../../../supersymmetry.md#boson-fermion-degeneracy-in-a-supermultiplet), **$n_B=n_F$**, for every positive-energy physical particle [supermultiplet](../../../supersymmetry.md#supermultiplet). Equivalently, the [supertrace](../../../quantum-mechanics.md#supertrace) of the supercharge [anticommutator](../../../vector-space.md#anticommutator) vanishes because odd operators interchange these two subspaces. A zero-energy vacuum is an exception to the literal claim about every possible representation: it can be a one-dimensional bosonic singlet with all [supercharges](../../../supersymmetry.md#supersymmetry-generator) acting trivially.

For a vacuum $|\Omega\rangle$, the sum-of-squares formula gives $E_0=0$ exactly when all [supercharges](../../../supersymmetry.md#supersymmetry-generator) and their adjoints annihilate it. If global [supersymmetry](../../../supersymmetry.md) is spontaneously broken and a vacuum exists, at least one such norm is nonzero, so **the vacuum energy is positive**. In infinite volume this is the statement about the [vacuum energy](../../../perturbative-quantum-field-theory.md#vacuum-energy) density, understood with a finite-volume regulator. Explicit [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) need not preserve the algebra used in the proof. The conclusion also does not extend to the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential), whose negative $-3e^K|W|^2$ term permits, for example, the zero-energy broken vacua of [no-scale supergravity](../../../supersymmetry.md#no-scale-supergravity).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Use [left Grassmann derivatives](../../../linear-algebra.md#left-grassmann-derivative) and place the odd constant transformation parameters on the left. A [scalar superfield transformation](../../../supersymmetry.md#scalar-superfield-transformation) can be written

$$
\delta S=(\epsilon^\alpha Q_\alpha+\bar\epsilon^{\dot\alpha}\bar Q_{\dot\alpha})S,
\qquad
Q_\alpha=\partial_\alpha-i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu,
\qquad
\bar Q_{\dot\alpha}=\bar\partial_{\dot\alpha}-i\theta^\beta\sigma^\mu_{\beta\dot\alpha}\partial_\mu.
$$

Equivalently, pull back the scalar function under the infinitesimal [superspace](../../../supersymmetry.md#superspace) translation

$$
\delta\theta=\epsilon,\qquad\delta\bar\theta=\bar\epsilon,
\qquad\delta x^\mu=i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta.
$$

The term involving $\bar\epsilon$ has the displayed sign because interchanging it with $\theta$ reverses the sign in the [Grassmann algebra](../../../linear-algebra.md#grassmann-algebra). Overall factors of $i$ in the definition of the [supercharges](../../../supersymmetry.md#supersymmetry-generator) can be changed together without changing this coordinate transformation.

For two even scalar [superfields](../../../supersymmetry.md#superfield) $S,T$, the odd generators obey the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule), while the full parameter-weighted variation $\delta$ is even. Thus

$$
\delta(ST)=(\delta S)T+S(\delta T).
$$

This is precisely the transformation of a [product of scalar superfields](../../../supersymmetry.md#product-of-scalar-superfields). The finite version is even clearer: if $S'(z)=S(z')$ and $T'(z)=T(z')$ for the same transformed [superspace](../../../supersymmetry.md#superspace) point, then $(ST)'(z)=S(z')T(z')=(ST)(z')$. No new representation law is required.

The expression $S(x,\theta,\bar\theta)=\phi(x)$ needs a distinction between a configuration and a closed field content. As a function on [superspace](../../../supersymmetry.md#superspace), it is a valid special configuration of an unconstrained [superfield](../../../supersymmetry.md#superfield). But its variation is

$$
\delta S=(i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta)\partial_\mu\phi.
$$

For nonconstant $\phi$, this generates nonzero components depending on [Grassmann variables](../../../linear-algebra.md#grassmann-variable). Therefore **the pure-scalar truncation is not a supersymmetric multiplet**: an isolated spacetime [scalar field](../../../quantum-field-theory.md#scalar-field) with all its partners permanently set to zero is not closed under [supersymmetry](../../../supersymmetry.md). This is the [pure-scalar truncation of a superfield](../../../supersymmetry.md#pure-scalar-truncation-of-a-superfield). A constant gauge-singlet $\phi$ is the trivial invariant exception. Calling $\phi(x)$ a special [superfield](../../../supersymmetry.md#superfield) configuration is consistent; claiming that its restricted field content remains a [superfield](../../../supersymmetry.md#superfield) representation is not.

## 2

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

All derivatives below are [left Grassmann derivatives](../../../linear-algebra.md#left-grassmann-derivative). Decompose the [supersymmetric covariant derivatives](../../../supersymmetry.md#supersymmetric-covariant-derivative) into odd pieces

$$
D_\alpha=\partial_\alpha+A_\alpha,\qquad
\bar D_{\dot\beta}=\bar\partial_{\dot\beta}+B_{\dot\beta},
\qquad
A_\alpha=i\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,
\quad B_{\dot\beta}=i\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu.
$$

When these operators act on an arbitrary [superfield](../../../supersymmetry.md#superfield), the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) gives

$$
\{\partial_\alpha,B_{\dot\beta}\}=i\sigma^\mu_{\alpha\dot\beta}\partial_\mu,
\qquad
\{A_\alpha,\bar\partial_{\dot\beta}\}=i\sigma^\mu_{\alpha\dot\beta}\partial_\mu.
$$

The [anticommutator](../../../vector-space.md#anticommutator) of the two pure Grassmann derivatives vanishes. Also $\{A_\alpha,B_{\dot\beta}\}=0$: the spacetime derivatives commute, while the $\theta$ and $\bar\theta$ coefficients anticommute. Adding these terms proves the [supercovariant derivative algebra with left derivatives](../../../supersymmetry.md#supercovariant-derivative-algebra-with-left-derivatives),

$$
\boxed{\{D_\alpha,\bar D_{\dot\beta}\}=2i\sigma^\mu_{\alpha\dot\beta}\partial_\mu}.
$$

For two unbarred derivatives, neither $\partial_\alpha$ differentiates the $\bar\theta$ coefficient of the other operator. Their coefficient products anticommute, so $\boxed{\{D_\alpha,D_\beta\}=0}$. The same argument with barred and unbarred coordinates exchanged gives $\boxed{\{\bar D_{\dot\alpha},\bar D_{\dot\beta}\}=0}$. These signs follow the derivatives printed in this paper; a convention replacing $\bar D$ by $-\bar D$ reverses the mixed sign as well.

Set $y^\mu=x^\mu+i\theta^\alpha\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}$. Left differentiation gives

$$
\bar\partial_{\dot\alpha}(\theta\sigma^\mu\bar\theta)
=-\theta^\beta\sigma^\mu_{\beta\dot\alpha},
\qquad\bar D_{\dot\alpha}y^\mu=0.
$$

The [chain rule](../../../calculus.md#chain-rule) therefore makes $\bar D_{\dot\alpha}$ simply $\bar\partial_{\dot\alpha}$ at fixed $y,\theta$. The [chiral superfield](../../../supersymmetry.md#chiral-superfield) constraint $\bar D_{\dot\alpha}\Phi=0$ means that $\Phi$ is independent of $\bar\theta$ in these coordinates. Since there are only two independent entries of $\theta$, its [Grassmann algebra](../../../linear-algebra.md#grassmann-algebra) expansion terminates at degree two. Naming the coefficients gives the [chiral-superfield component expansion](../../../supersymmetry.md#chiral-superfield-component-expansion)

$$
\boxed{\Phi(y,\theta)=\phi(y)+\sqrt2\theta\psi(y)+\theta\theta F(y)}.
$$

Here $\phi$ is a [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field), $\psi$ a [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor), and $F$ a nonpropagating [auxiliary field](../../../supersymmetry.md#auxiliary-field); the $\sqrt2$ is their conventional normalization.

## 3

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The renormalizable action for [chiral superfields](../../../supersymmetry.md#chiral-superfield) $\Phi_i$ and [vector superfields](../../../supersymmetry.md#vector-superfield) $V$ has the [superspace integration](../../../supersymmetry.md#superspace-integration) form

$$
S=\int d^4x\,d^4\theta\,K(\Phi^\dagger e^{2V},\Phi)
+\left[\int d^4x\,d^2\theta\left(W(\Phi)+\frac14 f_{ab}\mathcal W^{a\alpha}\mathcal W^b_\alpha\right)+\mathrm{h.c.}\right],
$$

where $K$ is a real [Kähler potential](../../../supersymmetry.md#kahler-potential), $\mathcal W_\alpha$ is the [chiral field-strength superfield](../../../supersymmetry.md#chiral-field-strength-superfield), and $W$ is a gauge-invariant [holomorphic function](../../../complex-analysis.md#holomorphic-function). For the renormalizable theory choose canonical positive kinetic terms, a polynomial $W$ of degree at most three, and field-independent gauge kinetic coefficients $f_{ab}$. We prove the [non-renormalization theorem](../../../supersymmetry.md#non-renormalization-theorem) for the local [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action), with a nonzero infrared cutoff and a regulator preserving [supersymmetry](../../../supersymmetry.md). The elementary [chiral superfields](../../../supersymmetry.md#chiral-superfield) are retained; this is not a claim that eliminating whole massive fields leaves the same polynomial.

Write $W=\sum_A\lambda_A\mathcal O_A(\Phi)$, treating masses and interaction coefficients alike as background chiral [spurions](../../../supersymmetry.md#spurion). A local [F-term](../../../supersymmetry.md#f-term) is chiral even when these backgrounds vary, so its coefficient depends holomorphically on $\Phi,\lambda_A$ and the holomorphic gauge couplings. Dependence on $\bar\lambda_A$ would not be chiral. Such dependence can enter [D-terms](../../../supersymmetry.md#d-term) or terms with supercovariant derivatives instead. With the infrared cutoff kept fixed, the perturbative local coefficients are regular power series around vanishing masses and interactions. This removes the inverse-mass and infrared singular terms that would spoil the following [spurion selection rule for perturbative non-renormalization](../../../supersymmetry.md#spurion-selection-rule-for-perturbative-non-renormalization).

Assign every elementary $\Phi_i$ [R-charge](../../../supersymmetry.md#r-charge) zero, every $\lambda_A$ [R-charge](../../../supersymmetry.md#r-charge) two, and $\theta$ [R-charge](../../../supersymmetry.md#r-charge) one. The [superpotential](../../../supersymmetry.md#superpotential) must have [R-charge](../../../supersymmetry.md#r-charge) two because $d^2\theta$ has [R-charge](../../../supersymmetry.md#r-charge) minus two. Holomorphy excludes the conjugate [spurions](../../../supersymmetry.md#spurion), so regularity and this formal [R-symmetry](../../../supersymmetry.md#r-symmetry) require exactly one factor of a superpotential [spurion](../../../supersymmetry.md#spurion) in any perturbative candidate. Thus $W_{\mathrm{eff}}$ is linear in the $\lambda_A$, with the ordinary flavor [spurion](../../../supersymmetry.md#spurion) charges fixing the permitted field monomials. An anomalous formal [R-symmetry](../../../supersymmetry.md#r-symmetry) is implemented by also transforming the holomorphic gauge coupling; its anomaly must not simply be ignored.

Gauge interactions cannot provide a perturbative coefficient modifying this conclusion. With $\tau=\vartheta/(2\pi)+4\pi i/g^2$, perturbative diagrams are independent of the topological angle $\vartheta$. A holomorphic coefficient invariant under continuous real shifts of $\tau$ is constant, by the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations). This is [perturbative gauge-coupling independence of the Wilsonian superpotential](../../../supersymmetry.md#perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential). Contributions involving $e^{2\pi i\tau}$ are nonperturbative and are outside this argument. For an Abelian factor the same angle-independent holomorphy argument applies. Hence a putative perturbative coefficient linear in $\lambda_A$ is independent of the gauge coupling and can be evaluated as that coupling tends to zero.

In this free-gauge limit, an interacting chiral loop needs additional superpotential vertices: the free chiral propagator connects $\Phi$ to $\Phi^\dagger$, so a single holomorphic vertex alone cannot produce a loop correcting its local [F-term](../../../supersymmetry.md#f-term). Extra vertices introduce extra [spurions](../../../supersymmetry.md#spurion) or their conjugates, both excluded by the preceding charge and holomorphy argument. The surviving coefficient is its tree value. Therefore

$$
\boxed{W_{\mathrm{Wilsonian}}^{\mathrm{pert}}(\Phi)=W_{\mathrm{tree}}(\Phi)}.
$$

For an explicit charge check, take $W=m\Phi^2/2+g\Phi^3/3$ in the [Wess–Zumino model](../../../supersymmetry.md#wess-zumino-model). Give $(\Phi,m,g)$ ordinary charges $(1,-2,-3)$ and [R-charges](../../../supersymmetry.md#r-charge) $(1,0,-1)$. A holomorphic monomial $m^a g^b\Phi^n$ of the required charges satisfies $n-2a-3b=0$ and $n-b=2$, giving $a=1-b$, $n=b+2$. Perturbative regularity requires $a,b\ge0$, hence only $(a,b,n)=(1,0,2)$ and $(0,1,3)$ survive. The free limit fixes their coefficients to $1/2$ and $1/3$; there is no room for a coupling-dependent loop correction. This illustrates the [holomorphy argument for superpotential non-renormalization](../../../supersymmetry.md#holomorphy-argument-for-superpotential-non-renormalization) explicitly.

The [Kähler potential](../../../supersymmetry.md#kahler-potential) can acquire [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization). Restoring [canonical field normalization](../../../perturbative-quantum-field-theory.md#canonical-field-normalization) changes physical masses and [Yukawa couplings](../../../standard-model.md#yukawa-interaction), so their running does not contradict the boxed statement about holomorphic coordinates. Gauge kinetic [F-terms](../../../supersymmetry.md#f-term) have their own renormalization and are not the [superpotential](../../../supersymmetry.md#superpotential). Infrared effects in the one-particle-irreducible [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action), tree-level elimination of retained fields, and genuine nonperturbative effects must likewise be distinguished from this perturbative [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) theorem.

## 4

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

First assume global [four-dimensional N=1 supersymmetry](../../../supersymmetry.md#four-dimensional-n-1-supersymmetry), canonical positive [Kähler potential](../../../supersymmetry.md#kahler-potential), and tree level. Write $W_i=\partial_i W$ and $m_{ij}=W_{ij}$ at the stationary vacuum. The [chiral-superfield fermion mass matrix](../../../supersymmetry.md#chiral-superfield-fermion-mass-matrix) is the symmetric matrix $m$, and the sum of squared [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) masses is $\operatorname{tr}(m^\dagger m)$. From the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) $V=\sum_k|W_k|^2$, its mixed and holomorphic [Hessian matrix](../../../calculus.md#hessian-matrix) blocks are

$$
V_{i\bar j}=\sum_kW_{ki}\overline{W_{kj}},
\qquad V_{ij}=\sum_k\overline{W_k}W_{kij}.
$$

For canonically normalized real and imaginary parts of the [scalar fields](../../../quantum-field-theory.md#scalar-field), the real [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix) has trace twice the mixed trace. Its holomorphic blocks can split the two real scalar masses but do not change their sum. Hence

$$
\sum_{a=1}^{2n}m_{B,a}^2=2\operatorname{tr}(m^\dagger m),
\qquad 2\sum_{r=1}^{n}m_{F,r}^2=2\operatorname{tr}(m^\dagger m).
$$

A [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) has two spin states, so this proves the [tree-level supertrace mass sum rule](../../../supersymmetry.md#tree-level-supertrace-mass-sum-rule),

$$
\boxed{\operatorname{STr}M^2=\sum_am_{B,a}^2-2\sum_rm_{F,r}^2=0}.
$$

The paper defines its supertrace with $(-1)^{2j+1}$, the negative of the conventional boson-minus-fermion [supertrace](../../../quantum-mechanics.md#supertrace) used here. The asserted zero is the same in either convention. The result requires the stated canonical tree-level hypotheses; a noncanonical [Kähler metric](../../../complex-geometry.md#kahler-metric), [supergravity](../../../supersymmetry.md#supergravity), or radiative corrections can change the sum rule.

If vector multiplets are also present, the [gauge contributions to the F-term supertrace](../../../supersymmetry.md#gauge-contributions-to-the-f-term-supertrace) cancel rather than being omitted. At $D_a=0$, define $C=\sum_a g_a^2\|T_av\|^2$ for the scalar expectation vector $v$. Differentiating $\tfrac12\sum_aD_a^2$ adds $2C$ to the real-scalar trace. The symmetric [gaugino](../../../supersymmetry.md#gaugino)-matter mass matrix has off-diagonal entries $\sqrt2g_aT_av$, giving an extra $4C$ in its fermion squared-mass trace. The covariant scalar [kinetic term](../../../quantum-field-theory.md#kinetic-term) gives vector squared-mass trace $2C$. Thus their contribution is $2C-2(4C)+3(2C)=0$. The gauge-theory result uses all spin states, including the vector weight three; it is not obtained by dropping massive gauge partners.

The [MSSM tree-level sfermion mass constraint](../../../supersymmetry.md#mssm-tree-level-sfermion-mass-constraint) explains the phenomenological difficulty with direct visible-sector breaking. If [F-term](../../../supersymmetry.md#f-term) breaking is neutral under an unbroken electric and color [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance), and no [D-term](../../../supersymmetry.md#d-term) shifts are present, the same trace argument applies within each conserved-charge fermion block. Its corresponding scalar partners cannot all have squared masses above the mean of the light fermion squared masses. Thus canonical tree-level visible-sector [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) alone cannot make every [squark](../../../supersymmetry.md#squark) and other scalar partner heavy while leaving the observed fermions light. The usual effective [soft supersymmetry breaking](../../../supersymmetry.md#soft-supersymmetry-breaking) terms arise after communicating breaking from a separate sector; integrating out that sector, noncanonical interactions and radiative effects evade the hypotheses. The global trace identity alone would not identify a particular light [squark](../../../supersymmetry.md#squark) without the conserved-charge block argument.

For the specified [O'Raifeartaigh model](../../../supersymmetry.md#o-raifeartaigh-model), phases may be chosen so that $\lambda,\mu,M$ are real and positive. Its [superpotential](../../../supersymmetry.md#superpotential) derivatives are

$$
W_X=\lambda(z^2-\mu^2),\qquad W_Y=Mz,\qquad W_Z=2\lambda xz+My,
$$

and its [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) is

$$
V=\lambda^2|z^2-\mu^2|^2+M^2|z|^2+|2\lambda xz+My|^2.
$$

For fixed $x,z$, choose $y=-2\lambda xz/M$ to minimize the final square. Since $|z^2-\mu^2|^2\ge(|z|^2-\mu^2)^2$,

$$
V\ge\lambda^2\mu^4+(M^2-2\lambda^2\mu^2)|z|^2+\lambda^2|z|^4.
$$

Thus **$M^2>2\lambda^2\mu^2$** makes $z=y=0$ a global minimum with arbitrary $x$. The hierarchy $M\gg\mu$ ensures this for fixed perturbative $\lambda$, rather than for arbitrarily large $\lambda$. The origin is one member of this classically flat family, with $V_0=\lambda^2\mu^4>0$ and $F_X=\lambda\mu^2$. The complex field $x$ is a [pseudomodulus](../../../supersymmetry.md#pseudomodulus).

At the origin the [chiral-superfield fermion mass matrix](../../../supersymmetry.md#chiral-superfield-fermion-mass-matrix), in the $(\psi_X,\psi_Y,\psi_Z)$ basis, is

$$
m=\begin{pmatrix}0&0&0\\0&0&M\\0&M&0\end{pmatrix}.
$$

Its physical fermion masses are **$0,M,M$**; the two massive [Weyl spinors](../../../relativistic-quantum-field.md#weyl-spinor) form one massive four-component fermion. The massless $\psi_X$ is the [goldstino](../../../supersymmetry.md#goldstino). More generally, stationarity gives $W_{ij}\overline{W_j}=0$, so the nonzero [auxiliary field](../../../supersymmetry.md#auxiliary-field) direction is a null vector of $m$, proving the [goldstino zero mode from vacuum stationarity](../../../supersymmetry.md#goldstino-zero-mode-from-vacuum-stationarity).

Writing $z=(z_R+iz_I)/\sqrt2$ and similarly for $x,y$, the quadratic [scalar potential](../../../quantum-field-theory.md#scalar-potential) is

$$
V^{(2)}=M^2|y|^2+M^2|z|^2-\lambda^2\mu^2(z^2+\bar z^2).
$$

The [mass spectrum of the quadratic-cubic O'Raifeartaigh model](../../../supersymmetry.md#mass-spectrum-of-the-quadratic-cubic-o-raifeartaigh-model) is therefore

$$
\boxed{\begin{array}{c|c}
\text{real scalar}&m^2\\\hline
x_R,x_I&0,0\\
y_R,y_I&M^2,M^2\\
z_R,z_I&M^2-2\lambda^2\mu^2,\ M^2+2\lambda^2\mu^2
\end{array}}.
$$

The scalar squared-mass sum is $4M^2$, while twice the fermion squared-mass sum is also $4M^2$, so **the supertrace is zero**, as required. The two massless real $x$ modes are tree-level [pseudomoduli](../../../supersymmetry.md#pseudomodulus), which can be lifted by a quantum effective potential; their tree-level masslessness is not the exact symmetry protection enjoyed by the [goldstino](../../../supersymmetry.md#goldstino).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
