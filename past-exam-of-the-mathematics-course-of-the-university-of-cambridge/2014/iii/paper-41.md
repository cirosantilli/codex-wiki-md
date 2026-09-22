# Paper 41

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_41.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_41.pdf)

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

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a [Lie bracket](../../../lie-algebra.md#lie-bracket) over $\mathbb R$ or $\mathbb C$, [antisymmetry of a Lie bracket](../../../lie-algebra.md#antisymmetry-of-a-lie-bracket) means $[x,y]=-[y,x]$. In particular $[x,x]=0$ in these characteristic-zero fields. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) is

$$
\boxed{[x,[y,z]]+[y,[z,x]]+[z,[x,y]]=0.}
$$

It expresses compatibility of the bracket with its own adjoint action. Bilinearity must hold over the chosen base field, and the bracket must take its values in the same [vector space](../../../vector-space.md).

For the [matrix](../../../vector-space.md#matrix) [commutator](../../../lie-algebra.md#commutator), bilinearity and antisymmetry follow directly from distributivity. Associativity of [matrix](../../../vector-space.md#matrix) multiplication gives

$$
[A,[B,C]]=ABC-ACB-BCA+CBA;
$$

adding the two cyclic permutations cancels every monomial. Thus the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) holds in the entire [matrix](../../../vector-space.md#matrix) algebra. For a specified linear subspace, the only additional bracket condition is **closure: $AB-BA$ must belong to the subspace whenever $A,B$ do**. It is unnecessary to require closure under the separate products $AB$ and $BA$.

To determine the [special unitary Lie algebra](../../../lie-algebra.md#special-unitary-lie-algebra), let $g(t)$ be a differentiable curve in the [special unitary group](../../../topological-group.md#special-unitary-group) with $g(0)=I$ and $A=g'(0)$. Differentiating $g(t)^\dagger g(t)=I$ gives $A^\dagger+A=0$. Differentiating $\det g(t)=1$ at the identity gives $\operatorname{tr}A=0$. Conversely a traceless [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix) has $e^{tA}$ unitary and $\det e^{tA}=e^{t\operatorname{tr}A}=1$, so it really is a tangent vector. Therefore

$$
\boxed{\mathfrak{su}(n)=\{A\in M_n(\mathbb C):A^\dagger=-A,\ \operatorname{tr}A=0\},
\qquad \dim_{\mathbb R}\mathfrak{su}(n)=n^2-1.}
$$

This is a real [Lie algebra](../../../lie-algebra.md) of complex [matrices](../../../vector-space.md#matrix): multiplication by $i$ generally leaves this real subspace. Its complexification is $\mathfrak{sl}_n(\mathbb C)$, not the compact algebra itself. For $A,B\in\mathfrak{su}(n)$,

$$
[A,B]^\dagger=B^\dagger A^\dagger-A^\dagger B^\dagger=BA-AB=-[A,B],
\qquad \operatorname{tr}[A,B]=0.
$$

Thus closure holds, and the already verified [commutator](../../../lie-algebra.md#commutator) identities establish all the [Lie algebra](../../../lie-algebra.md) axioms.

The [cross-product Lie algebra](../../../lie-algebra.md#cross-product-lie-algebra) on $\mathbb R^3$ is bilinear, antisymmetric and closed because the [cross product](../../../vector-space.md#cross-product) has those properties. Its [Jacobi identity](../../../lie-algebra.md#jacobi-identity) follows from the vector triple-product identity:

$$
\mathbf x\times(\mathbf y\times\mathbf z)
=\mathbf y(\mathbf x\cdot\mathbf z)-\mathbf z(\mathbf x\cdot\mathbf y).
$$

In the cyclic sum, the coefficients cancel by symmetry of the scalar product.

For the explicit relation to the [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra), take the three [Pauli matrices](../../../algebra.md#pauli-matrices) and define

$$
F(\mathbf x)=-\frac{i}{2}\sum_{a=1}^3x_a\sigma_a.
$$

These [matrices](../../../vector-space.md#matrix) are traceless and [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix), and the three images of the standard basis form a real basis of $\mathfrak{su}(2)$. Using the [Pauli matrix commutator identity](../../../algebra.md#pauli-matrix-commutator-identity),

$$
[F(\mathbf x),F(\mathbf y)]
=-\frac14\,2i\sum_c(\mathbf x\times\mathbf y)_c\sigma_c
=F(\mathbf x\times\mathbf y).
$$

Hence **$F$ is a real [Lie algebra isomorphism](../../../lie-algebra.md#lie-algebra-isomorphism)**. The factor and sign $-i/2$ are essential for preserving the unscaled cross-product bracket. At the group level there is an [Adjoint double cover from SU(2) to SO(3)](../../../lie-theory.md#adjoint-double-cover-from-su-2-to-so-3); the isomorphism of their tangent algebras does not identify the two global groups.

## 2

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take the [Minkowski metric](../../../special-relativity.md#minkowski-metric) with signature $(+---)$ and a coupling $e\ne0$. For a [charged scalar field](../../../quantum-field-theory.md#charged-scalar-field) use the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative)

$$
D_\mu\phi=(\partial_\mu-iea_\mu)\phi,
\qquad \phi'=e^{i\alpha}\phi,
\qquad a'_\mu=a_\mu+e^{-1}\partial_\mu\alpha.
$$

A [scalar electrodynamics](../../../relativistic-quantum-field.md#scalar-electrodynamics) Lagrangian is

$$
\boxed{\mathcal L=-\frac14f_{\mu\nu}f^{\mu\nu}
+(D_\mu\phi)^*D^\mu\phi-V(|\phi|^2).}
$$

Any real potential bounded below and depending only on the modulus gives [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance). Indeed,

$$
D'_\mu\phi'=e^{i\alpha}D_\mu\phi,
\qquad f'_{\mu\nu}=f_{\mu\nu},\qquad |\phi'|^2=|\phi|^2.
$$

The derivative of the phase cancels the shifted [gauge field](../../../relativistic-quantum-field.md#gauge-field) in the first identity; commuting partial derivatives proves the second. These identities verify invariance of every term, including the interaction hidden in the kinetic term.

For an unbroken example choose $V=m_\phi^2|\phi|^2+\lambda|\phi|^4$ with $m_\phi^2>0$ and $\lambda>0$. The minimum is at zero. There is no vector [mass](../../../classical-mechanics.md#mass) term in the quadratic expansion and no [Higgs mechanism](../../../standard-model.md#higgs-mechanism). Pure electromagnetic theory has a neutral massless [spin](../../../quantum-mechanics.md#spin)-one [photon](../../../quantum-mechanics.md#photon) with two physical transverse polarizations, equivalently helicities $+1$ and $-1$; longitudinal and time-component polarizations are gauge redundancies. In the unbroken scalar theory, the same massless [photon](../../../quantum-mechanics.md#photon) is accompanied by a [spin](../../../quantum-mechanics.md#spin)-zero charged particle and its oppositely charged [antiparticle](../../../relativistic-quantum-field.md#antiparticle), both of [mass](../../../classical-mechanics.md#mass) $m_\phi$. A complex scalar has two real physical [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom), rather than two unrelated charged species.

For a Higgs example choose

$$
V=\lambda\left(|\phi|^2-\frac{v^2}{2}\right)^2,\qquad \lambda>0,\quad v>0.
$$

The vacuum modulus is nonzero. Around one vacuum representative, [unitary gauge](../../../standard-model.md#unitary-gauge) removes the phase and writes $\phi=(v+h)/\sqrt2$. Then

$$
(D_\mu\phi)^*D^\mu\phi
=\frac12\partial_\mu h\partial^\mu h+\frac12e^2(v+h)^2a_\mu a^\mu,
\qquad V=\lambda\left(vh+\frac{h^2}{2}\right)^2.
$$

Thus the quadratic spectrum is

$$
\boxed{m_A^2=e^2v^2,\qquad m_h^2=2\lambda v^2.}
$$

The [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) is a massive [spin](../../../quantum-mechanics.md#spin)-one particle with three polarizations, and $h$ is a neutral massive [spin](../../../quantum-mechanics.md#spin)-zero [Higgs boson](../../../standard-model.md#higgs-boson). The scalar phase supplies the longitudinal vector polarization; it is not an extra physical massless [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson). The degree count is unchanged: two massless-vector polarizations plus two scalar degrees become three massive-vector polarizations plus one radial scalar degree. The underlying [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) remains a redundancy of the description.

For the two-charge theory, use

$$
D_\mu\phi=(\partial_\mu-iea_\mu)\phi,
\qquad D_\mu\psi=(\partial_\mu-2iea_\mu)\psi,
$$

and retain the same [gauge transformation](../../../electromagnetism.md#gauge-transformation) of $a_\mu$. Both derivatives transform with the phase of their own field. A manifestly stable [two-charge scalar gauge potential](../../../relativistic-quantum-field.md#two-charge-scalar-gauge-potential) is, for positive $m_\phi^2,M^2,\lambda_\phi,\lambda_\psi$, $g\ge0$ and a nonzero complex constant $b$,

$$
V(\phi,\psi)=m_\phi^2|\phi|^2+M^2|\psi-b\phi^2|^2
+\lambda_\phi|\phi|^4+\lambda_\psi|\psi|^4+g|\phi|^2|\psi|^2.
$$

Since $\psi-b\phi^2$ has charge $2e$, its modulus is [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance). Expanding its square exhibits the direct coupling

$$
-M^2\bigl(b\psi^*\phi^2+b^*\psi\phi^{*2}\bigr)
+M^2|b|^2|\phi|^4.
$$

In particular the charge in $\psi^*\phi^2$ is $-2e+2e=0$, which uses the stated charge ratio. The potential is real, bounded below and has the zero-field minimum, while the kinetic terms have the standard positive signs. A complete example is therefore

$$
\boxed{\mathcal L_2=-\frac14f_{\mu\nu}f^{\mu\nu}
+(D_\mu\phi)^*D^\mu\phi+(D_\mu\psi)^*D^\mu\psi-V(\phi,\psi).}
$$

There is genuine direct interaction even with $g=0$ because $b\ne0$. In four spacetime dimensions $b$ has [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) $-1$, but the expanded potential contains only quadratic, cubic and quartic field monomials; the cubic coefficient $M^2b$ has dimension one. Thus the example is also power-counting renormalizable.

## 3

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Treat the [quarks](../../../standard-model.md#quark) as the fundamental triplet of approximate [flavour symmetry](../../../standard-model.md#flavor-symmetry). The flavour product follows by splitting the first two [quarks](../../../standard-model.md#quark) into symmetric and antisymmetric pieces:

$$
\mathbf3\otimes\mathbf3=\mathbf6\oplus\overline{\mathbf3},\qquad
\mathbf6\otimes\mathbf3=\mathbf{10}\oplus\mathbf8,\qquad
\overline{\mathbf3}\otimes\mathbf3=\mathbf8\oplus\mathbf1.
$$

Therefore

$$
\boxed{\mathbf3^{\otimes3}=\mathbf{10}\oplus\mathbf8\oplus\mathbf8\oplus\mathbf1.}
$$

The dimension check is $27=10+8+8+1$. The [baryon decuplet](../../../standard-model.md#baryon-decuplet) is the completely symmetric flavour sector, the [three-quark flavour singlet](../../../standard-model.md#three-quark-flavour-singlet) is completely antisymmetric, and the two copies of the [baryon octet](../../../standard-model.md#baryon-octet) carry mixed permutation symmetry. The two octet copies are a multiplicity space for permutations of the three [quark](../../../standard-model.md#quark) slots, not automatically two distinct ground-state [baryon](../../../physics.md#baryon) octets.

For the [weight diagrams](../../../semisimple-lie-algebra.md#weight-diagram) use [isospin](../../../standard-model.md#isospin) projection $I_3$ and [flavour hypercharge](../../../standard-model.md#flavor-hypercharge) $Y$. The [quark](../../../standard-model.md#quark) weights are

$$
u:\left(\frac12,\frac13\right),\qquad
d:\left(-\frac12,\frac13\right),\qquad
s:\left(0,-\frac23\right).
$$

Weights add in a [tensor product](../../../linear-algebra.md#tensor-product). In a three-[quark](../../../standard-model.md#quark) composition, $Y=1-n_s$ and $I_3=(n_u-n_d)/2$. The [baryon decuplet](../../../standard-model.md#baryon-decuplet) has rows $(Y,I)=(1,3/2),(0,1),(-1,1/2),(-2,0)$. Its upper-right weight is $uuu$, the $\Delta^{++}$, while its bottom weight is $sss$, the $\Omega^-$. In the [baryon octet](../../../standard-model.md#baryon-octet), the upper weights are $uud$ and $udd$, giving the proton and neutron. The origin has two independent states with content $uds$: the $I=1$ $\Sigma^0$ and the $I=0$ $\Lambda$. Their equal weights do not make them the same state. The [three-quark flavour singlet](../../../standard-model.md#three-quark-flavour-singlet) has only $(I_3,Y)=(0,0)$ and content $uds$, with normalized flavour wavefunction

$$
|\mathbf1\rangle=\frac{1}{\sqrt6}
\bigl(|uds\rangle+|dsu\rangle+|sud\rangle-|usd\rangle-|dus\rangle-|sdu\rangle\bigr).
$$

This singlet is a different representation from the octet $\Lambda$, despite the same [quark](../../../standard-model.md#quark) content and weight.

<a id="3/image-flavour-weight-diagrams-for-the-baryon-decuplet-octet-singlet-and-pentaquark-antidecuplet-red-rings-mark-the-three-exotic-weights"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-41-flavour-weights.png)

**[Figure 1](#3/image-flavour-weight-diagrams-for-the-baryon-decuplet-octet-singlet-and-pentaquark-antidecuplet-red-rings-mark-the-three-exotic-weights). Flavour weight diagrams for the baryon decuplet, octet, singlet and pentaquark antidecuplet; red rings mark the three exotic weights**.

The [Pauli exclusion principle](../../../quantum-mechanics.md#pauli-exclusion-principle) requires the full three-[quark](../../../standard-model.md#quark) wavefunction to change sign under exchange of any two [quarks](../../../standard-model.md#quark), including their spatial, [spin](../../../quantum-mechanics.md#spin), flavour and colour labels. A [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet) has the antisymmetric colour factor $\epsilon_{abc}/\sqrt6$. Consequently the remaining spatial-[spin](../../../quantum-mechanics.md#spin)-flavour factor must be symmetric. The flavour representation alone is not the full exchange wavefunction.

For the lowest orbital state, the spatial wavefunction is symmetric. Completely symmetric decuplet flavour then requires the symmetric [spin](../../../quantum-mechanics.md#spin)-$3/2$ wavefunction; this includes states such as $uuu$ with aligned spins and does not violate Pauli because their colours are antisymmetrized. Mixed octet flavour combines with mixed [spin](../../../quantum-mechanics.md#spin)-$1/2$ wavefunctions to give a symmetric [spin](../../../quantum-mechanics.md#spin)-flavour factor. More explicitly, the two-dimensional permutation representation of mixed symmetry tensored with itself contains the trivial representation, which selects the physical symmetric combination. These are the familiar ground-state [spin](../../../quantum-mechanics.md#spin) assignments.

Antisymmetric singlet flavour in a symmetric orbital state would instead require a completely antisymmetric three-[quark](../../../standard-model.md#quark) [spin](../../../quantum-mechanics.md#spin) state. But $\bigwedge^3\mathbb C^2=0$, so three [spin](../../../quantum-mechanics.md#spin)-$1/2$ [quarks](../../../standard-model.md#quark) have no such state. **There is no flavour-singlet three-[quark](../../../standard-model.md#quark) ground-state S-wave [baryon](../../../physics.md#baryon).** A singlet is allowed with orbital excitation: mixed spatial and mixed [spin](../../../quantum-mechanics.md#spin) symmetry can combine antisymmetrically, and their product with the antisymmetric flavour sector is symmetric. For example an $L=1$, [spin](../../../quantum-mechanics.md#spin)-$1/2$ configuration can give negative-parity total spins $1/2$ or $3/2$. This [Pauli constraint on three-quark flavour multiplets](../../../physics.md#pauli-constraint-on-three-quark-flavour-multiplets) distinguishes a permitted representation in the flavour [tensor product](../../../linear-algebra.md#tensor-product) from its possible orbital-[spin](../../../quantum-mechanics.md#spin) realization.

For a [pentaquark](../../../physics.md#pentaquark), choose each of two [quark](../../../standard-model.md#quark) pairs in $\overline{\mathbf3}$. Their symmetric flavour combination lies in $\overline{\mathbf6}$, and combining with the [antiquark](../../../standard-model.md#antiquark) gives

$$
\boxed{\overline{\mathbf6}\otimes\overline{\mathbf3}
=\overline{\mathbf{10}}\oplus\mathbf8.}
$$

Thus $\mathbf3^{\otimes4}\otimes\overline{\mathbf3}$ contains a [pentaquark antidecuplet](../../../physics.md#pentaquark-antidecuplet). This identifies a flavour sector; it does not by itself prove binding or fix the [spin](../../../quantum-mechanics.md#spin) and orbital structure needed for overall fermion antisymmetry.

The antidecuplet is the conjugate of the symmetric decuplet, so its rows are $(Y,I)=(2,0),(1,1/2),(0,1),(-1,3/2)$. A three-[quark](../../../standard-model.md#quark) state only has $Y=1,0,-1,-2$, and at $Y=-1$ it contains two strange [quarks](../../../standard-model.md#quark) and one light [quark](../../../standard-model.md#quark), allowing only $I_3=\pm1/2$. Hence the exotic weights are precisely

$$
\boxed{(I_3,Y)=(0,2),\quad(-3/2,-1),\quad(3/2,-1):\quad\textbf{three states}.}
$$

Possible minimal contents are $uudd\bar s$, $ddss\bar u$, and $uuss\bar d$. By the [Gell-Mann--Nishijima formula](../../../standard-model.md#gell-mann-nishijima-formula), their charges are respectively $+1,-2,+1$. Every other antidecuplet weight is also a weight of some three-[quark](../../../standard-model.md#quark) composition, although its total [isospin](../../../standard-model.md#isospin) representation can differ.

Exotic weights do not imply a weak-decay lifetime. The [strong interaction](../../../standard-model.md#strong-interaction) can conserve all the quantum numbers in [baryon](../../../physics.md#baryon)-plus-[meson](../../../physics.md#meson) channels, for example

$$
uudd\bar s\ \longrightarrow\ pK^0\ \text{or}\ nK^+,
\qquad ddss\bar u\ \longrightarrow\ \Xi^-\pi^-,
\qquad uuss\bar d\ \longrightarrow\ \Xi^0\pi^+.
$$

These are [quark](../../../standard-model.md#quark) rearrangements into a three-[quark](../../../standard-model.md#quark) [baryon](../../../physics.md#baryon) and a [quark](../../../standard-model.md#quark)-[antiquark](../../../standard-model.md#antiquark) [meson](../../../physics.md#meson), not decay into a single three-[quark](../../../standard-model.md#quark) state. Accordingly **they are generically short-lived strong resonances if these channels are kinematically open**. Flavour representation theory alone gives no masses or widths; a state below all strong thresholds, or one with dynamically suppressed couplings, can be longer-lived. The quantum numbers provide no general protection against the displayed strong decays.

## 4

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use the metric in the question and fix the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) convention $\epsilon_{0123}=+1$. A consistent choice of rotation [Lie algebra generators](../../../lie-algebra.md#lie-algebra-generator) is

$$
\boxed{J_1=M^{23},\qquad J_2=M^{31},\qquad J_3=M^{12}.}
$$

Substituting the indices into the printed [Poincare algebra](../../../special-relativity.md#poincare-algebra) gives

$$
[J_1,J_2]=[M^{23},M^{31}]=\eta^{33}M^{21}
=-M^{21}=M^{12}=J_3.
$$

The other cyclic brackets follow the same way. The negative spatial metric and antisymmetry of $M^{\rho\sigma}$ both enter this sign.

The printed brackets are real [Lie algebra](../../../lie-algebra.md) brackets, without the factor $i$ used for ordinary [commutators](../../../lie-algebra.md#commutator) of Hermitian quantum observables. We use those brackets for the algebraic verifications. For physical eigenvalues below, angular momentum is Hermitian, its [spin](../../../quantum-mechanics.md#spin) projection is the real number $j_3$, and $\hbar=1$. In that quantum convention the ordinary operator [commutators](../../../lie-algebra.md#commutator) are $i$ times the displayed brackets. This distinction prevents identifying a real [spin](../../../quantum-mechanics.md#spin) projection with an anti-Hermitian [matrix](../../../vector-space.md#matrix) eigenvalue.

In the [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra), translations commute. The [Pauli-Lubanski pseudovector](../../../special-relativity.md#pauli-lubanski-pseudovector) therefore satisfies

$$
W_\mu P^\mu=\frac12\epsilon_{\mu\nu\rho\tau}M^{\nu\rho}P^\tau P^\mu=0.
$$

For fixed $\nu,\rho$, the product of momenta is symmetric in $\mu,\tau$ while the epsilon coefficient is antisymmetric in them. There is no need to commute the Lorentz generator through the momenta.

Using the [commutator derivation identity](../../../lie-algebra.md#commutator-derivation-identity) and the mixed bracket,

$$
\begin{aligned}
[W_\mu,P^\sigma]
&=\frac12\epsilon_{\mu\nu\rho\tau}
\bigl(\eta^{\rho\sigma}P^\nu-\eta^{\nu\sigma}P^\rho\bigr)P^\tau\\
&=\epsilon_{\mu\nu\rho\tau}\eta^{\rho\sigma}P^\nu P^\tau=0.
\end{aligned}
$$

The two terms become equal after swapping $\nu,\rho$, and the last expression vanishes by antisymmetry in $\nu,\tau$. In the Hermitian observable convention, the calculation has one overall extra $i$ and still vanishes. Thus **$W_\mu$ preserves each momentum eigenspace**.

For the specified epsilon orientation, two useful component identities are

$$
W_0=J_1P^1+J_2P^2+J_3P^3,
\qquad W_3=-J_3P^0+M^{02}P^1-M^{01}P^2.
$$

The order displayed matters: the momentum operator is on the right, so it can act first on the momentum eigenstate. At rest, $p^\mu=(m,0,0,0)$, and on a [spin](../../../quantum-mechanics.md#spin) state with $J_3|j,j_3\rangle=j_3|j,j_3\rangle$ these give

$$
\boxed{W_0|\psi\rangle=0,\qquad W_3|\psi\rangle=-mj_3|\psi\rangle.}
$$

These are [massive rest-frame Pauli-Lubanski eigenvalues](../../../special-relativity.md#massive-rest-frame-pauli-lubanski-eigenvalues). The raised component would be $W^3=+mj_3$; confusing $W_3$ with $W^3$ reverses the answer.

[Helicity](../../../special-relativity.md#helicity) is the projection of [spin angular momentum](../../../quantum-mechanics.md#spin), or equivalently the rotation generator acting internally, along the momentum direction:

$$
h=\frac{\mathbf J\cdot\mathbf p}{|\mathbf p|}.
$$

For the momentum $p^\mu=(k,0,0,k)$ with $k>0$, the [helicity](../../../special-relativity.md#helicity) operator is $J_3$. Hence a [helicity](../../../special-relativity.md#helicity)-$j_3$ state has

$$
\boxed{W_0|\psi\rangle=kj_3|\psi\rangle,\qquad
W_3|\psi\rangle=-kj_3|\psi\rangle.}
$$

The result uses only the two longitudinal components and does not need a separate assumption about the transverse little-group generators. These [massless longitudinal Pauli-Lubanski eigenvalues](../../../special-relativity.md#massless-longitudinal-pauli-lubanski-eigenvalues) agree with $W^\mu=j_3P^\mu$ for ordinary finite-[helicity](../../../special-relativity.md#helicity) representations.

Finally, at rest the contraction is $mW_0=0$. For the chosen null momentum it is $k(W_0+W_3)$, whose two eigenvalues cancel. Thus **both results obey $W_\mu P^\mu=0$**. Reversing the epsilon orientation reverses all $W$ eigenvalues together; it leaves both identities and both consistency checks intact. For a literal anti-Hermitian derived representation $\rho$ of the printed real algebra, write $H_X=i\rho(X)$ for the Hermitian observable. Since $W_\mu$ is bilinear in generators, its abstract enveloping-algebra image is $\rho(W_\mu)=-W_{\mu,\mathrm{phys}}$. Thus the corresponding formal-image eigenvalues, if that convention is intended, are

$$
\boxed{\text{rest}:\ (\rho(W_0),\rho(W_3))=(0,+mj_3),\qquad
\text{null}:\ (\rho(W_0),\rho(W_3))=(-kj_3,+kj_3).}
$$

Here $\rho(P^\mu)$ has eigenvalue $-ip^\mu$, while $p^\mu$ and $j_3$ themselves remain real physical labels. This is the same result after the [Hermitian quantum generator convention](../../../lie-algebra.md#hermitian-quantum-generator-convention) is applied to both factors, not an inconsistent choice of [spin](../../../quantum-mechanics.md#spin) sign. Both the Hermitian-observable and literal anti-Hermitian interpretations are consequently specified.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
