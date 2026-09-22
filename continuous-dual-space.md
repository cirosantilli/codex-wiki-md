# Continuous dual space

↑ **Parent:** [Functional analysis](functional-analysis.md)

The continuous dual $X^*$ of a topological vector space is the vector space of its continuous scalar-valued linear functionals. For a normed space these are exactly the bounded linear functionals.

This is the continuity-restricted subspace of the algebraic [dual space](linear-algebra.md#dual-space); in infinite dimension the two can differ.

**Table of contents**

- [Norming functional](#norming-functional)
- [Norming subspace of a dual space](#norming-subspace-of-a-dual-space)
  - [Vanishing sequences norm the summable sequence space](#vanishing-sequences-norm-the-summable-sequence-space)
  - [Finite-codimensional weak-star dense dual subspace is norming](#finite-codimensional-weak-star-dense-dual-subspace-is-norming)
- [Continuous-dual separation theorem for Hausdorff locally convex spaces](#continuous-dual-separation-theorem-for-hausdorff-locally-convex-spaces)
- [Strong dual topology](#strong-dual-topology)
- [Dual pairing](#dual-pairing)
- [Transpose of a bounded linear operator](#transpose-of-a-bounded-linear-operator)
- [Positive linear functional](#positive-linear-functional)
  - [Jordan decomposition of a bounded functional on C(K)](#jordan-decomposition-of-a-bounded-functional-on-c-k)
  - [Positive extension from a unital subspace of C(K)](#positive-extension-from-a-unital-subspace-of-c-k)
  - [Norm of a positive functional on C(K)](#norm-of-a-positive-functional-on-c-k)
  - [Unital contraction positivity criterion](#unital-contraction-positivity-criterion)
- [Operator norm](#operator-norm)
  - [Riesz-Thorin theorem](#riesz-thorin-theorem)
  - [Operator norm duality](#operator-norm-duality)
  - [Euclidean logarithmic norm](#euclidean-logarithmic-norm)
    - [Euclidean semigroup growth bounds](#euclidean-semigroup-growth-bounds)
  - [Submultiplicativity of the operator norm](#submultiplicativity-of-the-operator-norm)
  - [Telescoping bound for products of operators](#telescoping-bound-for-products-of-operators)
    - [Unitary product telescoping](#unitary-product-telescoping)
  - [Matrix 2-norm](#matrix-2-norm)
- [Completeness of the dual space](#completeness-of-the-dual-space)
- [Duality of sequence spaces](#duality-of-sequence-spaces)
  - [Duality of l1 and l infinity](#duality-of-l1-and-l-infinity)
    - [Schur property](#schur-property)
      - [Gliding hump argument](#gliding-hump-argument)
        - [Schur property of l1](#schur-property-of-l1)
- [Duality of Lp spaces](#duality-of-lp-spaces)
  - [Closed-hyperplane proof of Lp duality](#closed-hyperplane-proof-of-lp-duality)
  - [Lp duality on an arbitrary measure space](#lp-duality-on-an-arbitrary-measure-space)
    - [Support localization of an Lp functional](#support-localization-of-an-lp-functional)
  - [Dual of L infinity is larger than L1](#dual-of-l-infinity-is-larger-than-l1)
  - [Reflexivity of Lp spaces](#reflexivity-of-lp-spaces)
  - [Positive functional representation on Lp](#positive-functional-representation-on-lp)

## Norming functional

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

For a nonzero [vector](vector-space.md#vector) in a real or complex [normed vector space](functional-analysis.md#normed-vector-space), a [norming functional](#norming-functional) is a [continuous linear functional](topological-vector-space.md#continuous-linear-functional) satisfying the displayed conditions. The [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) extends the functional sending $av$ to $a\|v\|$ on its one-dimensional span. Consequently $\|w\|\geq\operatorname{Re}\ell(w)$, with equality at $v$, giving a supporting linear [lower bound](set.md#lower-bound-in-a-partially-ordered-set) for the [norm](functional-analysis.md#norm). At zero the zero functional can be used as a supporting functional.

## Norming subspace of a dual space

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

A [vector subspace](vector-space.md#vector-subspace) $Z\subseteq X^*$ is norming if some $c>0$ satisfies the displayed inequality. It retains enough continuous [linear functionals](linear-algebra.md#linear-functional) to control the [norm](functional-analysis.md#norm) of every vector. Every such [vector subspace](vector-space.md#vector-subspace) is dense for the [weak-star topology](weak-topology.md#weak-star-topology): otherwise a nonzero evaluation [linear functional](linear-algebra.md#linear-functional) would annihilate its weak-star closure, contradicting the inequality. In the real case its symmetric [unit ball](functional-analysis.md#unit-ball) makes the absolute-value and signed supremum versions equivalent.

### Vanishing sequences norm the summable sequence space

↑ **Parent:** [Norming subspace of a dual space](#norming-subspace-of-a-dual-space)

Finite truncations of the sign or phase sequence of $x\in\ell^1$ belong to $c_0$ and attain increasing partial sums of $\sum_n|x_n|$. Thus the [space of sequences converging to zero](functional-analysis.md#space-of-sequences-converging-to-zero) is 1-norming for the [absolutely summable sequence space](banach-space.md#absolutely-summable-sequence-space). Its codimension in $\ell^\infty$ is infinite: indicators of pairwise disjoint infinite subsets have linearly independent classes modulo $c_0$. Norming does not require finite codimension.

### Finite-codimensional weak-star dense dual subspace is norming

↑ **Parent:** [Norming subspace of a dual space](#norming-subspace-of-a-dual-space)

A norm-closed finite-codimensional [vector subspace](vector-space.md#vector-subspace) $Y\subseteq X^*$ that is weak-star dense is a [norming subspace](#norming-subspace-of-a-dual-space). Its annihilator $F=Y^\perp\subseteq X^{**}$ is finite-dimensional and disjoint from $JX$. The positive distance $d$ of the unit sphere from $F$ gives a triple-dual [linear functional](linear-algebra.md#linear-functional) vanishing on $F$ and taking a value at least $d$ at a unit vector. Apply the [finite-dimensional interpolation form of Goldstine's theorem](functional-analysis.md#finite-dimensional-interpolation-form-of-goldstine-s-theorem) to the [Banach space](banach-space.md) $X^*$, then normalize and take a supremum to obtain norming constant $d$.

## Continuous-dual separation theorem for Hausdorff locally convex spaces

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

In a Hausdorff [locally convex space](topological-vector-space.md#locally-convex-space), a separating family of continuous [seminorms](topological-vector-space.md#seminorm) has $p(x)>0$ for any chosen nonzero $x$ and some $p$. Define a [linear functional](linear-algebra.md#linear-functional) on its one-dimensional span attaining $p(x)$ and extend it under that [seminorm](topological-vector-space.md#seminorm) by the real [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem). The extension is continuous because it is seminorm-bounded, and distinguishes $x$ from zero. The Hausdorff condition is essential.

## Strong dual topology

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

For a [locally convex space](topological-vector-space.md#locally-convex-space) $E$, the [strong dual topology](#strong-dual-topology) on its [continuous dual space](continuous-dual-space.md) $E'$ is generated by seminorms $p_B(T)=\sup_{\varphi\in B}|\langle T,\varphi\rangle|$, where $B$ runs through the [bounded sets in a topological vector space](topological-vector-space.md#bounded-set-in-a-topological-vector-space) $E$. Convergence therefore means uniform convergence of pairings on every such set. For the [Schwartz space](fourier-analysis.md#schwartz-space), the defining boundedness is boundedness of every Schwartz seminorm, rather than one norm or one common compact support.

## Dual pairing

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

The dual pairing evaluates a linear functional on a vector: $\langle f,x\rangle=f(x)$. It is the basic pairing between a topological vector space and its continuous dual.

## Transpose of a bounded linear operator

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T:X\to Y$, its transpose or dual map is $T^*:Y^*\to X^*$ defined by

$$
(T^*y^*)(x)=y^*(Tx).
$$

It satisfies $\lVert T^*\rVert=\lVert T\rVert$.

## Positive linear functional

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_linear_functional)

A linear functional $\Lambda$ on an ordered vector space of functions is positive when $f\geq0$ implies $\Lambda(f)\geq0$. Positivity implies monotonicity: $f\leq g$ gives $\Lambda(f)\leq\Lambda(g)$.

<h3 id="jordan-decomposition-of-a-bounded-functional-on-c-k">Jordan decomposition of a bounded functional on C(K)</h3>

↑ **Parent:** [Positive linear functional](#positive-linear-functional)

For a bounded real [linear functional](linear-algebra.md#linear-functional) on the [space of continuous functions on a compact space](functional-analysis.md#space-of-continuous-functions-on-a-compact-space), define $\phi^+(f)=\sup_{0\leq g\leq f}\phi(g)$ for $f\geq0$. The decomposition $g=\min(g,f)+(g-f)^+$ for $0\leq g\leq f+h$ proves additivity on the positive cone; positive homogeneity is immediate. Extend by differences, and put $\phi^-=\phi^+-\phi$. Both are [positive linear functionals](#positive-linear-functional). Their norms sum to $2\phi^+(1)-\phi(1)=\sup_{\|g\|_\infty\leq1}\phi(g)=\|\phi\|$, using the substitution $g=2h-1$.

<h3 id="positive-extension-from-a-unital-subspace-of-c-k">Positive extension from a unital subspace of C(K)</h3>

↑ **Parent:** [Positive linear functional](#positive-linear-functional)

A real [positive linear functional](#positive-linear-functional) on a [vector subspace](vector-space.md#vector-subspace) of $C(K)$ containing $1$ extends positively to all of $C(K)$. Its norm is $\phi(1)$ by order bounds. If this is positive, apply the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) to obtain an extension of the same norm, normalize it to value one at $1$, and use the [unital contraction positivity criterion](#unital-contraction-positivity-criterion). If $\phi(1)=0$, the functional is zero and its zero extension suffices.

<h3 id="norm-of-a-positive-functional-on-c-k">Norm of a positive functional on C(K)</h3>

↑ **Parent:** [Positive linear functional](#positive-linear-functional)

For a real [positive linear functional](#positive-linear-functional) on the [space of continuous functions on a compact space](functional-analysis.md#space-of-continuous-functions-on-a-compact-space), $-\|f\|_\infty1\le f\le\|f\|_\infty1$ gives $|\phi(f)|\le\phi(1)\|f\|_\infty$. Evaluation at $1$ gives equality of the [operator norm](#operator-norm) and $\phi(1)$. Thus positivity alone already implies continuity in the [supremum norm](functional-analysis.md#supremum-norm).

### Unital contraction positivity criterion

↑ **Parent:** [Positive linear functional](#positive-linear-functional)

A real-linear contraction on $C(X)$ that preserves $1$ is positive: for $0\leq f\leq1$, $\|1-Tf\|_\infty\leq1$ forces $Tf\geq0$, then scale. In the complex case, a unital norm-one functional is real on real functions, since $|1+it\phi(g)|\leq\|1+itg\|_\infty=1+O(t^2)$ for both signs of $t$. The same [positivity](quantum-information-theory.md#positivity-linear-maps) argument applies pointwise to $\phi(f)=Tf(x)$. This turns a unital [contraction semigroup](functional-analysis.md#contraction-semigroup) into a [Feller semigroup](functional-analysis.md#feller-semigroup).

## Operator norm

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Operator_norm)

The operator norm is $\lVert T\rVert=\sup_{\lVert x\rVert\leq1}\lVert Tx\rVert$.

### Riesz-Thorin theorem

↑ **Parent:** [Operator norm](#operator-norm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz–Thorin_theorem)

For a [linear operator](vector-space.md#linear-operator) bounded from $L^{p_i}$ to $L^{q_i}$ with [norms](functional-analysis.md#norm) $M_i$, $i=0,1$, interpolate reciprocals by $1/p=(1-\theta)/p_0+\theta/p_1$ and $1/q=(1-\theta)/q_0+\theta/q_1$. The intermediate [operator norm](#operator-norm) is at most $M_0^{1-\theta}M_1^\theta$. The complex interpolation proof first treats [simple functions](measure-theory.md#simple-function); completeness and [continuity](calculus.md#continuous-function) on the endpoint sum spaces identify the extension with the original operator. On finite counting spaces it also gives [norm](functional-analysis.md#norm) bounds between sequence spaces.

### Operator norm duality

↑ **Parent:** [Operator norm](#operator-norm)

For bounded operators between [Hilbert spaces](hilbert-space.md), write the norm as the supremum of $|\langle Ax,y\rangle|$ over unit vectors $x,y$. Moving the operator to the other slot proves equality of its norm with that of its [adjoint operator](hilbert-space.md#adjoint-operator). Applied to the exponential matrix, this makes the primal and dual [analytic large sieve inequalities](analytic-number-theory.md#exponential-sum-large-sieve) equivalent.

### Euclidean logarithmic norm

↑ **Parent:** [Operator norm](#operator-norm)

The [Euclidean logarithmic norm](#euclidean-logarithmic-norm) is the largest [eigenvalue](linear-operator-theory.md#eigenvalue) of a [matrix](vector-space.md#matrix)'s Hermitian part. Differentiating $\|y\|_2^2$ along $y'=Ay$ gives $\|e^{tA}\|_2\leq e^{t\mu_2(A)}$. It is the least exponent for such a bound with prefactor one, as a first-order expansion at zero shows. It equals the [spectral abscissa](linear-operator-theory.md#spectral-abscissa) for a [normal matrix](linear-operator-theory.md#normal-matrix), but need not do so otherwise. A scalar rational [stability function](numerical-analysis.md#stability-function) does not generally inherit a bound by its value at this real number.

#### Euclidean semigroup growth bounds

↑ **Parent:** [Euclidean logarithmic norm](#euclidean-logarithmic-norm)

The [spectral radius](analysis.md#spectral-radius) of the [matrix exponential](linear-operator-theory.md#matrix-exponential) gives the lower bound through the [spectral abscissa](linear-operator-theory.md#spectral-abscissa) $s(A)$. Differentiating the squared [Euclidean norm](functional-analysis.md#euclidean-norm) along $q'=Aq$ and bounding its Hermitian quadratic form gives the upper bound through the [Euclidean logarithmic norm](#euclidean-logarithmic-norm) $\mu_2(A)$. A [non-normal matrix](linear-operator-theory.md#non-normal-matrix) can have $\mu_2(A)>0$ despite $s(A)<0$, allowing [transient growth](linear-operator-theory.md#transient-growth) before its ultimate decay.

### Submultiplicativity of the operator norm

↑ **Parent:** [Operator norm](#operator-norm)

For composable bounded [linear operators](vector-space.md#linear-operator), the [operator norm](#operator-norm) satisfies $\|AB\|\leq\|A\|\|B\|$. Indeed, $\|ABx\|\leq\|A\|\|Bx\|\leq\|A\|\|B\|\|x\|$, and taking the supremum over unit vectors proves the bound. It implies $\|[A,B]\|\leq2\|A\|\|B\|$ by the [triangle inequality](topological-analysis.md#triangle-inequality).

### Telescoping bound for products of operators

↑ **Parent:** [Operator norm](#operator-norm)

If $A_j$ and $B_j$ have [operator norm](#operator-norm) at most one, then inserting and subtracting one factor at a time gives

$$
\left\|\prod_{j=1}^mA_j-\prod_{j=1}^mB_j\right\|
\leq\sum_{j=1}^m\|A_j-B_j\|.
$$

#### Unitary product telescoping

↑ **Parent:** [Telescoping bound for products of operators](#telescoping-bound-for-products-of-operators)

Insert one factor difference at a time: the $j$th term is $U_m\cdots U_{j+1}(U_j-V_j)V_{j-1}\cdots V_1$. Multiplication by the surrounding [unitary operators](vector-space.md#unitary-operator) preserves the [spectral norm](#matrix-2-norm), so the triangle inequality gives the displayed dimension-independent bound. No commutation assumption is required.

### Matrix 2-norm

↑ **Parent:** [Operator norm](#operator-norm)

The matrix 2-norm is the [operator norm](#operator-norm) induced by the [Euclidean norm](functional-analysis.md#euclidean-norm):

$$
\|A\|_2=\sup_{x\ne0}\frac{\|Ax\|_2}{\|x\|_2}.
$$

It equals the largest [singular value](linear-algebra.md#singular-value) of $A$ and is invariant under multiplication by [orthogonal](linear-algebra.md#orthogonal-matrix) or [unitary](vector-space.md#unitary-operator) matrices.

The [matrix norm](vector-space.md#matrix-norm) induced by Euclidean vector norms is $\|A\|_2=\sup_{x\ne0}\|Ax\|_2/\|x\|_2$, equal to the largest singular value.

## Completeness of the dual space

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

The continuous dual of every normed space is Banach because an operator-norm Cauchy sequence converges pointwise to a bounded linear functional and then uniformly on the unit ball.

## Duality of sequence spaces

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

Coordinate pairing gives $(\ell^p)^*=\ell^q$ for $1<p<\infty$, $(\ell^1)^*=\ell^\infty$, and $(c_0)^*=\ell^1$.

These are continuous-dual identifications under coordinate pairing, related to but distinct from the definition of an [Lp space](measure-theory.md#lp-space).

### Duality of l1 and l infinity

↑ **Parent:** [Duality of sequence spaces](#duality-of-sequence-spaces)

For $y\in\ell^\infty$, the formula $\phi_y(x)=\sum_nx_ny_n$ defines a bounded functional on $\ell^1$ with $\|\phi_y\|=\|y\|_\infty$. Conversely, every $\phi\in(\ell^1)^*$ is represented this way by the bounded sequence $y_n=\phi(e_n)$. This is an [isometric isomorphism of normed spaces](functional-analysis.md#isometric-isomorphism-of-normed-spaces).

#### Schur property

↑ **Parent:** [Duality of l1 and l infinity](#duality-of-l1-and-l-infinity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_property)

A [Banach space](banach-space.md) has the Schur property when every [weakly convergent](weak-topology.md#weak-convergence) sequence converges with respect to the [norm topology](functional-analysis.md#norm-topology).

##### Gliding hump argument

↑ **Parent:** [Schur property](#schur-property)

A gliding hump argument selects a subsequence and successive finite coordinate blocks so that each selected vector has little mass before and after its assigned block. A bounded dual vector can then align its signs independently on those disjoint blocks.

###### Schur property of l1

↑ **Parent:** [Gliding hump argument](#gliding-hump-argument)

The [l-p sequence space](banach-space.md#l-p-sequence-space) $\ell^1$ has the [Schur property](#schur-property). If a weakly null sequence stayed bounded below in norm, coordinatewise convergence and summability would select disjoint blocks containing almost all of successive terms. A sequence in $\ell^\infty$ matching their signs on those blocks would pair uniformly positively with a subsequence, contradicting [weak convergence](weak-topology.md#weak-convergence) through the [duality of l1 and l infinity](#duality-of-l1-and-l-infinity).

## Duality of Lp spaces

↑ **Parent:** [Continuous dual space](continuous-dual-space.md)

For $1\leq p<\infty$ and conjugate exponent $q$, every bounded linear functional on $L^p$ over a sigma-finite measure space has the form

$$
f\longmapsto\int f\omega
$$

for a unique $\omega\in L^q$, and its operator norm is $\|\omega\|_q$. At the endpoint $p=1$, this says $(L^1)^*=L^\infty$.

This identifies the [continuous dual space](continuous-dual-space.md) of an [Lp space](measure-theory.md#lp-space); it is not an alternative definition of the entire Lp-space topic.

### Closed-hyperplane proof of Lp duality

↑ **Parent:** [Duality of Lp spaces](#duality-of-lp-spaces)

Let $1<p<\infty$ and $q=p/(p-1)$. For a nonzero [bounded linear functional](topological-vector-space.md#continuous-linear-functional) $\ell$ on an [Lp space](measure-theory.md#lp-space), choose $f_0$ with $\ell(f_0)=1$ and a closest point $h$ in its closed kernel. Put $z=f_0-h$. The variational condition is $\int |z|^{p-2}\overline z\,k=0$ for every kernel element $k$. Since $f-\ell(f)z$ lies in the kernel, $\ell(f)=\int fg$ with $g=|z|^{p-2}\overline z/\|z\|_p^p\in L^q$. [Hölder's inequality](real-analysis.md#holder-s-inequality) gives the upper norm bound; testing against $|g|^{q-2}\overline g$ gives equality. Thus the representation is an isometric linear isomorphism when the pairing is bilinear.

### Lp duality on an arbitrary measure space

↑ **Parent:** [Duality of Lp spaces](#duality-of-lp-spaces)

For conjugate exponents $p,q\in(1,\infty)$, every [bounded linear functional](topological-vector-space.md#continuous-linear-functional) on an [Lp space](measure-theory.md#lp-space) is uniquely $h\mapsto\int hg\,d\mu$ for $g\in L^q$, with functional norm $\|g\|_q$. This holds on arbitrary [measure spaces](measure-theory.md#measure-space). Apply the [Radon-Nikodym theorem](measure-theory.md#radon-nikodym-theorem) on finite-measure pieces, then use [support localization of an Lp functional](#support-localization-of-an-lp-functional) to obtain one global density without assuming sigma-finiteness of the entire measure.

#### Support localization of an Lp functional

↑ **Parent:** [Lp duality on an arbitrary measure space](#lp-duality-on-an-arbitrary-measure-space)

For $1<p<\infty$, local [Radon-Nikodym derivatives](measure-theory.md#radon-nikodym-derivative) $g_E$ representing an $L^p$ functional on finite-measure sets have uniformly bounded $L^q$ mass. Choose a sequence of finite-measure sets approaching the supremum of that mass, and glue their compatible densities on their union $S$. Any finite-measure set outside $S$ must have zero local density, since otherwise it would increase the supremum. Every [Lp space](measure-theory.md#lp-space) function is approximable by [simple functions](measure-theory.md#simple-function) of finite-measure support, so the glued density represents the functional on the whole space.

### Dual of L infinity is larger than L1

↑ **Parent:** [Duality of Lp spaces](#duality-of-lp-spaces)

On $\mathbb R^n$, integration embeds $L^1$ isometrically into $(L^\infty)^*$, but this is not surjective. For example, the functional taking the limit at infinity on $\mathbb C1\oplus C_0(\mathbb R^n)$ extends to $L^\infty$ by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem); it vanishes on compactly supported functions and is one on the constant function, so no $L^1$ density represents it.

### Reflexivity of Lp spaces

↑ **Parent:** [Duality of Lp spaces](#duality-of-lp-spaces)

For $1<p<\infty$, the identifications $(L^p)^*=L^q$ and $(L^q)^*=L^p$ make $L^p$ reflexive. On a non-atomic space such as $\mathbb R^n$, neither $L^1$ nor $L^\infty$ is reflexive.

### Positive functional representation on Lp

↑ **Parent:** [Duality of Lp spaces](#duality-of-lp-spaces)

On a finite measure space, a positive functional $\Lambda\in(L^p)^*$ defines the finite measure $\nu(E)=\Lambda(\mathbf1_E)$. The [Radon-Nikodym theorem](measure-theory.md#radon-nikodym-theorem) gives $d\nu=\omega\,d\mu$ with $\omega\geq0$. The bound

$$
\int|f|\omega=\Lambda(|f|)
\leq\|\Lambda\|\,\|f\|_p
$$

and $L^p$-$L^q$ norm duality imply $\omega\in L^q$, after which density extends the integral representation to every $f\in L^p$.

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (43)

- [Closed unit ball](functional-analysis.md#closed-unit-ball)
- [Compactly supported distribution space](distribution-theory.md#compactly-supported-distribution-space)
- [Continuous linear functional](topological-vector-space.md#continuous-linear-functional)
- [Duality of Lp spaces](#duality-of-lp-spaces)
- [Original and weak continuity of linear maps between Fréchet spaces](weak-topology.md#original-and-weak-continuity-of-linear-maps-between-frechet-spaces)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#21f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#22f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#21f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#22h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#22i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#22i/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#22i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327.md#1/a/solution)
- [2](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327.md#2)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#22f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#22f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-106.md#4/a/solution)
- [Regular Borel measure](measure-theory.md#regular-borel-measure)
- [Separable Banach space](banach-space.md#separable-banach-space)
- [Strong dual topology](#strong-dual-topology)
- [Weak convergence](weak-topology.md#weak-convergence)
- [Weakly bounded set](weak-topology.md#weakly-bounded-set)
- [Weakly compact set is norm bounded](weak-topology.md#weakly-compact-set-is-norm-bounded)
- [Weakly null sequence](weak-topology.md#weakly-null-sequence)
