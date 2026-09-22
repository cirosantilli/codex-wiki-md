# Paper 48

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_48.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_48.pdf)

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

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Set $\hbar=1$ and let $N=2I\in\mathbb Z_{\geq0}$. A concrete [irreducible spin representation](../../../quantum-mechanics.md#irreducible-spin-representation) is the [symmetric power](../../../linear-algebra.md#symmetric-power)

$$
\mathcal H_I=\operatorname{Sym}^{N}\mathbb C^2.
$$

Start with $N$ copies of the defining [SU(2)](../../../topological-group.md#su-2-group) doublet and restrict their [tensor product representation](../../../representation-theory.md#tensor-product-of-group-representations) to the completely symmetric subspace. Its orthonormal basis consists of symmetric states with $I+m$ up components and $I-m$ down components, where $m=I,I-1,\ldots,-I$. There are $N+1=2I+1$ such states. The total generators are $J_i=\sum_{a=1}^N\sigma_i^{(a)}/2$, acting on this subspace, where $\sigma_i$ are the [Pauli matrices](../../../algebra.md#pauli-matrices). This also constructs the trivial representation when $I=0$.

The [spin ladder operators](../../../quantum-mechanics.md#spin-ladder-operator) $J_\pm=J_1\pm iJ_2$ satisfy

$$
[J_3,J_\pm]=\pm J_\pm,\qquad [J_+,J_-]=2J_3.
$$

The [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) $J^2=\sum_iJ_i^2$ commutes with every generator. On the [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) $|I,I\rangle$, the identity $J^2=J_-J_++J_3(J_3+1)$ gives its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $I(I+1)$. With phases chosen to make the lowering coefficients positive,

$$
\boxed{J_-|I,m\rangle=\sqrt{(I+m)(I-m+1)}\,|I,m-1\rangle,}
$$



$$
J_+|I,m\rangle=\sqrt{(I-m)(I+m+1)}\,|I,m+1\rangle.
$$

The squared [norm](../../../functional-analysis.md#norm) of the lowered state follows from $J_+J_-=J^2-J_3(J_3-1)$. The ladder stops exactly at $m=-I$. Every weight is connected to every other by these operators, and $J_3$ has distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Hence any [invariant subspace](../../../representation-theory.md#invariant-subspace) contains a weight vector and then the whole ladder: the representation is irreducible.

For $k=I-m$, successive lowering has squared [norm](../../../functional-analysis.md#norm)

$$
\prod_{r=0}^{k-1}(2I-r)(r+1)=\frac{(2I)!k!}{(2I-k)!}.
$$

Thus the [normalized highest-weight lowering formula](../../../quantum-mechanics.md#normalized-highest-weight-lowering-formula) is

$$
\boxed{|I,m\rangle=\sqrt{\frac{(I+m)!}{(2I)!(I-m)!}}\,(J_-)^{I-m}|I,I\rangle.}
$$

All factorial arguments are nonnegative integers, including for half-integral $I$.

The [unitary representation](../../../representation-theory.md#unitary-representation) of an [isospin rotation](../../../standard-model.md#isorotation) is

$$
\boxed{U[R(\theta,\mathbf n)]=e^{-i\theta\mathbf n\cdot\mathbf J}.}
$$

Its [matrix](../../../vector-space.md#matrix) in the weight basis is $D^{(I)}_{m'm}(R)=\langle I,m'|U[R]|I,m\rangle$. Insert the completeness relation between two operators to obtain

$$
D^{(I)}(g_1g_2)=D^{(I)}(g_1)D^{(I)}(g_2),\quad
D^{(I)}(1)=I,\quad D^{(I)}(g^{-1})=D^{(I)}(g)^\dagger.
$$

These verify the [group representation](../../../representation-theory.md#group-representation) and unitarity properties, and the ladder argument gives irreducibility. Here rotations carry their [SU(2)](../../../topological-group.md#su-2-group) lifts: $U(2\pi)=(-1)^{2I}I$. Integer $I$ descends to the ordinary [SO(3) group](../../../linear-algebra.md#so-3-group); half-integral $I$ is a representation of its double cover, not a single-valued representation of $SO(3)$.

For $I=1$, order the basis as $(|1,1\rangle,|1,0\rangle,|1,-1\rangle)$. The lowering and raising coefficients give the [spin-one half-turn matrix](../../../quantum-mechanics.md#spin-one-half-turn-matrix)

$$
J_2^{(1)}=\frac1{\sqrt2}\begin{pmatrix}0&-i&0\\i&0&-i\\0&i&0\end{pmatrix},\qquad
(J_2^{(1)})^2=\frac12\begin{pmatrix}1&0&-1\\0&2&0\\-1&0&1\end{pmatrix}.
$$

Multiplication shows $(J_2^{(1)})^3=J_2^{(1)}$. Reduce the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) using this identity:

$$
e^{-i\theta J_2}=I-i\sin\theta\,J_2+(\cos\theta-1)J_2^2.
$$

At $\theta=\pi$ it becomes

$$
\boxed{e^{-i\pi J_2}=\begin{pmatrix}0&0&1\\0&-1&0\\1&0&0\end{pmatrix},\qquad
e^{-i\pi J_2}|1,m\rangle=-(-1)^m|1,-m\rangle.}
$$

Thus its [matrix](../../../vector-space.md#matrix) elements are $-(-1)^m\delta_{m',-m}$. In the [pion](../../../standard-model.md#pion) phases $|\pi^\pm\rangle=|1,\pm1\rangle$, $|\pi^0\rangle=|1,0\rangle$, this [isospin rotation](../../../standard-model.md#isorotation) exchanges the two charged states with positive coefficients and negates the neutral state.

[Charge conjugation](../../../quantum-field-theory.md#charge-conjugation) is linear and unitary here. Similarity preserves [commutators](../../../lie-algebra.md#commutator), so

$$
[\mathcal CJ_i\mathcal C^{-1},\mathcal CJ_j\mathcal C^{-1}]
=\mathcal C[J_i,J_j]\mathcal C^{-1}
=i\epsilon_{ijk}\mathcal CJ_k\mathcal C^{-1}.
$$

Consequently the conjugated generators obey the same [Lie algebra](../../../lie-algebra.md). The specified signs also give $\mathcal CJ_\pm\mathcal C^{-1}=-J_\mp$. Since $|\pi^\pm\rangle=J_\pm|\pi^0\rangle/\sqrt2$ and the neutral state has positive [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) [eigenvalue](../../../linear-operator-theory.md#eigenvalue),

$$
\boxed{\mathcal C|\pi^\pm\rangle=-|\pi^\mp\rangle.}
$$

The signs depend on the chosen charged-state phases, which have been fixed by the ladder convention.

Conjugation by $R_\pi=e^{-i\pi J_2}$ changes $(J_1,J_2,J_3)$ to $(-J_1,J_2,-J_3)$, exactly as [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) does. Their product, the [G parity](../../../standard-model.md#g-parity) operator, therefore satisfies

$$
GJ_iG^{-1}=\mathcal C(R_\pi J_iR_\pi^{-1})\mathcal C^{-1}=J_i.
$$

The [Schur lemma](../../../representation-theory.md#schur-s-lemma) makes $G$ scalar on each irreducible [isospin](../../../standard-model.md#isospin) multiplet, hence independent of $m$. On the neutral [pion](../../../standard-model.md#pion), $G|\pi^0\rangle=-\mathcal C|\pi^0\rangle=-|\pi^0\rangle$. Therefore the [pion G-parity](../../../standard-model.md#pion-g-parity) is

$$
\boxed{G=-1\quad\text{on all three pion states}.}
$$

## 2

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the full definition of the [special unitary group](../../../topological-group.md#special-unitary-group): $A^\dagger A=I$ and $\det A=1$. The [determinant](../../../linear-algebra.md#determinant) condition is essential for the alternating [tensors](../../../linear-algebra.md#tensor); unitarity alone would instead define $U(n)$. Assume $n\geq2$ when discussing proper [invariant subspaces](../../../representation-theory.md#invariant-subspace).

Let $V=\mathbb C^n$ be the [fundamental representation](../../../semisimple-lie-algebra.md#fundamental-representation). A $(j,k)$ [tensor](../../../linear-algebra.md#tensor) belongs to $V^{\otimes j}\otimes(V^*)^{\otimes k}$. Its [SU(n) tensor transformation](../../../representation-theory.md#su-n-tensor-transformation) is

$$
\boxed{T'{}^{\alpha_1\cdots\alpha_j}_{\beta_1\cdots\beta_k}
=A^{\alpha_1}{}_{\gamma_1}\cdots A^{\alpha_j}{}_{\gamma_j}
(A^{-1})^{\delta_1}{}_{\beta_1}\cdots(A^{-1})^{\delta_k}{}_{\beta_k}
T^{\gamma_1\cdots\gamma_j}_{\delta_1\cdots\delta_k}.}
$$

Since $(A^{-1})^\delta{}_{\beta}=\overline{A^\beta{}_{\delta}}$, [complex conjugation](../../../complex-analysis.md#complex-conjugation) exchanges upper fundamental and lower dual factors. Reordering the two index groups shows that $\overline T$ is a $(k,j)$ [tensor](../../../linear-algebra.md#tensor).

The [invariant tensors](../../../representation-theory.md#invariant-tensor) follow directly. The [Kronecker delta](../../../linear-algebra.md#kronecker-delta) transforms to $A^\alpha{}_{\gamma}(A^{-1})^\gamma{}_{\beta}=\delta^\alpha{}_{\beta}$. For the alternating [tensors](../../../linear-algebra.md#tensor), the [determinant](../../../linear-algebra.md#determinant) expansion gives

$$
A^{\alpha_1}{}_{\gamma_1}\cdots A^{\alpha_n}{}_{\gamma_n}\epsilon^{\gamma_1\cdots\gamma_n}
=(\det A)\epsilon^{\alpha_1\cdots\alpha_n}=\epsilon^{\alpha_1\cdots\alpha_n}.
$$

The lower [tensor](../../../linear-algebra.md#tensor) is preserved in the same way using $\det A^{-1}=1$. Thus **$\delta$, $\epsilon^{\alpha_1\cdots\alpha_n}$ and $\epsilon_{\beta_1\cdots\beta_n}$ are invariant.**

When $j\geq2$, the permutation of two upper slots commutes with the [tensor product representation](../../../representation-theory.md#tensor-product-of-group-representations). Its $+1$ and $-1$ [eigenspaces](../../../linear-operator-theory.md#eigenspace) are nonzero proper [invariant subspaces](../../../representation-theory.md#invariant-subspace). The same argument uses two lower slots when $k\geq2$. The remaining rank-two case $(j,k)=(1,1)$ splits into scalar multiples of $\delta$ and [traceless second-rank tensors](../../../linear-algebra.md#traceless-second-rank-tensor), since [tensor contraction](../../../linear-algebra.md#tensor-contraction) is equivariant. This covers every case except the fundamental, dual fundamental and scalar cases specified in the question. Those three are irreducible: the [special unitary group](../../../topological-group.md#special-unitary-group) acts transitively on unit vectors in its fundamental space, so a nonzero [invariant subspace](../../../representation-theory.md#invariant-subspace) must be the full space, and the dual has the same property.

A [symmetric tensor](../../../linear-algebra.md#symmetric-tensor) of upper rank $j$ has one component for each multiplicity vector $(r_1,\ldots,r_n)$ with nonnegative entries and $\sum r_i=j$. Equivalently it is a homogeneous degree-$j$ polynomial in $n$ variables. Counting these monomials gives

$$
\boxed{\dim\operatorname{Sym}^jV=\binom{n+j-1}{j}=\frac{(n+j-1)!}{j!(n-1)!}.}
$$

For a [totally antisymmetric tensor](../../../linear-algebra.md#totally-antisymmetric-tensor), any repeated index gives zero and the remaining components are indexed by increasing $j$-element subsets. Hence

$$
\boxed{\dim\bigwedge^jV=\binom nj\quad(0\leq j\leq n),\qquad \dim\bigwedge^jV=0\quad(j>n).}
$$

These are the dimensions of the [symmetric power](../../../linear-algebra.md#symmetric-power) and [exterior power](../../../linear-algebra.md#exterior-power), respectively.

For [SU(4)](../../../topological-group.md#su-4-group), the [two-index antisymmetric representation](../../../semisimple-lie-algebra.md#two-index-antisymmetric-representation) has complex dimension six. To establish a six-dimensional [real representation](../../../representation-theory.md#real-representation), one must exhibit a real structure; simply counting six complex components would give twelve real components. Normalize $\epsilon^{1234}=1$ and define the [antilinear map](../../../vector-space.md#antilinear-map)

$$
(\mathcal JT)^{ab}=\frac12\epsilon^{abcd}\overline{T^{cd}}.
$$

The invariant Hermitian form identifies the conjugate indices with lower indices, and the invariant volume [tensor](../../../linear-algebra.md#tensor) then returns an upper pair. Thus $\mathcal J$ commutes with [SU(4)](../../../topological-group.md#su-4-group). The identity

$$
\epsilon^{abcd}\epsilon_{cdef}=2(\delta^a_e\delta^b_f-\delta^a_f\delta^b_e)
$$

gives $\mathcal J^2=1$. Its fixed space has

$$
T^{12}=\overline{T^{34}},\qquad T^{13}=-\overline{T^{24}},\qquad T^{14}=\overline{T^{23}}.
$$

Three arbitrary complex entries specify all the others, giving exactly six real degrees of freedom. The [real structure of the SU4 exterior square](../../../semisimple-lie-algebra.md#real-structure-of-the-su4-exterior-square) therefore proves

$$
\boxed{\bigwedge^2\mathbb C^4\text{ is the complexification of a real six-dimensional representation}.}
$$

The ordinary Hermitian [norm](../../../functional-analysis.md#norm) restricts to an invariant positive real [inner product](../../../linear-algebra.md#inner-product) on this fixed space.

[Irreducible representations](../../../representation-theory.md#irreducible-representation) classify states because an exact symmetry commutes with the [Hamiltonian](../../../classical-mechanics.md#hamiltonian), preserving energy [eigenspaces](../../../linear-operator-theory.md#eigenspace). Irreducible multiplets are the smallest sets closed under all symmetry transformations; their labels and [Casimir operators](../../../semisimple-lie-algebra.md#casimir-element) provide quantum numbers. Approximate [flavour symmetry](../../../standard-model.md#flavor-symmetry) gives approximate multiplets and mass relations, with splittings caused by its breaking. Spin and internal quantum numbers are distinct labels.

For the light-quark [flavour symmetry](../../../standard-model.md#flavor-symmetry) in [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics), the quark flavours form $\mathbf3$. Their [Triple tensor decomposition for the defining sl3 representation](../../../semisimple-lie-algebra.md#triple-tensor-decomposition-for-the-defining-sl3-representation) is

$$
\mathbf3^{\otimes3}=\mathbf{10}_{\rm sym}\oplus\mathbf8_{\rm mixed}\oplus\mathbf8_{\rm mixed}\oplus\mathbf1_{\rm antisym}.
$$

This algebraic decomposition alone does not determine the allowed ground-state [baryons](../../../physics.md#baryon). The [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet) is antisymmetric. The no-orbital-excitation ground state has a symmetric spatial wavefunction, so the [Pauli exclusion principle](../../../quantum-mechanics.md#pauli-exclusion-principle) requires the combined spin-flavour wavefunction to be symmetric. The three spin-one-half factors have

$$
\mathbf2^{\otimes3}=\mathbf4_{\rm sym}\oplus\mathbf2_{\rm mixed}\oplus\mathbf2_{\rm mixed},\qquad \bigwedge^3\mathbb C^2=0.
$$

Here the four-dimensional spin representation has spin $3/2$, while each doublet has spin $1/2$. Symmetric decuplet flavour pairs with symmetric spin $3/2$. The two flavour-octet copies and two spin-doublet copies carry the two-dimensional standard permutation multiplicity space; its [tensor square](../../../linear-algebra.md#tensor-square) contains one symmetric singlet. Their invariant pairing therefore supplies one octet with spin $1/2$, not two independent ground-state octets. Antisymmetric flavour would need a completely antisymmetric three-quark spin state, which does not exist.

Equivalently the [symmetric spin-flavour SU6 representation](../../../physics.md#symmetric-spin-flavour-su6-representation) has

$$
\operatorname{Sym}^3(\mathbb C^3\otimes\mathbb C^2)
=(\mathbf{10},\mathbf4)\oplus(\mathbf8,\mathbf2),\qquad 56=40+16.
$$

Thus the [Pauli constraint on three-quark flavour multiplets](../../../physics.md#pauli-constraint-on-three-quark-flavour-multiplets) gives the concise spectrum classification

$$
\boxed{\mathbf8\text{ with }J^P=\tfrac12^+,\qquad \mathbf{10}\text{ with }J^P=\tfrac32^+.}
$$

These are the [baryon octet](../../../standard-model.md#baryon-octet) and [baryon decuplet](../../../standard-model.md#baryon-decuplet). The [three-quark flavour singlet](../../../standard-model.md#three-quark-flavour-singlet) requires a different spatial permutation symmetry and belongs to excited states, outside the symmetric ground-state approximation used here. If low-lying spatially excited states are also included while their orbital labels are merely suppressed, singlets can occur; the full flavour tensor cube has types $\mathbf1,\mathbf8,\mathbf{10}$. The absence of the singlet from the unexcited ground multiplet is a permutation-symmetry constraint, not a prohibition by $SU(3)$ alone. Light-quark mass differences make the [flavour symmetry](../../../standard-model.md#flavor-symmetry) approximate rather than exact.

## 3

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use a real [Lie algebra](../../../lie-algebra.md) convention $[T_a,T_b]=f_{ab}{}^cT_c$. Its [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) acts on $\mathfrak g$ itself:

$$
\boxed{\operatorname{ad}_X(Y)=[X,Y].}
$$

Linearity is immediate. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]Z
=[X,[Y,Z]]-[Y,[X,Z]]=[[X,Y],Z],
$$

so $[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}$, the defining [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) condition. In the basis $T_b$, its [matrix](../../../vector-space.md#matrix) entries are

$$
\boxed{(T_a^{\rm ad})^c{}_b=f_{ab}{}^c.}
$$

Thus the adjoint generators are the [structure constants](../../../algebra.md#structure-constant) arranged as [matrices](../../../vector-space.md#matrix). The representation has kernel equal to the [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra); it need not be faithful for an arbitrary algebra.

The [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group) is $\operatorname{Ad}_g(Y)=gYg^{-1}$. It satisfies $\operatorname{Ad}_{gh}=\operatorname{Ad}_g\operatorname{Ad}_h$, preserves the identity, and sends inverses to inverse [matrices](../../../vector-space.md#matrix). Differentiating $e^{tX}Ye^{-tX}$ gives $[X,e^{tX}Ye^{-tX}]$, so

$$
\boxed{\operatorname{Ad}_{e^X}=e^{\operatorname{ad}_X},\qquad e^{-X}Ye^X=e^{-\operatorname{ad}_X}Y.}
$$

Consequently the positive adjoint exponentials furnish the representation on elements $g=e^X$ and their products, and the intrinsic conjugation action defines it globally.

**The inverse-conjugation formula in the PDF needs a minus adjoint exponent with this standard definition.** Its first-order term is $Y-[X,Y]$, whereas $e^{+\operatorname{ad}_X}Y$ has first-order term $Y+[X,Y]$. For example $X=T_1,Y=T_2$ in a nonabelian algebra with $[T_1,T_2]\neq0$ already distinguishes the two. The [inverse conjugation and adjoint antirepresentations](../../../lie-theory.md#inverse-conjugation-and-adjoint-antirepresentations) identity explains the group-order issue as well: $F(g)=\operatorname{Ad}_{g^{-1}}$ satisfies $F(gh)=F(h)F(g)$. Retaining the printed inverse conjugation as a left action without this order reversal would not give an ordinary [group representation](../../../representation-theory.md#group-representation).

The [Killing form](../../../lie-algebra.md#killing-form) is the symmetric [bilinear form](../../../linear-algebra.md#bilinear-form)

$$
\boxed{B(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).}
$$

To prove degeneracy for a non-[semisimple Lie algebra](../../../semisimple-lie-algebra.md), take its nonzero [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) and the last nonzero member $\mathfrak a$ of its [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra). This is a nonzero abelian [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra). For $x\in\mathfrak a$, $\operatorname{ad}_x$ maps $\mathfrak g$ into $\mathfrak a$ and kills $\mathfrak a$. Every $\operatorname{ad}_y$ preserves $\mathfrak a$. Hence $\operatorname{ad}_x\operatorname{ad}_y$ maps the full space into $\mathfrak a$ and has zero restriction there, so its trace is zero. Thus $B(x,y)=0$ for every $y$. This is the [abelian ideals lie in the radical of the Killing form](../../../lie-algebra.md#abelian-ideals-lie-in-the-radical-of-the-killing-form) argument, and establishes a nonzero kernel and vanishing [determinant](../../../linear-algebra.md#determinant).

For a compact real [semisimple Lie algebra](../../../semisimple-lie-algebra.md), the adjoint action is unitary in an invariant positive [inner product](../../../linear-algebra.md#inner-product). Its infinitesimal generators are skew-Hermitian, giving

$$
B(X,X)=-\operatorname{tr}(\operatorname{ad}_X^\dagger\operatorname{ad}_X)<0\qquad(X\neq0).
$$

Strictness follows because the adjoint kernel is the zero center. This explains the [compactness criterion from the Killing form](../../../lie-algebra.md#compactness-criterion-from-the-killing-form): “strictly negative” means negative-definite, not that every entry of its [matrix](../../../vector-space.md#matrix) is negative.

In the first three-generator example, take columns to be images of the basis $(X,Y,H)$. Direct use of the brackets gives

$$
\boxed{\operatorname{ad}_X=\begin{pmatrix}0&0&0\\0&0&2\\0&2&0\end{pmatrix},\quad
\operatorname{ad}_Y=\begin{pmatrix}0&0&2\\0&0&0\\-2&0&0\end{pmatrix},\quad
\operatorname{ad}_H=\begin{pmatrix}0&-2&0\\-2&0&0\\0&0&0\end{pmatrix}.}
$$

Taking traces of products yields the [Killing form for cyclic three-generator brackets](../../../lie-algebra.md#killing-form-for-cyclic-three-generator-brackets)

$$
\boxed{[B]_{(X,Y,H)}=\operatorname{diag}(8,-8,8).}
$$

It is nondegenerate, hence semisimple by the preceding degeneracy result, but it has mixed signature and is not compact. An explicit realization is

$$
X=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
Y=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\quad
H=\begin{pmatrix}-1&0\\0&1\end{pmatrix},
$$

which span the real traceless two-by-two [matrices](../../../vector-space.md#matrix) and satisfy exactly these brackets.

Changing the sign of $[X,H]$ changes the first and third adjoint [matrices](../../../vector-space.md#matrix) to

$$
\operatorname{ad}_X=\begin{pmatrix}0&0&0\\0&0&-2\\0&2&0\end{pmatrix},\qquad
\operatorname{ad}_H=\begin{pmatrix}0&-2&0\\2&0&0\\0&0&0\end{pmatrix},
$$

while $\operatorname{ad}_Y$ is unchanged. Now

$$
\boxed{[B]=-8I_3,}
$$

the negative-definite compact case. The basis $X=-i\sigma_1$, $Y=-i\sigma_2$, $H=-i\sigma_3$ realizes it as the real [special unitary Lie algebra](../../../lie-algebra.md#special-unitary-lie-algebra) $\mathfrak{su}(2)$.

## 4

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use signature $\eta=\operatorname{diag}(1,-1,-1,-1)$, the numerical [matrices](../../../vector-space.md#matrix) $\sigma_\mu=(I,\sigma_i)$ and $\bar\sigma_\mu=(I,-\sigma_i)$ given in the question, and raise genuine [tensor](../../../linear-algebra.md#tensor) indices with $\eta$. A real [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) vector corresponds to the [Hermitian matrix](../../../hilbert-space.md#hermitian-operator)

$$
X=x^0I+\mathbf x\cdot\boldsymbol\sigma,\qquad \det X=(x^0)^2-|\mathbf x|^2.
$$

For [SL(2,C)](../../../group-theory.md#complex-special-linear-group-in-dimension-two) [matrices](../../../vector-space.md#matrix), $X'=AXA^\dagger$ is Hermitian and has the same [determinant](../../../linear-algebra.md#determinant). It therefore induces a real linear [Lorentz transformation](../../../special-relativity.md#lorentz-transformation); composition of the congruence actions agrees with [matrix](../../../vector-space.md#matrix) multiplication. The kernel consists of $\pm I$: preservation of $X=I$ makes a kernel element unitary, and preservation of every Hermitian $X$ makes it scalar.

[Polar decomposition of an invertible complex matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-complex-matrix) connects every determinant-one complex [matrix](../../../vector-space.md#matrix) to its unitary factor, so the group is connected. The action gives the [Lorentz spinor double cover](../../../special-relativity.md#lorentz-spinor-double-cover) of the [Proper orthochronous Lorentz group](../../../special-relativity.md#proper-orthochronous-lorentz-group). It covers rotations via $A_R=e^{-i\vartheta\mathbf n\cdot\boldsymbol\sigma/2}$ and boosts via the positive Hermitian [matrices](../../../vector-space.md#matrix) below. Every proper orthochronous transformation is a boost followed by a rotation, since one can first match its image of the future unit time vector and then use its rotation stabilizer. **The congruence construction does not cover spatial parity or time reversal.** In particular parity has [determinant](../../../linear-algebra.md#determinant) $-1$ as a four-vector transformation; all transformations continuously produced from [SL(2,C)](../../../group-theory.md#complex-special-linear-group-in-dimension-two) have [determinant](../../../linear-algebra.md#determinant) $+1$.

Set $c_\theta=\cosh(\theta/2)$, $s_\theta=\sinh(\theta/2)$ and $N=\mathbf n\cdot\boldsymbol\sigma$. The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives $N^2=I$. The proposed boost [matrix](../../../vector-space.md#matrix) is $A_B=c_\theta I+s_\theta N$, with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $e^{\pm\theta/2}$, [determinant](../../../linear-algebra.md#determinant) one and $A_B^\dagger=A_B$. Split $\mathbf x=x_\parallel\mathbf n+\mathbf x_\perp$. The perpendicular Pauli part anticommutes with $N$, so multiplication gives

$$
\boxed{x'^0=\cosh\theta\,x^0+\sinh\theta\,x_\parallel,\qquad
x'_\parallel=\sinh\theta\,x^0+\cosh\theta\,x_\parallel,\qquad
\mathbf x'_\perp=\mathbf x_\perp.}
$$

This is an active [Lorentz boost](../../../special-relativity.md#lorentz-boost). The image of a rest worldline has velocity **$\mathbf v=\tanh\theta\,\mathbf n$**, fixing the velocity sign convention.

For two nonzero boosts, write $A'=c'I+s'\mathbf n'\cdot\boldsymbol\sigma$ and $A=cI+s\mathbf n\cdot\boldsymbol\sigma$. Their product is

$$
A'A=(c'c+s's\mathbf n'\cdot\mathbf n)I
+(c's\mathbf n+s'c\mathbf n')\cdot\boldsymbol\sigma
+i s's(\mathbf n'\times\mathbf n)\cdot\boldsymbol\sigma.
$$

The last term is anti-Hermitian. Thus $A'A$ is not Hermitian unless the axes are collinear; a pure boost has Hermitian lifts $\pm A_B$, so it cannot give the same Lorentz transformation. The [noncollinear boost obstruction from Pauli products](../../../special-relativity.md#noncollinear-boost-obstruction-from-pauli-products) is therefore

$$
\boxed{\text{two nonzero noncollinear boosts require an accompanying rotation}.}
$$

That rotation is a [Wigner rotation](../../../special-relativity.md#wigner-rotation). A zero-rapidity factor is the trivial exception, regardless of the arbitrary axis assigned to it.

Define $J_i=\tfrac12\epsilon_{ijk}M_{jk}$ and $K_i=M_{0i}$. The printed [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra) brackets give

$$
[J_i,J_j]=i\epsilon_{ijk}J_k,\qquad
[J_i,K_j]=i\epsilon_{ijk}K_k,\qquad
[K_i,K_j]=-i\epsilon_{ijk}J_k.
$$

Set $L_i=(J_i+iK_i)/2$, $R_i=(J_i-iK_i)/2$. Then

$$
\boxed{[L_i,L_j]=i\epsilon_{ijk}L_k,\quad
[R_i,R_j]=i\epsilon_{ijk}R_k,\quad [L_i,R_j]=0.}
$$

This is the [chiral decomposition of the complex Lorentz algebra](../../../semisimple-lie-algebra.md#chiral-decomposition-of-the-complex-lorentz-algebra). The two copies are the complexifications of the [SU(2)](../../../topological-group.md#su-2-group) algebras conventionally labelled left and right. They are not two independent compact real subalgebras of the real Lorentz algebra: $L,R$ are complex linear combinations of the real generators. The distinction is needed for noncompact boosts.

To verify the infinitesimal two-component action, put

$$
a=\frac14\omega^{\mu\nu}\sigma_\mu\bar\sigma_\nu,\qquad A=I+a+O(\omega^2).
$$

Its trace vanishes by antisymmetry, so $\det A=1+O(\omega^2)$. The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) implies

$$
\sigma_\mu\bar\sigma_\nu\sigma_\rho+\sigma_\rho\bar\sigma_\nu\sigma_\mu
=2(\eta_{\mu\nu}\sigma_\rho+\eta_{\nu\rho}\sigma_\mu-\eta_{\mu\rho}\sigma_\nu).
$$

Since $a^\dagger=\tfrac14\omega^{\mu\nu}\bar\sigma_\nu\sigma_\mu$, antisymmetrizing this identity yields

$$
a\sigma_\rho+\sigma_\rho a^\dagger
=\omega^\mu{}_{\rho}\sigma_\mu.
$$

Consequently $AXA^\dagger=X+\sigma_\mu\omega^\mu{}_{\nu}x^\nu+O(\omega^2)$, exactly the claimed infinitesimal coordinate transformation with $\omega^\mu{}_{\nu}=\omega^{\mu\rho}\eta_{\rho\nu}$.

The two [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) representations transform as

$$
\boxed{\psi_L\mapsto A\psi_L,\qquad \psi_R\mapsto(A^\dagger)^{-1}\psi_R.}
$$

Both maps preserve group multiplication. For $\Lambda=e^\omega$, choose its spin lift and write the finite [matrices](../../../vector-space.md#matrix) as

$$
A=\exp\left(\frac14\omega^{\mu\nu}\sigma_\mu\bar\sigma_\nu\right),\qquad
(A^\dagger)^{-1}=\exp\left(\frac14\omega^{\mu\nu}\bar\sigma_\mu\sigma_\nu\right).
$$

For rotations these coincide as the [SU(2)](../../../topological-group.md#su-2-group) doublet; for boosts their generator signs are opposite. Any complex-linear intertwiner would commute with all rotations and hence be scalar by the [Schur lemma](../../../representation-theory.md#schur-s-lemma), but a nonzero scalar cannot intertwine the opposite boost [matrices](../../../vector-space.md#matrix). They are therefore inequivalent. Infinitesimally their $K_i$ [matrices](../../../vector-space.md#matrix) are $-i\sigma_i/2$ and $+i\sigma_i/2$, while their $J_i$ [matrices](../../../vector-space.md#matrix) are both $\sigma_i/2$. Thus they have chiral labels $(1/2,0)$ and $(0,1/2)$. The finite [matrices](../../../vector-space.md#matrix) are representations of the spin cover; choosing $A$ or $-A$ matters for spinors even though their four-vector transformations coincide.

Using the supplied block [gamma matrices](../../../algebra.md#gamma-matrices), the generator of the [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) is

$$
\Omega=\frac14\omega^{\mu\nu}\gamma_{\mu\nu}
=\begin{pmatrix}\tfrac14\omega^{\mu\nu}\sigma_\mu\bar\sigma_\nu&0\\0&\tfrac14\omega^{\mu\nu}\bar\sigma_\mu\sigma_\nu\end{pmatrix}.
$$

The antisymmetry of $\omega$ removes the symmetric Clifford part. Hence

$$
\boxed{\psi\mapsto S\psi,\qquad S=e^\Omega=\operatorname{diag}(A,(A^\dagger)^{-1}).}
$$

There is a conjugation-order error in the last displayed gamma identity in the PDF. The [Clifford algebra](../../../algebra.md#clifford-algebra) gives, with $\gamma^\rho=\eta^{\rho\sigma}\gamma_\sigma$,

$$
[\gamma_{\mu\nu},\gamma^\rho]=2(\delta_\nu^\rho\gamma_\mu-\delta_\mu^\rho\gamma_\nu),\qquad
[\Omega,\gamma^\rho]=-\omega^\rho{}_{\mu}\gamma^\mu.
$$

Exponentiating this linear [commutator](../../../lie-algebra.md#commutator) action proves the [inverse Lorentz action on gamma matrices](../../../relativistic-quantum-field.md#inverse-lorentz-action-on-gamma-matrices)

$$
\boxed{S\gamma^\rho S^{-1}=(\Lambda^{-1})^\rho{}_{\mu}\gamma^\mu,\qquad
S^{-1}\gamma^\rho S=\Lambda^\rho{}_{\mu}\gamma^\mu.}
$$

The second identity is the order required for the requested bilinears when $\psi\mapsto S\psi$. An explicit countercheck to the printed order is a positive boost along the third axis: $\omega^{03}=-\theta$ gives

$$
S\gamma^0S^{-1}=\cosh\theta\,\gamma^0-\sinh\theta\,\gamma^3,
$$

whereas the printed right side has a plus sign. This cannot be repaired by dropping index raising; the same raising convention is needed in the preceding coordinate transformation.

The adjoint relation supplied in the question gives $\Omega^\dagger\gamma^0=-\gamma^0\Omega$, hence the [Dirac spinor pseudo-unitarity](../../../relativistic-quantum-field.md#dirac-spinor-pseudo-unitarity) identity $S^\dagger\gamma^0S=\gamma^0$. The [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) therefore transforms as $\bar\psi\mapsto\bar\psi S^{-1}$. It now follows that the [Dirac scalar bilinear](../../../relativistic-quantum-field.md#dirac-scalar-bilinear) is

$$
\boxed{\bar\psi'\psi'=\bar\psi S^{-1}S\psi=\bar\psi\psi,}
$$

the vector is

$$
\boxed{\bar\psi'\gamma^\rho\psi'=\Lambda^\rho{}_{\mu}\bar\psi\gamma^\mu\psi,}
$$

and the antisymmetric second-rank [tensor](../../../linear-algebra.md#tensor) is

$$
\boxed{\bar\psi' i[\gamma^\rho,\gamma^\sigma]\psi'
=\Lambda^\rho{}_{\mu}\Lambda^\sigma{}_{\nu}\bar\psi i[\gamma^\mu,\gamma^\nu]\psi.}
$$

These are respectively a [Lorentz scalar](../../../special-relativity.md#lorentz-scalar), [Lorentz four-vector](../../../special-relativity.md#four-vector) and [Lorentz tensor](../../../special-relativity.md#lorentz-tensor). The source's inconsistent gamma identity is replaced by its correct inverse/order pair; all three transformation laws then follow with the stated spinor transformation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
