# Dual space

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_space)

The [dual space](dual-space.md) of a [vector space](vector-space.md) $V$ over a [field](algebra.md#field) $F$ is the [vector space](vector-space.md) of all [linear functionals](#linear-functional) $\varphi:V\to F$. Think of a [vector](vector-space.md#vector) as an input and a [linear functional](#linear-functional) as a scalar-valued measurement of that input. For $V=\mathbb R^2$, the rules $(x,y)\mapsto x$, $(x,y)\mapsto y$, and $(x,y)\mapsto2x-y$ are different elements of the [dual space](dual-space.md). None needs a notion of [length](physics.md#length) or [angle](geometry-and-topology.md#angle).

Its operations combine measurements pointwise:

$$
(\varphi+\psi)(v)=\varphi(v)+\psi(v),\qquad
(a\varphi)(v)=a\varphi(v).
$$

The [dual basis](#dual-basis) explains the finite-dimensional structure: specifying a [linear functional](#linear-functional)'s values on a [basis](vector-space.md#basis) determines its value on every [vector](vector-space.md#vector). Thus an $n$-dimensional [vector space](vector-space.md) has an $n$-dimensional [dual space](dual-space.md). The spaces have the same [dimension](vector-space.md#dimension-vector-space), but their elements play different roles: an input and a rule that measures an input. [Axler, Linear Algebra Done Right, fourth edition, §3F, definitions 3.109–3.112](mathematics-bibliography.md#linear-algebra-done-right-by-sheldon-axler-4th-edition).

This separation is useful when changing coordinates. The [dual pairing](#dual-pairing) $\varphi(v)$ must stay the same while the component lists for $v$ and $\varphi$ change in opposite ways. [Covector transformation under a change of basis](#covector-transformation-under-a-change-of-basis) makes the compensation explicit. An [inner product](inner-product.md) on a finite-dimensional real [vector space](vector-space.md) gives one way to represent each [linear functional](#linear-functional) by a [vector](vector-space.md#vector), but that representation uses the chosen [inner product](inner-product.md); the [dual space](dual-space.md) itself does not require one.

Here [dual space](dual-space.md) means the [algebraic dual](dual-space.md): all [linear functionals](#linear-functional). For a [topological vector space](topological-vector-space.md), the [continuous dual space](continuous-dual-space.md) keeps only the [continuous linear functionals](topological-vector-space.md#continuous-linear-functional). In infinite [dimension](vector-space.md#dimension-vector-space), this can be a proper [vector subspace](vector-space.md#vector-subspace); [discontinuous functional detected by vanishing sequence tails](#discontinuous-functional-detected-by-vanishing-sequence-tails) gives an example. The distinction matters when a scalar-valued measurement must respond continuously to small input changes.

**Table of contents**

- [Dual pairing](#dual-pairing)
- [Algebraic dual of a direct sum](#algebraic-dual-of-a-direct-sum)
- [Bidual of a normed space](#bidual-of-a-normed-space)
- [Perfect pairing](#perfect-pairing)
- [Separating subspace of an algebraic dual](#separating-subspace-of-an-algebraic-dual)
- [Bidual evaluation map](#bidual-evaluation-map)
- [Covector](#covector)
  - [Covector transformation under a change of basis](#covector-transformation-under-a-change-of-basis)
- [Linear functional](#linear-functional)
  - [Minimizing a linear functional on a sphere](#minimizing-a-linear-functional-on-a-sphere)
  - [Discontinuous functional detected by vanishing sequence tails](#discontinuous-functional-detected-by-vanishing-sequence-tails)
- [Dual basis](#dual-basis)
  - [Coordinate functional](#coordinate-functional)
  - [Factorial monomial basis for polynomial differentiation](#factorial-monomial-basis-for-polynomial-differentiation)
- [Annihilator of a vector subspace](#annihilator-of-a-vector-subspace)
- [Transpose of a linear map](#transpose-of-a-linear-map)
  - [Dual image and kernel annihilator identity](#dual-image-and-kernel-annihilator-identity)
  - [Equality of row rank and column rank](#equality-of-row-rank-and-column-rank)
    - [Simultaneous basis exchange from a nonzero minor](#simultaneous-basis-exchange-from-a-nonzero-minor)
  - [Duals of a subspace and its quotient](#duals-of-a-subspace-and-its-quotient)
- [Surjectivity of independent linear functionals](#surjectivity-of-independent-linear-functionals)
- [Polynomial moment functional](#polynomial-moment-functional)

## Dual pairing

↑ **Parent:** [Dual space](dual-space.md)

The [dual pairing](#dual-pairing) evaluates a [linear functional](#linear-functional) on a [vector](vector-space.md#vector):

$$
\langle\varphi,v\rangle=\varphi(v),\qquad (\varphi,v)\in V^*\times V.
$$

It is [bilinear](multilinear-algebra.md#bilinear-map): it is linear in each argument separately. Even over the [complex numbers](complex-analysis.md#complex-number), this algebraic evaluation has no [complex conjugation](complex-analysis.md#complex-conjugation). An [inner product](inner-product.md) instead has two [vectors](vector-space.md#vector) as inputs and, over the [complex numbers](complex-analysis.md#complex-number), is [sesquilinear](linear-algebra.md#sesquilinear-form). For $\varphi(x,y)=2x-y$ and $v=(3,1)$, the [dual pairing](#dual-pairing) equals five. Its value is independent of the [basis](vector-space.md#basis) used to describe its two inputs.

## Algebraic dual of a direct sum

↑ **Parent:** [Dual space](dual-space.md)

Restricting a [linear functional](#linear-functional) to each summand gives a family of functionals, with no finite-support restriction. Conversely an arbitrary such family acts on a vector by the finite sum of its nonzero coordinates. These constructions are inverse and prove the displayed algebraic [dual space](dual-space.md) identity. A group action on the summands induces the product action by their algebraic contragredients.

## Bidual of a normed space

↑ **Parent:** [Dual space](dual-space.md)

The bidual of a [normed vector space](normed-vector-space.md) $X$ is the continuous dual $X^{**}=(X^*)^*$. Evaluation defines the [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual) $J_X(x)(f)=f(x)$. The [norm](normed-vector-space.md#norm) inequality gives $\|J_Xx\|\le\|x\|$, and a norming functional from the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) gives equality. Thus $J_X$ is isometric, and its image is dense in its closure, a [completion of a normed space](normed-vector-space.md#completion-of-a-normed-space).

## Perfect pairing

↑ **Parent:** [Dual space](dual-space.md)

For finite-dimensional [vector spaces](vector-space.md) $V,W$ over a [field](algebra.md#field) $F$, a bilinear pairing $B:V\times W\to F$ is perfect when the induced [linear maps](vector-space.md#linear-map) $V\to W^*$ and $W\to V^*$ are [isomorphisms](algebra.md#isomorphism). Equivalently, both dimensions agree and the matrix of the pairing in any two bases is invertible. The evaluation pairing between a finite-dimensional [vector space](vector-space.md) and its [dual space](dual-space.md) is perfect. This notion allows two different spaces; a [nondegenerate bilinear form](bilinear-form.md#nondegenerate-bilinear-form) is the case $V=W$.

## Separating subspace of an algebraic dual

↑ **Parent:** [Dual space](dual-space.md)

A [linear subspace](vector-space.md#vector-subspace) $W\subseteq X^*$ is separating if every nonzero $x\in X$ has $T(x)\ne0$ for some $T\in W$. For finite-dimensional $X$, an evaluation map $X\to F^{\dim W}$ is [injective](algebra.md#injective-function), so the [rank-nullity theorem](kernel-of-a-linear-map.md#rank-nullity-theorem) forces $\dim W\geq\dim X=\dim X^*$ and $W=X^*$. For the infinite-dimensional [polynomial](polynomial.md) space, the span of its coefficient functionals is a proper separating [linear subspace](vector-space.md#vector-subspace) of the [dual space](dual-space.md), which contains all sequences of coefficients, not just finitely supported ones.

## Bidual evaluation map

↑ **Parent:** [Dual space](dual-space.md)

For an algebraic [dual space](dual-space.md) $X^*=\operatorname{Hom}_F(X,F)$, the [linear map](vector-space.md#linear-map) $J:X\to X^{**}$ sends $x$ to evaluation at $x$. It is [injective](algebra.md#injective-function) because [linear functionals](#linear-functional) separate nonzero vectors: extend any nonzero vector to a [basis](vector-space.md#basis) and use its coordinate functional. If $X$ has a finite [basis](vector-space.md#basis) $e_i$ with [dual basis](#dual-basis) $e_i^*$, every $B\in X^{**}$ equals $J(\sum_iB(e_i^*)e_i)$, so $J$ is an [isomorphism](algebra.md#isomorphism). For infinite-dimensional spaces, [surjection](algebra.md#surjective-function) does not follow from this finite sum argument.

## Covector

↑ **Parent:** [Dual space](dual-space.md)

A [covector](#covector) is an element of the [dual space](dual-space.md), hence a [linear functional](#linear-functional) on a [vector space](vector-space.md). In finite-dimensional coordinates, it acts as a row multiplied by a [coordinate vector](vector-space.md#coordinate-vector) column. The row $\begin{pmatrix}2&-1\end{pmatrix}$ acts on $\begin{pmatrix}3\\1\end{pmatrix}$ to give five. The terminology emphasizes its role as a scalar-valued measurement and its behavior under a [change of basis](linear-algebra.md#change-of-basis).

For example, the [total derivative](calculus.md#total-derivative) of $f(x,y)=x^2+y^2$ at $(1,2)$ sends a small displacement $h$ to the linear change $df(h)=2h_x+4h_y$. This [covector](#covector) describes the first-order response. The [gradient](multivariable-calculus.md#gradient) $\nabla f=(2,4)$ represents the same rule through the chosen Euclidean [inner product](inner-product.md). In [differential geometry](differential-geometry.md), the [cotangent space](tangent-vector.md#cotangent-space) collects these scalar-valued measurements of [tangent vectors](tangent-vector.md).

### Covector transformation under a change of basis

↑ **Parent:** [Covector](#covector)

Let the columns of an [invertible matrix](linear-algebra.md#invertible-matrix) $B$ be a new [basis](vector-space.md#basis) expressed in the old [basis](vector-space.md#basis). The same [vector](vector-space.md#vector) has old [coordinate vector](vector-space.md#coordinate-vector) $x$ and new [coordinate vector](vector-space.md#coordinate-vector) $x'=B^{-1}x$. If a [covector](#covector) has old row $\ell$, its new row is $\ell'=\ell B$, since

$$
\ell'x'=\ell B B^{-1}x=\ell x.
$$

Thus the scalar [dual pairing](#dual-pairing) stays unchanged. If [covector](#covector) coefficients are stored as a column $c=\ell^T$, their new column is $c'=B^Tc$; this is the inverse transpose of the transformation $x\mapsto B^{-1}x$ on [vector](vector-space.md#vector) coordinates. These conventions express the [covariance and contravariance of vectors](multilinear-algebra.md#covariance-and-contravariance-of-vectors). [Sergei Treil, Linear Algebra Done Wrong, §8.1.1: coordinate changes in the dual space](https://www.math.brown.edu/streil/papers/LADW/HTML_2026_04-30/Ch8.html).

For the [basis](vector-space.md#basis) $b_1=(1,0)$, $b_2=(1,1)$,

$$
B=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
x=\begin{pmatrix}3\\1\end{pmatrix},\qquad
x'=\begin{pmatrix}2\\1\end{pmatrix}.
$$

The [linear functional](#linear-functional) $\varphi(x,y)=2x-y$ has rows $\ell=\begin{pmatrix}2&-1\end{pmatrix}$ and $\ell'=\begin{pmatrix}2&1\end{pmatrix}$. Both calculations give five: $2\cdot3-1\cdot1=2\cdot2+1\cdot1$. Changing the [basis](vector-space.md#basis) changes the descriptions, not the measured value.

## Linear functional

↑ **Parent:** [Dual space](dual-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_functional)

A [linear functional](#linear-functional) is a [linear map](vector-space.md#linear-map) from a [vector space](vector-space.md) $V$ to its scalar [field](algebra.md#field) $F$:

$$
\varphi(av+bw)=a\varphi(v)+b\varphi(w),\qquad a,b\in F,\quad v,w\in V.
$$

Its output is one [scalar](vector-space.md#scalar), rather than an arbitrary [vector](vector-space.md#vector) in another space. In $\mathbb R^2$, $\varphi(x,y)=2x-y$ gives $\varphi(3,1)=5$, $\varphi(1,2)=0$, and $\varphi(4,3)=5$: adding the two inputs adds their measured values.

The [level sets](topology.md#level-set) $\varphi(v)=c$ visualize what the measurement retains and discards. For this example they are parallel [straight lines](euclidean-geometry.md#straight-line) $y=2x-c$. Moving parallel to $(1,2)$ changes the input but leaves $\varphi$ unchanged. The zero [level set](topology.md#level-set) is its [kernel of a linear map](kernel-of-a-linear-map.md), while the other [level sets](topology.md#level-set) are translates of that [vector subspace](vector-space.md#vector-subspace).

<a id="image-a-linear-functional-groups-vectors-into-parallel-level-sets-with-the-same-measured-value"></a>
![](linear-functional-level-sets.png)

**[Figure 1](#image-a-linear-functional-groups-vectors-into-parallel-level-sets-with-the-same-measured-value). A linear functional groups vectors into parallel level sets with the same measured value**.

Inputs need not be geometric arrows. On the [vector space](vector-space.md) of [polynomials](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most two, evaluating at zero is a [linear functional](#linear-functional), as is taking the [definite integral](integral.md#definite-integral) from zero to one. For $p(t)=a+bt+ct^2$, they give $p(0)=a$ and $\int_0^1p(t)\,dt=a+b/2+c/3$. Thus [polynomial evaluation](polynomial.md#polynomial-evaluation) and [integration](integral.md) are two different measurements of the same [polynomial](polynomial.md). Coordinate extraction is another measurement, developed under [dual basis](#dual-basis).

A [linear functional](#linear-functional) is defined by [linearity](vector-space.md#linearity), not by [continuity](calculus.md#continuous-function). In finite-dimensional real or complex [normed vector spaces](normed-vector-space.md) it is automatically continuous; in infinite [dimension](vector-space.md#dimension-vector-space) it need not be. The [continuous dual space](continuous-dual-space.md) adds this requirement when small changes in the input should give small changes in the output.

### Minimizing a linear functional on a sphere

↑ **Parent:** [Linear functional](#linear-functional)

For a nonzero Euclidean vector $w$, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $z\cdot w\geq-\|w\|$ when $\|z\|=1$. Equality is attained uniquely at $z=-w/\|w\|$. On a sphere of radius $r>0$ the minimizer is $-rw/\|w\|$, and the minimum is $-r\|w\|$. This turns many constrained vector problems into a normalization of one fixed vector. If $w=0$, every point minimizes the functional.

### Discontinuous functional detected by vanishing sequence tails

↑ **Parent:** [Linear functional](#linear-functional)

If a [linear functional](#linear-functional) on a [normed vector space](normed-vector-space.md) has $f(v_N)=1$ for a sequence tending to zero in norm, it is discontinuous and unbounded. An explicit example is the algebraic span in $\ell^2$ of the coordinate vectors and $w=(2^{-n})_{n\geq1}$. Define $f(w)=1$ and $f(e_n)=0$. The tails $v_N=w-\sum_{n=1}^N2^{-n}e_n$ have norm $2^{-N}/\sqrt3$ but image one. Thus the functional vanishes on the dense finite-support subspace while being nonzero elsewhere.

## Dual basis

↑ **Parent:** [Dual space](dual-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_basis)

For a [basis](vector-space.md#basis) $e_1,\ldots,e_n$ of a finite-dimensional [vector space](vector-space.md) $V$, its [dual basis](#dual-basis) consists of [linear functionals](#linear-functional) $e_1^*,\ldots,e_n^*$ satisfying

$$
e_i^*(e_j)=\delta_{ij}.
$$

The [Kronecker delta](multilinear-algebra.md#kronecker-delta) means that each rule gives one on its own [basis vector](vector-space.md#basis-vector) and zero on the others. These rules extract coordinates:

$$
v=\sum_{i=1}^n e_i^*(v)e_i.
$$

Applying $e_i^*$ to a [linear combination](vector-space.md#linear-combination) removes every term except the $i$th. Consequently the [dual basis](#dual-basis) is a [basis](vector-space.md#basis) of the [dual space](dual-space.md), and every [linear functional](#linear-functional) has expansion $\varphi=\sum_i\varphi(e_i)e_i^*$. [Axler, Linear Algebra Done Right, fourth edition, §3F, definitions and results 3.112–3.116](mathematics-bibliography.md#linear-algebra-done-right-by-sheldon-axler-4th-edition).

Coordinate extraction works for a nonorthogonal [basis](vector-space.md#basis) too. With $b_1=(1,0)$ and $b_2=(1,1)$, the [dual basis](#dual-basis) is

$$
b_1^*(x,y)=x-y,\qquad b_2^*(x,y)=y.
$$

The checks $b_1^*(b_1)=1$, $b_1^*(b_2)=0$, $b_2^*(b_1)=0$, and $b_2^*(b_2)=1$ fix the two rules. For $v=(3,1)$ they give **coordinates $(2,1)$**, so $v=2b_1+b_2$. The usual [dot products](inner-product.md#dot-product) with $b_1,b_2$ instead give $3,4$ and do not extract these coordinates: simple projection formulas depend on an [orthonormal basis](inner-product.md#orthonormal-basis).

<a id="image-the-dual-basis-extracts-coefficients-in-a-skew-basis-by-two-scalar-valued-measurements"></a>
![](dual-basis-skew-coordinates.png)

**[Figure 2](#image-the-dual-basis-extracts-coefficients-in-a-skew-basis-by-two-scalar-valued-measurements). The dual basis extracts coefficients in a skew basis by two scalar-valued measurements**.

The same idea explains [polynomial interpolation](interpolation.md#polynomial-interpolation). On [polynomials](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$, evaluation at distinct [interpolation nodes](interpolation.md#interpolation-node) $x_0,\ldots,x_n$ gives the [dual basis](#dual-basis) to the [Lagrange cardinal polynomials](interpolation.md#lagrange-cardinal-polynomial), because $\ell_i(x_j)=\delta_{ij}$. Samples are coordinates in this [basis](vector-space.md#basis), so the reconstruction $p=\sum_i p(x_i)\ell_i$ is a dual-basis expansion. [Differentiation weights from nodal evaluations](interpolation.md#differentiation-weights-from-nodal-evaluations) and [factorial monomial basis for polynomial differentiation](#factorial-monomial-basis-for-polynomial-differentiation) apply the same principle to different measurements.

### Coordinate functional

↑ **Parent:** [Dual basis](#dual-basis)

A [coordinate functional](#coordinate-functional) extracts one coefficient in a specified finite [basis](vector-space.md#basis). It is an element of that [basis](vector-space.md#basis)'s [dual basis](#dual-basis), rather than a coordinate rule independent of the [basis](vector-space.md#basis). For the [standard basis](vector-space.md#standard-basis) of $F^n$, the $i$th [coordinate functional](#coordinate-functional) sends $(a_1,\ldots,a_n)$ to $a_i$.

### Factorial monomial basis for polynomial differentiation

↑ **Parent:** [Dual basis](#dual-basis)

On polynomials of degree at most $n$, the derivative-evaluation functionals $e_j(\phi)=\phi^{(j)}(0)$ are dual to $p_j=x^j/j!$, since $e_i(p_j)=\delta_{ij}$. Differentiation maps $p_j$ to $p_{j-1}$, with $p_0$ mapped to zero. Its matrix is a single nilpotent Jordan block with ones above the diagonal, and its dual has the transpose matrix.

## Annihilator of a vector subspace

↑ **Parent:** [Dual space](dual-space.md)

For a [vector subspace](vector-space.md#vector-subspace) $U\leq V$,

$$
U^\circ=\{f\in V^*:f|_U=0\}.
$$

In finite [dimension](vector-space.md#dimension-vector-space), $\dim U^\circ=\dim V-\dim U$.

An [annihilator of a vector subspace](#annihilator-of-a-vector-subspace) collects the [linear functionals](#linear-functional) that ignore every input from that [vector subspace](vector-space.md#vector-subspace). For $U=\operatorname{span}\{(1,2)\}\subseteq\mathbb R^2$, a [linear functional](#linear-functional) $\varphi(x,y)=ax+by$ vanishes on $U$ exactly when $a+2b=0$. Hence $U^\circ$ is the one-dimensional [span](vector-space.md#linear-span) of $(x,y)\mapsto2x-y$. The zero [level set](topology.md#level-set) in the [linear functional](#linear-functional) diagram is precisely $U$.

## Transpose of a linear map

↑ **Parent:** [Dual space](dual-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transpose_of_a_linear_map)

For a [linear map](vector-space.md#linear-map) $T:V\to W$, the [dual map](#transpose-of-a-linear-map) $T^*:W^*\to V^*$ sends a [linear functional](#linear-functional) $\varphi$ on the output space to the input measurement $T^*(\varphi)=\varphi\circ T$. It reverses direction because a measurement of the output can be evaluated on an input by first applying $T$:

$$
(T^*\varphi)(v)=\varphi(Tv).
$$

For $T(x,y)=(x+y,2y)$ and $\varphi(u,v)=2u-v$, the input measurement is $T^*\varphi(x,y)=2(x+y)-2y=2x$. The output measurement ignores the part of this transformation contributed by $y$.

If $T$ has [matrix](vector-space.md#matrix) $A$ in specified [bases](vector-space.md#basis), a row representing $\varphi$ changes to $\ell A$. Storing the coefficients of a [linear functional](#linear-functional) as a column in the corresponding [dual basis](#dual-basis) gives $A^T\ell^T$, explaining why the [transpose of a linear map](#transpose-of-a-linear-map) is represented by the [matrix transpose](vector-space.md#transpose). This algebraic operation uses no [inner product](inner-product.md); it agrees with a matrix transpose even over the [complex numbers](complex-analysis.md#complex-number), rather than automatically introducing [complex conjugation](complex-analysis.md#complex-conjugation). The [adjoint operator](hilbert-space.md#adjoint-operator) is defined using an [inner product](inner-product.md) and is a different construction. [Treil, Linear Algebra Done Wrong, §8.3: dual transformations and transpose](https://www.math.brown.edu/streil/papers/LADW/HTML_2026_04-30/Ch8.html).

In finite [dimension](vector-space.md#dimension-vector-space), the [kernel](kernel-of-a-linear-map.md) and image of the [dual map](#transpose-of-a-linear-map) are described by [annihilators of vector subspaces](#annihilator-of-a-vector-subspace):

$$
\ker T^*=(\operatorname{im}T)^\circ,
\qquad
\operatorname{im}T^*=(\ker T)^\circ.
$$

### Dual image and kernel annihilator identity

↑ **Parent:** [Transpose of a linear map](#transpose-of-a-linear-map)

For a [linear map](vector-space.md#linear-map) between finite-dimensional [vector spaces](vector-space.md), the image of its [dual map](#transpose-of-a-linear-map) is the [annihilator of a vector subspace](#annihilator-of-a-vector-subspace) given by its kernel. Inclusion follows by composition. Conversely a [linear functional](#linear-functional) vanishing on the kernel descends to the image and extends to the target by [basis extension](vector-space.md#basis-extension). The identity and the [rank-nullity theorem](kernel-of-a-linear-map.md#rank-nullity-theorem) show that a linear map and its dual have equal rank.

### Equality of row rank and column rank

↑ **Parent:** [Transpose of a linear map](#transpose-of-a-linear-map)

For the map represented by a matrix $A$, column rank is the rank of the map and row rank is the rank of its dual. Since the dual map has kernel equal to the annihilator of the original image, rank-nullity gives equal ranks.

#### Simultaneous basis exchange from a nonzero minor

↑ **Parent:** [Equality of row rank and column rank](#equality-of-row-rank-and-column-rank)

If the columns $v_1,\ldots,v_m$ of an $n$ by $m$ matrix are independent, some $m$ by $m$ row minor is nonzero. A nonzero term of that minor's determinant selects distinct nonzero coordinates $f(i)$, and replacing the corresponding standard basis vectors $e_{f(i)}$ by the $v_i$ leaves a basis.

### Duals of a subspace and its quotient

↑ **Parent:** [Transpose of a linear map](#transpose-of-a-linear-map)

For a finite-dimensional vector space and $U\leq V$, dualizing the quotient and inclusion maps gives

$$
(V/U)^*\cong U^\circ,
\qquad
U^*\cong V^*/U^\circ.
$$

## Surjectivity of independent linear functionals

↑ **Parent:** [Dual space](dual-space.md)

If $q_1,\ldots,q_n\in V^*$ are linearly independent, then

$$
x\longmapsto(q_1(x),\ldots,q_n(x))
$$

maps $V$ onto $F^n$. Otherwise a nonzero functional annihilating its proper image would give a nontrivial linear relation among the $q_j$.

## Polynomial moment functional

↑ **Parent:** [Dual space](dual-space.md)

A polynomial moment functional evaluates a polynomial through a weighted integral, such as $p\mapsto\int p(t)w(t)dt$; finitely many moments determine it on a bounded-degree polynomial space.

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (46)

- [Algebraic contragredient representation](representation-theory.md#algebraic-contragredient-representation)
- [Algebraic dual of a direct sum](#algebraic-dual-of-a-direct-sum)
- [Bidual evaluation map](#bidual-evaluation-map)
- [Bilinear form](bilinear-form.md)
- [Category theory](category-theory.md)
- [Coadjoint representation](lie-theory.md#coadjoint-representation)
- [Continuous dual space](continuous-dual-space.md)
- [Covector](#covector)
- [Differentiation weights from nodal evaluations](interpolation.md#differentiation-weights-from-nodal-evaluations)
- [Dual basis](#dual-basis)
- [Dual isomorphisms induced by a nondegenerate pairing](bilinear-form.md#dual-isomorphisms-induced-by-a-nondegenerate-pairing)
- [Dual Lie algebra representation](lie-algebra.md#dual-lie-algebra-representation)
- [Dual space](dual-space.md)
- [Exterior algebra](multilinear-algebra.md#exterior-algebra)
- [Lie-Poisson bracket](symplectic-geometry.md#lie-poisson-bracket)
- [Nondegenerate bilinear form](bilinear-form.md#nondegenerate-bilinear-form)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2.md#15c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2.md#8b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4.md#15f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4.md#15g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2.md#10e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1.md#9g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#21f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#22f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#3/2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#3/2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4.md#1f/solution)
- [Perfect pairing](#perfect-pairing)
- [Poincare duality pairing](cohomology.md#poincare-duality-pairing)
- [Separating subspace of an algebraic dual](#separating-subspace-of-an-algebraic-dual)
- [Sobolev duality](sobolev-space.md#sobolev-duality)
