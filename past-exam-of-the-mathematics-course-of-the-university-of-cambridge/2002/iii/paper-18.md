# Paper 18

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper18.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper18.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
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

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The displayed torus-only [Weyl integration formula](../../../lie-theory.md#weyl-integration-formula) needs $\varphi$ to be a [class function](../../../representation-theory.md#class-function), meaning $\varphi(xgx^{-1})=\varphi(g)$. This hypothesis is implicit in the usual formula but is not printed here. We prove the general version for a continuous function, then specialize:

$$
\int_G\varphi(g)\,dg
=\frac1{|W|}\int_T\int_{G/T}\varphi(xtx^{-1})\,d\mu(xT)\,|\Delta(t)|^2\,dt.
$$

Here $dg$ and $dt$ are probability [Haar measures](../../../measure-theory.md#haar-measure); $d\mu$ is the invariant probability measure on the [homogeneous space](../../../lie-theory.md#homogeneous-space) $G/T$; and $W=N_G(T)/T$ is the finite [Weyl group](../../../semisimple-lie-algebra.md#weyl-group).

We use the following standard maximal-torus facts, as permitted: every element of a connected [compact Lie group](../../../lie-theory.md#compact-lie-group) lies in some [maximal torus](../../../lie-theory.md#maximal-torus); all maximal tori are conjugate; two elements of a fixed $T$ are conjugate in $G$ exactly when they are in the same $W$-orbit; and the complexified [Lie algebra](../../../lie-algebra.md) decomposes into $\mathfrak t_{\mathbb C}$ and one-dimensional [root spaces](../../../semisimple-lie-algebra.md#root-space). Opposite [roots of a root system](../../../semisimple-lie-algebra.md#root-of-a-root-system) give real two-dimensional planes in $\mathfrak t^\perp$. At an element $t$ for which no root character has value one, the identity component of its centralizer is $T$.

Choose a positive [root system](../../../semisimple-lie-algebra.md#root-system) $\Phi^+$. Regard each root $\alpha$ as a [character](../../../representation-theory.md#character-of-a-representation) $\alpha:T\to U(1)$ through the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). A convenient globally defined denominator is

$$
\Delta_0(t)=\prod_{\alpha\in\Phi^+}(1-\alpha(t)^{-1}).
$$

The usual [Weyl denominator](../../../semisimple-lie-algebra.md#weyl-denominator) additionally has a unit-modulus factor $e^\rho(t)$, with $\rho$ half the sum of positive roots. Where that half-weight is not a global torus character, it may be interpreted on a covering torus; the squared modulus is nevertheless unambiguous. In either convention,

$$
|\Delta(t)|^2=|\Delta_0(t)|^2
=\prod_{\alpha\in\Phi^+}|1-\alpha(t)|^2.
$$

Average an [inner product](../../../linear-algebra.md#inner-product) on $\mathfrak g$ over the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) to make it invariant. It defines a bi-invariant [Riemannian metric](../../../differential-geometry.md#riemannian-metric) on $G$ and the quotient metric on $G/T$. Consider the conjugation map

$$
q:G/T\times T\to G,\qquad q(xT,t)=xtx^{-1}.
$$

At $(T,t)$, identify the source tangent directions with $X\in\mathfrak t^\perp$ and $Y\in\mathfrak t$, and translate the target tangent vector to the identity by $t^{-1}$. Differentiating gives

$$
dq_{(T,t)}(X,Y)=(\operatorname{Ad}(t^{-1})-I)X+Y.
$$

The two summands are orthogonal. On a real root plane, $\operatorname{Ad}(t^{-1})$ is a rotation with complex eigenvalues $\alpha(t)^{-1},\alpha(t)$. Thus the absolute real [Jacobian determinant](../../../calculus.md#jacobian-determinant) on this plane is $|1-\alpha(t)|^2$. The torus direction contributes one. Therefore the [conjugation Jacobian for a compact Lie group](../../../lie-theory.md#conjugation-jacobian-for-a-compact-lie-group) is

$$
\boxed{J_q(t)=|\Delta(t)|^2.}
$$

This is also the Jacobian for the normalized measures: the Riemannian submersion has fibers isometric to $T$, so $\operatorname{vol}(G)=\operatorname{vol}(G/T)\operatorname{vol}(T)$; the probability-volume normalization factors cancel.

Let $T_{\rm reg}$ be the elements for which $J_q\neq0$. The restriction of $q$ is a local [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) onto the regular elements of $G$. It is $|W|$-to-one. Indeed, fixing $t_0\in T_{\rm reg}$, any pair with $xtx^{-1}=t_0$ has $xTx^{-1}=T$, because conjugation identifies the identity components of the two centralizers. Thus $x\in N_G(T)$, and there is exactly one pair $(xT,x^{-1}t_0x)$ for each coset in $N_G(T)/T$. This argument does not require the full centralizer of $t_0$ to be connected.

The nonregular locus has measure zero. In $T$ it is a finite union of sets $\alpha(t)=1$ of smaller dimension; their conjugation images are images of smaller-dimensional manifolds under $q$, and hence have zero volume in $G$. The change-of-variables formula for the regular covering therefore gives

$$
|W|\int_G\varphi(g)\,dg
=\int_T\int_{G/T}\varphi(xtx^{-1})\,d\mu(xT)\,|\Delta(t)|^2\,dt.
$$

For a [class function](../../../representation-theory.md#class-function), the inner integral is $\varphi(t)$, proving the required formula with its correct hypothesis.

Without conjugation invariance, the torus-only expression can be false. For $G=SU(2)$ with diagonal $T$, take $\varphi(g)=|g_{12}|^2$. It vanishes on $T$, whereas its group integral is $1/2$: the two squared coordinates of a Haar-distributed unit column have equal means and sum to one. Thus the conjugacy average cannot simply be dropped.

## 2

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $V=\mathbb C^n$ and $m\geq0$. Identify the [symmetric power](../../../linear-algebra.md#symmetric-power) $\operatorname{Sym}^mV$ with the degree-$m$ part of the symmetric algebra on the basis vectors $e_1,\ldots,e_n$, using formal variables $x_i$ for these vectors. Its monomial basis is

$$
x^a=x_1^{a_1}\cdots x_n^{a_n},\qquad a_i\geq0,\qquad\sum_i a_i=m.
$$

The diagonal [maximal torus](../../../lie-theory.md#maximal-torus) of the [unitary group](../../../topological-group.md#unitary-group) acts on this monomial by the character $z_1^{a_1}\cdots z_n^{a_n}$. Distinct tuples give distinct characters, so each [weight space](../../../semisimple-lie-algebra.md#weight-space) is one-dimensional.

Suppose $M$ is a nonzero invariant complex subspace. For a nonzero vector $w\in M$, select a monomial with nonzero coefficient and extract it by torus averaging:

$$
\int_T z_1^{-a_1}\cdots z_n^{-a_n}\,t\cdot w\,dt.
$$

[Fourier orthogonality](../../../fourier-series.md#fourier-orthogonality) makes this a nonzero scalar multiple of $x^a$. It belongs to $M$, so $M$ contains a monomial.

Differentiating the [unitary group](../../../topological-group.md#unitary-group) action makes $M$ invariant under $\mathfrak u(n)$ and hence under its complexification $\mathfrak{gl}_n(\mathbb C)$. The matrix unit $E_{ij}$ replaces an occurrence of $e_j$ by $e_i$, so its action on the symmetric algebra is

$$
E_{ij}\cdot x^a=x_i\partial_{x_j}x^a
=a_jx^{a+e_i-e_j}.
$$

Whenever $a_j>0$, this transfers one unit of degree from coordinate $j$ to coordinate $i$ with a nonzero coefficient. Starting with any monomial, such transfers can produce every other tuple of nonnegative integers summing to $m$. Thus $M$ contains every monomial and equals $\operatorname{Sym}^mV$.

Consequently

$$
\boxed{\operatorname{Sym}^m\mathbb C^n\text{ is irreducible for every }m\geq0.}
$$

For $m=0$ this is the one-dimensional trivial representation, and for $n=1$ every symmetric power is also one-dimensional. This [weight-transfer proof of irreducibility of symmetric powers](../../../linear-algebra.md#weight-transfer-proof-of-irreducibility-of-symmetric-powers) uses neither the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) nor the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula), so no unproved dimension formula enters the argument.

## 3

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write the diagonal [maximal torus](../../../lie-theory.md#maximal-torus) of $U(n)$ as $t=\operatorname{diag}(z_1,\ldots,z_n)$, $|z_i|=1$, and let $\delta=(n-1,n-2,\ldots,0)$. Irreducible complex representations are indexed by dominant integer tuples $\lambda_1\geq\cdots\geq\lambda_n$, their [highest weights](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation). The [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) in integer-exponent form is

$$
\boxed{\chi_\lambda(t)
=\frac{\det(z_i^{\lambda_j+n-j})_{i,j=1}^n}
{\det(z_i^{n-j})_{i,j=1}^n}.}
$$

The ratio initially uses distinct $z_i$, and extends to repeated eigenvalues by continuity. Every unitary matrix is conjugate to such a diagonal matrix, so this determines the [character](../../../representation-theory.md#character-of-a-representation) on the entire group. The shift $\delta$ differs from the usual [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) $\rho=((n-1)/2,(n-3)/2,\ldots,(1-n)/2)$ by a multiple of $(1,\ldots,1)$; the corresponding determinant factors cancel between numerator and denominator.

We first justify the highest-weight information needed in the proof. Restriction to the torus splits a representation into integer [weight spaces](../../../semisimple-lie-algebra.md#weight-space). In an irreducible representation choose a lexicographically largest weight $\lambda$ and a nonzero vector $v$ of that weight. A matrix unit $E_{ij}$ with $i<j$ raises the weight by $e_i-e_j$, so it annihilates $v$. The character is invariant under permutations of diagonal coordinates, because permutation matrices conjugate the torus. Hence permutations of $\lambda$ are also weights, and lexical maximality forces $\lambda_1\geq\cdots\geq\lambda_n$.

Irreducibility implies that $v$ generates the representation under the complexified [Lie algebra](../../../lie-algebra.md). Indeed, a Lie-algebra invariant subspace is preserved by exponentials of skew-Hermitian matrices, which generate $U(n)$. Reorder any product of matrix units into lower-triangular units, diagonal units and upper-triangular units, using

$$
[E_{ij},E_{kl}]=\delta_{jk}E_{il}-\delta_{li}E_{kj}.
$$

Induction on length and on the number of out-of-order pairs gives the required spanning version of the [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem). Upper-triangular units kill $v$, and diagonal units act by scalars. Every nonempty product of lower-triangular units lowers its weight by a nonzero sum of positive roots. Therefore the top weight space is exactly $\mathbb Cv$, and its multiplicity is one. This supplies the leading coefficient without assuming a character formula.

For completeness, every dominant integer tuple occurs. Put $d_j=\lambda_j-\lambda_{j+1}\geq0$ and form the representation

$$
(\det)^{\lambda_n}\otimes
\bigotimes_{j=1}^{n-1}(\Lambda^j\mathbb C^n)^{\otimes d_j}.
$$

Its lexicographically highest weight is $\lambda$, with one-dimensional highest space, represented by the tensor products of $e_1\wedge\cdots\wedge e_j$. A negative determinant exponent is a legitimate one-dimensional unitary-group character. Averaging an [inner product](../../../linear-algebra.md#inner-product) over normalized [Haar measure](../../../measure-theory.md#haar-measure) gives invariant orthogonal complements, so the tensor representation splits into irreducible summands. One of them has highest weight $\lambda$. Uniqueness will also follow from the formula and [Schur orthogonality relations](../../../representation-theory.md#schur-orthogonality-relations).

Define the alternant $A_\kappa(z)=\det(z_i^{\kappa_j})$ for a strictly decreasing integer tuple $\kappa$. The denominator

$$
A_\delta(z)=\prod_{i<j}(z_i-z_j)
$$

is the [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant), and its modulus is the denominator modulus in the [Weyl integration formula](../../../lie-theory.md#weyl-integration-formula). The [Laurent polynomial](../../../polynomial.md#laurent-polynomial) $\chi_\lambda A_\delta$ is alternating. Any alternating Laurent polynomial decomposes as a finite sum

$$
\chi_\lambda A_\delta=\sum_\kappa c_\kappa A_\kappa:
$$

monomials with repeated exponents have zero coefficient, and the remaining permutation orbits are indexed uniquely by strictly decreasing tuples.

The lexicographically highest monomial in the product is $z^{\lambda+\delta}$ with coefficient one. Indeed, the highest monomial of the character is $z^\lambda$ with coefficient one, and the unique lexical maximum among permutations of $\delta$ is $\delta$ itself. It follows that $c_{\lambda+\delta}=1$.

[Fourier orthogonality](../../../fourier-series.md#fourier-orthogonality) on the torus, whose probability measure is $\prod_i d\theta_i/(2\pi)$, gives [alternant orthogonality on a unitary torus](../../../semisimple-lie-algebra.md#alternant-orthogonality-on-a-unitary-torus):

$$
\int_T A_\kappa\overline{A_\eta}\,dt
=n!\,\delta_{\kappa\eta}.
$$

Expand both determinants: an integral survives exactly when the two exponent tuples are identical up to permutation. Strict decreasing order then forces $\kappa=\eta$, and its $n!$ matching terms each contribute one.

Finally, [Schur orthogonality relations](../../../representation-theory.md#schur-orthogonality-relations) give $\int_{U(n)}|\chi_\lambda|^2=1$. Applying the allowed [Weyl integration formula](../../../lie-theory.md#weyl-integration-formula) to this class function gives

$$
1=\frac1{n!}\int_T|\chi_\lambda A_\delta|^2\,dt
=\sum_\kappa|c_\kappa|^2.
$$

Since the coefficient $c_{\lambda+\delta}$ already equals one, every other coefficient vanishes. Thus $\chi_\lambda A_\delta=A_{\lambda+\delta}$, proving the formula. If two irreducible representations had the same highest weight, their characters would now coincide; the [Schur orthogonality relations](../../../representation-theory.md#schur-orthogonality-relations) imply that they are isomorphic. Apparent singularities at repeated diagonal eigenvalues are removable because the quotient equals the actual finite Laurent-polynomial character. No dimension formula has been assumed.

## 4

↑ **Parent:** [Paper 18](paper-18.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $v_{1,+}=e_1+ie_2$, $v_{1,-}=e_1-ie_2$, $v_{2,+}=e_3+ie_4$, $v_{2,-}=e_3-ie_4$ and $v_0=e_5$. Direct multiplication by the printed rotation blocks gives their torus eigenvalues

$$
e^{ix_1},\ e^{-ix_1},\ e^{ix_2},\ e^{-ix_2},\ 1.
$$

Thus the differentiated [weights of a representation](../../../semisimple-lie-algebra.md#weight-of-a-representation) are $ix_1,-ix_1,ix_2,-ix_2,0$, with this sign convention fixed by the given matrix blocks.

A wedge of two distinct eigenvectors has the product eigenvalue, so its differentiated weight is the sum. The ten vectors in a [basis](../../../vector-space.md#basis) of the [exterior square](../../../linear-algebra.md#exterior-square) split into three groups:

$$
\begin{array}{c|c|c}
\text{vectors}&\text{weights}&\text{number}\\
 v_{1,\sigma}\wedge v_{2,\tau}&i(\sigma x_1+\tau x_2),\ \sigma,\tau=\pm1&4\\
 v_{j,\sigma}\wedge v_0&i\sigma x_j,\ j=1,2,\ \sigma=\pm1&4\\
 v_{1,+}\wedge v_{1,-},\ v_{2,+}\wedge v_{2,-}&0&2
\end{array}
$$

The eight nonzero weights are distinct, so each has multiplicity one; the zero [weight space](../../../semisimple-lie-algebra.md#weight-space) has dimension two. The multiplicities add to $\binom52=10$, accounting for the entire representation.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a real [inner product space](../../../linear-algebra.md#inner-product-space) $V=\mathbb R^5$, define

$$
\Phi(u\wedge v)(w)=\langle v,w\rangle u-\langle u,w\rangle v.
$$

This map takes values in the [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra): its matrices are skew-symmetric. It sends $e_i\wedge e_j$ to $E_{ij}-E_{ji}$, so it is an isomorphism between the two ten-dimensional spaces. For $g\in SO(5)$, invariance of the inner product gives

$$
\Phi(gu\wedge gv)=g\Phi(u\wedge v)g^{-1}.
$$

This proves the [exterior square realization of the orthogonal adjoint representation](../../../semisimple-lie-algebra.md#exterior-square-realization-of-the-orthogonal-adjoint-representation), including equivariance, rather than merely matching dimensions.

After complexification, part (a) is therefore the [weight decomposition](../../../semisimple-lie-algebra.md#weight-decomposition) of the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Its zero [weight space](../../../semisimple-lie-algebra.md#weight-space) is the complex centralizer of $\mathfrak t$. The two zero-weight wedges are nonzero multiples of $e_1\wedge e_2$ and $e_3\wedge e_4$, which map under $\Phi$ to the two infinitesimal rotation generators of $T$. Hence

$$
Z_{\mathfrak{so}(5)}(\mathfrak t)=\mathfrak t.
$$

If a larger torus contained $T$, its Lie algebra would commute with $\mathfrak t$ and therefore lie in $\mathfrak t$. Equality of Lie algebras and connectedness of both tori force equality of the groups. Thus **$T$ is a maximal torus**.

Let $\varepsilon_j$ denote the real coordinate functional $x_j$. In the real weight convention, with the common factor $i$ removed from the differentiated torus weights, the [root system](../../../semisimple-lie-algebra.md#root-system) is

$$
\boxed{\Phi=\{\pm\varepsilon_1,\pm\varepsilon_2,
\pm(\varepsilon_1+\varepsilon_2),\pm(\varepsilon_1-\varepsilon_2)\}.}
$$

These are the [roots of a root system](../../../semisimple-lie-algebra.md#root-of-a-root-system) of type [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system). In the imaginary-valued compact Lie-algebra convention each displayed functional is multiplied by $i$. Every root space is one-dimensional, as part (a) explicitly shows.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [root hyperplanes](../../../semisimple-lie-algebra.md#root-hyperplane) are $x_1=0$, $x_2=0$, $x_1=x_2$ and $x_1=-x_2$. Their reflections are coordinate sign changes, coordinate interchange and a signed interchange. They generate all signed permutations of the two coordinates:

$$
\boxed{W\cong(\mathbb Z/2\mathbb Z)^2\rtimes S_2,\qquad |W|=8.}
$$

Geometrically this is the dihedral symmetry group of a square, with order eight. It preserves both the four short roots and the four long roots of the [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system).

Representatives in $SO(5)$ can be given explicitly. The matrix

$$
D_1=\operatorname{diag}(1,-1,1,1,-1)
$$

has determinant one and conjugates the first rotation block to its inverse, giving $(x_1,x_2)\mapsto(-x_1,x_2)$. The matrix $D_2=\operatorname{diag}(1,1,1,-1,-1)$ similarly reverses $x_2$. Flipping the fifth coordinate compensates for the determinant of the planar reflection.

The permutation matrix

$$
P=\begin{pmatrix}
0&0&1&0&0\\
0&0&0&1&0\\
1&0&0&0&0\\
0&1&0&0&0\\
0&0&0&0&1
\end{pmatrix}
$$

swaps the two coordinate planes. Its permutation is $(1\ 3)(2\ 4)$, so its determinant is also one. Conjugation gives $(x_1,x_2)\mapsto(x_2,x_1)$, the reflection in $x_1=x_2$. These elements normalize $T$, and $P,D_1$ generate all eight Weyl actions. For example, $PD_1$ induces $(x_1,x_2)\mapsto(x_2,-x_1)$, a quarter-turn, and $D_1D_2$ induces the half-turn. The representatives supply the specified reflections and their typical products inside the actual special orthogonal group.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Choose positive roots

$$
\Phi^+=\{\varepsilon_1-\varepsilon_2,\varepsilon_2,
\varepsilon_1,\varepsilon_1+\varepsilon_2\}.
$$

The corresponding simple roots are $\varepsilon_1-\varepsilon_2$ and $\varepsilon_2$. The vector $v_{1,+}\wedge v_{2,+}$ has weight $\lambda=\varepsilon_1+\varepsilon_2$. Adding any positive root to this weight produces a weight absent from part (a), so every positive root vector annihilates it. It is consequently a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) with highest weight $\lambda$.

A representation of a [compact Lie group](../../../lie-theory.md#compact-lie-group) is completely reducible: Haar averaging makes an inner product invariant, and orthogonal complements of invariant subspaces remain invariant. Therefore the [exterior square](../../../linear-algebra.md#exterior-square) contains an irreducible summand $L_\lambda$ of this highest weight. This can also be seen by projecting the displayed highest-weight vector into irreducible summands; a nonzero projection remains annihilated by all positive root vectors and has the same weight. Its multiplicity is one because the weight space at $\lambda$ is one-dimensional.

Use the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula), expressly allowed in this part:

$$
\dim L_\lambda=\prod_{\alpha\in\Phi^+}
\frac{\langle\lambda+\rho,\alpha\rangle}{\langle\rho,\alpha\rangle}.
$$

Here $L_\lambda$ is the irreducible highest-weight representation, $\Phi^+$ is the chosen positive root system, $\rho$ is half its sum, and the pairing is the invariant Euclidean inner product on the real weight plane, with $\varepsilon_1,\varepsilon_2$ orthonormal. Using coroots instead gives the same ratio because the length factor cancels for each root. In this convention,

$$
\rho=\tfrac32\varepsilon_1+\tfrac12\varepsilon_2,
\qquad\lambda+\rho=\tfrac52\varepsilon_1+\tfrac32\varepsilon_2.
$$

The four factors, in the listed positive-root order, are respectively

$$
\frac{1}{1},\qquad\frac{3/2}{1/2},\qquad
\frac{5/2}{3/2},\qquad\frac{4}{2}.
$$

Their product is $10$. Since $\dim\Lambda^2\mathbb C^5=\binom52=10$, this irreducible summand occupies the entire exterior square. Hence

$$
\boxed{\Lambda^2\mathbb C^5\text{ is irreducible as an }SO(5)\text{-representation}.}
$$

The proof uses the dimension formula only where it is allowed, not in the symmetric-power argument of Question 2. Its [B2 adjoint representation weight diagram](../../../semisimple-lie-algebra.md#b2-adjoint-representation-weight-diagram) is exactly the eight roots and the double zero weight obtained above.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
