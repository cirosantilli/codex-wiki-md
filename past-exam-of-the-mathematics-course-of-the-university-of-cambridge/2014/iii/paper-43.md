# Paper 43

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_43.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_43.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [hypercharge](../../../standard-model.md#hypercharge) normalization $Q_{\rm electric}=T^3+Y$. All matter [chiral superfields](../../../supersymmetry.md#chiral-superfield) are written with left-handed [Weyl spinors](../../../relativistic-quantum-field.md#weyl-spinor), so the fields denoted by a superscript $c$ contain the charge conjugates of the usual right-handed [Standard Model fermions](../../../standard-model.md#standard-model-fermion). The [MSSM superfield representations](../../../supersymmetry.md#mssm-superfield-representations) are

$$
\begin{array}{c|c|c}
\text{chiral superfield}&SU(3)_c\times SU(2)_L\times U(1)_Y&\text{multiplicity}\\\hline
Q&(\mathbf3,\mathbf2,1/6)&3\\
U^c&(\overline{\mathbf3},\mathbf1,-2/3)&3\\
D^c&(\overline{\mathbf3},\mathbf1,1/3)&3\\
L&(\mathbf1,\mathbf2,-1/2)&3\\
E^c&(\mathbf1,\mathbf1,1)&3\\
H_u&(\mathbf1,\mathbf2,1/2)&1\\
H_d&(\mathbf1,\mathbf2,-1/2)&1
\end{array}
$$

Each [fermion generation](../../../standard-model.md#fermion-generation) contributes the first five [chiral superfields](../../../supersymmetry.md#chiral-superfield). Their [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field) partners are [squarks](../../../supersymmetry.md#squark) for the [quarks](../../../standard-model.md#quark) and [sleptons](../../../supersymmetry.md#slepton) for the [leptons](../../../standard-model.md#lepton). Each [Higgs chiral doublet](../../../supersymmetry.md#higgs-chiral-doublet) contains a Higgs [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field) and a [higgsino](../../../supersymmetry.md#higgsino). Every [chiral superfield](../../../supersymmetry.md#chiral-superfield) also has a complex [auxiliary field](../../../supersymmetry.md#auxiliary-field). The [vector superfields](../../../supersymmetry.md#vector-superfield) are

$$
\boxed{V_3:(\mathbf8,\mathbf1,0),\qquad V_2:(\mathbf1,\mathbf3,0),\qquad V_1:(\mathbf1,\mathbf1,0).}
$$

They contain the corresponding [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson), [gauginos](../../../supersymmetry.md#gaugino) in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), and real [auxiliary fields](../../../supersymmetry.md#auxiliary-field). A right-handed neutrino [chiral superfield](../../../supersymmetry.md#chiral-superfield) is not part of the minimal field content.

A [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly) is a quantum obstruction to a classical [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance). For [hypercharge](../../../standard-model.md#hypercharge), triangle diagrams with left-handed [Weyl spinors](../../../relativistic-quantum-field.md#weyl-spinor) can violate the Ward identity of the [gauge boson](../../../relativistic-quantum-field.md#gauge-boson); an uncancelled [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly) makes the [gauge theory](../../../quantum-field-theory.md#gauge-theory) inconsistent. [Anomaly cancellation](../../../relativistic-quantum-field.md#anomaly-cancellation) sums over every component, including colour and weak multiplicities. [Complex scalar fields](../../../scalar-field-theory.md#complex-scalar-field) do not contribute to these chiral [gauge anomalies](../../../relativistic-quantum-field.md#gauge-anomaly). For one [fermion generation](../../../standard-model.md#fermion-generation), the cubic [hypercharge](../../../standard-model.md#hypercharge) coefficient is

$$
\begin{aligned}
\mathcal A_{Y^3}
&=6(1/6)^3+3(-2/3)^3+3(1/3)^3+2(-1/2)^3+1^3\\
&=\frac1{36}-\frac89+\frac19-\frac14+1=\boxed{0}.
\end{aligned}
$$

The other coefficients involving a [hypercharge](../../../standard-model.md#hypercharge) [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) vanish too. With the fundamental index $T(\mathbf N)=1/2$,

$$
\begin{aligned}
\mathcal A_{SU(3)^2Y}&=2(1/2)(1/6)+(1/2)(-2/3)+(1/2)(1/3)=0,\\
\mathcal A_{SU(2)^2Y}&=3(1/2)(1/6)+(1/2)(-1/2)=0,\\
\mathcal A_{\mathrm{grav}^2Y}&=6(1/6)+3(-2/3)+3(1/3)+2(-1/2)+1=0.
\end{aligned}
$$

The last line is the [mixed gauge-gravitational anomaly](../../../relativistic-quantum-field.md#mixed-gauge-gravitational-anomaly). Coefficients with one non-Abelian generator and two [hypercharge](../../../standard-model.md#hypercharge) generators vanish by tracelessness. For completeness, the purely colour cubic [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly) cancels between the two fundamental quark components and the two antifundamentals; the weak group has no perturbative cubic [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly). Its four left-handed doublets per [fermion generation](../../../standard-model.md#fermion-generation) also avoid the [Witten SU(2) anomaly](../../../relativistic-quantum-field.md#witten-su-2-anomaly). Thus **each family is separately anomaly-free**, not merely their sum.

The [gauginos](../../../supersymmetry.md#gaugino) do not spoil this result: their [hypercharge](../../../standard-model.md#hypercharge) is zero and their [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is real. One extra [Higgs chiral doublet](../../../supersymmetry.md#higgs-chiral-doublet) is different because its [higgsino](../../../supersymmetry.md#higgsino) is chiral. For $H_u$, its contributions are

$$
\mathcal A_{Y^3}=2(1/2)^3=1/4,\qquad
\mathcal A_{SU(2)^2Y}=(1/2)(1/2)=1/4,\qquad
\mathcal A_{\mathrm{grav}^2Y}=2(1/2)=1.
$$

They have no compensating contribution from the Higgs [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field). The [higgsino](../../../supersymmetry.md#higgsino) in $H_d$ supplies precisely the negative of each coefficient. **Opposite-hypercharge Higgs chiral doublets restore anomaly cancellation.** The same pair restores an even number of weak fermion doublets, so the [Witten SU(2) anomaly](../../../relativistic-quantum-field.md#witten-su-2-anomaly) provides an additional check of the [higgsino anomaly cancellation](../../../supersymmetry.md#higgsino-anomaly-cancellation).

The independent reason is the [holomorphic need for two Higgs chiral doublets](../../../supersymmetry.md#holomorphic-need-for-two-higgs-chiral-doublets). A [superpotential](../../../supersymmetry.md#superpotential) is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) of [chiral superfields](../../../supersymmetry.md#chiral-superfield), so it cannot use a conjugate Higgs [superfield](../../../supersymmetry.md#superfield) to generate the missing [Yukawa couplings](../../../standard-model.md#yukawa-interaction). The ordinary [Standard Model](../../../standard-model.md) can use a Higgs scalar and its conjugate, but the [MSSM](../../../supersymmetry.md#minimal-supersymmetric-standard-model) needs distinct [chiral superfields](../../../supersymmetry.md#chiral-superfield) of both [hypercharges](../../../standard-model.md#hypercharge). For example,

$$
W_{\rm Yukawa}=y_u^{ij}U_i^c Q_j\mathbin{\cdot}H_u-y_d^{ij}D_i^c Q_j\mathbin{\cdot}H_d-y_e^{ij}E_i^c L_j\mathbin{\cdot}H_d,
$$

where the dot contracts weak indices with the antisymmetric tensor. All three terms are gauge-invariant [holomorphic functions](../../../complex-analysis.md#holomorphic-function). **$H_u$ supplies up-type masses, while $H_d$ supplies down-type and charged-lepton masses.** Replacing either by the conjugate of the other would violate the [holomorphic closure of chiral superfields](../../../supersymmetry.md#holomorphic-closure-of-chiral-superfields).

## 2

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use [left Grassmann derivatives](../../../linear-algebra.md#left-grassmann-derivative) and the usual contractions $\partial^2=\partial^\alpha\partial_\alpha$ and $\bar\partial^2=\bar\partial_{\dot\alpha}\bar\partial^{\dot\alpha}$. Set $a=\theta^1,b=\theta^2,c=\bar\theta^{\dot1},d=\bar\theta^{\dot2}$. The printed epsilon convention gives

$$
\theta_1=-b,\quad\theta_2=a,\qquad
\bar\theta_{\dot1}=-d,\quad\bar\theta_{\dot2}=c,
\qquad \theta\theta=-2ab,\quad\bar\theta\bar\theta=2cd.
$$

The reversal of the barred contraction is essential. The [left Grassmann derivative](../../../linear-algebra.md#left-grassmann-derivative) obeys the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule), so $\partial_a(ab)=b$ but $\partial_b(ab)=-a$. With the index-raising convention,

$$
\partial^2=2\partial_b\partial_a,\qquad
\bar\partial^2=2\partial_c\partial_d.
$$

Applying these to the displayed [Grassmann algebra](../../../linear-algebra.md#grassmann-algebra) monomials gives **$A=B=-4$**. Since every antisymmetric two-index product is proportional to epsilon, the $12$ and $\dot1\dot2$ components give

$$
\theta^\alpha\theta^\beta=-\frac12\epsilon^{\alpha\beta}(\theta\theta),\qquad
\bar\theta^{\dot\alpha}\bar\theta^{\dot\beta}=\frac12\epsilon^{\dot\alpha\dot\beta}(\bar\theta\bar\theta).
$$

Thus **$C=-2$ and $D=2$**.

In the remaining contraction, moving the first barred [Grassmann variable](../../../linear-algebra.md#grassmann-variable) past the second unbarred one introduces a minus sign. Inserting the two spinor identities then gives

$$
\begin{aligned}
(\theta\sigma^\mu\bar\theta)(\theta\sigma^\nu\bar\theta)
&=\frac14(\theta\theta)(\bar\theta\bar\theta)\epsilon^{\alpha\beta}\epsilon^{\dot\alpha\dot\beta}
\sigma^\mu_{\alpha\dot\alpha}\sigma^\nu_{\beta\dot\beta}\\
&=\frac14(\theta\theta)(\bar\theta\bar\theta)\operatorname{Tr}(\sigma^\mu\bar\sigma^\nu)\\
&=\frac12(\theta\theta)(\bar\theta\bar\theta)\eta^{\mu\nu}.
\end{aligned}
$$

The trace normalization is the one explicitly supplied in the paper. These [two-component superspace contraction signs](../../../supersymmetry.md#two-component-superspace-contraction-signs) therefore give

$$
\boxed{(A,B,C,D,E)=(-4,-4,-2,2,2).}
$$

As a direct check in the mostly-minus convention, $\sigma^0=I$ gives $(ac+bd)^2=-2abcd$, whereas $(\theta\theta)(\bar\theta\bar\theta)=-4abcd$. Their ratio is $+1/2$. A convention with $\operatorname{Tr}(\sigma^\mu\bar\sigma^\nu)=-2\eta^{\mu\nu}$ would change this last metric-relative sign; it is not the printed trace convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The defining restriction is the reality condition

$$
\boxed{V^\dagger=V.}
$$

For a non-Abelian [gauge group](../../../relativistic-quantum-field.md#gauge-group), write the [vector superfield](../../../supersymmetry.md#vector-superfield) in a Hermitian generator basis with real [superfield](../../../supersymmetry.md#superfield) coefficients. This is a condition on the full [superfield](../../../supersymmetry.md#superfield), not a chirality constraint. It relates conjugate component coefficients and makes the vector and $D$ [auxiliary field](../../../supersymmetry.md#auxiliary-field) real. [Wess-Zumino gauge](../../../supersymmetry.md#wess-zumino-gauge) is a further [supergauge transformation](../../../supersymmetry.md#supergauge-transformation) choice removing redundant components; it is not the defining condition for a [vector superfield](../../../supersymmetry.md#vector-superfield).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Introduce $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$ and retain the same [Grassmann variables](../../../linear-algebra.md#grassmann-variable). The [supersymmetric derivatives in chiral coordinates](../../../supersymmetry.md#supersymmetric-derivatives-in-chiral-coordinates) follow from the [left Grassmann derivative](../../../linear-algebra.md#left-grassmann-derivative) chain rule. Differentiating $y$ gives

$$
\partial_\alpha y^\mu=i(\sigma^\mu\bar\theta)_\alpha,\qquad
\bar\partial_{\dot\alpha}y^\mu=-i(\theta\sigma^\mu)_{\dot\alpha}.
$$

The minus sign in the second relation comes from moving the odd [Grassmann derivative](../../../linear-algebra.md#grassmann-derivative) past $\theta$. Hence, as operators on a [superfield](../../../supersymmetry.md#superfield) expressed in $(y,\theta,\bar\theta)$,

$$
\left.\partial_\alpha\right|_x=\left.\partial_\alpha\right|_y+i(\sigma^\mu\bar\theta)_\alpha\partial_{y^\mu},\qquad
\left.\bar\partial_{\dot\alpha}\right|_x=\left.\bar\partial_{\dot\alpha}\right|_y-i(\theta\sigma^\mu)_{\dot\alpha}\partial_{y^\mu},
\qquad \partial_{x^\mu}=\partial_{y^\mu}.
$$

Substitution into the two [supersymmetric covariant derivatives](../../../supersymmetry.md#supersymmetric-covariant-derivative) adds the two unbarred spacetime terms and cancels the two barred ones:

$$
\boxed{D_\alpha=\left.\partial_\alpha\right|_y+2i(\sigma^\mu\bar\theta)_\alpha\partial_{y^\mu},\qquad
\bar D_{\dot\alpha}=-\left.\bar\partial_{\dot\alpha}\right|_y.}
$$

These operator equalities prove both requested actions on $V$. In particular, a [chiral superfield](../../../supersymmetry.md#chiral-superfield) becomes independent of $\bar\theta$ at fixed $y$. The TeX aid corrupts the second formula by replacing its ordinary barred derivative with a covariant one; the original PDF has the ordinary $-\bar\partial_{\dot\alpha}$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Abelian field-strength chiral projection](../../../supersymmetry.md#abelian-field-strength-chiral-projection) is linear in the [vector superfield](../../../supersymmetry.md#vector-superfield), so isolate the terms containing the [gaugino](../../../supersymmetry.md#gaugino) $\lambda$ and the $D$ [auxiliary field](../../../supersymmetry.md#auxiliary-field). Replacing $x$ by $y-i\theta\sigma\bar\theta$ leaves these terms unchanged: the shift of the [gaugino](../../../supersymmetry.md#gaugino) term would contain three barred [Grassmann variables](../../../linear-algebra.md#grassmann-variable), and the shift of the $D$ term would contain three of each chirality, hence both vanish. Their contribution is therefore

$$
V_{\lambda,D}(y,\theta,\bar\theta)=(\bar\theta\bar\theta)\theta^\beta\lambda_\beta(y)
+\frac12(\theta\theta)(\bar\theta\bar\theta)D(y).
$$

The $2i(\sigma^\mu\bar\theta)_\alpha\partial_\mu$ part of the [supersymmetric covariant derivative](../../../supersymmetry.md#supersymmetric-covariant-derivative) also adds a third barred factor, so it vanishes on these two terms. The ordinary [left Grassmann derivative](../../../linear-algebra.md#left-grassmann-derivative), with $\partial_\alpha(\theta\theta)=2\theta_\alpha$, gives

$$
D_\alpha V_{\lambda,D}=(\bar\theta\bar\theta)\{\lambda_\alpha(y)+\theta_\alpha D(y)\}.
$$

At fixed $y$, $\bar D=-\bar\partial$ and $\bar D^2(\bar\theta\bar\theta)=-4$. Thus the [chiral field-strength superfield](../../../supersymmetry.md#chiral-field-strength-superfield) has

$$
\boxed{W_\alpha(y,\theta)=\lambda_\alpha(y)+\theta_\alpha D(y)+\text{terms containing }V_\mu\text{ or }\bar\lambda.}
$$

The remaining components come from the other independent terms in the [vector superfield](../../../supersymmetry.md#vector-superfield); linearity ensures they cannot alter the two coefficients just calculated. This proves the requested components without computing the omitted terms. The [gaugino](../../../supersymmetry.md#gaugino) phase and the sign of the vector component are those in the printed [Wess-Zumino gauge](../../../supersymmetry.md#wess-zumino-gauge) expansion.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**$W_\alpha$ is a fermionic chiral spinor superfield.** Its chirality follows directly from the [Abelian field-strength chiral projection](../../../supersymmetry.md#abelian-field-strength-chiral-projection):

$$
\bar D_{\dot\beta}W_\alpha=-\frac14\bar D_{\dot\beta}\bar D^2D_\alpha V=0.
$$

There are only two independent barred [supersymmetric covariant derivatives](../../../supersymmetry.md#supersymmetric-covariant-derivative), and their equal-chirality [anticommutators](../../../vector-space.md#anticommutator) vanish. Every product of three barred derivatives therefore vanishes. Equivalently, the previous calculation has no independent barred [Grassmann variable](../../../linear-algebra.md#grassmann-variable) at fixed $y$. The free undotted index makes this a [chiral spinor superfield](../../../supersymmetry.md#chiral-spinor-superfield), rather than a scalar [chiral superfield](../../../supersymmetry.md#chiral-superfield); its lowest component is the odd [gaugino](../../../supersymmetry.md#gaugino) $\lambda_\alpha$.

## 3

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the [Polonyi model](../../../supersymmetry.md#polonyi-model), the [Kähler metric](../../../complex-geometry.md#kahler-metric) is $K_{z\bar z}=1$. The relevant [Kähler covariant derivative of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) is

$$
D_zW=m^2\{1+\bar z(z+\beta)\}.
$$

The [supergravity auxiliary field](../../../supersymmetry.md#supergravity-auxiliary-field) is $F^z=-e^{|z|^2/2}\overline{D_zW}$, up to an irrelevant common phase convention. Thus a constant vacuum preserves [supersymmetry](../../../supersymmetry.md) exactly when this [auxiliary field](../../../supersymmetry.md#auxiliary-field) vanishes. For **$m=0$**, the [superpotential](../../../supersymmetry.md#superpotential) and [scalar potential](../../../quantum-field-theory.md#scalar-potential) vanish identically, and every constant scalar value is a [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum).

For $m\ne0$, put $\langle z\rangle=x+iy$. Its [supersymmetry](../../../supersymmetry.md) condition becomes

$$
1+x^2+y^2+\beta x-i\beta y=0.
$$

Since $\beta>0$, it requires $y=0$ and $x^2+\beta x+1=0$. Hence the [Polonyi supersymmetry branches](../../../supersymmetry.md#polonyi-supersymmetry-branches) are

$$
\boxed{\text{unbroken supersymmetry: }\beta\geq2,\quad
\langle z\rangle=\frac{-\beta\pm\sqrt{\beta^2-4}}2,\quad m\ne0.}
$$

At these points $W\ne0$, so the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) is negative, $V=-3e^K|W|^2$: these are supersymmetric [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime) vacua, not zero-energy ones. The condition $D_zW=0$ also makes them stationary, as follows by differentiating the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential).

For $0<\beta<2$ and $m\ne0$, the [auxiliary field](../../../supersymmetry.md#auxiliary-field) cannot vanish anywhere, so any vacuum has [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking). For $\beta\geq2$, a stationary vacuum at any other scalar value still breaks [supersymmetry](../../../supersymmetry.md); the parameter condition alone does not determine which vacuum is selected. In particular, a nontrivial zero-energy vacuum cannot preserve [supersymmetry](../../../supersymmetry.md): $D_zW=0$ and $V=0$ would also imply $W=0$, whereas $W=0$ gives $z=-\beta$ and $D_zW=m^2\ne0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) gives $e^K=e^{|z|^2}$ and inverse [Kähler metric](../../../complex-geometry.md#kahler-metric) one. Substituting the [superpotential](../../../supersymmetry.md#superpotential) and its [Kähler covariant derivative of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) into the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) yields

$$
\boxed{V(z)=|m|^4e^{|z|^2}\left(\left|1+\bar z(z+\beta)\right|^2-3|z+\beta|^2\right).}
$$

For real $m$, the prefactor is simply $m^4$; the modulus form also covers a complex phase. To keep both scalar directions explicit, write $z=x+iy$ and $P=1+x^2+y^2+\beta x$. Then

$$
V=|m|^4e^{x^2+y^2}H(x,y),\qquad
H=P^2+\beta^2y^2-3\{(x+\beta)^2+y^2\}.
$$

The negative term is essential: unlike the global [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential), the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) need not be nonnegative. This is why cancelling the [cosmological constant](../../../cosmology.md#cosmological-constant) does not force the [auxiliary field](../../../supersymmetry.md#auxiliary-field) to vanish.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Assume $m\ne0$, since the trivial $m=0$ theory cannot fix $\beta$ or the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value). A zero-energy vacuum must satisfy both $V=0$ and stationarity in both real scalar directions. With the notation from the preceding solution, these become $H=H_x=H_y=0$, because the prefactor $|m|^4e^{x^2+y^2}$ is positive. The derivatives are

$$
H_x=2P(2x+\beta)-6(x+\beta),\qquad
H_y=2y(2P+\beta^2-3).
$$

These conditions also show that the zero-energy [stationary point](../../../calculus-of-variations.md#stationary-point) must be real. If $y\ne0$, the second equation gives $P=(3-\beta^2)/2$; the first then gives $x=-(\beta^2+3)/(2\beta)$. Substituting into the definition of $P$ gives $x^2+y^2=2$. But

$$
x^2=\frac{(\beta^2+3)^2}{4\beta^2}\geq3,
$$

which is impossible. Thus $y=0$, without assuming a real vacuum in advance.

Set $t=x+\beta$ and $F=1+xt$. Since $t=0$ would give $H=1$, it cannot occur. The zero-energy equation gives $F=s\sqrt3\,t$, $s\in\{1,-1\}$. Stationarity gives

$$
2F(2x+\beta)-6t=0\quad\Longrightarrow\quad 2x+\beta=s\sqrt3.
$$

Combining these equations gives $1=(s\sqrt3-x)t=t^2$. Writing $t=\varepsilon\in\{1,-1\}$ produces

$$
x=s\sqrt3-\varepsilon,\qquad \beta=2\varepsilon-s\sqrt3.
$$

The condition $\beta>0$ leaves exactly $(s,\varepsilon)=(1,1)$ and $(-1,1)$. The second branch is a [saddle point](../../../analysis.md#saddle-point), as its real-direction curvature is negative; the stability calculation in the next solution verifies this explicitly. The [stable zero-energy Polonyi vacuum](../../../supersymmetry.md#stable-zero-energy-polonyi-vacuum) therefore selects

$$
\boxed{\beta=2-\sqrt3,\qquad A=3,\quad B=2.}
$$

Zero energy alone, without stationarity and stability, would not imply this parameter value. Even zero energy plus stationarity also admits $\beta=2+\sqrt3$ on the unstable branch.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For the stable branch found above, $t=x+\beta=1$ and $s=1$. Hence the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) is

$$
\boxed{\langle z\rangle=\sqrt3-1,\qquad C=3,\quad D=-1,}
$$

in the stated Planck units. To verify that it is a vacuum rather than merely a zero-energy [stationary point](../../../calculus-of-variations.md#stationary-point), evaluate the [Hessian matrix](../../../calculus.md#hessian-matrix). At either zero-energy stationary branch,

$$
H_{xx}=4s\sqrt3,\qquad H_{yy}=8-4s\sqrt3,\qquad H_{xy}=0.
$$

Because $H$ and its first derivatives vanish there, the [Hessian matrix](../../../calculus.md#hessian-matrix) of $V$ is just $|m|^4e^{x^2}$ times this [Hessian matrix](../../../calculus.md#hessian-matrix). For $s=1$, both eigenvalues are positive. This proves a strict [local minimum](../../../analysis.md#local-minimum) in both real scalar directions. For $s=-1$, $H_{xx}<0$, so the alternative $\beta=2+\sqrt3$, $\langle z\rangle=-\sqrt3-1$ is a [saddle point](../../../analysis.md#saddle-point) and is excluded from the [stable zero-energy Polonyi vacuum](../../../supersymmetry.md#stable-zero-energy-polonyi-vacuum).

There is also a useful global check. Set $u=x-(\sqrt3-1)$ on the stable branch. Directly completing squares gives

$$
H=\left(u^2+y^2+\sqrt3\,u\right)^2+(2\sqrt3-3)u^2+(4-2\sqrt3)y^2.
$$

Both remaining coefficients are positive. Thus $H\geq0$ everywhere, with equality only at $u=y=0$. The positive exponential prefactor proves that this is the unique [global minimum](../../../analysis.md#global-minimum), not just a metastable vacuum.

Finally, at the stable vacuum $z+\beta=1$ and $D_zW=\sqrt3\,m^2$. Its [supergravity auxiliary field](../../../supersymmetry.md#supergravity-auxiliary-field) has

$$
\boxed{|F^z|=\sqrt3\,|m|^2e^{(\sqrt3-1)^2/2}>0\qquad(m\ne0).}
$$

Thus **the Minkowski vacuum breaks supersymmetry**, even though its [cosmological constant](../../../cosmology.md#cosmological-constant) vanishes. If $m=0$, the potential is flat and the displayed tuned parameter and scalar value are not selected.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
