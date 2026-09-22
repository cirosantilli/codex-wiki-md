# Paper 63

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper63.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper63.pdf)

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

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use $|m,m'\rangle$ as shorthand for the [tensor product](../../../linear-algebra.md#tensor-product) of two total-[isospin](../../../standard-model.md#isospin)-one states with third components $m,m'$. A total-[isospin](../../../standard-model.md#isospin)-zero state must have total third component zero, so write $a|1,-1\rangle+b|0,0\rangle+c|-1,1\rangle$. Applying the total [raising operator](../../../semisimple-lie-algebra.md#raising-operator) gives

$$
I_+\bigl(a|1,-1\rangle+b|0,0\rangle+c|-1,1\rangle\bigr)
=\sqrt2\bigl[(a+b)|1,0\rangle+(b+c)|0,1\rangle\bigr].
$$

An [isospin](../../../standard-model.md#isospin) singlet must be annihilated by this operator; hence $b=-a$ and $c=a$. Normalization gives the [two-isovector singlet](../../../standard-model.md#two-isovector-singlet)

$$
\boxed{|I=0,M=0\rangle=\frac{|1,-1\rangle-|0,0\rangle+|-1,1\rangle}{\sqrt3}.}
$$

It is also annihilated by the total [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator). A raising or lowering action changes the third-component label by one; the unchanged output label in the PDF's preliminary ladder formula is a typographical omission, not the action used here.

Exchange commutes with the total [isospin](../../../standard-model.md#isospin) operators. The displayed singlet is symmetric. The $I=2$ multiplet has symmetric highest state $|1,1\rangle$; applying the symmetric total [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator) preserves that exchange symmetry. The symmetric square of a three-dimensional space has dimension six, exactly $1+5$, while its antisymmetric square has dimension three. The remaining $I=1$ multiplet is therefore antisymmetric. Thus the [Clebsch-Gordan decomposition](../../../quantum-mechanics.md#clebsch-gordan-decomposition) is

$$
\mathbf3\otimes\mathbf3=\mathbf1_S\oplus\mathbf3_A\oplus\mathbf5_S.
$$

[Pions](../../../standard-model.md#pion) have zero intrinsic [spin](../../../quantum-mechanics.md#spin) and form an [isospin](../../../standard-model.md#isospin) triplet. [Bose-Einstein statistics](../../../statistical-physics.md#bose-einstein-statistics) requires the complete two-pion state to be symmetric under exchange. Its relative orbital state changes by $(-1)^\ell$, so odd [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) requires antisymmetric [isospin](../../../standard-model.md#isospin): **an odd-$\ell$ two-pion state has $I=1$**. This statement treats the charge components as states of the same [isospin](../../../standard-model.md#isospin) multiplet, rather than ignoring exchange when their charges differ.

For the decay, let $|\chi\rangle=H_I|K^0\rangle$. The stated commutator with $I_3$ gives $I_3|\chi\rangle=0$. More decisively, the commuting [raising operator](../../../semisimple-lie-algebra.md#raising-operator) gives

$$
I_+^2|\chi\rangle=H_I I_+^2|K^0\rangle=0.
$$

The kaon doublet cannot be raised twice. An $I=2,M=0$ component would survive two raisings, so it is excluded. Meanwhile a spinless [kaon](../../../physics.md#kaon) decaying into two spinless [pions](../../../standard-model.md#pion) has $\ell=0$ by conservation of total [angular momentum](../../../classical-mechanics.md#angular-momentum), independently of whether parity is conserved by the decay. The exchange condition excludes $I=1$. This proves the [highest-weight weak-isospin selection in kaon decay](../../../standard-model.md#highest-weight-weak-isospin-selection-in-kaon-decay): **the two-pion final state has $I=0$**.

In a consistent pion phase convention, the singlet's charge components have the structure

$$
|0,0\rangle=\frac{|\pi^+\pi^-\rangle+|\pi^-\pi^+\rangle-|\pi^0\pi^0\rangle}{\sqrt3}.
$$

The normalized symmetric charged channel has coefficient $\sqrt{2/3}$ and the neutral channel coefficient $-1/\sqrt3$. Thus, in the [isospin](../../../standard-model.md#isospin) limit with equal pion masses and matching two-body phase space,

$$
\boxed{\frac{\Gamma(K^0\to\pi^+\pi^-)}{\Gamma(K^0\to\pi^0\pi^0)}=2.}
$$

Equivalently, ordered charged and neutral amplitudes have equal magnitudes, but neutral identical particles contribute the phase-space factor $1/2!$. This is the same counting expressed in another basis, and must not be included a second time after using the normalized charge-channel coefficients. Small pion-mass and electromagnetic effects can modify the ideal ratio.

## 2

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Kronecker delta](../../../linear-algebra.md#kronecker-delta) is the identity map on the defining representation. Its transformation is $A^\alpha{}_\gamma\delta^\gamma{}_\delta(A^{-1})^\delta{}_\beta=\delta^\alpha{}_\beta$. For the alternating [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol), the determinant identity gives

$$
A^\alpha{}_aA^\beta{}_bA^\gamma{}_c\epsilon^{abc}=(\det A)\epsilon^{\alpha\beta\gamma}=\epsilon^{\alpha\beta\gamma}.
$$

The lower-index alternating [tensor](../../../linear-algebra.md#tensor) transforms with three inverse [matrices](../../../vector-space.md#matrix) and acquires $\det(A^{-1})=1$ instead. Thus **$\delta^\alpha{}_\beta$, $\epsilon^{\alpha\beta\gamma}$ and $\epsilon_{\alpha\beta\gamma}$ are invariant [tensors](../../../linear-algebra.md#tensor)** of [SU(3)](../../../topological-group.md#su-3-group). These identities use unimodularity; unitarity identifies the dual representation with the complex-conjugate defining representation.

For a [mixed SU(3) tensor representation](../../../topological-group.md#mixed-su-3-tensor-representation) $T^a{}_b$, the [matrix trace](../../../linear-algebra.md#matrix-trace) is invariant. Hence

$$
T^a{}_b=\frac13\delta^a{}_b\,T^c{}_c+Q^a{}_b,\qquad Q^a{}_a=0,
$$

gives

$$
\boxed{\mathbf3\otimes\overline{\mathbf3}=\mathbf1\oplus\mathbf8.}
$$

The trace is the singlet. The traceless [matrix](../../../vector-space.md#matrix) transforms by conjugation, so it is the [adjoint representation of SU(3)](../../../lie-algebra.md#adjoint-representation-of-su-3). It is irreducible: an invariant complex subspace is invariant under commutators with the complexified algebra $\mathfrak{sl}_3$, and would be an ideal in that simple [Lie algebra](../../../lie-algebra.md). Only the zero and full traceless-[matrix](../../../vector-space.md#matrix) spaces are possible.

For the cubic [tensor](../../../linear-algebra.md#tensor), define its symmetric and antisymmetric first-pair parts by

$$
T_+^{abc}=\frac12(T^{abc}+T^{bac}),\qquad
T_-^{abc}=\frac12(T^{abc}-T^{bac}),
$$

and let $S^{abc}=T^{(abc)}$ be its completely symmetric part. This has $\binom{5}{3}=10$ independent components and transforms as the [symmetric cubic representation of SU(3)](../../../topological-group.md#symmetric-cubic-representation-of-su-3). Its irreducibility can be seen in the homogeneous cubic-polynomial realization: the simultaneous highest-weight conditions $z_1\partial_{z_2}P=0$ and $z_2\partial_{z_3}P=0$ leave only $P\propto z_1^3$. A finite-dimensional unitary representation is completely reducible, and each irreducible summand has a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector), so this single highest-weight line implies a single irreducible summand. Lowering generates all ten monomials.

Remove this fully symmetric part from $T_+$, putting $M^{abc}=T_+^{abc}-S^{abc}$. Define

$$
O^a{}_d=\epsilon_{dbc}M^{abc}.
$$

Its trace vanishes because $M$ is symmetric in its first two indices. Invariance of $\epsilon$ makes $O$ transform as one upper and one lower index. The inverse map is

$$
M^{abc}=\frac13\left(\epsilon^{bcd}O^a{}_d+\epsilon^{acd}O^b{}_d\right).
$$

Indeed contraction with $\epsilon_{ebc}$ gives $(2O^a{}_e+O^a{}_e-\delta^a{}_e\operatorname{tr}O)/3=O^a{}_e$. The inverse has the required first-pair symmetry and zero completely symmetric part. Thus this eight-dimensional remainder is another [adjoint representation of SU(3)](../../../lie-algebra.md#adjoint-representation-of-su-3).

For the antisymmetric part, define

$$
N^c{}_d=\frac12\epsilon_{dab}T_-^{abc},\qquad
T_-^{abc}=\epsilon^{abd}N^c{}_d.
$$

Now decompose $N^c{}_d=U^c{}_d+\delta^c{}_d\operatorname{tr}N/3$, with $U$ traceless. The first term supplies a second independent octet; the trace supplies a singlet proportional to $\epsilon^{abc}$. With $q=\epsilon_{abc}T^{abc}/6=\operatorname{tr}N/3$, the [explicit cubic SU3 tensor projections](../../../topological-group.md#explicit-cubic-su3-tensor-projections) reconstruct the entire [tensor](../../../linear-algebra.md#tensor):

$$
T^{abc}=S^{abc}
+\frac13\left(\epsilon^{bcd}O^a{}_d+\epsilon^{acd}O^b{}_d\right)
+\epsilon^{abd}U^c{}_d+q\epsilon^{abc}.
$$

All projections commute with the [SU(3)](../../../topological-group.md#su-3-group) action because they use permutations and [invariant tensors](../../../representation-theory.md#invariant-tensor). Their inverse maps and the dimension count $10+8+8+1=27$ establish

$$
\boxed{\mathbf3\otimes\mathbf3\otimes\mathbf3=\mathbf{10}\oplus\mathbf8\oplus\mathbf8\oplus\mathbf1.}
$$

The two octets are equivalent as group representations but distinct subspaces in this decomposition; one comes from the first-pair symmetric sector and the other from the first-pair antisymmetric sector. General permutations can mix these equivalent copies.

In the [quark model](../../../physics.md#quark-model), the [up quark](../../../standard-model.md#up-quark), [down quark](../../../standard-model.md#down-quark) and [strange quark](../../../standard-model.md#strange-quark) form the defining triplet of approximate [flavor symmetry](../../../standard-model.md#flavor-symmetry). Three-quark [baryons](../../../physics.md#baryon) therefore have precisely these possible flavor representations. The fully symmetric decuplet corresponds to the observed spin-$3/2$ [baryon decuplet](../../../standard-model.md#baryon-decuplet): the four [Delta baryons](../../../physics.md#delta-baryon), three $\Sigma^*$ states, two $\Xi^*$ states and the [Omega baryon](../../../physics.md#omega-baryon). Their strangeness rows have [flavor hypercharge](../../../standard-model.md#flavor-hypercharge) and [isospin](../../../standard-model.md#isospin) $(Y,I)=(1,3/2),(0,1),(-1,1/2),(-2,0)$; $uuu$ and $sss$ occupy the extreme $\Delta^{++}$ and $\Omega^-$ weights.

The observed spin-$1/2$ [baryon octet](../../../standard-model.md#baryon-octet) contains the [nucleons](../../../physics.md#nucleon), three [Sigma baryons](../../../physics.md#sigma-baryon), the [Lambda baryon](../../../physics.md#lambda-baryon) and two [Xi baryons](../../../physics.md#xi-baryon). In its $Y=0$ row, $\Sigma^0$ and $\Lambda$ share the same third-component/hypercharge weight but have different total [isospin](../../../standard-model.md#isospin). Approximate flavor symmetry explains multiplet organization, not exact equality of all their masses: the strange-quark mass and electromagnetic interactions break it.

The two octet copies in the flavor [tensor](../../../linear-algebra.md#tensor) do not require two identical ground-state octets. A [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet) is antisymmetric in color; for a symmetric ground-state orbital wavefunction, the [Pauli exclusion principle](../../../quantum-mechanics.md#pauli-exclusion-principle) requires a symmetric combined spin-flavor state. The mixed flavor octet [tensors](../../../linear-algebra.md#tensor) combine with the mixed spin-$1/2$ [tensors](../../../linear-algebra.md#tensor) to supply that symmetry. The symmetric flavor decuplet combines with symmetric spin $3/2$. Together they form the [symmetric spin-flavour SU6 representation](../../../physics.md#symmetric-spin-flavour-su6-representation), with $10\times4+8\times2=56$ spin-flavor states. A completely antisymmetric flavor singlet cannot appear in this spatial ground state because three spin-$1/2$ indices have no fully antisymmetric spin state: $\bigwedge^3\mathbb C^2=0$. [Three-quark flavour singlet](../../../standard-model.md#three-quark-flavour-singlet) configurations instead require a suitable excited spatial/spin symmetry. Flavor [SU(3)](../../../topological-group.md#su-3-group) here is distinct from the exact color gauge symmetry; treating them as the same group action would misidentify the physical multiplets.

## 3

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [Cartan-Weyl basis](../../../semisimple-lie-algebra.md#cartan-weyl-basis), the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[H_i,[E_\alpha,E_\beta]]=[[H_i,E_\alpha],E_\beta]+[E_\alpha,[H_i,E_\beta]]
=(\alpha_i+\beta_i)[E_\alpha,E_\beta].
$$

Thus the bracket has joint Cartan weight $\alpha+\beta$. If $\beta=-\alpha$, it belongs to the zero-weight space, which is the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra), and so is a [linear combination](../../../vector-space.md#linear-combination) $\widetilde\alpha_iH_i$. If $\alpha+\beta$ is a nonzero [root](../../../semisimple-lie-algebra.md#root-of-a-root-system), its [root space](../../../semisimple-lie-algebra.md#root-space) is one-dimensional and the bracket is proportional to $E_{\alpha+\beta}$. If that nonzero sum is not a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system), the bracket vanishes. This proves the asserted forms without assuming every pair of [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) has a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) sum.

With the stated normalization, put $H_\alpha=2\alpha_iH_i/\alpha^2$. The commutators become

$$
[H_\alpha,E_\alpha]=2E_\alpha,\qquad [H_\alpha,E_{-\alpha}]=-2E_{-\alpha},\qquad
[E_\alpha,E_{-\alpha}]=H_\alpha.
$$

The adjoint relations make $J_3=H_\alpha/2$, $J_+=E_\alpha$, $J_-=E_{-\alpha}$ the usual [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra) generators. Hence every finite-dimensional [SU(2)](../../../topological-group.md#su-2-group) irreducible component has $J_3$ [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $m=-j,-j+1,\ldots,j$, with $2j$ an integer. Therefore **$H_\alpha$ has integer [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2m$**, including in the finite-dimensional [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Algebraically this is the [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root).

If $[H_\alpha,X_\lambda]=\lambda X_\lambda$, another use of the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[H_\alpha,[E_\alpha,X_\lambda]]=(\lambda+2)[E_\alpha,X_\lambda].
$$

The bracket is therefore zero or lies in the [eigenvalue](../../../linear-operator-theory.md#eigenvalue)-$\lambda+2$ space. Within one irreducible [SU(2)](../../../topological-group.md#su-2-group) ladder it is proportional to the next chosen vector $X_{\lambda+2}$. If the full eigenspace has multiplicity, the weight statement is the general one; proportionality to one named vector presupposes the ladder choice. Similarly $E_{-\alpha}$ lowers this [eigenvalue](../../../linear-operator-theory.md#eigenvalue) by two, and the ladder weights run from $-n$ to $n$ in steps of two.

For a [root vector](../../../semisimple-lie-algebra.md#root-vector) $E_\beta$, its $H_\alpha$ weight is

$$
m_{\alpha\beta}=\frac{2\alpha\cdot\beta}{\alpha^2}.
$$

The adjoint [SU(2)](../../../topological-group.md#su-2-group) ladder therefore proves

$$
\boxed{\frac{2\alpha\cdot\beta}{\alpha^2}\in\mathbb Z.}
$$

For nonparallel $\alpha,\beta$, raising and lowering $E_\beta$ move its joint Cartan weight through the [root string](../../../semisimple-lie-algebra.md#root-string) $\beta+k\alpha$. The finite irreducible ladder has weights symmetric about zero. Starting at $m_{\alpha\beta}$, reaching its partner $-m_{\alpha\beta}$ requires $k=-m_{\alpha\beta}$. The corresponding nonzero vector lies in the [root space](../../../semisimple-lie-algebra.md#root-space) of $\beta-m_{\alpha\beta}\alpha$, proving the [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) property:

$$
\boxed{s_\alpha(\beta)=\beta-\frac{2\alpha\cdot\beta}{\alpha^2}\alpha\text{ is a root}.}
$$

There is no zero joint [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) in this string when $\alpha,\beta$ are nonparallel. Its one-dimensional [root spaces](../../../semisimple-lie-algebra.md#root-space) prevent two irreducible ladders with the same weight parity from overlapping, so the ladder argument applies to the entire string. For $\beta=\pm\alpha$, reflection simply interchanges the two opposite [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system), which already exist by the adjoint relation.

For angle and length restrictions, set $p=2\alpha\cdot\beta/\alpha^2$ and $q=2\alpha\cdot\beta/\beta^2$. These [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) have the same sign when nonzero and obey

$$
pq=4\cos^2\theta,\qquad \frac{\alpha^2}{\beta^2}=\frac qp.
$$

For nonparallel, nonorthogonal [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system), $pq$ is an integer strictly between zero and four. The possibilities are consequently:

- $pq=1$: $|p|=|q|=1$, equal lengths, and $\theta=\pi/3$ or $2\pi/3$.
- $pq=2$: $\{|p|,|q|\}=\{1,2\}$, squared-length ratio $2$ or $1/2$, and $\theta=\pi/4$ or $3\pi/4$.
- $pq=3$: $\{|p|,|q|\}=\{1,3\}$, squared-length ratio $3$ or $1/3$, and $\theta=\pi/6$ or $5\pi/6$.

[Orthogonal](../../../linear-algebra.md#orthogonal-vectors) [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) have $p=q=0$ and $\theta=\pi/2$. Parallel [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) have $pq=4$; the integer pairs would allow only length multiples $1,2,1/2$. The stated reducedness condition excludes the latter two, so parallel [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are equal or opposite, with angles zero or $\pi$ and equal lengths. Thus

$$
\boxed{\theta\in\{0,\pi/6,\pi/4,\pi/3,\pi/2,2\pi/3,3\pi/4,5\pi/6,\pi\}.}
$$

Not every [root system](../../../semisimple-lie-algebra.md#root-system) realizes every listed angle.

The [orthogonal](../../../linear-algebra.md#orthogonal-vectors) pair alone gives no ratio through $q/p$. To finish the length restriction for a [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra), use irreducibility of its [root system](../../../semisimple-lie-algebra.md#root-system). Let $U$ span the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) orbit of $\alpha$. Both $U$ and $U^\perp$ are invariant under the [orthogonal](../../../linear-algebra.md#orthogonal-vectors) [root reflections](../../../semisimple-lie-algebra.md#root-reflection). If a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) had nonzero projections in both, reflection of its projection in $U$ would have a nonzero $U^\perp$ component, violating invariance. Hence every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) is entirely in one of these subspaces. A proper nonzero $U$ would split the [root system](../../../semisimple-lie-algebra.md#root-system) into two [orthogonal](../../../linear-algebra.md#orthogonal-vectors) parts, contradicting irreducibility. This proves that the [Weyl orbit spans an irreducible root space](../../../semisimple-lie-algebra.md#weyl-orbit-spans-an-irreducible-root-space).

In particular, some orbit [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) $\gamma$ is nonorthogonal to any chosen $\beta$, and $\gamma^2=\alpha^2$. Applying the previous integer-pair restriction to $\gamma,\beta$ therefore also handles [orthogonal](../../../linear-algebra.md#orthogonal-vectors) $\alpha,\beta$:

$$
\boxed{\frac{\alpha^2}{\beta^2}\in\{1,2,1/2,3,1/3\}.}
$$

There can be at most two different [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) lengths: three lengths would have ratios two and three relative to the shortest, but then the longest-to-middle squared-length ratio would be $3/2$, which is forbidden. A reducible collection of [orthogonal](../../../linear-algebra.md#orthogonal-vectors) rank-one factors could have independently chosen scales; the simple-algebra assumption excludes that exception.

Choose a generic linear functional to define [positive roots](../../../semisimple-lie-algebra.md#positive-root). The [simple roots](../../../semisimple-lie-algebra.md#simple-root) are those positive [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) which cannot be written as sums of two positive [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system); they form a basis in which all [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) coefficients are integers of one sign. Distinct simple [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) have nonpositive inner product: if their inner product were positive, their [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) string would contain their difference, and whichever difference is positive would decompose one of them. In rank two, irreducibility excludes the [orthogonal](../../../linear-algebra.md#orthogonal-vectors) case. The allowed simple-[root](../../../semisimple-lie-algebra.md#root-of-a-root-system) angles are therefore $120^\circ,135^\circ,150^\circ$, giving the three irreducible diagrams in the [classification of rank-two root systems](../../../semisimple-lie-algebra.md#classification-of-rank-two-root-systems): [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system), [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system) and [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system). Reflections in the two simple [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) generate their respective six, eight and twelve [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system).

Here are explicit simple-[root](../../../semisimple-lie-algebra.md#root-of-a-root-system) choices and positive [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system); adding their negatives gives each complete diagram.

- For [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system), take $\alpha_1=(1,0)$ and $\alpha_2=(-1/2,\sqrt3/2)$. The positive [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are $\alpha_1,\alpha_2,\alpha_1+\alpha_2$; all have squared length one.
- For [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system), take the long $\alpha_1=(1,-1)$ and short $\alpha_2=(0,1)$. The positive [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are $\alpha_1,\alpha_2,\alpha_1+\alpha_2,\alpha_1+2\alpha_2$. These give the four axis [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) and four diagonal [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system), with squared lengths one and two. The rank-two $C_2$ [Lie algebra](../../../lie-algebra.md) is isomorphic to this one; changing the long/short ordering changes its Cartan presentation.
- For [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system), take short $\alpha_1=(1,0)$ and long $\alpha_2=(-3/2,\sqrt3/2)$. The positive [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are $\alpha_1,\alpha_2,\alpha_1+\alpha_2,2\alpha_1+\alpha_2,3\alpha_1+\alpha_2,3\alpha_1+2\alpha_2$. They give two hexagons rotated by $30^\circ$, with squared lengths one and three.

The nonnegative coefficients in each positive-[root](../../../semisimple-lie-algebra.md#root-of-a-root-system) list verify the chosen [simple roots](../../../semisimple-lie-algebra.md#simple-root) explicitly. The [orthogonal](../../../linear-algebra.md#orthogonal-vectors) four-[root system](../../../semisimple-lie-algebra.md#root-system) $A_1\times A_1$ is rank two but reducible, so it is not a diagram for the simple algebra assumed here.

Define the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) in the column-coroot convention:

$$
C_{ij}=\langle\alpha_i,\alpha_j^\vee\rangle=\frac{2\alpha_i\cdot\alpha_j}{\alpha_j^2},\qquad
[H_{\alpha_j},E_{\alpha_i}]=C_{ij}E_{\alpha_i}.
$$

Using the ordered [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) above gives

$$
\boxed{C_{A_2}=\begin{pmatrix}2&-1\\-1&2\end{pmatrix},\qquad
C_{B_2}=\begin{pmatrix}2&-2\\-1&2\end{pmatrix},\qquad
C_{G_2}=\begin{pmatrix}2&-1\\-3&2\end{pmatrix}.}
$$

The alternative row-coroot convention transposes these [matrices](../../../vector-space.md#matrix). Stating the convention and [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) ordering avoids a spurious disagreement in the unequal-length cases.

<a id="3/image-the-irreducible-rank-two-root-systems-a2-b2-and-g2-with-long-and-short-roots-and-explicit-ordered-simple-roots-highlighted"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-63-rank-two-roots.png)

**[Figure 1](#3/image-the-irreducible-rank-two-root-systems-a2-b2-and-g2-with-long-and-short-roots-and-explicit-ordered-simple-roots-highlighted). The irreducible rank-two root systems A2, B2 and G2, with long and short roots and explicit ordered simple roots highlighted**.

## 4

↑ **Parent:** [Paper 63](paper-63.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) acts on the algebra itself: $\operatorname{ad}_X(Y)=[X,Y]$. In the basis $T_b$, its [matrices](../../../vector-space.md#matrix) are

$$
\boxed{(T_a^{\rm ad})^c{}_b=c^c{}_{ab}.}
$$

For any algebra element $X$, the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[T_a^{\rm ad},T_b^{\rm ad}]X=[T_a,[T_b,X]]-[T_b,[T_a,X]]=[[T_a,T_b],X].
$$

Therefore the $D\times D$ [matrices](../../../vector-space.md#matrix) satisfy the same [Lie bracket](../../../lie-algebra.md#lie-bracket) relations:

$$
\boxed{[T_a^{\rm ad},T_b^{\rm ad}]=c^c{}_{ab}T_c^{\rm ad}.}
$$

This construction does not require that the algebra be simple or that the adjoint action be faithful.

For the field calculation, write $A_\mu=A_\mu^aT_a$ and $\lambda=\lambda^aT_a$. In the derivative-plus-connection convention the [Yang-Mills field strength](../../../relativistic-quantum-field.md#gauge-field-strength) is

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\qquad
\delta A_\mu=\partial_\mu\lambda+[A_\mu,\lambda].
$$

The sign of the parameter here is the negative of the matter-field parameter in the usual [gauge transformation in the derivative-plus-connection convention](../../../relativistic-quantum-field.md#gauge-transformation-in-the-derivative-plus-connection-convention). Work with the stated $\lambda$ throughout. Expanding the variation gives

$$
\begin{aligned}
\delta F_{\mu\nu}={}&[\partial_\mu A_\nu-\partial_\nu A_\mu,\lambda]
+[A_\nu,\partial_\mu\lambda]-[A_\mu,\partial_\nu\lambda]\\
&+[\partial_\mu\lambda,A_\nu]+[A_\mu,\partial_\nu\lambda]
+[[A_\mu,\lambda],A_\nu]+[A_\mu,[A_\nu,\lambda]].
\end{aligned}
$$

The second derivatives cancel by commutativity of partial derivatives, and all remaining derivatives of $\lambda$ cancel by antisymmetry of the [Lie bracket](../../../lie-algebra.md#lie-bracket). The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) makes the last two terms $[[A_\mu,A_\nu],\lambda]$. Hence

$$
\boxed{\delta F_{\mu\nu}=[F_{\mu\nu},\lambda],\qquad
\delta F^a_{\mu\nu}=c^a{}_{bc}F^b_{\mu\nu}\lambda^c.}
$$

Unlike the connection, the curvature has no inhomogeneous derivative term: it transforms in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

The quadratic form $\kappa_{ab}=\operatorname{tr}(T_a^{\rm ad}T_b^{\rm ad})$ is the [Killing form](../../../lie-algebra.md#killing-form). Its symmetry follows from cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace). Using the just-proved adjoint commutators,

$$
\begin{aligned}
c^d{}_{ca}\kappa_{db}+c^d{}_{cb}\kappa_{ad}
&=\operatorname{tr}\left([T_c^{\rm ad},T_a^{\rm ad}]T_b^{\rm ad}
+T_a^{\rm ad}[T_c^{\rm ad},T_b^{\rm ad}]\right)\\
&=\operatorname{tr}[T_c^{\rm ad},T_a^{\rm ad}T_b^{\rm ad}]=0.
\end{aligned}
$$

Thus

$$
\boxed{c^d{}_{ca}\kappa_{db}+c^d{}_{cb}\kappa_{ad}=0.}
$$

Equivalently, each adjoint generator is skew with respect to this invariant bilinear form. This invariance holds even when the [Killing form](../../../lie-algebra.md#killing-form) is degenerate; no inverse form is needed here.

The spacetime metric used to raise Lorentz indices is unaffected by the internal [gauge transformation](../../../electromagnetism.md#gauge-transformation). Since $\delta F=-\operatorname{ad}_\lambda F$, invariance gives

$$
\begin{aligned}
\delta\bigl(\kappa_{ab}F^{a\mu\nu}F^b_{\mu\nu}\bigr)
&=\kappa(\delta F^{\mu\nu},F_{\mu\nu})+\kappa(F^{\mu\nu},\delta F_{\mu\nu})\\
&=-\lambda^c\left[c^d{}_{ca}\kappa_{db}+c^d{}_{cb}\kappa_{ad}\right]
F^{a\mu\nu}F^b_{\mu\nu}=0.
\end{aligned}
$$

Therefore **the Killing-form contraction of the field strengths is gauge invariant**, as required for the internal contraction in a [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
