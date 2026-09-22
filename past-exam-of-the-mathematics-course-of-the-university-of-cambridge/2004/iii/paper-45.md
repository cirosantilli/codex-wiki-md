# Paper 45

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper45.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper45.pdf)

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

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For the [addition of angular momentum](../../../quantum-mechanics.md#addition-of-angular-momentum), the uncoupled orthonormal [basis](../../../vector-space.md#basis) is $|j_1m_1\rangle\otimes|j_2m_2\rangle$, whereas the coupled orthonormal [basis](../../../vector-space.md#basis) diagonalizes $\mathbf J^2$ and $J_3$ for $\mathbf J=\mathbf J_1+\mathbf J_2$. Define the [Clebsch-Gordan coefficients](../../../representation-theory.md#clebsch-gordan-coefficients) by

$$
|JM\rangle=\sum_{m_1,m_2}C^{JM}_{m_1m_2}|j_1m_1\rangle|j_2m_2\rangle,\qquad
C^{JM}_{m_1m_2}=\langle j_1m_1,j_2m_2\mid JM\rangle.
$$

The [Clebsch-Gordan decomposition](../../../quantum-mechanics.md#clebsch-gordan-decomposition) allows $|j_1-j_2|\leq J\leq j_1+j_2$ in unit steps, and a coefficient vanishes unless $m_1+m_2=M$. Taking the inner product of the expansion with itself proves

$$
\sum_{m_1,m_2}|C^{JM}_{m_1m_2}|^2=\langle JM|JM\rangle=1.
$$

With the customary real phase convention the modulus signs can be omitted, giving the sum of squares used in the question. In an arbitrary phase convention the modulus-square identity is the invariant statement.

Treat the [strong interaction](../../../standard-model.md#strong-interaction) as exactly [isospin](../../../standard-model.md#isospin)-invariant for this calculation. Its transition operator $T$ commutes with the three [isospin](../../../standard-model.md#isospin) generators and hence with their [quadratic Casimir operator](../../../semisimple-lie-algebra.md#quadratic-casimir-operator). Acting on the initial state $|IM\rangle$, it can therefore produce only final states with the same $I$ and $M$. The [tensor product representation](../../../representation-theory.md#tensor-product-of-group-representations) of final multiplets $I_1,I_2$ contains one copy of each permitted total [isospin](../../../standard-model.md#isospin), so $T|IM\rangle=a_M|(I_1I_2)IM\rangle$. Commuting $T$ with the lowering operator gives

$$
a_M\sqrt{(I+M)(I-M+1)}=a_{M-1}\sqrt{(I+M)(I-M+1)}.
$$

Every connecting ladder factor is nonzero, so all $a_M$ coincide with one reduced coefficient $a$. Expanding the final coupled state now gives the [isospin-invariant two-body decay amplitude](../../../standard-model.md#isospin-invariant-two-body-decay-amplitude)

$$
\boxed{A_{M_1M_2;M}=a\,\langle I_1M_1,I_2M_2\mid IM\rangle.}
$$

The reduced coefficient may depend on the particle species, momenta and [spin](../../../quantum-mechanics.md#spin) channel, but not on the three [isospin](../../../standard-model.md#isospin) projections. Summing the squared amplitude over the orthogonal charge channels gives

$$
\boxed{\sum_{M_1,M_2}|A_{M_1M_2;M}|^2=|a|^2.}
$$

A physical [decay rate](../../../relativistic-quantum-field.md#decay-width) also includes phase space, angular integration and any [spin](../../../quantum-mechanics.md#spin) sums. In the [isospin](../../../standard-model.md#isospin)-degenerate limit these factors are common to the charge channels; absorbing their square root into $a$ gives $\Gamma_{IM}=|a|^2$ for this specified two-body multiplet channel. If several distinct species or independent [spin](../../../quantum-mechanics.md#spin) channels are included in “anything”, their reduced rates must additionally be summed. There is no extra factor $2I+1$ when the initial magnetic component is fixed.

The [Delta baryon](../../../physics.md#delta-baryon) states have $I=3/2$ and projections $3/2,1/2,-1/2,-3/2$ for $\Delta^{++},\Delta^+,\Delta^0,\Delta^-$. The [proton](../../../physics.md#proton) and [neutron](../../../physics.md#neutron) form $I=1/2$, with projections $+1/2,-1/2$, and the [pion](../../../standard-model.md#pion) triplet has $I=1$ with projections $+1,0,-1$. The highest coupled state is

$$
|3/2,3/2\rangle=|p\pi^+\rangle.
$$

Apply the total lowering operator $I_-=I_-^{(N)}+I_-^{(\pi)}$. Its coefficient on the left is $\sqrt3$, while on the right the nucleon and [pion](../../../standard-model.md#pion) coefficients are $1$ and $\sqrt2$:

$$
\sqrt3\,|3/2,1/2\rangle=|n\pi^+\rangle+\sqrt2\,|p\pi^0\rangle.
$$

The squared [Clebsch-Gordan coefficients](../../../representation-theory.md#clebsch-gordan-coefficients) are consequently $1/3$ and $2/3$, compared with coefficient one for the $\Delta^{++}$ channel. Thus the [Delta baryon pion branching ratios](../../../physics.md#delta-baryon-pion-branching-ratios) are

$$
\boxed{\frac{\Gamma(\Delta^+\to p\pi^0)}{\Gamma(\Delta^{++}\to p\pi^+)}=\frac23,\qquad
\frac{\Gamma(\Delta^+\to n\pi^+)}{\Gamma(\Delta^{++}\to p\pi^+)}=\frac13.}
$$

At the opposite end of the same [isospin multiplet](../../../standard-model.md#isospin-multiplet), $|3/2,-3/2\rangle=|n\pi^-\rangle$, so **the strong decay is $\Delta^-\to n\pi^-$**, with the same reduced rate in this symmetry limit. Physical mass splittings and electromagnetic effects perturb these idealized equal-kinematics ratios.

## 2

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $V=\mathbb C^3$ be the defining flavor [SU(3)](../../../topological-group.md#su-3-group) [representation](../../../representation-theory.md#group-representation). Under $U\in SU(3)$, $q^\alpha\mapsto U^\alpha{}_{\beta}q^\beta$. The [antiquark](../../../standard-model.md#antiquark) transforms in the [dual representation](../../../representation-theory.md#dual-representation):

$$
\bar q_\alpha\mapsto (U^{-1})^\beta{}_{\alpha}\bar q_\beta.
$$

Since $U$ is unitary, its lower-index column of components transforms by $U^*$, the complex conjugate numerical matrix. Thus $q^\alpha\bar q_\alpha$ is invariant. The defining triplet and its conjugate are inequivalent complex [representations](../../../representation-theory.md#group-representation); conjugation reverses their [weights](../../../semisimple-lie-algebra.md#weight-representation-theory). Write $\mathbf3=V$ and $\overline{\mathbf3}=V^*$, and distinguish a [direct sum](../../../vector-space.md#direct-sum) $\oplus$ from a [tensor product](../../../linear-algebra.md#tensor-product) $\otimes$.

First split $V\otimes V$ into [symmetric tensors](../../../linear-algebra.md#symmetric-tensor) and [totally antisymmetric tensors](../../../linear-algebra.md#totally-antisymmetric-tensor):

$$
V\otimes V=\operatorname{Sym}^2V\oplus\Lambda^2V.
$$

The symmetric part has dimension $3(3+1)/2=6$. Contracting the antisymmetric part with the invariant [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) gives $A_\gamma=\tfrac12\epsilon_{\gamma\alpha\beta}A^{\alpha\beta}$, which transforms as a dual vector because $\det U=1$. Its inverse is $A^{\alpha\beta}=\epsilon^{\alpha\beta\gamma}A_\gamma$. Hence

$$
\boxed{\mathbf3\otimes\mathbf3=\overline{\mathbf3}\oplus\mathbf6.}
$$

The symmetric part is the irreducible [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation) with [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) $(2,0)$; its six monomials give the standard symmetric-square [representation](../../../representation-theory.md#group-representation).

For three triplets, the antisymmetric first-pair sector becomes $V^*\otimes V$. Its [tensors](../../../linear-algebra.md#tensor) $M^\alpha{}_{\beta}$ split into their scalar trace and traceless part:

$$
V^*\otimes V=\mathbf1\oplus\mathbf8,\qquad
M=\frac{\operatorname{tr}M}{3}\mathbf1+\left(M-\frac{\operatorname{tr}M}{3}\mathbf1\right).
$$

The traceless part is the [adjoint representation of SU(3)](../../../lie-algebra.md#adjoint-representation-of-su-3); conjugation acts as $M\mapsto UMU^{-1}$. It is irreducible because an invariant subspace would be an ideal in the simple complex [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}_3$.

The symmetric first-pair sector consists of $T^{abc}=T^{bac}$ and has dimension $6\cdot3=18$. Complete symmetrization maps it onto $\operatorname{Sym}^3V$, whose dimension is $\binom53=10$. Its kernel is the mixed-symmetry eight-dimensional sector. More explicitly, the equivariant map $T^{abc}\mapsto M^a{}_e=\epsilon_{ebc}T^{abc}$ has trace zero because the first two indices of $T$ are symmetric; it annihilates the completely symmetric part and is not identically zero. Since the target adjoint module is irreducible, the map is onto its eight-dimensional space. Its kernel is consequently exactly the ten-dimensional completely symmetric part. Complete symmetrization supplies an invariant splitting, so this sector is $\mathbf{10}\oplus\mathbf8$. Combining the sectors gives the [tensor cube of the defining SU(3) representation](../../../semisimple-lie-algebra.md#tensor-cube-of-the-defining-su-3-representation)

$$
\boxed{\mathbf3^{\otimes3}=\mathbf1\oplus\mathbf8\oplus\mathbf8\oplus\mathbf{10}.}
$$

Here the decuplet has [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) $(3,0)$, and the singlet is the fully antisymmetric contraction $\epsilon_{abc}T^{abc}$. The two octets are distinct copies, not two different irreducible types.

For [two conjugate SU(3) triplets with a triplet](../../../semisimple-lie-algebra.md#two-conjugate-su-3-triplets-with-a-triplet), begin with $T^a{}_{bc}$ and split its lower pair. An antisymmetric lower pair is identified by $\epsilon^{bcd}$ with an upper index, giving $V\otimes V=\mathbf6\oplus\overline{\mathbf3}$. The symmetric lower-pair sector has dimension $3\cdot6=18$, and its contraction is the equivariant map

$$
C(T)_b=\sum_aT^a{}_{ba}.
$$

It is onto $V^*$, since the invariant embedding

$$
\iota(v)^a{}_{bc}=\frac14(\delta^a_bv_c+\delta^a_cv_b)
$$

satisfies $C\iota(v)=v$. Every such [tensor](../../../linear-algebra.md#tensor) therefore splits uniquely as $\iota(C(T))+(T-\iota(C(T)))$. The latter [tensor](../../../linear-algebra.md#tensor) is symmetric in its lower indices and has zero contraction, with dimension $18-3=15$. It contains the [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) $e_1\otimes(e_3^*)^2$ of [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) $(1,2)$; contraction vanishes because its upper and lower indices differ. The [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) for an [SU(3)](../../../topological-group.md#su-3-group) module with labels $(p,q)$ is $\dim V_{(p,q)}=(p+1)(q+1)(p+q+2)/2$, which gives $15$ for $(1,2)$. These [tensor](../../../linear-algebra.md#tensor) [representations](../../../representation-theory.md#group-representation) are unitary, so invariant subspaces have invariant orthogonal complements; the irreducible highest-[weight](../../../semisimple-lie-algebra.md#weight-representation-theory) summand containing this vector exhausts the fifteen-dimensional kernel. Thus

$$
\boxed{\overline{\mathbf3}\otimes\overline{\mathbf3}\otimes\mathbf3
=\overline{\mathbf3}\oplus\overline{\mathbf3}\oplus\mathbf6\oplus V_{(1,2)}.}
$$

The question's dimension label $15$ denotes $V_{(1,2)}$, rather than its conjugate $V_{(2,1)}$; they have equal dimensions but different [tensors](../../../linear-algebra.md#tensor). Conjugating the triplet-cube decomposition gives

$$
\boxed{\overline{\mathbf3}^{\otimes3}=\mathbf1\oplus\mathbf8\oplus\mathbf8\oplus\overline{\mathbf{10}}.}
$$

The octet is self-conjugate, whereas the symmetric decuplet changes $(3,0)$ to $(0,3)$.

Now consider the flavor [diquark](../../../physics.md#diquark) $D_\alpha\propto\epsilon_{\alpha\beta\gamma}q^\beta q^\gamma$. This notation describes an antisymmetric two-[quark](../../../standard-model.md#quark) flavor state; color and [spin](../../../quantum-mechanics.md#spin) factors are separate. In particular $D_3=(ud-du)/\sqrt2$ has [isospin](../../../standard-model.md#isospin) zero, [baryon number](../../../standard-model.md#baryon-number) $2/3$, [strangeness](../../../standard-model.md#strangeness) zero and [flavor hypercharge](../../../standard-model.md#flavor-hypercharge) $2/3$. The strange [antiquark](../../../standard-model.md#antiquark) has $I=0$, $B=-1/3$, $S=+1$ and $Y=2/3$. Thus $D_3D_3\bar s$ has

$$
\boxed{B=1,\qquad S=+1,\qquad Y=2,\qquad I=0,\qquad Q=+1.}
$$

The charge follows from the [Gell-Mann--Nishijima formula](../../../standard-model.md#gell-mann-nishijima-formula). Each of the three factors has lower flavor index $3$, so their product is the completely symmetric [tensor](../../../linear-algebra.md#tensor) component $A_{333}$. It lies entirely in $\operatorname{Sym}^3V^*=\overline{\mathbf{10}}$, the [pentaquark antidecuplet](../../../physics.md#pentaquark-antidecuplet). Equivalently, the symmetric diquark pair belongs to $\overline{\mathbf6}$, and $\overline{\mathbf6}\otimes\overline{\mathbf3}=\overline{\mathbf{10}}\oplus\mathbf8$, with this highest-hypercharge state in the antidecuplet.

It cannot be in an octet. The octet has the [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) of a traceless $q^\alpha\bar q_\beta$ [tensor](../../../linear-algebra.md#tensor), whose hypercharges are $Y_\alpha-Y_\beta$. For $(u,d,s)$ the [quark](../../../standard-model.md#quark) values are $1/3,1/3,-2/3$, so these differences are only $0,+1,-1$; there is no $Y=2$ [weight](../../../semisimple-lie-algebra.md#weight-representation-theory). The octet's top row instead has $Y=1$ and $I=1/2$. This is a flavor-[representation](../../../representation-theory.md#group-representation) assignment for a possible [pentaquark](../../../physics.md#pentaquark), not a proof that the configuration binds or that its full color-[spin](../../../quantum-mechanics.md#spin)-orbital wavefunction satisfies all [Fermi statistics](../../../quantum-mechanics.md#fermi-dirac-statistics) constraints.

## 3

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In the two-body centre-of-mass frame, [spatial reflection](../../../quantum-mechanics.md#spatial-reflection) reverses the relative coordinate of a [quark](../../../standard-model.md#quark)-[antiquark](../../../standard-model.md#antiquark) pair. Its orbital state of angular momentum $L$ has [orbital parity](../../../quantum-mechanics.md#orbital-parity) $(-1)^L$, as follows from $Y_{Lm}(-\widehat{\mathbf r})=(-1)^LY_{Lm}(\widehat{\mathbf r})$. Opposite constituent [intrinsic parities](../../../quantum-field-theory.md#intrinsic-parity) multiply to minus one. Thus the [meson parity and charge conjugation](../../../physics.md#meson-parity-and-charge-conjugation) rules begin with

$$
\boxed{P=\eta_q\eta_{\bar q}(-1)^L=(-1)^{L+1}.}
$$

To obtain [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), consider a self-conjugate flavor state and write its [spin](../../../quantum-mechanics.md#spin)-orbital wavefunction using ordered [creation operators](../../../quantum-mechanics.md#creation-operator) $b_\sigma^\dagger(\mathbf p)d_\tau^\dagger(-\mathbf p)$. [Charge conjugation](../../../quantum-field-theory.md#charge-conjugation) interchanges the [quark](../../../standard-model.md#quark) and [antiquark](../../../standard-model.md#antiquark) operators. Reordering them back to [quark](../../../standard-model.md#quark)-first order produces a [fermionic sign](../../../perturbative-quantum-field-theory.md#fermionic-sign) minus one. Interchanging the two [spin](../../../quantum-mechanics.md#spin)-$1/2$ labels has eigenvalue $-1$ in the [spin singlet state](../../../bell-state.md#spin-singlet-state) ($S=0$) and $+1$ in the [spin](../../../quantum-mechanics.md#spin) triplet ($S=1$), namely $(-1)^{S+1}$. Reversing the relative momentum contributes $(-1)^L$. Therefore

$$
\boxed{C=-(-1)^{S+1}(-1)^L=(-1)^{L+S}.}
$$

Reciprocal phases for the two conjugate [creation operators](../../../quantum-mechanics.md#creation-operator) cancel, so the result is independent of that convention. This applies to a state that is mapped to itself by [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), not to every electrically neutral flavor state. For example a neutral [meson](../../../physics.md#meson) with unequal [quark](../../../standard-model.md#quark) and [antiquark](../../../standard-model.md#antiquark) flavors can be exchanged with a different antimeson. Charged states have no individual $C$ eigenvalue.

Restrict flavor to the $u,d$ [isospin](../../../standard-model.md#isospin) doublet. Its product with the conjugate doublet decomposes as $\mathbf2\otimes\overline{\mathbf2}=\mathbf3\oplus\mathbf1$. Convenient normalized flavor states, with irrelevant overall phase choices, are

$$
|1,+1\rangle=u\bar d,\quad |1,0\rangle=\frac{u\bar u-d\bar d}{\sqrt2},\quad |1,-1\rangle=d\bar u,\quad
|0,0\rangle=\frac{u\bar u+d\bar d}{\sqrt2}.
$$

Orbital excitation normally costs energy, so the simplest low-lying [quark model](../../../physics.md#quark-model) states have $L=0$. Coupling the two constituent spins gives $S=0$ or $S=1$, and then $J=S$. The isotriplet with $S=0$ is the [pion](../../../standard-model.md#pion) triplet, while the isotriplet with $S=1$ is the [rho meson](../../../physics.md#rho-meson) triplet. The isosinglet with $S=1$ is the nonstrange component of the [omega meson](../../../physics.md#omega-meson). Their quantum numbers are

$$
\boxed{\pi^0:\ I=1,\ J^{PC}=0^{-+};\qquad
\rho^0:\ I=1,\ J^{PC}=1^{--};\qquad
\omega:\ I=0,\ J^{PC}=1^{--}.}
$$

The charged [pions](../../../standard-model.md#pion) have $J^P=0^-$ and the charged rho [mesons](../../../physics.md#meson) have $J^P=1^-$; [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) exchanges the positive and negative members. The same [tensor](../../../linear-algebra.md#tensor) product also allows an $S=0$, $I=0$ pseudoscalar state, so symmetry alone does not assert that only the listed [mesons](../../../physics.md#meson) exist or predict their masses. The physical isosinglet spectrum involves further dynamics and, when strange flavor is included, mixing.

For a vector-[meson](../../../physics.md#meson) decay to two spinless [pions](../../../standard-model.md#pion), conservation of [angular momentum](../../../classical-mechanics.md#angular-momentum) forces their relative orbital value to be $L=1$. Their combined [parity](../../../quantum-mechanics.md#parity) is $(-1)^2(-1)^L=-1$, and the neutral charge combination has $C=(-1)^L=-1$, matching both $\rho^0$ and $\omega$. Thus $C$ and $P$ alone do not distinguish these two decays. The decisive restriction is [isospin](../../../standard-model.md#isospin) together with [Bose statistics](../../../statistical-physics.md#bose-einstein-statistics).

Two isotriplet [pions](../../../standard-model.md#pion) have $\mathbf3\otimes\mathbf3=\mathbf1\oplus\mathbf3\oplus\mathbf5$, or total $I=0,1,2$. Under exchange the [isospin](../../../standard-model.md#isospin)-$I$ state has sign $(-1)^{2-I}$: the $I=2$ highest state and its lowered partners are symmetric, the $I=1$ highest combination $(|+0\rangle-|0+\rangle)/\sqrt2$ is antisymmetric, and the singlet $(|+-\rangle+|-+\rangle-|00\rangle)/\sqrt3$ is symmetric. The $L=1$ orbital state is antisymmetric. Since [pions](../../../standard-model.md#pion) are [spin](../../../quantum-mechanics.md#spin)-zero [bosons](../../../quantum-mechanics.md#boson), their total state must be symmetric, requiring the antisymmetric [isospin](../../../standard-model.md#isospin) sector $I=1$. This allows $\rho^0\to\pi^+\pi^-$ but excludes an [isospin](../../../standard-model.md#isospin)-conserving $\omega\to\pi^+\pi^-$ amplitude.

There is no analogous obstruction for three [pions](../../../standard-model.md#pion). In a Cartesian [isospin](../../../standard-model.md#isospin) basis $a,b,c$, their totally antisymmetric combination $\epsilon_{abc}|\pi^a\pi^b\pi^c\rangle$ is an $I=0$ state. It can multiply a totally antisymmetric momentum amplitude proportional in the rest frame to

$$
\boldsymbol\epsilon_\omega\cdot(\mathbf p_1\times\mathbf p_2).
$$

Momentum conservation $\mathbf p_1+\mathbf p_2+\mathbf p_3=0$ makes this amplitude change sign under every exchange of two [pion](../../../standard-model.md#pion) labels. The product of the flavor and momentum factors therefore obeys [Bose statistics](../../../statistical-physics.md#bose-einstein-statistics). The cross product supplies $J=1$ and an even [orbital parity](../../../quantum-mechanics.md#orbital-parity); multiplying by the three negative [pion](../../../standard-model.md#pion) [intrinsic parities](../../../quantum-field-theory.md#intrinsic-parity) gives total $P=-1$. In the charged component, [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) exchanges $\pi^+$ and $\pi^-$ and changes the momentum factor's sign, giving $C=-1$. Thus **$\omega\to\pi^+\pi^-\pi^0$ is compatible with $I=0$ and $J^{PC}=1^{--}$**.

The same distinction is encoded in [G parity](../../../standard-model.md#g-parity): $G=C(-1)^I$ for the neutral member gives $G_\pi=-1$, $G_\rho=+1$, $G_\omega=-1$. An $n$-[pion](../../../standard-model.md#pion) state has $G=(-1)^n$, so the [G-parity selection rule for pion multiplicities](../../../standard-model.md#g-parity-selection-rule-for-pion-multiplicities) allows two [pions](../../../standard-model.md#pion) for the rho and three for the omega. The printed prohibition of the omega two-[pion](../../../standard-model.md#pion) mode is an exact-[isospin](../../../standard-model.md#isospin) strong-interaction selection rule. In the physical theory, [isospin](../../../standard-model.md#isospin)-breaking effects allow a small two-[pion](../../../standard-model.md#pion) mode; it is not an absolute prohibition. The scope of C [parity](../../../quantum-mechanics.md#parity) is also stated in the [Particle Data Group quark-model review](https://pdg.lbl.gov/2024/reviews/rpp2024-rev-quark-model.pdf), and the physical two-[pion](../../../standard-model.md#pion) mode is recorded in its [omega listing](https://pdg.lbl.gov/2024/listings/rpp2024-list-omega-782.pdf).

## 4

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In the finite-dimensional complex [semisimple Lie algebra](../../../semisimple-lie-algebra.md) setting, the [rank of a semisimple Lie algebra](../../../semisimple-lie-algebra.md#rank-of-a-semisimple-lie-algebra) is the dimension of a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) $\mathfrak h$, equivalently the number of independent commuting Cartan generators. For a compact real algebra, use its complexification and the corresponding maximal torus. Simultaneously diagonalizing the commuting adjoint actions of $\mathfrak h$ gives the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
\mathcal L=\mathfrak h\oplus\bigoplus_{\alpha\ne0}\mathcal L_\alpha,\qquad
\mathcal L_\alpha=\{X:[H,X]=\alpha(H)X\text{ for every }H\in\mathfrak h\}.
$$

The nonzero linear functionals $\alpha$ for which this space is nonzero are the [roots of a root system](../../../semisimple-lie-algebra.md#root-of-a-root-system). An invariant inner product identifies them with vectors in a real Euclidean root space. These are the usual semisimple assumptions behind the rank and root language here.

The displayed generators $H,E^+,E^-$ form an [sl2 triple](../../../semisimple-lie-algebra.md#sl2-triple). Start with a nonzero lowest-[weight](../../../semisimple-lie-algebra.md#weight-representation-theory) element $X_0$ and define $X_{n+1}=[E^+,X_n]$. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[H,X_{n+1}]=[[H,E^+],X_n]+[E^+,[H,X_n]].
$$

Induction starting with $[H,X_0]=-\lambda X_0$ consequently gives the [finite sl2 lowest-weight ladder](../../../semisimple-lie-algebra.md#finite-sl2-lowest-weight-ladder) [weights](../../../semisimple-lie-algebra.md#weight-representation-theory)

$$
\boxed{[H,X_n]=(2n-\lambda)X_n.}
$$

Now commute the lowering equation with $E^+$ and again use the [Jacobi identity](../../../lie-algebra.md#jacobi-identity):

$$
[E^+,[E^-,X_n]]=[[E^+,E^-],X_n]+[E^-,[E^+,X_n]]
=(2n-\lambda)X_n+q_{n+1}X_n.
$$

The left side is $q_nX_n$. Whenever $X_n\ne0$, coefficient comparison gives

$$
\boxed{q_{n+1}=q_n+\lambda-2n.}
$$

The initial condition is $q_0=0$, meaning $[E^-,X_0]=0$; directly $[E^-,X_1]=[-H,X_0]=\lambda X_0$, so $q_1=\lambda$. Summing the recurrence from $0$ to $n-1$ yields

$$
\boxed{q_n=n\lambda-2\sum_{k=0}^{n-1}k=n(\lambda-n+1).}
$$

In fact the vector identity $[E^-,X_n]=n(\lambda-n+1)X_{n-1}$ follows inductively from the same [Jacobi identity](../../../lie-algebra.md#jacobi-identity) without needing a separately assumed lowering coefficient.

If $X_{n_0}$ is the last nonzero element and $[E^+,X_{n_0}]=0$, apply $E^-$ to this zero next element. The lowering identity gives

$$
0=[E^-,X_{n_0+1}]=(n_0+1)(\lambda-n_0)X_{n_0},
$$

so **$\lambda=n_0$**, a nonnegative [integer](../../../number-theory.md#integer). The nonzero endpoint is necessary. Literally allowing $X_{n_0}=0$ would make the printed conclusion false: take $X_0=E^-$ in the adjoint [representation](../../../representation-theory.md#group-representation) of $\mathfrak{sl}_2$. Then $\lambda=2$, $X_1=H$, $X_2=-2E^+$, $X_3=0$. Choosing $n_0=3$ gives a vanishing next bracket but not $\lambda=3$. The intended endpoint is the first terminating bracket after the nonzero ladder.

For the plus-sign nested [commutators](../../../lie-algebra.md#commutator), use $H=H_1$, $E^\pm=E_1^\pm$ and $X_0=E_2^+$. The cross relation gives $[E_1^-,E_2^+]=0$, while $[H_1,E_2^+]=K_{21}E_2^+$. Thus the lowest-[weight](../../../semisimple-lie-algebra.md#weight-representation-theory) label is $\lambda=-K_{21}$. If the $n$-fold raised element is nonzero and the $(n+1)$-fold element vanishes, the preceding endpoint argument gives $\lambda=n$ and hence

$$
\boxed{K_{21}=-n.}
$$

For the minus-sign ladder, use the [sl2 triple](../../../semisimple-lie-algebra.md#sl2-triple) $H'=-H_1$, $E'^+=E_1^-$, $E'^-=E_1^+$ and start at $X_0=E_2^-$. Its lowest-[weight](../../../semisimple-lie-algebra.md#weight-representation-theory) equation is again $[H',X_0]=K_{21}X_0$, and its lowering bracket vanishes by the cross relation. The same argument proves exactly the same result, including the endpoint assumption that is explicit in the nested-[commutator](../../../lie-algebra.md#commutator) question.

For arbitrary [roots of a root system](../../../semisimple-lie-algebra.md#root-of-a-root-system) $\alpha,\beta$, choose the normalized [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root) $\beta$, whose generators obey $[H_\beta,E_\beta^\pm]=\pm2E_\beta^\pm$ and $[E_\beta^+,E_\beta^-]=H_\beta$. The [coroot](../../../semisimple-lie-algebra.md#coroot) normalization gives

$$
\alpha(H_\beta)=\frac{2\alpha\cdot\beta}{\beta\cdot\beta}.
$$

The normalization has a concrete construction. Use the nondegenerate [Killing form](../../../lie-algebra.md#killing-form) $B$, and define $t_\beta\in\mathfrak h$ by $B(t_\beta,H)=\beta(H)$. Invariance makes root spaces orthogonal unless their roots sum to zero, so there exist $e\in\mathcal L_\beta$ and $f\in\mathcal L_{-\beta}$ with $B(e,f)=1$. Invariance then gives $B([e,f],H)=B(e,[f,H])=\beta(H)$, hence $[e,f]=t_\beta$. With $(\beta,\beta)=\beta(t_\beta)$, take $E_\beta^+=e$, $E_\beta^-=2f/(\beta,\beta)$ and $H_\beta=2t_\beta/(\beta,\beta)$. Their brackets have the required normalization and $\alpha(H_\beta)=2(\alpha,\beta)/(\beta,\beta)$. Let $v$ be a nonzero $\alpha$ [root vector](../../../semisimple-lie-algebra.md#root-vector) with $H_\beta$ [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $w=\alpha(H_\beta)$. Repeatedly apply $\operatorname{ad}E_\beta^-$ until reaching a last nonzero vector $v_0=(\operatorname{ad}E_\beta^-)^pv$. Its [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) is $w-2p$. This process terminates because different [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) are linearly independent and the [Lie algebra](../../../lie-algebra.md) is finite-dimensional. Starting at $v_0$, repeatedly raise; this also terminates for the same reason. The proven lowest-[weight](../../../semisimple-lie-algebra.md#weight-representation-theory) endpoint formula says $w-2p=-N$ for a nonnegative integer $N$. Therefore

$$
\boxed{\frac{2\alpha\cdot\beta}{\beta^2}=w=2p-N\in\mathbb Z.}
$$

This proves integrality of [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) directly from the finite ladder, rather than assuming the crystallographic axiom.

Finally use the indices actually printed in the PDF: $E_1^+=R^1{}_2$, $E_2^+=R^2{}_3$, $E_1^-=R^2{}_1$, $E_2^-=R^3{}_2$. The converted TeX has corrupted these indices. The prescribed bracket is that of trace-free [matrix units](../../../vector-space.md#matrix-unit). The sum of the diagonal generators is zero, leaving two independent diagonal elements, and their pair brackets give

$$
\boxed{H_1=R^1{}_1-R^2{}_2,\qquad H_2=R^2{}_2-R^3{}_3.}
$$

For example $[R^1{}_2,R^2{}_1]=R^1{}_1-R^2{}_2$, and the analogous second pair gives $H_2$. The cross raising-lowering brackets vanish. A diagonal $H$ with entries $h_r$ has $[H,R^r{}_s]=(h_r-h_s)R^r{}_s$. Thus $H_1$ acts on $E_1^+,E_2^+$ with [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $2,-1$, and $H_2$ acts on them with [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $-1,2$. The negative generators have the opposite [weights](../../../semisimple-lie-algebra.md#weight-representation-theory). In the question's index ordering,

$$
\boxed{(K_{ji})=\begin{pmatrix}2&-1\\-1&2\end{pmatrix}.}
$$

This is the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) of the [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system), and the [Lie algebra](../../../lie-algebra.md) generated by these matrix units has rank two. As an additional bracket check, $[E_1^+,E_2^+]=R^1{}_3\ne0$ whereas $[E_1^+,R^1{}_3]=0$, so the nested ladder has $n=1$ and indeed $K_{21}=-1$. The negative ladder likewise terminates after one nonzero bracket.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
