# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_302.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Over $\mathbb R$ or $\mathbb C$, a [Lie algebra](../../../lie-algebra.md) is a [vector space](../../../vector-space.md) with a [bilinear map](../../../linear-algebra.md#bilinear-map) $[\ ,\ ]$ which is alternating and obeys the [Jacobi identity](../../../lie-algebra.md#jacobi-identity):

$$
[X,X]=0,\qquad [X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]]=0.
$$

Bilinearity and alternation imply $[X,Y]=-[Y,X]$.

For a [Matrix Lie group](../../../lie-theory.md#matrix-lie-group), identify the [tangent space](../../../differential-geometry.md#tangent-space) $\mathfrak g=T_I G$ with derivatives $\gamma'(0)$ of smooth curves through $I$. Product curves show that the sum of two such derivatives is again tangent, and reparametrization supplies scalar multiples. In particular this is a real [vector space](../../../vector-space.md), even when the matrices have complex entries. For $X,Y\in\mathfrak g$, choose a curve $\gamma(s)$ with $\gamma'(0)=X$. Conjugating a curve with derivative $Y$ shows that

$$
\gamma(s)Y\gamma(s)^{-1}\in\mathfrak g\qquad\text{for every sufficiently small }s.
$$

Differentiate this curve in the finite-dimensional [vector space](../../../vector-space.md) $\mathfrak g$. The result is

$$
\boxed{[X,Y]=XY-YX\in\mathfrak g.}
$$

The matrix [commutator](../../../lie-algebra.md#commutator) is bilinear and alternating, and expanding the six terms proves its [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Thus this construction gives the [Lie algebra of a matrix Lie group](../../../lie-algebra.md#lie-algebra-of-a-matrix-lie-group), with the appropriate bracket, using actual group curves rather than an assumed commutator closure.

For the [unitary group](../../../topological-group.md#unitary-group), differentiating $\gamma(t)^\dagger\gamma(t)=I$ gives $X^\dagger+X=0$. Conversely, if $X^\dagger=-X$, then $e^{tX}$ is unitary and is a curve with derivative $X$. Consequently

$$
\boxed{\mathfrak u(N)=\{X:X^\dagger=-X\},\qquad\dim_{\mathbb R}\mathfrak u(N)=N^2.}
$$

This is the [unitary Lie algebra](../../../lie-algebra.md#unitary-lie-algebra). The diagonal entries are purely imaginary, contributing $N$ real parameters, and each upper off-diagonal entry contributes two real parameters. A [matrix-unit basis of the unitary Lie algebra](../../../lie-algebra.md#matrix-unit-basis-of-the-unitary-lie-algebra) is

$$
 iE^{(i,i)}\quad(1\leq i\leq N),\qquad E^{(i,j)}-E^{(j,i)},\quad i(E^{(i,j)}+E^{(j,i)})\quad(1\leq i<j\leq N).
$$

These $N+2\binom N2=N^2$ anti-Hermitian [matrix units](../../../vector-space.md#matrix-unit) and their combinations are linearly independent over $\mathbb R$ and span every allowed entry.

The symplectic stabilizer is a [subgroup](../../../group.md#subgroup): the identity preserves $J$, and if $MJM^T=J$ and $NJN^T=J$, then

$$
(MN)J(MN)^T=M(NJN^T)M^T=J.
$$

Multiplying $MJM^T=J$ on the left by $M^{-1}$ and on the right by $M^{-T}$ gives $M^{-1}JM^{-T}=J$. Products and inverses remain unitary. This is the [compact symplectic group](../../../topological-group.md#compact-symplectic-group), often denoted $USp(2n)$ or $Sp(n)$.

Differentiating the stabilizer equation gives $XJ+JX^T=0$. For $X=\begin{pmatrix}A&B\\C&D\end{pmatrix}$, this says

$$
B^T=B,\qquad C^T=C,\qquad D=-A^T.
$$

Together with $X^\dagger=-X$, these are equivalently

$$
\boxed{X=\begin{pmatrix}A&B\\-\overline B&\overline A\end{pmatrix},\qquad A^\dagger=-A,\quad B^T=B.}
$$

These conditions are also sufficient: $e^{tX}$ is unitary, and

$$
\frac{d}{dt}\bigl(e^{tX}Je^{tX^T}\bigr)=e^{tX}(XJ+JX^T)e^{tX^T}=0.
$$

Hence it stays in the subgroup. They characterize its [compact symplectic Lie algebra](../../../semisimple-lie-algebra.md#compact-symplectic-lie-algebra) without adding any trace condition. In fact the trace automatically vanishes. The free anti-Hermitian block $A$ has $n^2$ real parameters, and the complex [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $B$ has $n(n+1)$ real parameters. Thus

$$
\boxed{\dim_{\mathbb R}\mathfrak h=n^2+n(n+1)=n(2n+1).}
$$

Here is a complete [matrix-unit basis of the compact symplectic Lie algebra](../../../semisimple-lie-algebra.md#matrix-unit-basis-of-the-compact-symplectic-lie-algebra). The generators supplying $A$ are

$$
H_i=i(E^{(i,i)}-E^{(i+n,i+n)})\quad(1\leq i\leq n),
$$



$$
P_{ij}=E^{(i,j)}-E^{(j,i)}+E^{(i+n,j+n)}-E^{(j+n,i+n)},
$$



$$
Q_{ij}=i\bigl(E^{(i,j)}+E^{(j,i)}-E^{(i+n,j+n)}-E^{(j+n,i+n)}\bigr)\quad(i<j).
$$

The two families supplying the real and imaginary parts of $B$ are, for $1\leq i\leq j\leq n$,

$$
U_{ij}=\frac{E^{(i,j+n)}+E^{(j,i+n)}-E^{(i+n,j)}-E^{(j+n,i)}}{1+\delta_{ij}},
$$



$$
V_{ij}=\frac{i\bigl(E^{(i,j+n)}+E^{(j,i+n)}+E^{(i+n,j)}+E^{(j+n,i)}\bigr)}{1+\delta_{ij}}.
$$

The denominator merely avoids double-counting diagonal entries. Each displayed generator obeys both defining tangent conditions. The $H,P,Q$ generators form a real basis of the allowed $A$ blocks, and the $U,V$ generators form a real basis of the complex symmetric $B$ blocks. Thus they are independent and their total number is $n(2n+1)$. **They give all generators required by the real compact algebra, including the case $n=1$.**

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) on a [vector space](../../../vector-space.md) $V$ is a linear map $R:\mathfrak g\to\operatorname{End}(V)$ preserving the [Lie bracket](../../../lie-algebra.md#lie-bracket):

$$
R([X,Y])=[R(X),R(Y)].
$$

The [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) acts on $V=\mathfrak g$ by $\operatorname{ad}_X(Y)=[X,Y]$. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}.
$$

If $\mathfrak g$ is nonabelian, some $[X,Y]$ is nonzero, so this [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is not the [trivial Lie algebra representation](../../../lie-algebra.md#trivial-lie-algebra-representation). **It is the required nontrivial representation of dimension $\dim\mathfrak g$.** Nontriviality does not require its homomorphism to be injective.

For the finite-dimensional algebras here, with normalization one, the [Killing form](../../../lie-algebra.md#killing-form) is

$$
\boxed{\kappa(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).}
$$

It is a [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) by cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace). To prove its invariance, write $A=\operatorname{ad}_X$, $B=\operatorname{ad}_Y$, $C=\operatorname{ad}_Z$. Then

$$
\begin{aligned}
\kappa([Z,X],Y)+\kappa(X,[Z,Y])&=\operatorname{tr}([C,A]B+A[C,B])\\
&=\operatorname{tr}(CAB-ABC)=0.
\end{aligned}
$$

This also gives $\kappa([X,Y],Z)=\kappa(X,[Y,Z])$, the equivalent [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra) identity.

For the unheaded structural requests, a [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra) is nonabelian and has no [ideals of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) other than zero and itself. A [semisimple Lie algebra](../../../semisimple-lie-algebra.md) has no nonzero solvable [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra); in finite dimension over $\mathbb R$ or $\mathbb C$ this is equivalently a direct sum of [simple Lie algebras](../../../semisimple-lie-algebra.md#simple-lie-algebra).

Suppose first that the [Killing form](../../../lie-algebra.md#killing-form) is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form). If $I$ is an abelian [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) and $X\in I$, then $\operatorname{ad}_X$ maps $\mathfrak g$ into $I$ and vanishes on $I$. Every $\operatorname{ad}_Y$ preserves $I$. Therefore $\operatorname{ad}_X\operatorname{ad}_Y$ has zero diagonal blocks relative to a basis adapted to $I$, and

$$
\kappa(X,Y)=0\qquad(X\in I,\ Y\in\mathfrak g).
$$

Nondegeneracy forces $I=0$. If a nonzero solvable [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) existed, its last nonzero [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) term would be a nonzero abelian [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), again impossible. Hence the [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is zero, proving

$$
\boxed{\kappa\text{ nondegenerate}\quad\Longrightarrow\quad\mathfrak g\text{ semisimple}.}
$$

This argument proves the needed implication rather than assuming the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity).

One can also see the direct-sum formulation explicitly through [orthogonal ideal splitting for a nondegenerate Killing form](../../../lie-algebra.md#orthogonal-ideal-splitting-for-a-nondegenerate-killing-form). For an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) $I$, invariance makes $I^\perp$ an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra). If $X\in I\cap I^\perp$, then $\kappa([X,Y],Z)=\kappa(X,[Y,Z])=0$ for $Y\in I$, $Z\in\mathfrak g$, so $[X,I]=0$. Thus $I\cap I^\perp$ is an abelian [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), and must vanish. Consequently $\mathfrak g=I\oplus I^\perp$ and the two summands commute. Select a minimal nonzero ideal; it is nonabelian, and any ideal inside it is an ideal of $\mathfrak g$ because the complementary summand commutes with it. It is therefore simple. The restricted form is the remaining summand’s own [Killing form](../../../lie-algebra.md#killing-form), because the two ideals commute. Repeating the splitting there terminates in a direct sum of simple ideals.

Conversely the [radical of the Killing form](../../../lie-algebra.md#radical-of-the-killing-form)

$$
K=\{X:\kappa(X,Y)=0\text{ for all }Y\}
$$

is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) by the invariance just proved. For a [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra) it is either zero or the whole algebra. The permitted hypothesis that $\kappa$ is not identically zero excludes the second alternative. Thus

$$
\boxed{\mathfrak g\text{ simple and }\kappa\not\equiv0\quad\Longrightarrow\quad\kappa\text{ nondegenerate}.}
$$

The computations in the two following parts illustrate both a nondegenerate compact example and a degenerate algebra with an abelian ideal.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Pauli matrix commutator identity](../../../algebra.md#pauli-matrix-commutator-identity) gives

$$
[T^a,T^b]=\varepsilon^{abc}T^c
$$

for the anti-Hermitian basis of the [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra). In the ordered basis $(T^1,T^2,T^3)$ the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) matrices, with columns recording the images of basis elements, are

$$
\operatorname{ad}_{T^1}=\begin{pmatrix}0&0&0\\0&0&-1\\0&1&0\end{pmatrix},\quad
\operatorname{ad}_{T^2}=\begin{pmatrix}0&0&1\\0&0&0\\-1&0&0\end{pmatrix},\quad
\operatorname{ad}_{T^3}=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix}.
$$

Their squared [matrix traces](../../../linear-algebra.md#matrix-trace) are $-2$, and the mixed products have zero trace. Therefore the [Killing form of the SU(2) Lie algebra](../../../semisimple-lie-algebra.md#killing-form-of-the-su-2-lie-algebra) is

$$
\boxed{\kappa(T^a,T^b)=-2\delta^{ab},\qquad\kappa(X,Y)=-2\sum_{a=1}^3x_ay_a.}
$$

It is negative definite and [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form), so this real [Lie algebra](../../../lie-algebra.md) is semisimple. It is also simple: the displayed bracket is the three-dimensional [cross product](../../../vector-space.md#cross-product); if an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) contains nonzero $x$, the vectors $[y,x]$ span the plane perpendicular to $x$, and together with $x$ span the whole algebra. This confirms that the simplicity implication applies with a nonzero [Killing form](../../../lie-algebra.md#killing-form).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For the [Euclidean motion Lie algebra in two dimensions](../../../lie-algebra.md#euclidean-motion-lie-algebra-in-two-dimensions), use the ordered basis $(J,E_1,E_2)$ and keep the printed rotation signs. The [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) matrices are

$$
\operatorname{ad}_J=\begin{pmatrix}0&0&0\\0&0&1\\0&-1&0\end{pmatrix},\qquad
\operatorname{ad}_{E_1}=\begin{pmatrix}0&0&0\\0&0&0\\1&0&0\end{pmatrix},\qquad
\operatorname{ad}_{E_2}=\begin{pmatrix}0&0&0\\-1&0&0\\0&0&0\end{pmatrix}.
$$

Only the square of $\operatorname{ad}_J$ has a nonzero trace. Hence the [Killing form of the planar Euclidean motion Lie algebra](../../../lie-algebra.md#killing-form-of-the-planar-euclidean-motion-lie-algebra) has matrix

$$
\boxed{[\kappa]_{(J,E_1,E_2)}=\operatorname{diag}(-2,0,0),\qquad\kappa(aJ+u_1E_1+u_2E_2,bJ+v_1E_1+v_2E_2)=-2ab.}
$$

Its [radical of the Killing form](../../../lie-algebra.md#radical-of-the-killing-form) is $\operatorname{span}\{E_1,E_2\}$, precisely the translation subspace. This is a nonzero abelian [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), so the [Lie algebra](../../../lie-algebra.md) is neither simple nor semisimple. In fact its first [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) term is this translation ideal and its next is zero. Thus the degeneracy and the failure of semisimplicity agree with the structural proofs above; the adjoint action nevertheless remains nontrivial.

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\alpha_i^\vee=2\alpha_i/(\alpha_i,\alpha_i)$ be the [coroots](../../../semisimple-lie-algebra.md#coroot). With a chosen set of [simple roots](../../../semisimple-lie-algebra.md#simple-root), the [root lattice](../../../semisimple-lie-algebra.md#root-lattice) and [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) are

$$
\boxed{Q=\bigoplus_{i=1}^r\mathbb Z\alpha_i,\qquad P=\{\lambda:\langle\lambda,\alpha_i^\vee\rangle\in\mathbb Z\text{ for every }i\}.}
$$

The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) $\omega_j$ are defined by $\langle\omega_j,\alpha_i^\vee\rangle=\delta_{ij}$, and form an integral basis of $P$. We use the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) convention $A_{ij}=\langle\alpha_j,\alpha_i^\vee\rangle$.

For the [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system), inversion of its [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) yields the [A2 fundamental weights and weight lattice](../../../semisimple-lie-algebra.md#a2-fundamental-weights-and-weight-lattice):

$$
\boxed{\omega_1=\frac{2\alpha_1+\alpha_2}{3},\qquad\omega_2=\frac{\alpha_1+2\alpha_2}{3},\qquad P=\mathbb Z\omega_1\oplus\mathbb Z\omega_2.}
$$

Equivalently $\alpha_1=2\omega_1-\omega_2$ and $\alpha_2=-\omega_1+2\omega_2$. The [root lattice](../../../semisimple-lie-algebra.md#root-lattice) has index three in the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice), since the change-of-basis matrix has determinant three. For a planar realization take

$$
\alpha_1=(1,0),\quad\alpha_2=(-\tfrac12,\tfrac{\sqrt3}{2}),\quad\omega_1=(\tfrac12,\tfrac{\sqrt3}{6}),\quad\omega_2=(0,\tfrac{\sqrt3}{3}).
$$

The [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is triangular. In [fundamental weight](../../../semisimple-lie-algebra.md#fundamental-weight) coordinates $(a,b)$, a point is in the [root lattice](../../../semisimple-lie-algebra.md#root-lattice) exactly when $a-b$ is divisible by three. The following sketch marks both bases and the sublattice:

<a id="3/image-a2-weight-lattice-root-sublattice-fundamental-weights-and-simple-roots"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302-a2-weight-lattice.png)

**[Figure 1](#3/image-a2-weight-lattice-root-sublattice-fundamental-weights-and-simple-roots). A2 weight lattice, root sublattice, fundamental weights and simple roots**.

The integers called Dynkin indices here are the [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) of the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation):

$$
\boxed{\Lambda_i=\langle\Lambda,\alpha_i^\vee\rangle,\qquad\Lambda=\sum_i\Lambda_i\omega_i.}
$$

For finite-dimensional [Irreducible Lie algebra representations](../../../lie-algebra.md#irreducible-lie-algebra-representation), they are nonnegative integers. All weight coordinates below are these [Dynkin label](../../../semisimple-lie-algebra.md#dynkin-label) coordinates, not simple-root coordinates.

A [weight-string enumeration algorithm](../../../semisimple-lie-algebra.md#weight-string-enumeration-algorithm) gives the set of weights without their [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity). Begin with $\Lambda$ and process known weights by increasing height below $\Lambda$. For each simple root and known weight $\mu$, find the largest $p\geq0$ with $\mu+p\alpha_i$ a weight; all such higher weights have already been processed. The [weight string](../../../semisimple-lie-algebra.md#weight-string) theorem says that the string has endpoints $\mu+p\alpha_i$, $\mu-q\alpha_i$, with

$$
q-p=\langle\mu,\alpha_i^\vee\rangle,
$$

and includes every intermediate step. Append $\mu-\alpha_i,\ldots,\mu-q\alpha_i$ and repeat until no new weights appear. This terminates in finite dimension and supplies all weights; every nonhighest weight can be reached by simple-root lowering. A string can contain contributions from several sl2 summands, so the resulting set does not by itself determine [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity).

For the explicit calculation we use the following general facts: finite-dimensional representations of a complex [semisimple Lie algebra](../../../semisimple-lie-algebra.md) are completely reducible by the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem); the [symmetric powers of the defining sln representation](../../../semisimple-lie-algebra.md#symmetric-powers-of-the-defining-sln-representation) are irreducible of highest weight $m\omega_1$; and weights in a [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations) add with multiplicities multiplied. We also use the [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation) classification: each finite-dimensional irreducible has a unique dominant integral [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation), and a nonzero vector killed by all simple-root raising operators supplies an irreducible summand with that highest weight in a completely reducible module. For $A_2$, the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) specializes to

$$
\dim R(p,q)=\frac12(p+1)(q+1)(p+q+2).
$$

For $A_2\cong\mathfrak{sl}_3(\mathbb C)$, the defining [fundamental representation](../../../semisimple-lie-algebra.md#fundamental-representation) has weights $(1,0),(-1,1),(0,-1)$. Thus the [A2 representation of highest weight (2,0)](../../../semisimple-lie-algebra.md#a2-representation-of-highest-weight-2-0) is $\operatorname{Sym}^2\mathbb C^3$, with the six distinct weights

$$
\boxed{W_6=\{(2,0),(0,1),(1,-1),(-2,2),(-1,0),(0,-2)\}.}
$$

Each has multiplicity one: these are the weights of the six quadratic monomials.

For the [tensor square of the A2 representation of highest weight (2,0)](../../../semisimple-lie-algebra.md#tensor-square-of-the-a2-representation-of-highest-weight-2-0), add every ordered pair of elements of $W_6$. To list the complete answer compactly, define four disjoint weight sets:

$$
C=\{(4,0),(-4,4),(0,-4)\},
$$



$$
E=\{(2,1),(3,-1),(-2,3),(-3,2),(1,-3),(-1,-2)\},
$$



$$
M=\{(0,2),(2,-2),(-2,0)\},\qquad I=\{(1,0),(-1,1),(0,-1)\}.
$$

The tensor product has multiplicity one at each point of $C$, two at each point of $E$, three at each point of $M$, and four at each point of $I$. These fifteen distinct weights account for $3+12+9+12=36$ states.

We next identify the irreducible summands rather than just their dimensions. Split the [tensor square](../../../linear-algebra.md#tensor-square) of the six-dimensional space into its [symmetric power](../../../linear-algebra.md#symmetric-power) and [exterior power](../../../linear-algebra.md#exterior-power), of dimensions $21$ and $15$. The square of a highest-weight vector in the symmetric part has [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $(4,0)$, giving $R(4,0)$ of dimension $15$.

Let $v_a,v_b$ be vectors of weights $a=(2,0)$ and $b=(0,1)=a-\alpha_1$. In the exterior part $v_a\wedge v_b$ has weight $(2,1)$ and is killed by both simple-root raising operators: raising $v_b$ along $\alpha_1$ gives a multiple of $v_a$, whose wedge with itself is zero, and the other raising actions vanish. Thus it is a highest-weight vector. The [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) gives $\dim R(2,1)=15$, so the entire exterior part is this irreducible summand.

The remaining symmetric part has dimension six. To identify it, the fifteen weights of $R(4,0)=\operatorname{Sym}^4\mathbb C^3$ are exactly

$$
(a-b,b-c),\qquad a,b,c\geq0,\quad a+b+c=4,
$$

each once. Subtract them from the unordered-pair weights of $\operatorname{Sym}^2R(2,0)$. The residual weights are $M\cup I$, each once, with highest weight $(0,2)$. They are the negatives of $W_6$, so this six-dimensional summand is $R(0,2)$. Consequently

$$
\boxed{R(2,0)\otimes R(2,0)=R(4,0)\oplus R(2,1)\oplus R(0,2).}
$$

The corresponding dimensions are $15+15+6=36$; complete reducibility and the exhibited highest weights ensure that no summands are missing.

The full [weight multiplicities in the A2 tensor square of highest weight (2,0)](../../../semisimple-lie-algebra.md#weight-multiplicities-in-the-a2-tensor-square-of-highest-weight-2-0) are summarized below. An entry is the multiplicity of each individual weight in that row's set:

$$
\begin{array}{c|rrrr}
\text{weight set}&R(2,0)\otimes R(2,0)&R(4,0)&R(2,1)&R(0,2)\\\hline
C&1&1&0&0\\
E&2&1&1&0\\
M&3&1&1&1\\
I&4&1&2&1
\end{array}
$$

Thus $R(4,0)$ has all fifteen weights once, $R(0,2)$ has the six weights $M\cup I$ once, and $R(2,1)$ has its nine boundary weights $E\cup M$ once and its three interior weights $I$ twice. **Only the three interior weights of $R(2,1)$ are degenerate among the irreducible components.**

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Non-Abelian gauge theory](../../../relativistic-quantum-field.md#yang-mills-theory) promotes an internal [group representation](../../../representation-theory.md#group-representation) symmetry to a spacetime-dependent transformation and introduces a [gauge field](../../../relativistic-quantum-field.md#gauge-field) so that differentiation transforms covariantly. The symmetry is a [gauge redundancy](../../../relativistic-quantum-field.md#gauge-redundancy): physically meaningful quantities must be invariant under local changes of field representative. We work in four-dimensional [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with signature $(+---)$, and use [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix) generators throughout.

For the compact [Simple Lie group](../../../lie-theory.md#simple-lie-group) $G$, its real [Lie algebra](../../../lie-algebra.md) has a negative-definite [Killing form](../../../lie-algebra.md#killing-form). Hence $B=-\kappa$ is a positive [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra). Choose a $B$-orthonormal basis $T_a$, $a=1,\ldots,\dim G$, with $[T_a,T_b]=f_{ab}{}^cT_c$. Invariance makes $f_{abc}=B([T_a,T_b],T_c)$ fully antisymmetric. This construction uses the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) and works independently of any chosen scalar representation.

Let $\mathcal A_\mu=\mathcal A_\mu^aT_a$ be a Lie-algebra-valued [gauge potential](../../../relativistic-quantum-field.md#gauge-field), with the coupling absorbed into this connection. If $R$ is the given finite-dimensional [irreducible representation](../../../representation-theory.md#irreducible-representation) of $G$, its [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $\rho=dR$ defines

$$
\boxed{D_\mu\Phi=\partial_\mu\Phi+\rho(\mathcal A_\mu)\Phi.}
$$

For a finite local transformation $U(x)\in G$, require $\Phi'=R(U)\Phi$ and $D'_\mu\Phi'=R(U)D_\mu\Phi$. Differentiating the first equation forces the [gauge-field transformation law](../../../relativistic-quantum-field.md#gauge-field-transformation-law)

$$
\boxed{\mathcal A'_\mu=U\mathcal A_\mu U^{-1}-(\partial_\mu U)U^{-1}.}
$$

Thus the [gauge potential](../../../relativistic-quantum-field.md#gauge-field) transforms inhomogeneously; an ordinary derivative alone would leave an uncancelled derivative of $U$.

The commutator of [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative) determines the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength):

$$
[D_\mu,D_\nu]=\rho(\mathcal F_{\mu\nu}),\qquad\mathcal F_{\mu\nu}=\partial_\mu\mathcal A_\nu-\partial_\nu\mathcal A_\mu+[\mathcal A_\mu,\mathcal A_\nu].
$$

The [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) preserves the bracket, so this formula holds for any $R$, including a trivial scalar representation. The [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) itself is defined in the gauge algebra. The transformation of the connection implies

$$
\boxed{\mathcal F'_{\mu\nu}=U\mathcal F_{\mu\nu}U^{-1}.}
$$

It is therefore covariant, rather than invariant as a Lie-algebra-valued quantity.

For infinitesimal $U=1+\epsilon+O(\epsilon^2)$, the same equations give the [infinitesimal gauge transformation with an anti-Hermitian connection](../../../relativistic-quantum-field.md#infinitesimal-gauge-transformation-with-an-anti-hermitian-connection):

$$
\boxed{\delta\Phi=\rho(\epsilon)\Phi,\qquad\delta\mathcal A_\mu=-\partial_\mu\epsilon+[\epsilon,\mathcal A_\mu],\qquad\delta\mathcal F_{\mu\nu}=[\epsilon,\mathcal F_{\mu\nu}].}
$$

Substitution into $\delta(D_\mu\Phi)$ cancels the terms containing $\partial_\mu\epsilon$ and gives $\delta(D_\mu\Phi)=\rho(\epsilon)D_\mu\Phi$, the [gauge covariance of a scalar covariant derivative](../../../relativistic-quantum-field.md#gauge-covariance-of-a-scalar-covariant-derivative).

The [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) has [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density)

$$
\boxed{\mathcal L_{\mathrm{YM}}=-\frac1{4g_{\mathrm{YM}}^2}B(\mathcal F_{\mu\nu},\mathcal F^{\mu\nu})=\frac1{4g_{\mathrm{YM}}^2}\kappa(\mathcal F_{\mu\nu},\mathcal F^{\mu\nu}).}
$$

This is the [Killing-form Yang-Mills Lagrangian](../../../relativistic-quantum-field.md#killing-form-yang-mills-lagrangian). Its sign uses a positive internal form $B$ and the stated spacetime signature. In a $B$-orthonormal basis it is $-\mathcal F^a_{\mu\nu}\mathcal F^{a\mu\nu}/(4g_{\mathrm{YM}}^2)$. [Gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) follows because $B$ is invariant under the adjoint group action. Infinitesimally, the variation is proportional to

$$
B([\epsilon,\mathcal F_{\mu\nu}],\mathcal F^{\mu\nu})+B(\mathcal F_{\mu\nu},[\epsilon,\mathcal F^{\mu\nu}])=0.
$$

After rescaling $\mathcal A_\mu=g_{\mathrm{YM}}A_\mu$, the [gauge coupling](../../../relativistic-quantum-field.md#gauge-coupling) appears in $D_\mu=\partial_\mu+g_{\mathrm{YM}}\rho(A_\mu)$ and in the non-Abelian part of the canonically normalized field strength. Squaring that field strength gives cubic and quartic gauge-field self-interactions. An ordinary local quadratic mass term in the [gauge potential](../../../relativistic-quantum-field.md#gauge-field) is not invariant because its transformation contains $\partial_\mu\epsilon$.

For the [scalar field](../../../quantum-field-theory.md#scalar-field) kinetic term, compactness supplies a positive invariant [Hermitian form](../../../linear-algebra.md#hermitian-form) $h$ on its representation space. One can obtain it by averaging any positive form with normalized [Haar measure](../../../measure-theory.md#haar-measure), the [unitarization of a compact-group representation](../../../representation-theory.md#unitarization-of-a-compact-group-representation). Then $R(U)$ is unitary for $h$, and $\rho(\epsilon)$ is anti-Hermitian. The [Yang-Mills theory coupled to an arbitrary scalar representation](../../../relativistic-quantum-field.md#yang-mills-theory-coupled-to-an-arbitrary-scalar-representation) has

$$
\boxed{\mathcal L=\mathcal L_{\mathrm{YM}}+h(D_\mu\Phi,D^\mu\Phi)-V(\Phi).}
$$

Here $V$ is any real [gauge-invariant scalar potential](../../../relativistic-quantum-field.md#gauge-invariant-scalar-potential), so $V(R(U)\Phi)=V(\Phi)$. For example,

$$
V(\Phi)=m^2h(\Phi,\Phi)+\lambda\,h(\Phi,\Phi)^2
$$

is available for every unitary representation, with $\lambda\geq0$ giving a bounded quartic contribution. Other invariant interactions may exist for particular representations; the potential is not required to depend only on $h(\Phi,\Phi)$.

The scalar kinetic term is [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance) because both covariant derivatives transform by the same unitary $R(U)$. Infinitesimally its variation vanishes by

$$
h(\rho(\epsilon)u,v)+h(u,\rho(\epsilon)v)=0.
$$

The potential is invariant by its defining condition. For a real irreducible representation, use the averaged positive symmetric form instead and write the kinetic term as $\tfrac12 h(D_\mu\Phi,D^\mu\Phi)$; all transformation and invariance arguments remain valid. Expansion of the covariant kinetic term produces both the linear gauge-scalar interaction and the quadratic term needed by local [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance).

**The invariant [inner products](../../../linear-algebra.md#inner-product), [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative) and [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) together construct the full theory for every compact [Simple Lie group](../../../lie-theory.md#simple-lie-group) and every supplied finite-dimensional [irreducible representation](../../../representation-theory.md#irreducible-representation) of the scalar fields.** Both finite and infinitesimal transformation laws have been included, and every sign follows the same anti-Hermitian convention.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
