# Paper 53

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper53.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper53.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

There are two distinct parts of the [hierarchy problem](../../../standard-model.md#hierarchy-problem). The first asks why the scale of [electroweak symmetry breaking](../../../standard-model.md#electroweak-symmetry-breaking) is so much smaller than a fundamental scale such as the [Planck mass](../../../physics.md#planck-mass). The second, the [technical hierarchy problem](../../../standard-model.md#technical-hierarchy-problem), asks why that separation survives quantum corrections once it is chosen. With a fundamental [Higgs boson](../../../standard-model.md#higgs-boson), a mass term $m_H^2H^\dagger H$ is allowed by the ordinary [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance), so heavy thresholds can contribute additive terms of order a heavy mass squared. This is different from the [chiral protection of a fermion mass](../../../standard-model.md#chiral-protection-of-a-fermion-mass) and the [gauge protection of a vector mass](../../../standard-model.md#gauge-protection-of-a-vector-mass).

For example, a cutoff description of the [Standard Model](../../../standard-model.md) gives the schematic one-loop sensitivity

$$
\delta m_H^2\simeq\frac{\Lambda^2}{16\pi^2}\left(6\lambda_H+\frac94g^2+\frac34g'^2-6y_t^2\right).
$$

The regulator-dependent quadratic term is not itself an observable, but a physical heavy particle of mass $M$ coupled to the Higgs likewise produces a matching correction of order coupling squared times $M^2/(16\pi^2)$. Maintaining $|m_H^2|\ll M^2$ then generically requires cancellation between large unrelated terms. This is the [naturalness](../../../standard-model.md#naturalness-physics) concern; changing the regulator does not eliminate the heavy-threshold issue.

Exact [supersymmetry](../../../supersymmetry.md) relates bosonic and fermionic couplings and masses. Their loop contributions have opposite signs, and the relations enforce [supersymmetric cancellation of quadratic divergences](../../../supersymmetry.md#supersymmetric-cancellation-of-quadratic-divergences). [Boson-fermion degeneracy in a supermultiplet](../../../supersymmetry.md#boson-fermion-degeneracy-in-a-supermultiplet) also transfers fermionic mass protection to its scalar partners. It is not sufficient merely to add arbitrary scalars: the supersymmetric coupling relations are what make the cancellation persist. Perturbative [superpotential non-renormalization](../../../supersymmetry.md#non-renormalization-theorem) further protects holomorphic mass parameters, although [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) still makes canonically normalized couplings run.

For a realistic separation between ordinary particles and their partners, [supersymmetry](../../../supersymmetry.md) must be broken. [Soft supersymmetry breaking](../../../supersymmetry.md#soft-supersymmetry-breaking) introduces masses and selected positive-mass-dimension interactions without reinstating the original ultraviolet quadratic divergence. A paired propagator difference behaves at high Euclidean momentum as

$$
\frac1{k^2+m_B^2}-\frac1{k^2+m_F^2}=\frac{m_F^2-m_B^2}{k^4}+O(k^{-6}),
$$

so a residual scalar correction is of the order

$$
\boxed{\delta m_H^2\sim\frac{|y|^2}{16\pi^2}m_{\rm soft}^2\log\frac{\Lambda}{m_{\rm soft}},\qquad\text{rather than order }\Lambda^2.}
$$

This [soft scalar-mass sensitivity](../../../supersymmetry.md#soft-scalar-mass-sensitivity) controls the technical problem if the relevant soft masses and thresholds are not too far above the weak scale. Very heavy partners can still require tuning through finite and logarithmic terms. Supersymmetric cancellations alone therefore do not guarantee a naturally small weak scale for an arbitrary broken spectrum.

The origin of the hierarchy needs further dynamics. In [dynamical supersymmetry breaking](../../../supersymmetry.md#dynamical-supersymmetry-breaking), an asymptotically free [hidden supersymmetry-breaking sector](../../../supersymmetry.md#hidden-supersymmetry-breaking-sector) can generate an exponentially smaller scale by [dimensional transmutation](../../../perturbative-quantum-field-theory.md#dimensional-transmutation),

$$
\Lambda_{
m hid}=M\exp\left[-\frac{8\pi^2}{b_0g^2(M)}\right],\qquad b_0>0.
$$

If that sector actually has no supersymmetric vacuum, its breaking can be communicated to the visible sector to produce small soft terms. The exponential creates a hierarchy without specifying a tiny dimensionless coupling at the high scale, but the existence of breaking and its mediation are additional model-building requirements. In the [MSSM](../../../supersymmetry.md#minimal-supersymmetric-standard-model), running Higgs soft masses can trigger [electroweak symmetry breaking](../../../standard-model.md#electroweak-symmetry-breaking). The [supersymmetric mu problem](../../../supersymmetry.md#supersymmetric-mu-problem) remains: the allowed superpotential mass $\mu H_uH_d$ must also be near the soft scale, and non-renormalization protects a chosen small $\mu$ without explaining its origin.

Extra-dimensional proposals use geometry to explain why observable gravitational and weak scales differ. In [large extra dimensions](../../../physics.md#large-extra-dimensions), assume gravity propagates in $4+n$ dimensions with fundamental scale $M_*$, while ordinary fields are localized on a [brane](../../../string-theory.md#brane). Integrating the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) over compact volume $V_n$ gives the [Planck mass from compactification volume](../../../physics.md#planck-mass-from-compactification-volume) relation

$$
\boxed{M_{\rm Pl}^2=M_*^{n+2}V_n.}
$$

Here $M_{\rm Pl}$ denotes the four-dimensional [reduced Planck mass](../../../physics.md#reduced-planck-mass). A sufficiently large internal volume lets $M_*$ be near the weak scale even though $M_{\rm Pl}$ is enormous. The Higgs need then be stable only up to the lower fundamental cutoff. This explains the weakness of long-distance gravity geometrically but trades the scale question for the origin and stabilization of a large compact volume. Ordinary matter is localized to avoid an unwanted low-mass tower of its own [Kaluza-Klein modes](../../../physics.md#kaluza-klein-mode); gravitational modes, departures from four-dimensional gravity and bulk energy loss impose phenomenological requirements.

The [Randall–Sundrum model](../../../physics.md#randall-sundrum-model) instead uses a warped five-dimensional interval, conventionally the doubled $S^1/\mathbb Z_2$ orbifold with fixed branes at $0$ and $L$:

$$
ds^2=e^{-2k|y|}\eta_{\mu\nu}dx^\mu dx^\nu+dy^2,\qquad M_{\rm Pl}^2=\frac{M_5^3}{k}(1-e^{-2kL}).
$$

For a scalar confined to the distant brane, the kinetic and mass terms carry factors $e^{-2kL}$ and $e^{-4kL}$. Canonical rescaling therefore produces

$$
\boxed{m_{\rm IR}=e^{-kL}m_0.}
$$

A moderately large $kL$ yields an exponentially small observable mass without a comparably large compact-volume factor. The inter-brane size is the [radion](../../../physics.md#radion), so one still needs a mechanism fixing its expectation value. Consistent curvature, brane tensions and ultraviolet physics are also part of the model. Warping is a redshift mechanism; it does not provide the same cancellation of arbitrary scalar loops as supersymmetry.

Finally, protecting a Higgs mass is not the same as solving the vacuum-energy hierarchy. Exact global [supersymmetry](../../../supersymmetry.md) has zero-energy supersymmetric vacua, but broken supersymmetry generically leaves vacuum energy set by its breaking dynamics. In [supergravity](../../../supersymmetry.md#supergravity), positive auxiliary-field contributions coexist with a negative superpotential term, and obtaining a very small cosmological constant requires further structure or cancellation. Neither soft supersymmetry nor the two geometric mechanisms automatically resolves that problem. The mechanisms can also coexist in one higher-dimensional supersymmetric theory.

**Supersymmetry protects a chosen hierarchy radiatively and can accompany dynamics generating a small scale; extra-dimensional volume or warping generates the scale separation geometrically, with stabilization still required.**

## 2

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Work with a supersymmetry-preserving regulator and a local [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) at a nonzero infrared cutoff, in holomorphic field variables. Its two-derivative terms have the form

$$
\int d^4\theta\,K(\Phi,\Phi^\dagger,V)+\left[\int d^2\theta\left\{W(\Phi)+\frac14f_{ab}(\Phi)\mathcal W^{a\alpha}\mathcal W^b_\alpha\right\}+\mathrm{h.c.}\right].
$$

Here $\mathcal W_\alpha$ is the gauge field-strength superfield, distinct from the [superpotential](../../../supersymmetry.md#superpotential) $W$, and the [gauge kinetic function](../../../supersymmetry.md#gauge-kinetic-function) $f_{ab}$ is symmetric and holomorphic. The perturbative [non-renormalization theorem](../../../supersymmetry.md#non-renormalization-theorem) states

$$
\boxed{W_{\rm Wilsonian}^{\rm pert}=W_{\rm tree},\qquad f_{\rm Wilsonian}^{\rm pert}=f_{\rm tree}+f_{\rm one\ loop}.}
$$

The same elementary light fields are retained in the first equality. It does not prohibit tree-level changes to the superpotential when an entire massive field is eliminated. The [Kähler potential](../../../supersymmetry.md#kahler-potential) may be renormalized at every loop order, nonperturbative effects are separate, and canonically normalized physical couplings need not satisfy these holomorphic statements.

First prove [superpotential non-renormalization](../../../supersymmetry.md#non-renormalization-theorem). Promote every coupling in $W_{\rm tree}=\sum_A\lambda_A\mathcal O_A(\Phi)$ to a background [chiral superfield](../../../supersymmetry.md#chiral-superfield), or [spurion](../../../supersymmetry.md#spurion). A local [F-term](../../../supersymmetry.md#f-term) must remain chiral for arbitrary backgrounds, so its coefficient is holomorphic in $\Phi$ and the $\lambda_A$, not in their complex conjugates. Give the matter superfields formal [R-charge](../../../supersymmetry.md#r-charge) zero, $\theta$ charge one, and every $\lambda_A$ charge two. The superpotential then has charge two. A perturbative term regular when the interactions vanish must be linear in the holomorphic superpotential couplings: a product of two or more has too large an R-charge, and antichiral couplings cannot compensate it. Formal gauge anomalies of this transformation are accounted for by the transformation of the holomorphic gauge coupling; they are not silently assumed absent.

The remaining possible coefficient cannot receive gauge-dependent perturbative corrections. The [holomorphic gauge coupling](../../../supersymmetry.md#holomorphic-gauge-coupling) may be written $S=g_h^{-2}-i\vartheta/(8\pi^2)$. Perturbation theory is insensitive to the topological angle, so any ordinary superpotential coefficient is invariant under $S\mapsto S+ic$, with real $c$. A holomorphic function with this continuous imaginary-shift invariance is constant in $S$ by the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations). This is [perturbative gauge-coupling independence of the Wilsonian superpotential](../../../supersymmetry.md#perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential).

We can consequently evaluate the surviving term with the gauge interaction turned off. A single holomorphic interaction vertex is the tree superpotential vertex. It cannot make a loop using free $\Phi$-$\Phi^\dagger$ propagators without additional vertices and antichiral couplings. Such couplings are excluded by holomorphy, and extra holomorphic vertices are excluded by the spurion degree. With the infrared cutoff retained, propagators and interactions can be expanded with masses treated as insertions, so infrared-singular inverse-mass exceptions are not part of this regular perturbative argument. The coefficient must therefore equal its tree value. This proves the [spurion selection rule for perturbative non-renormalization](../../../supersymmetry.md#spurion-selection-rule-for-perturbative-non-renormalization) for arbitrary superpotential monomials.

Now prove [one-loop exactness of the holomorphic gauge kinetic function](../../../supersymmetry.md#one-loop-exactness-of-the-holomorphic-gauge-kinetic-function). Add an independent constant background coupling $S$ to the gauge kinetic function. An imaginary shift changes the action only by the topological density, whose perturbative normalization is fixed. Thus the holomorphic perturbative coefficient transforms as

$$
f_{\rm pert}(S+ic)=f_{\rm pert}(S)+ic.
$$

Differentiating with respect to $c$ gives $\partial_Sf_{\rm pert}=1$. Therefore the correction $f_{\rm pert}-S$ is independent of $S$; nonlinear inverse powers of $\operatorname{Re}S$ cannot be holomorphic shift-invariant corrections. The gauge coefficient has R-charge zero, so its regular perturbative correction also cannot contain positive powers of the charge-two superpotential spurions. The anomalous shift of $S$ accounts for the allowed one-loop anomaly; it does not permit arbitrary higher-loop spurion dependence.

To connect this constraint to loop order, use gauge fields whose bare kinetic term has coefficient $1/g_h^2$. After factoring this tree normalization, an $L$-loop gauge-kinetic correction scales as $g_h^{2L-2}$. Equivalently, a gauge propagator contributes $S^{-1}$ and a pure-gauge vertex contributes $S$; with no superpotential interactions, closed matter lines give equal numbers of matter propagators and matter vertices. The connected graph identity $L=I-V+1$ then gives $S^{1-L}$ for the gauge coefficient. Tree order is linear in $S$, one loop is independent of $S$, and every higher loop has forbidden inverse-coupling dependence. Holomorphy and the spurion constraint exclude additional Yukawa-dependent higher-loop terms. Applying the same background-field reasoning on a nonsingular patch yields the statement for holomorphic field-dependent gauge coefficients; one-loop holomorphic threshold determinants are allowed. Thus the only perturbative correction to $f$ is the one-loop correction.

For one simple gauge factor with $\operatorname{tr}_R(T_aT_b)=T(R)\delta_{ab}$, the [one-loop beta function of a supersymmetric gauge theory](../../../supersymmetry.md#one-loop-beta-function-of-a-supersymmetric-gauge-theory) has $b_0=3C_2(G)-\sum_iT(R_i)$. The vector and adjoint Weyl contributions give $(11/3-2/3)C_2(G)=3C_2(G)$, while one matter Weyl fermion and complex scalar contribute $-(2/3+1/3)T(R)=-T(R)$. Consequently, away from thresholds,

$$
\boxed{f(\mu)=f(M)+\frac{b_0}{8\pi^2}\log\frac\mu M,\qquad\mu\frac{df}{d\mu}=\frac{b_0}{8\pi^2}.}
$$

This sign makes the real inverse coupling decrease toward the infrared in an asymptotically free theory.

Finally, [holomorphic and canonically normalized superpotential couplings](../../../supersymmetry.md#holomorphic-and-canonically-normalized-superpotential-couplings) are different. For example, if $K=Z\Phi^\dagger\Phi$, then $\Phi_c=Z^{1/2}\Phi$ changes $m\Phi^2/2+y\Phi^3/3$ to coefficients $m/Z$ and $y/Z^{3/2}$. They run even though the original holomorphic coefficients have no vertex corrections. Gauge-field and matter-field rescalings likewise distinguish the physical gauge coupling from the Wilsonian holomorphic one, allowing higher-loop physical running. Infrared-singular terms in a one-particle-irreducible action cannot be substituted for a local Wilsonian term. Nonperturbative terms such as $e^{-8\pi^2S}$ evade continuous topological-angle shift invariance and may generate superpotentials or gauge-kinetic effects when the symmetries and dynamics permit them. These qualifications are essential to the theorem's statement.

## 3

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Regard the antisymmetric tensor as a real differential-form potential $A_p$. For a free [massless p-form gauge field](../../../relativistic-quantum-field.md#massless-p-form-gauge-field), its field strength is $F_{p+1}=dA_p$ and its gauge transformation is $A_p\mapsto A_p+d\Lambda_{p-1}$. The [Bianchi identity for an Abelian p-form](../../../relativistic-quantum-field.md#bianchi-identity-for-an-abelian-p-form) and the source-free field equation are

$$
dF=0,\qquad d*F=0.
$$

The [Hodge star](../../../differential-form.md#hodge-star-operator) makes $*F$ a closed $(D-p-1)$-form. On a contractible patch, the [Poincaré lemma](../../../differential-form.md#poincare-lemma) gives $*F=dB_q$, hence

$$
\boxed{q_{\rm massless}=D-p-2,\qquad dB=*dA.}
$$

Conversely, the original Bianchi identity becomes the dual field equation $d*dB=0$, up to the harmless signature sign in $**$. The original equation becomes the dual Bianchi identity. This establishes [massless p-form duality](../../../relativistic-quantum-field.md#massless-p-form-duality) between gauge-equivalence classes of local solutions. It requires $0\le p\le D-2$ for an ordinary dual potential; global flux sectors and sources require extra data.

For a [massive p-form field](../../../relativistic-quantum-field.md#massive-p-form-field) of mass $m>0$, let $\delta$ denote the formal [codifferential](../../../differential-form.md#codifferential) and take its free equation to be

$$
\delta F+m^2A=0,\qquad F=dA.
$$

Applying $\delta$ yields $\delta A=0$, since $\delta^2=0$. Define

$$
B_q=\frac1m*F,\qquad\boxed{q_{\rm massive}=D-p-1.}
$$

Here the dual field is the Hodge dual of the field strength itself, rather than a potential for it. For definiteness, use one timelike direction and $**\omega_r=(-1)^{r(D-r)+1}\omega_r$. With $\delta\omega_r=(-1)^{D(r+1)}*d*\omega_r$, write $\eta=(-1)^{D(p+2)}$. The massive equation implies

$$
*dB=-\eta mA,\qquad A=-\frac\eta m*dB.
$$

This gives an invertible differential map at nonzero mass. Also $\delta B=0$ follows from $dF=0$, and substitution yields $\delta dB+m^2B=0$. Indeed the two codifferential signs multiply to $(-1)^{D(p+q+4)}=(-1)^{D(D+3)}=1$. Thus [massive p-form duality](../../../relativistic-quantum-field.md#massive-p-form-duality) exchanges the equations of two massive tensors of the displayed ranks.

The polarization counts confirm the distinction: a massive tensor in its rest frame has $\binom{D-1}{p}$ states, equal to $\binom{D-1}{D-p-1}$, whereas a massless gauge field has $\binom{D-2}{p}$, equal to $\binom{D-2}{D-p-2}$. The ordinary massive dual applies for $0\le p\le D-1$. A massless $(D-1)$-form has no local wave but may carry a constant top-form flux; its formal negative dual rank is a warning that it is not described by an ordinary dual potential. A degree-$D$ potential likewise has no local propagating field strength. These nondynamical endpoint cases do not change the duality of propagating fields.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a null momentum, use [light cone gauge](../../../relativistic-quantum-field.md#light-cone-gauge) to remove potential components along one null direction; the free field equations remove the remaining longitudinal components. The physical polarizations of a [massless p-form gauge field](../../../relativistic-quantum-field.md#massless-p-form-gauge-field) are therefore antisymmetric tensors on the $D-2$ transverse directions, transforming under the rotational [little group](../../../special-relativity.md#little-group) $SO(D-2)$. Choosing $p$ distinct transverse indices gives

$$
\boxed{n_p(D)=\binom{D-2}{p}.}
$$

This already takes account of the reducibility of the higher-form gauge parameter; naïvely subtracting just one gauge-parameter component count would not give the right answer. No self-duality constraint is being imposed.

For [dimensional reduction](../../../physics.md#dimensional-reduction) to four dimensions, retain the zero modes on a flat $(D-4)$-torus, without fluxes or projections. Write $d=D-4$ and split tensor indices into spacetime indices $\mu$ and internal indices $i$. A component with $r$ spacetime indices is a four-dimensional $r$-form, with $p-r$ internal indices and hence multiplicity $\binom d{p-r}$. The complete field decomposition is

$$
A_p\longrightarrow\bigoplus_{r=0}^{\min(p,4)}\binom d{p-r}\ A_r^{(4)}.
$$

Use the convention that a binomial coefficient vanishes when its lower entry lies outside its range. In four dimensions the scalar, vector and two-form have respectively $1,2,1$ local polarizations, while the three- and four-form potentials have none. Hence [toroidal reduction of a p-form gauge field](../../../physics.md#toroidal-reduction-of-a-p-form-gauge-field) gives

$$
\begin{aligned}
n_{\rm reduced}&=\binom dp+2\binom d{p-1}+\binom d{p-2}\\
&=\sum_r\binom2r\binom d{p-r}=\binom{d+2}p=\binom{D-2}p.
\end{aligned}
$$

The middle identity follows by comparing the coefficient of $t^p$ in $(1+t)^2(1+t)^d=(1+t)^{d+2}$. Therefore

$$
\boxed{n_{\rm reduced}=n_p(D).}
$$

A four-dimensional two-form may instead be counted as one scalar by [two-form scalar duality](../../../relativistic-quantum-field.md#two-form-scalar-duality), with the same result. Higher-form zero modes can describe nondynamical flux data, which are distinct from these propagating degrees of freedom. Nonzero [Kaluza-Klein modes](../../../physics.md#kaluza-klein-mode) form massive lower-dimensional multiplets with longitudinal components supplied by the associated gauge fields; the displayed matching concerns the massless zero-mode sector.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A massless [graviton](../../../quantum-theory.md#graviton) in $D$ dimensions has a symmetric traceless transverse polarization tensor. Its state count is

$$
\frac{(D-2)(D-1)}2-1=\frac{D(D-3)}2.
$$

Thus the metric of [eleven-dimensional supergravity](../../../supersymmetry.md#eleven-dimensional-supergravity) has $44$ polarizations, while its three-form has $\binom93=84$. The total bosonic count is $128$.

For circle reduction to ten dimensions, split $M=(\mu,10)$. The metric supplies $g_{\mu\nu}$, a [Kaluza-Klein](../../../physics.md#kaluza-klein-theory) vector from $G_{\mu,10}$, and a scalar from $G_{10,10}$, conventionally the [dilaton](../../../string-theory.md#dilaton). The three-form supplies $C_{\mu\nu\rho}=A_{\mu\nu\rho}$ and $B_{\mu\nu}=A_{\mu\nu,10}$. Their ten-dimensional counts are

$$
\begin{array}{c|c|c}
\text{eleven-dimensional field}&\text{ten-dimensional fields}&\text{polarizations}\\\hline
G_{MN}&g_{\mu\nu},\ C_\mu,\ \phi&35+8+1=44\\
A_{MNP}&C_{\mu\nu\rho},\ B_{\mu\nu}&\binom83+\binom82=56+28=84.
\end{array}
$$

This is the bosonic content of [type IIA supergravity](../../../supersymmetry.md#type-iia-supergravity): $g$, $B_2$ and the dilaton together with $C_1$ and $C_3$. Consequently

$$
\boxed{128=35+8+1+56+28.}
$$

For flat seven-torus reduction directly to four dimensions, split $M=(\mu,i)$, $i=1,\ldots,7$. The metric yields one four-dimensional metric, seven vectors $G_{\mu i}$ and $7\cdot8/2=28$ scalars $G_{ij}$. Their polarizations are $2+7\cdot2+28=44$. The three-form gives

$$
\begin{array}{c|c|c}
\text{component}&\text{multiplicity and rank}&\text{polarizations}\\\hline
A_{\mu\nu\rho}&1\text{ three-form}&0\\
A_{\mu\nu i}&7\text{ two-forms}&7\\
A_{\mu ij}&\binom72=21\text{ vectors}&42\\
A_{ijk}&\binom73=35\text{ scalars}&35.
\end{array}
$$

The three-form count is $0+7+42+35=84$, as required by [toroidal reduction of a p-form gauge field](../../../physics.md#toroidal-reduction-of-a-p-form-gauge-field). Applying [two-form scalar duality](../../../relativistic-quantum-field.md#two-form-scalar-duality) to the seven two-forms, the propagating four-dimensional spectrum is

$$
\boxed{1\text{ graviton},\quad28\text{ vectors},\quad70\text{ real scalars};\qquad2+28\cdot2+70=128.}
$$

This is the bosonic content of [four-dimensional N=8 supergravity](../../../supersymmetry.md#four-dimensional-n-8-supergravity). The remaining four-dimensional three-form has no local polarization and can be omitted from the propagating spectrum, though a flux choice can matter in other backgrounds. The [toroidal reduction of eleven-dimensional supergravity](../../../supersymmetry.md#toroidal-reduction-of-eleven-dimensional-supergravity) here retains all zero modes; fixing moduli, introducing fluxes or using an orbifold projection would change the spectrum and would not be this unprojected counting problem.

## 4

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use four-dimensional Minkowski signature $(+---)$, $\sigma^\mu=(I,\sigma^i)$ and $\bar Q_{\dot\alpha}=(Q_\alpha)^\dagger$. The odd [supercharges](../../../supersymmetry.md#supersymmetry-generator) transform as a [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) and its conjugate. In the ordinary particle [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra), [Lorentz covariance](../../../special-relativity.md#lorentz-covariance) makes the mixed anticommutator a vector, since $(1/2,0)\otimes(0,1/2)=(1/2,1/2)$. The even vector generator is the translation generator $P_\mu$, so the anticommutator is a real normalization constant times $\sigma^\mu P_\mu$. Unitarity makes that constant positive, and rescaling the charges sets it to two.

The same-chirality anticommutator is symmetric in its two spinor indices. A Lorentz-scalar term would require $\epsilon_{\alpha\beta}$ and hence an antisymmetric internal charge label, unavailable for $\mathcal N=1$. A term in the Lorentz generators would violate the translation Jacobi identity. Excluding additional tensorial brane charges, as in the ordinary particle algebra, the same-chirality anticommutators therefore vanish. Lorentz covariance could initially allow $[P_\mu,Q_\alpha]=a\sigma_{\mu\alpha\dot\gamma}\bar Q^{\dot\gamma}$. The [graded Jacobi identity](../../../lie-algebra.md#graded-jacobi-identity) with $P_\mu,Q_\alpha,Q_\beta$, using their zero same-chirality anticommutator, then forces $a=0$. Thus the part of the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) involving the odd generators is

$$
\boxed{\begin{gathered}
\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu,\qquad\{Q_\alpha,Q_\beta\}=\{\bar Q_{\dot\alpha},\bar Q_{\dot\beta}\}=0,\\
[P_\mu,Q_\alpha]=[P_\mu,\bar Q_{\dot\alpha}]=0.
\end{gathered}}
$$

The last identity means that a supercharge preserves momentum and mass.

The remaining odd-generator commutators express their spinor transformation under rotations and boosts. One consistent lower-index component convention is

$$
\begin{aligned}
[J_i,Q_\alpha]&=-\tfrac12(\sigma_i)_\alpha{}^\beta Q_\beta,&[K_i,Q_\alpha]&=\tfrac i2(\sigma_i)_\alpha{}^\beta Q_\beta,\\
[J_i,\bar Q_{\dot\alpha}]&=\tfrac12(\sigma_i^*)_{\dot\alpha}{}^{\dot\beta}\bar Q_{\dot\beta},&[K_i,\bar Q_{\dot\alpha}]&=\tfrac i2(\sigma_i^*)_{\dot\alpha}{}^{\dot\beta}\bar Q_{\dot\beta}.
\end{aligned}
$$

The barred formulas follow by Hermitian conjugation. Component coefficient matrices act in the dual representation; the signs therefore must be kept consistent, as in the [Jacobi sign test for supercharge components](../../../supersymmetry.md#jacobi-sign-test-for-supercharge-components).

One can also derive and check the odd brackets directly in [superspace](../../../supersymmetry.md#superspace). With [left Grassmann derivatives](../../../linear-algebra.md#left-grassmann-derivative), take

$$
P_\mu=-i\partial_\mu,\qquad Q_\alpha=\partial_{\theta^\alpha}+i\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,\qquad\bar Q_{\dot\beta}=-\partial_{\bar\theta^{\dot\beta}}-i\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu.
$$

The two cross terms in the mixed anticommutator each give $-i\sigma^\mu\partial_\mu$, totaling $2\sigma^\mu P_\mu$. Equal-chirality terms vanish because the Grassmann derivatives anticommute and their coordinate dependence is of opposite chirality. All coefficients are independent of $x$, so the charges commute with translations. This realizes the displayed algebra rather than merely postulating its brackets.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $\Gamma=(-1)^F$ be [fermion parity](../../../topological-quantum-matter.md#fermion-parity). It acts as $+1$ on [bosons](../../../quantum-mechanics.md#boson) and $-1$ on [fermions](../../../quantum-mechanics.md#fermion), and anticommutes with every odd [supercharge](../../../supersymmetry.md#supersymmetry-generator). In a finite physical [supermultiplet](../../../supersymmetry.md#supermultiplet) at fixed positive energy $E$, trace cyclicity gives

$$
\operatorname{Tr}\bigl[\Gamma\{Q_\alpha,Q_\alpha^\dagger\}\bigr]=0.
$$

Indeed, cycling $Q_\alpha$ in the second term and using $Q_\alpha\Gamma=-\Gamma Q_\alpha$ cancels the first term. Summing diagonal spinor components of the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) gives $\sum_\alpha\{Q_\alpha,Q_\alpha^\dagger\}=4H$, since the Pauli matrices are traceless. Hence [supertrace pairing at positive energy](../../../supersymmetry.md#supertrace-pairing-at-positive-energy) yields

$$
4E\operatorname{Tr}\Gamma=4E(n_B-n_F)=0,\qquad\boxed{n_B=n_F\quad(E>0).}
$$

This is [boson-fermion degeneracy in a supermultiplet](../../../supersymmetry.md#boson-fermion-degeneracy-in-a-supermultiplet). Equivalently, a nonzero charge combination with positive anticommutator gives an invertible parity-changing map between the two sectors. The positive-energy qualification is important: a zero-energy supersymmetric vacuum may be a one-state bosonic representation and need not have a fermionic vacuum partner.

For any normalizable state $|v\rangle$, the same algebra gives [energy positivity in global supersymmetry](../../../supersymmetry.md#energy-positivity-in-global-supersymmetry):

$$
\langle v|H|v\rangle=\frac14\sum_{\alpha=1}^2\left(\|Q_\alpha|v\rangle\|^2+\|Q_\alpha^\dagger|v\rangle\|^2\right)\ge0.
$$

It vanishes exactly when every supercharge and its adjoint annihilates the state. In particular, for an existing translation-invariant vacuum, this proves

$$
\boxed{E_{\rm vac}=0\iff Q_\alpha|0\rangle=\bar Q_{\dot\alpha}|0\rangle=0\ \text{for all components};\qquad\text{spontaneously broken global SUSY}\iff E_{\rm vac}>0.}
$$

In infinite volume, interpret the statement as one about vacuum energy density, using finite-volume normalization first. The energy zero is fixed by the supersymmetry algebra; adding an arbitrary constant to the Hamiltonian while leaving that algebra unchanged is not allowed. For a canonical matter and gauge action, the same positivity is seen from $V=\sum_i|F_i|^2+\tfrac12\sum_aD_a^2$, so a nonzero auxiliary-field expectation breaks the symmetry. This global Minkowski statement does not apply unchanged to the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential), which can have negative-energy supersymmetric vacua.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Choose a positive-energy massless momentum $P^\mu=(E,0,0,E)$. Then $\sigma^\mu P_\mu=E(I-\sigma^3)$, so the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) gives

$$
\{Q_1,Q_1^\dagger\}=0,\qquad\{Q_2,Q_2^\dagger\}=4E.
$$

Unitarity forces $Q_1$ and its adjoint to vanish on this representation: the sum of their squared state norms is zero. Set $a=Q_2/\sqrt{4E}$. The surviving operators obey

$$
\{a,a^\dagger\}=1,\qquad a^2=(a^\dagger)^2=0.
$$

The [helicity](../../../special-relativity.md#helicity) operator is $h=J_3$ for this momentum. In the component convention above, $[h,a]=a/2$ and $[h,a^\dagger]=-a^\dagger/2$. A highest-helicity state $|\lambda\rangle$ with $a|\lambda\rangle=0$ therefore generates exactly two states,

$$
\boxed{\bigl(\lambda,\lambda-\tfrac12\bigr),}
$$

one bosonic and one fermionic. This is the $\mathcal N=1$ [helicity spectrum of a massless supermultiplet](../../../supersymmetry.md#helicity-spectrum-of-a-massless-supermultiplet). The [CPT theorem](../../../quantum-field-theory.md#cpt-theorem) reverses helicity and conjugates internal charges, so [CPT completion of a supermultiplet](../../../supersymmetry.md#cpt-completion-of-a-supermultiplet) adds $(-\lambda,-\lambda+1/2)$ when that pair is not already present.

For the usual integer and half-integer helicities up to spin two, the CPT-complete contents are

$$
\begin{array}{c|c|c}
\text{multiplet}&\text{bosonic helicities}&\text{fermionic helicities}\\\hline
\text{chiral}&0,0&+\tfrac12,-\tfrac12\\
\text{vector}&+1,-1&+\tfrac12,-\tfrac12\\
\text{gravitino}&+1,-1&+\tfrac32,-\tfrac32\\
\text{gravity}&+2,-2&+\tfrac32,-\tfrac32.
\end{array}
$$

The [chiral superfield](../../../supersymmetry.md#chiral-superfield) describes one complex scalar and one Weyl fermion; the [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) has a massless gauge vector and its gaugino. The gravitino multiplet contains a spin-one vector and a spin-three-halves field, while the [supergravity multiplet](../../../supersymmetry.md#supergravity-multiplet) contains the graviton and gravitino. All have two physical bosonic and two physical fermionic helicity states after CPT completion. The general two-state construction also describes higher-helicity formal multiplets; their existence as representations alone does not establish a consistent interacting higher-spin theory.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

In [extended supersymmetry](../../../supersymmetry.md#extended-supersymmetry) there are $\mathcal N$ Weyl-spinor charges $Q_\alpha^A$, $A=1,\ldots,\mathcal N$. A positive Hermitian mixed bracket can be diagonalized and normalized in this internal index. The ordinary four-dimensional particle algebra is

$$
\boxed{\begin{aligned}
\{Q_\alpha^A,\bar Q_{\dot\beta B}\}&=2\delta^A{}_B\sigma^\mu_{\alpha\dot\beta}P_\mu,\\
\{Q_\alpha^A,Q_\beta^B\}&=\epsilon_{\alpha\beta}Z^{AB},\qquad Z^{AB}=-Z^{BA},\\
\{\bar Q_{\dot\alpha A},\bar Q_{\dot\beta B}\}&=\epsilon_{\dot\alpha\dot\beta}(Z^{AB})^*.
\end{aligned}}
$$

All supercharges commute with translations. The new [central charges in supersymmetry](../../../supersymmetry.md#central-charge-in-supersymmetry) are Lorentz scalars commuting with momentum, Lorentz generators and supercharges. Their antisymmetry follows because the full anticommutator is symmetric under interchange of the two paired spinor/internal labels, while $\epsilon_{\alpha\beta}$ is antisymmetric. They can be nonzero only for $\mathcal N>1$. Internal [R-symmetry](../../../supersymmetry.md#r-symmetry) automorphisms rotate the supercharge index; the algebra without specified central charges admits unitary rotations, and a chosen central-charge matrix restricts the subgroup preserving it. Central charges allow [BPS states](../../../supersymmetry.md#bps-state) and shortened massive representations, with the numerical BPS normalization depending on whether a factor two is included in the definition of $Z$.

For a massless unitary representation at the momentum used above, every $Q_1^A$ has zero anticommutator with its adjoint and hence vanishes. Its mixed same-chirality bracket with $Q_2^B$ then forces $Z^{AB}=0$ on that representation. The surviving $\mathcal N$ charges give $\mathcal N$ independent [fermionic creation operators](../../../relativistic-quantum-field.md#fermionic-creation-operator), each lowering helicity by one half. Starting from helicity $\lambda$, their antisymmetric products give

$$
h_k=\lambda-\frac k2,\qquad\text{multiplicity }\binom{\mathcal N}{k},\qquad k=0,\ldots,\mathcal N.
$$

Thus the [helicity spectrum of a massless supermultiplet](../../../supersymmetry.md#helicity-spectrum-of-a-massless-supermultiplet) occupies an interval of width $\mathcal N/2$ and has $2^{\mathcal N}$ states before any separate CPT completion.

The assumption excluding helicity above two also excludes helicity below minus two in a CPT-complete physical spectrum. Therefore both ends of the interval must obey

$$
\lambda\le2,\qquad\lambda-\mathcal N/2\ge-2,
$$

and the [spin bound for massless supermultiplets](../../../supersymmetry.md#spin-bound-for-massless-supermultiplets) gives

$$
\boxed{\mathcal N\le8.}
$$

This bound is attained: for $\mathcal N=8$ and highest helicity two, the helicities are $2,3/2,1,1/2,0,-1/2,-1,-3/2,-2$ with multiplicities $1,8,28,56,70,56,28,8,1$. They form the CPT-self-conjugate multiplet of [four-dimensional N=8 supergravity](../../../supersymmetry.md#four-dimensional-n-8-supergravity), with $128$ bosonic and $128$ fermionic states. Its bosonic graviton, $28$ vectors and $70$ scalars agree with the toroidal reduction counted above. Here $\mathcal N=8$ means eight Weyl-spinor supersymmetries, or $32$ real supercharge components, not eight real components.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
