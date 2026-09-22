# Paper 19

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper19.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper19.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [1](#6/1)
    - [Solution](#6/1/solution)
  - [2](#6/2)
    - [Solution](#6/2/solution)

## 1

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For $G=U(n)$ take the diagonal [maximal torus](../../../lie-theory.md#maximal-torus)

$$
T=\{\operatorname{diag}(z_1,\ldots,z_n):|z_i|=1\}.
$$

The [spectral theorem](../../../hilbert-space.md#spectral-theorem) for [unitary matrices](../../../linear-operator-theory.md#unitary-matrix) says that every element is conjugate to an element of $T$. A diagonal element with pairwise distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) has centralizer exactly $T$. Its conjugates therefore determine its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) up to [permutation](../../../combinatorics.md#permutation), and the normalizer quotient is $W=N_G(T)/T\cong S_n$. The [character lattice of a torus](../../../lie-theory.md#character-lattice-of-a-torus) $T$ is $\mathbb Z^n$, with $e^\lambda(z)=z_1^{\lambda_1}\cdots z_n^{\lambda_n}$. [Conjugation](../../../group-theory.md#conjugation) on the [matrix unit](../../../vector-space.md#matrix-unit) $E_{ij}$ has [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $e_i-e_j$, so these are the [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system). Choose $e_i-e_j$ positive for $i<j$; then

$$
\rho=\frac12(n-1,n-3,\ldots,1-n).
$$

[Dominant integral weights](../../../semisimple-lie-algebra.md#dominant-integral-weight) are precisely the integer tuples $\lambda_1\geq\cdots\geq\lambda_n$. Negative entries are allowed: they correspond to [determinant twists](../../../lie-theory.md#determinant-twist), so [polynomial representations](../../../lie-theory.md#polynomial-representation-of-the-general-linear-group) alone do not exhaust the [irreducible representations](../../../representation-theory.md#irreducible-representation) of $U(n)$.

Normalize [Haar measure](../../../measure-theory.md#haar-measure) on $G$ and $T$ to have mass one, and put

$$
\Delta(z)=\det(z_i^{n-j})_{i,j=1}^n=\prod_{i<j}(z_i-z_j).
$$

The [Weyl integration formula for U(n)](../../../lie-theory.md#weyl-integration-formula-for-u-n) for a [continuous](../../../calculus.md#continuous-function) [class function](../../../representation-theory.md#class-function) is

$$
\boxed{\int_{U(n)}f(g)\,dg
=\frac1{n!}\int_{[0,2\pi)^n} f(\operatorname{diag}(e^{i\theta_1},\ldots,e^{i\theta_n}))
\prod_{i<j}|e^{i\theta_i}-e^{i\theta_j}|^2
\prod_{i=1}^n\frac{d\theta_i}{2\pi}.}
$$

For a general [continuous function](../../../calculus.md#continuous-function), replace $f(t)$ in the [torus](../../../topology.md#torus) integral by $\int_{G/T}f(gtg^{-1})\,d(gT)$, using the normalized invariant quotient measure.

To prove the formula, consider the [conjugation](../../../group-theory.md#conjugation) map $q:G/T\times T\to G$, $q(gT,t)=gtg^{-1}$. On regular [torus](../../../topology.md#torus) elements its fibres have exactly $n!$ points: the possible orderings of the distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Equip the [group](../../../group.md) with an invariant [inner product](../../../linear-algebra.md#inner-product) on its [Lie algebra](../../../lie-algebra.md) and split $\mathfrak u(n)=\mathfrak t\oplus\mathfrak t^\perp$. After translating the derivative back to the identity, its [torus](../../../topology.md#torus) directions contribute the identity, while its transverse directions contribute $\operatorname{Ad}_{t^{-1}}-I$. Each pair $i<j$ supplies a real two-dimensional off-diagonal plane. On that plane $\operatorname{Ad}_t$ is multiplication by $z_i/z_j$, regarded as a plane rotation, so the absolute real [determinant](../../../linear-algebra.md#determinant) of the transverse derivative is

$$
J(t)=\prod_{i<j}|z_i/z_j-1|^2=|\Delta(z)|^2.
$$

The change-of-variables theorem, divided by the covering multiplicity, now gives the desired weighted integral up to the constant relating the normalized [invariant measures](../../../measure-theory.md#invariant-measure). The nonregular locus has measure zero: repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are the zero-set of the nonzero discriminant, and the [torus](../../../topology.md#torus) coincidence sets likewise have measure zero. Thus its omission causes no change to the integral. To determine the normalization, expand $\Delta$ as a sum of $n!$ distinct [torus characters](../../../fourier-analysis.md#characters-of-a-real-torus). [Fourier orthogonality](../../../fourier-series.md#fourier-orthogonality) gives $\int_T|\Delta|^2\,dt=n!$. Applying the formula to $f=1$ fixes the coefficient to $1/n!$. This proves both the class-function and conjugacy-averaged forms.

We can now derive the [character](../../../representation-theory.md#character-of-a-representation) formula from integration, rather than merely quote it. Use the basic highest-weight theorem: a finite-dimensional [irreducible representation](../../../representation-theory.md#irreducible-representation) has a unique [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\lambda$ with a one-dimensional highest-weight space; all its other [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) are $\lambda$ minus a nonnegative sum of [positive roots](../../../semisimple-lie-algebra.md#positive-root). Its [character](../../../representation-theory.md#character-of-a-representation) is Weyl invariant. Also, [character orthogonality for compact groups](../../../representation-theory.md#character-orthogonality-for-compact-groups) gives $\int_G|\chi_\lambda|^2=1$. This [orthogonality](../../../linear-algebra.md#orthogonal-vectors) follows by averaging the [representation](../../../representation-theory.md#group-representation) on $\operatorname{End}(V_\lambda)$: the integral projects onto [intertwining operators](../../../representation-theory.md#intertwining-operator), whose [dimension](../../../vector-space.md#dimension-vector-space) is one by the [Schur lemma](../../../representation-theory.md#schur-s-lemma).

Let $\delta=(n-1,n-2,\ldots,0)$ and, for a strictly decreasing integer tuple $\eta$, put $A_\eta(z)=\det(z_i^{\eta_j})$. The finite [Laurent polynomial](../../../polynomial.md#laurent-polynomial) $\Delta\chi_\lambda$ is alternating. Every alternating [Laurent polynomial](../../../polynomial.md#laurent-polynomial) is a [linear combination](../../../vector-space.md#linear-combination) of the $A_\eta$: collect its monomials by [permutation](../../../combinatorics.md#permutation) orbits, and observe that an orbit with repeated exponents has zero coefficient by antisymmetry. Different $A_\eta$ are [orthogonal](../../../linear-algebra.md#orthogonal-vectors) on $T$ and each has squared norm $n!$.

The coefficient of $z^{\lambda+\delta}$ in $\Delta\chi_\lambda$ is exactly one. Indeed, a contribution from the term $z^{w\delta}$ would require a [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $\lambda+\delta-w\delta$ in $V_\lambda$. For $w\ne1$, the vector $\delta-w\delta$ is a nonzero nonnegative combination of the positive [simple roots](../../../semisimple-lie-algebra.md#simple-root), so that [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) lies above $\lambda$ and is impossible. The identity [permutation](../../../combinatorics.md#permutation) supplies the highest-weight coefficient one. Consequently

$$
\Delta\chi_\lambda=A_{\lambda+\delta}+\sum_{\eta\ne\lambda+\delta}c_\eta A_\eta.
$$

Apply the integration formula to $|\chi_\lambda|^2$. [Torus](../../../topology.md#torus) [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives

$$
1=\frac1{n!}\int_T|\Delta\chi_\lambda|^2\,dt
=1+\sum_{\eta\ne\lambda+\delta}|c_\eta|^2.
$$

All the other coefficients vanish, proving

$$
\boxed{\chi_\lambda(z)=\frac{\det(z_i^{\lambda_j+n-j})}{\det(z_i^{n-j})}.}
$$

The quotient extends across repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) because its product with the denominator is the already defined [continuous](../../../calculus.md#continuous-function) [character](../../../representation-theory.md#character-of-a-representation). Equivalently, alternant divisibility makes it a [Laurent polynomial](../../../polynomial.md#laurent-polynomial) invariant under [permutations](../../../combinatorics.md#permutation); multiply by a [determinant](../../../linear-algebra.md#determinant) power if negative exponents must first be removed.

Finally, $\delta-\rho=\frac{n-1}{2}(1,\ldots,1)$ is fixed by the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), so its common factor cancels in the quotient. Since $A_\rho=e^\rho\prod_{\alpha>0}(1-e^{-\alpha})$, the [determinant](../../../linear-algebra.md#determinant) expression is exactly

$$
\chi_\lambda=\frac{\sum_{w\in W}\varepsilon(w)e^{w(\lambda+\rho)-\rho}}{\prod_{\alpha>0}(1-e^{-\alpha})}.
$$

Using $\delta$ in the derivation avoids treating a possibly half-integral $\rho$ as an actual [character](../../../representation-theory.md#character-of-a-representation) of the [torus](../../../topology.md#torus). At the identity, taking the leading Vandermonde term of the two [determinants](../../../linear-algebra.md#determinant) gives the accompanying [dimension](../../../vector-space.md#dimension-vector-space) formula

$$
\dim V_\lambda=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}.
$$

## 2

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

There are two necessary qualifications to the literal formulation. The whole [group](../../../group.md) $G$ is itself a closed [normal subgroup](../../../group-theory.md#normal-subgroup), so the claim about containment in the centre must concern **proper closed [normal subgroups](../../../group-theory.md#normal-subgroup)**. Also, the homomorphism conclusion needs **a nontrivial target $H$**: for example, $SU(2)\to\{1\}$ has [surjective](../../../algebra.md#surjective-function) differential onto the zero [Lie algebra](../../../lie-algebra.md), but its [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) is all of $SU(2)$ and no quotient by a finite subgroup is a one-point [group](../../../group.md). We prove the precise assertions, including these exceptional cases.

Write $\mathfrak g=\operatorname{Lie}(G)$. The centre $\mathfrak z(\mathfrak g)$ is invariant under the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), so irreducibility makes it either zero or all of $\mathfrak g$. In the latter case $\mathfrak g$ is [Abelian](../../../group.md#abelian-group). For [connected](../../../geometry-and-topology.md#connected-space) $G$, the [adjoint action](../../../lie-theory.md#adjoint-representation-of-a-lie-group) is then trivial: the [group](../../../group.md) is generated by exponentials, and $\operatorname{Ad}_{\exp X}=e^{\operatorname{ad}X}=I$. A nonzero [trivial representation](../../../representation-theory.md#trivial-representation) is [irreducible](../../../representation-theory.md#irreducible-representation) only in [dimension](../../../vector-space.md#dimension-vector-space) one. A [connected](../../../geometry-and-topology.md#connected-space) [compact](../../../topology.md#compact-space) one-dimensional [Lie group](../../../lie-theory.md#lie-group) is a circle, so $G\cong U(1)$.

For every other $G$, the [Lie algebra](../../../lie-algebra.md) of its centre is zero. The centre is a closed [compact](../../../topology.md#compact-space) [Lie subgroup](../../../lie-theory.md#lie-subgroup); a zero-dimensional [compact Lie group](../../../lie-theory.md#compact-lie-group) is finite. Let $N$ be a closed [normal subgroup](../../../group-theory.md#normal-subgroup). The [closed-subgroup theorem](../../../lie-theory.md#closed-subgroup-theorem) identifies $\mathfrak n=\operatorname{Lie}(N)$ as an adjoint-invariant subspace of $\mathfrak g$, hence $\mathfrak n=0$ or $\mathfrak n=\mathfrak g$. If the latter holds, $N$ contains an identity neighbourhood and is open, so connectedness forces $N=G$. If $N$ is proper, it therefore has zero [Lie algebra](../../../lie-algebra.md) and is finite. For any $a\in N$, the [continuous map](../../../topology.md#continuous-map) $g\mapsto gag^{-1}$ takes [connected](../../../geometry-and-topology.md#connected-space) $G$ into the [finite set](../../../set.md#finite-set) $N$, so it is constant and equal to $a$. Thus

$$
\boxed{G\not\cong U(1)\Longrightarrow Z(G)\text{ is finite};\qquad N\lhd G, N\text{ closed and proper}\Longrightarrow N\subseteq Z(G).}
$$

Proper [closed subgroups](../../../topological-group.md#closed-subgroup) of the circle are finite as well, and of course central.

Now let $d\Phi$ be [surjective](../../../algebra.md#surjective-function). The [submersion theorem](../../../differential-geometry.md#submersion-theorem) makes $\Phi(G)$ contain an identity neighbourhood in $H$, so it is an [open subgroup](../../../topological-group.md#open-subgroup). Since $H$ is [connected](../../../geometry-and-topology.md#connected-space), $\Phi(G)=H$. Its [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) $F$ is closed and normal. If $H$ is nontrivial, $F$ is proper and the preceding argument gives a finite central [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism); this also holds for $G\cong U(1)$, whose proper [closed subgroups](../../../topological-group.md#closed-subgroup) are finite. The Lie-group [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem) gives

$$
\boxed{H\cong G/F,\qquad F\subseteq Z(G)\text{ finite},\quad H\ne\{1\}.}
$$

If $H$ is trivial, the correct statement is instead $H=G/G$.

For the [Spin groups](../../../semisimple-lie-algebra.md#spin-group), use the real [Clifford algebra](../../../algebra.md#clifford-algebra) with $v^2=-\|v\|^2$. The [group](../../../group.md) $\operatorname{Spin}(m)$ consists of products of an [even number](../../../number-theory.md#even-number) of [unit vectors](../../../vector-space.md#unit-vector) inside its invertible even part. [Conjugation](../../../group-theory.md#conjugation) on the embedded $\mathbb R^m$ defines the standard double covering $\operatorname{Spin}(m)\to SO(m)$ with [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) $\{\pm1\}$. The Clifford relations show that a unit-vector reflection, with the usual twisted [conjugation](../../../group-theory.md#conjugation), is a hyperplane reflection; the even products give orientation-preserving transformations. The [Cartan–Dieudonné theorem](../../../linear-algebra.md#cartan-dieudonne-theorem) states that every [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) is a product of reflections, proving [surjectivity](../../../algebra.md#surjective-function). For $m\geq3$ this [connected](../../../geometry-and-topology.md#connected-space) covering [group](../../../group.md) is [simply connected](../../../algebraic-topology.md#simply-connected-space); $\operatorname{Spin}(2)$ is a circle.

Here is an explicit exterior-square construction of the requested six-dimensional map. Put $E=\mathbb C^4$ with its standard [Hermitian form](../../../linear-algebra.md#hermitian-form) and [volume](../../../geometry-and-topology.md#volume) $e_1\wedge e_2\wedge e_3\wedge e_4$. On $\Lambda^2E$, write $e_{ij}=e_i\wedge e_j$ and define an [antilinear map](../../../vector-space.md#antilinear-map) $J$ by

$$
Je_{12}=e_{34},\quad Je_{13}=-e_{24},\quad Je_{14}=e_{23},\quad
Je_{34}=e_{12},\quad Je_{24}=-e_{13},\quad Je_{23}=e_{14}.
$$

It satisfies $J^2=1$. Intrinsically, if $u\wedge v=B(u,v)\,\mathrm{vol}$ and the [Hermitian inner product](../../../linear-algebra.md#hermitian-form) $h$ is [linear](../../../vector-space.md#linearity) in its first variable, then $B(u,Jv)=h(u,v)$. Because $SU(4)$ preserves both $B$ and $h$, it commutes with $J$. This is the [real structure of the SU4 exterior square](../../../semisimple-lie-algebra.md#real-structure-of-the-su4-exterior-square).

The fixed space $W$ has the following real [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), with all vectors divided by $\sqrt2$:

$$
e_{12}+e_{34},\quad i(e_{12}-e_{34}),\quad
e_{13}-e_{24},\quad i(e_{13}+e_{24}),\quad
e_{14}+e_{23},\quad i(e_{14}-e_{23}).
$$

Thus $W$ is six-dimensional over $\mathbb R$, its complexification is $\Lambda^2E$, and the exterior-square action restricts to an [orthogonal representation](../../../representation-theory.md#orthogonal-representation) on $W$. Its [determinant](../../../linear-algebra.md#determinant) is one because $SU(4)$ is [connected](../../../geometry-and-topology.md#connected-space). We obtain $R:SU(4)\to SO(W)\cong SO(6)$.

To compute the [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism), diagonalize $g\in SU(4)$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $z_1,\ldots,z_4$. If $R(g)=I$, its complexified exterior-square action is the identity, hence $z_i z_j=1$ for every $i<j$. Comparing pairs shows that all $z_i$ are equal, and their common value has square one. A [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) with that single [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is scalar, so $\ker R=\{\pm I_4\}$. Conversely, those two [scalar matrices](../../../linear-algebra.md#scalar-matrix) plainly act trivially on the [exterior square](../../../linear-algebra.md#exterior-square).

The differential of $R$ is [injective](../../../algebra.md#injective-function) because its [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) is finite. Both [Lie algebras](../../../lie-algebra.md) have [dimension](../../../vector-space.md#dimension-vector-space) $15$, so the differential is an [isomorphism](../../../algebra.md#isomorphism). Its image is consequently open in [connected](../../../geometry-and-topology.md#connected-space) $SO(6)$, hence all of $SO(6)$. Therefore

$$
\boxed{SU(4)/\{\pm I_4\}\cong SO(6).}
$$

This also realizes $SU(4)$ as $\operatorname{Spin}(6)$, since $SU(4)$ is [simply connected](../../../algebraic-topology.md#simply-connected-space), by uniqueness of the [connected](../../../geometry-and-topology.md#connected-space) [simply connected](../../../algebraic-topology.md#simply-connected-space) covering [group](../../../group.md).

## 3

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $v=(v_1,v_2,v_3)$ define the [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix)

$$
\widehat v=\begin{pmatrix}0&-v_3&v_2\\v_3&0&-v_1\\-v_2&v_1&0\end{pmatrix}.
$$

Then $\widehat v x=v\times x$. This is a [linear isomorphism](../../../vector-space.md#linear-isomorphism) $\mathbb R^3\to\mathfrak{so}(3)$, with inverse $\phi(\xi)=(\xi_{32},\xi_{13},\xi_{21})$. Since rotations preserve the [cross product](../../../vector-space.md#cross-product),

$$
R\widehat vR^{-1}=\widehat{Rv}\qquad(R\in SO(3)).
$$

Thus $\phi$ intertwines the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) with the standard [representation](../../../representation-theory.md#group-representation). The vector triple-product identity gives, for every $x$,

$$
[\widehat v,\widehat w]x=v\times(w\times x)-w\times(v\times x)=(v\times w)\times x.
$$

Consequently $[\widehat v,\widehat w]=\widehat{v\times w}$ and the chosen normalization satisfies

$$
\boxed{\phi([\xi,\eta])=\phi(\xi)\times\phi(\eta).}
$$

No undetermined scale remains in this explicit [matrix](../../../vector-space.md#matrix) convention.

Identify $SU(2)$ with the [unit quaternions](../../../algebra.md#unit-quaternion) using

$$
q=z+w j\longmapsto\begin{pmatrix}z&w\\-\overline w&\overline z\end{pmatrix},\qquad |z|^2+|w|^2=1.
$$

The relations $jz=\overline z j$ and $j^2=-1$ verify multiplication, and every [matrix](../../../vector-space.md#matrix) in $SU(2)$ has this form. If $v$ is imaginary, then $\overline v=-v$. Quaternionic [conjugation](../../../group-theory.md#conjugation) reverses [product order](../../../set.md#product-order) and $q^{-1}=\overline q$, so

$$
\overline{qvq^{-1}}=q\overline v q^{-1}=-qvq^{-1}.
$$

Thus [conjugation](../../../group-theory.md#conjugation) preserves $\operatorname{Im}\mathbb H\cong\mathbb R^3$. Multiplicativity of the [quaternion](../../../algebra.md#quaternion) norm shows that this action preserves the [inner product](../../../linear-algebra.md#inner-product). The [unit quaternions](../../../algebra.md#unit-quaternion) form the [connected](../../../geometry-and-topology.md#connected-space) three-sphere, so its [determinant](../../../linear-algebra.md#determinant), equal to one at the identity, is always one. We obtain a homomorphism $C:SU(2)\to SO(3)$.

Its [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) consists of [unit quaternions](../../../algebra.md#unit-quaternion) commuting with every imaginary [quaternion](../../../algebra.md#quaternion). Commuting with both $i$ and $j$ forces a [quaternion](../../../algebra.md#quaternion) to be real, so the [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) is exactly $\{\pm1\}$. To prove [surjectivity](../../../algebra.md#surjective-function) explicitly, let $u$ be a unit imaginary [quaternion](../../../algebra.md#quaternion) and put $q=\cos(\theta/2)+u\sin(\theta/2)$. For imaginary $u,v$, multiplication satisfies $uv=-u\cdot v+u\times v$. Expanding $qvq^{-1}$ therefore gives

$$
qvq^{-1}=v\cos\theta+(u\times v)\sin\theta+u(u\cdot v)(1-\cos\theta).
$$

This is the [Rodrigues rotation formula](../../../mathematics.md#rodrigues-rotation-formula) about axis $u$. Every element of $SO(3)$ has such an axis-angle description: an odd-dimensional [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) of [determinant](../../../linear-algebra.md#determinant) one has an eigenvector of [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one, and its action on the perpendicular plane is a plane rotation. Hence $C$ is onto, and

$$
\boxed{SU(2)/\{\pm I_2\}\cong SO(3).}
$$

This is the quaternionic form of the [Adjoint double cover from SU(2) to SO(3)](../../../lie-theory.md#adjoint-double-cover-from-su-2-to-so-3). Its differential sends an imaginary [quaternion](../../../algebra.md#quaternion) $u$ to $2\widehat u$, because $[u,v]=2u\times v$, consistent with the bracket normalization used above.

## 4

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Put $V=\mathbb C^n$. We use [complete reducibility of compact-group representations](../../../representation-theory.md#complete-reducibility-of-compact-group-representations), and the highest-weight classification: the multiplicity of $V_\lambda$ in a completely [reducible representation](../../../representation-theory.md#reducible-representation) is the [dimension](../../../vector-space.md#dimension-vector-space) of its weight-$\lambda$ subspace killed by all [positive root](../../../semisimple-lie-algebra.md#positive-root) vectors. Each [irreducible](../../../representation-theory.md#irreducible-representation) summand contributes just its one-dimensional highest-weight line to that subspace.

Symmetrizing and antisymmetrizing the three tensor factors give [invariant subspaces](../../../representation-theory.md#invariant-subspace) $\operatorname{Sym}^3V$ and $\Lambda^3V$ of $V^{\otimes3}$. The vectors $e_1^{\otimes3}$ and $e_1\wedge e_2\wedge e_3$ are [highest-weight vectors](../../../semisimple-lie-algebra.md#highest-weight-vector) of [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $(3,0,\ldots,0)$ and $(1,1,1,0,\ldots,0)$ respectively. The unitary version of the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) is

$$
\dim V_\lambda=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}.
$$

It gives

$$
\dim V_{(3)}=\prod_{j=2}^n\frac{j+2}{j-1}=\binom{n+2}3,
\qquad
\dim V_{(1,1,1)}=\prod_{i=1}^3\frac{n-i+1}{4-i}=\binom n3.
$$

These are exactly the [dimensions](../../../vector-space.md#dimension-vector-space) of the third [symmetric power](../../../linear-algebra.md#symmetric-power) and [exterior power](../../../linear-algebra.md#exterior-power), so each is [irreducible](../../../representation-theory.md#irreducible-representation) and occurs once in those subspaces.

The [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $(2,1,0,\ldots,0)$ in $V^{\otimes3}$ has basis

$$
a=e_1\otimes e_1\otimes e_2,\quad
b=e_1\otimes e_2\otimes e_1,\quad
c=e_2\otimes e_1\otimes e_1.
$$

The only [positive root](../../../semisimple-lie-algebra.md#positive-root) vector that acts nontrivially on this [weight space](../../../semisimple-lie-algebra.md#weight-space) is $E_{12}$. Acting on the [tensor product](../../../linear-algebra.md#tensor-product) as the sum of its actions on the three factors, it sends each of $a,b,c$ to $e_1^{\otimes3}$. Consequently the [highest-weight vectors](../../../semisimple-lie-algebra.md#highest-weight-vector) in this space are precisely

$$
Aa+Bb+Cc\quad\text{with}\quad A+B+C=0.
$$

This is a two-dimensional space, so $V_{(2,1)}$ occurs exactly twice. Its [dimension](../../../vector-space.md#dimension-vector-space) is

$$
\dim V_{(2,1)}=2\prod_{j=3}^n\frac{j+1}{j-2}
=\frac{n(n^2-1)}3.
$$

The [dimensions](../../../vector-space.md#dimension-vector-space) of the summands already found add to

$$
\binom{n+2}3+\binom n3+2\frac{n(n^2-1)}3=n^3.
$$

Thus no other [irreducible](../../../representation-theory.md#irreducible-representation) summand can remain. We have proved the full decomposition

$$
\boxed{V^{\otimes3}\cong V_{(3,0,\ldots)}\oplus V_{(1,1,1,0,\ldots)}\oplus V_{(2,1,0,\ldots)}^{\oplus2}.}
$$

There are four summands counted with multiplicity and three distinct [isomorphism](../../../algebra.md#isomorphism) types.

For $n=2$, the exterior cube vanishes. The third [symmetric power](../../../linear-algebra.md#symmetric-power) still has [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $(3,0)$ and [dimension](../../../vector-space.md#dimension-vector-space) $4$, while the same two-dimensional highest-vector calculation gives two copies of the [representation](../../../representation-theory.md#group-representation) of [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $(2,1)$ and [dimension](../../../vector-space.md#dimension-vector-space) $2$. It is $\det\otimes V$, since a [determinant twist](../../../lie-theory.md#determinant-twist) shifts the standard [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $(1,0)$ to $(2,1)$. Hence

$$
\boxed{(\mathbb C^2)^{\otimes3}\cong\operatorname{Sym}^3\mathbb C^2\oplus(\det\otimes\mathbb C^2)^{\oplus2},\qquad8=4+2+2.}
$$

## 5

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Choose the [maximal torus](../../../lie-theory.md#maximal-torus) of $SO(2n)$ consisting of rotations in $n$ [orthogonal](../../../linear-algebra.md#orthogonal-vectors) planes, and write $z_i=e^{i\theta_i}$. In the complexified standard [representation](../../../representation-theory.md#group-representation) $E=\mathbb C^{2n}$ the [torus](../../../topology.md#torus) [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $z_1,z_1^{-1},\ldots,z_n,z_n^{-1}$, with [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $e_i,-e_i$. For $n\geq2$ the complexified [Lie algebra](../../../lie-algebra.md) has the [Dn root system](../../../semisimple-lie-algebra.md#dn-root-system) $\{\pm e_i\pm e_j:i<j\}$. The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) theorem splits this [Lie algebra](../../../lie-algebra.md) into its [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) and one-dimensional [root spaces](../../../semisimple-lie-algebra.md#root-space). The [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) contributes the zero [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) with multiplicity $n$. Therefore its [character](../../../representation-theory.md#character-of-a-representation) is

$$
\boxed{\chi_{\mathrm{ad}}(z)=n+\sum_{i<j}\left(z_i z_j+\frac{z_i}{z_j}+\frac{z_j}{z_i}+\frac1{z_i z_j}\right).}
$$

Take [positive roots](../../../semisimple-lie-algebra.md#positive-root) $e_i-e_j,e_i+e_j$ for $i<j$, so $\rho=(n-1,n-2,\ldots,0)$. For $n>2$ the [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) $\theta=e_1+e_2$ is a [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation): its [root vector](../../../semisimple-lie-algebra.md#root-vector) is killed by every [positive root](../../../semisimple-lie-algebra.md#positive-root) vector, since $\theta+\alpha$ is never a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) for positive $\alpha$. To verify irreducibility without relying on an unstated simplicity theorem, apply complete reducibility and compare [dimensions](../../../vector-space.md#dimension-vector-space). For the [Dn root system](../../../semisimple-lie-algebra.md#dn-root-system) the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) reads

$$
\dim V_\lambda=\prod_{i<j}\frac{(\lambda_i+\rho_i)^2-(\lambda_j+\rho_j)^2}{\rho_i^2-\rho_j^2}.
$$

For $\lambda=(1,1,0,\ldots,0)$ only pairs involving the first two indices change. With $s=0,\ldots,n-3$, cancellation gives

$$
\dim V_\theta
=\frac{2n-1}{2n-3}\prod_{s=0}^{n-3}\frac{n^2-s^2}{(n-2)^2-s^2}
=\frac{2n-1}{2n-3}\left(\frac{n(n-1)}2\right)\left(\frac{2(2n-3)}{n-1}\right)
=n(2n-1).
$$

This is exactly $\dim\mathfrak{so}_{2n}(\mathbb C)$, so the [irreducible](../../../representation-theory.md#irreducible-representation) summand containing the [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) exhausts the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Thus **for $n>2$ the complexified [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is [irreducible](../../../representation-theory.md#irreducible-representation), with [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $e_1+e_2$**.

For $n=2$, the [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) split into the two independent systems $\{\pm(e_1+e_2)\}$ and $\{\pm(e_1-e_2)\}$. The [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) splits into two [irreducibles](../../../representation-theory.md#irreducible-representation) of [dimension](../../../vector-space.md#dimension-vector-space) three, with respective [highest weights](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $(1,1)$ and $(1,-1)$. Equivalently these are the self-dual and anti-self-dual exterior two-forms in four [dimensions](../../../vector-space.md#dimension-vector-space). Their [characters](../../../representation-theory.md#character-of-a-representation) are

$$
1+z_1z_2+(z_1z_2)^{-1},\qquad
1+z_1/z_2+z_2/z_1.
$$

They add to the displayed adjoint [character](../../../representation-theory.md#character-of-a-representation). This agrees with the [Chiral decomposition of the complexified so4 Lie algebra](../../../semisimple-lie-algebra.md#chiral-decomposition-of-the-complexified-so4-lie-algebra).

For a direct [character](../../../representation-theory.md#character-of-a-representation) comparison, put $s(z)=\sum_i(z_i+z_i^{-1})$. The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) formula for an [exterior square](../../../linear-algebra.md#exterior-square) gives

$$
\chi_{\Lambda^2 E}(z)=\frac12\left(s(z)^2-\sum_i(z_i^2+z_i^{-2})\right)
=n+\sum_{i<j}\left(z_i z_j+z_i/z_j+z_j/z_i+(z_i z_j)^{-1}\right).
$$

This is precisely $\chi_{\mathrm{ad}}$. More intrinsically, let $B$ be the nondegenerate [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) preserved by $SO(2n)$ and define

$$
\Psi(u\wedge v)(x)=B(v,x)u-B(u,x)v.
$$

This endomorphism is skew with respect to $B$, so $\Psi$ maps $\Lambda^2E$ to $\mathfrak{so}(E,B)$. In an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) the bivectors $e_i\wedge e_j$ map to a basis of skew [skew-symmetric matrices](../../../linear-algebra.md#skew-symmetric-matrix), proving that it is an [isomorphism](../../../algebra.md#isomorphism). Since $B$ is invariant,

$$
\Psi(gu\wedge gv)=g\Psi(u\wedge v)g^{-1}.
$$

Thus **the [exterior square](../../../linear-algebra.md#exterior-square) and the complexified [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) are naturally isomorphic**, explaining the [character](../../../representation-theory.md#character-of-a-representation) equality without a [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) calculation.

The [symmetric square](../../../linear-algebra.md#symmetric-square) is not [irreducible](../../../representation-theory.md#irreducible-representation). The [inverse metric](../../../general-relativity.md#inverse-metric) tensor $\Omega$ is a nonzero invariant vector, and contraction with $B$ splits off its trivial line:

$$
\operatorname{Sym}^2E=\mathbb C\Omega\oplus\operatorname{Sym}^2_0E.
$$

The contraction sends $\Omega$ to $2n$, so this is indeed a [direct sum](../../../vector-space.md#direct-sum). A [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) $f_1\otimes f_1$, where $f_1$ has [torus](../../../topology.md#torus) [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $e_1$, lies in the traceless part because $B(f_1,f_1)=0$, and has [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $2e_1$. The same [dimension](../../../vector-space.md#dimension-vector-space) formula gives, for $n\geq2$,

$$
\dim V_{2e_1}=\prod_{s=0}^{n-2}\frac{(n+1)^2-s^2}{(n-1)^2-s^2}
=\left(\frac{n(n+1)}2\right)\left(\frac{2(2n-1)}n\right)
=(n+1)(2n-1).
$$

This equals $\dim\operatorname{Sym}^2E-1=n(2n+1)-1$. Complete reducibility therefore proves that the traceless part is [irreducible](../../../representation-theory.md#irreducible-representation), including the dimension-nine case for $SO(4)$. In particular,

$$
\boxed{\operatorname{Sym}^2(\mathbb C^{2n})\cong\mathbf1\oplus V_{2e_1}\quad(n\geq2),\quad\text{so it is reducible}.}
$$

If the circle case $n=1$ is included, the adjoint [character](../../../representation-theory.md#character-of-a-representation) is $1$ and the [symmetric square](../../../linear-algebra.md#symmetric-square) instead has three one-dimensional [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $2,0,-2$.

## 6

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="6/1">1</h3>

↑ **Parent:** [6](#6)

<h4 id="6/1/solution">Solution</h4>

↑ **Parent:** [1](#6/1)

The printed identity has a sign error. With the defined [Kostant partition function](../../../semisimple-lie-algebra.md#kostant-partition-function) and the exponent $e^{-\nu}$, the cancelling factors must be $1-e^{-\alpha}$. This is already visible for $SU(2)$ with [positive root](../../../semisimple-lie-algebra.md#positive-root) $\alpha$: the formal series $\sum_{k\geq0}e^{-k\alpha}$ multiplied by $1-e^\alpha$ is $-e^\alpha$, not $1$.

For the corrected formula, a partition of $\nu$ is a tuple of [nonnegative integers](../../../arithmetic.md#natural-number) $(k_\alpha)_{\alpha>0}$ satisfying $\nu=\sum_{\alpha>0}k_\alpha\alpha$. The order of summands is not counted. Multiplying the formal [geometric series](../../../real-analysis.md#geometric-series) yields

$$
\prod_{\alpha>0}\left(\sum_{k\geq0}e^{-k\alpha}\right)
=\sum_\nu p(\nu)e^{-\nu}.
$$

This product is coefficientwise meaningful. Choose a [linear functional](../../../linear-algebra.md#linear-functional) strictly positive on every [positive root](../../../semisimple-lie-algebra.md#positive-root). For a fixed $\nu$ it bounds each $k_\alpha$, so only finitely many tuples contribute. We are working in the completion supported on the negative positive-root cone, not claiming convergence of an ordinary [Fourier series](../../../fourier-series.md) on the [torus](../../../topology.md#torus).

Each [geometric series](../../../real-analysis.md#geometric-series) cancels its factor $1-e^{-\alpha}$, proving

$$
\boxed{\left(\sum_\nu p(\nu)e^{-\nu}\right)\prod_{\alpha>0}(1-e^{-\alpha})=1.}
$$

Equivalently, reversing all the exponential signs gives $(\sum_\nu p(\nu)e^{\nu})\prod_{\alpha>0}(1-e^\alpha)=1$ in the opposite completion. More generally, if $N$ is the number of [positive roots](../../../semisimple-lie-algebra.md#positive-root), the expression literally printed in the paper equals

$$
(-1)^N e^{2\rho},
$$

since $\prod_{\alpha>0}(1-e^\alpha)=(-1)^N e^{2\rho}\prod_{\alpha>0}(1-e^{-\alpha})$. Thus the correction is substantive, not merely a choice of Fourier convention.

<h3 id="6/2">2</h3>

↑ **Parent:** [6](#6)

<h4 id="6/2/solution">Solution</h4>

↑ **Parent:** [2](#6/2)

Use the corrected [generating series of the Kostant partition function](../../../semisimple-lie-algebra.md#generating-series-of-the-kostant-partition-function) and the permitted [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula):

$$
\chi_\lambda
=\left(\sum_{w\in W}\varepsilon(w)e^{w(\lambda+\rho)-\rho}\right)
\left(\sum_\nu p(\nu)e^{-\nu}\right).
$$

For a fixed $w$, the coefficient of $e^\mu$ arises exactly when

$$
w(\lambda+\rho)-\rho-\nu=\mu,
\qquad\text{that is,}\qquad
\nu=w(\lambda+\rho)-(\mu+\rho).
$$

There are only finitely many Weyl-group terms, and the [partition function](../../../statistical-physics.md#canonical-partition-function) vanishes outside the cone of nonnegative [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) combinations. [Coefficient extraction](../../../polynomial.md#coefficient-extraction) is therefore legitimate in the formal completion used in the preceding part. Summing the signed contributions proves

$$
\boxed{m_\lambda(\mu)=\sum_{w\in W}\varepsilon(w)\,p\bigl(w(\lambda+\rho)-(\mu+\rho)\bigr).}
$$

This proves the [Kostant multiplicity formula](../../../semisimple-lie-algebra.md#kostant-multiplicity-formula) for every [compact](../../../topology.md#compact-space) [connected](../../../geometry-and-topology.md#connected-space) [Lie group](../../../lie-theory.md#lie-group), not just the [unitary groups](../../../topological-group.md#unitary-group). In the presence of a central [torus](../../../topology.md#torus), [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) have zero central component, so the [partition function](../../../statistical-physics.md#canonical-partition-function) automatically gives zero for any incompatible central [weight](../../../semisimple-lie-algebra.md#weight-representation-theory). Also $\rho$ need not itself be an integral [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) for the given global [group](../../../group.md): $w\rho-\rho$ always belongs to the [root lattice](../../../semisimple-lie-algebra.md#root-lattice), so every argument in the formula is nevertheless integral whenever $\lambda$ and $\mu$ are integral [group](../../../group.md) [weights](../../../semisimple-lie-algebra.md#weight-representation-theory).

As a normalization check, for $SU(2)$ write a [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) as the [nonnegative integer](../../../arithmetic.md#natural-number) $\ell$, with [positive root](../../../semisimple-lie-algebra.md#positive-root) $2$ and $\rho=1$. The two Weyl-group terms give

$$
m_\ell(\mu)=p(\ell-\mu)-p(-\ell-\mu-2).
$$

Since $p(a)=1$ precisely when $a$ is even and nonnegative, this is one for $\mu=\ell,\ell-2,\ldots,-\ell$ and zero otherwise, including the cancellation below the lowest [weight](../../../semisimple-lie-algebra.md#weight-representation-theory). This recovers the full familiar [weight string](../../../semisimple-lie-algebra.md#weight-string).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
