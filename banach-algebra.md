# Banach algebra

↑ **Parent:** [Functional analysis](functional-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Banach_algebra)

A Banach algebra is an associative algebra with a complete submultiplicative norm, $\lVert ab\rVert\leq\lVert a\rVert\lVert b\rVert$.

**Table of contents**

- [Semisimple Banach algebra](#semisimple-banach-algebra)
  - [Automatic continuity onto a semisimple Banach algebra](#automatic-continuity-onto-a-semisimple-banach-algebra)
- [Volterra convolution algebra on a finite interval](#volterra-convolution-algebra-on-a-finite-interval)
- [Renorming a separately continuous Banach algebra](#renorming-a-separately-continuous-banach-algebra)
- [Hermitian Banach algebra](#hermitian-banach-algebra)
  - [Spectral permanence for Hermitian Banach algebras](#spectral-permanence-for-hermitian-banach-algebras)
- [L1 convolution algebra](#l1-convolution-algebra)
  - [Character space of an Abelian L1 group algebra](#character-space-of-an-abelian-l1-group-algebra)
- [Closed subalgebra of a Banach algebra](#closed-subalgebra-of-a-banach-algebra)
- [Continuously differentiable functions on a compact interval form a Banach algebra](#continuously-differentiable-functions-on-a-compact-interval-form-a-banach-algebra)
  - [Character space of C1 on a compact interval](#character-space-of-c1-on-a-compact-interval)
- [Uniform algebra](#uniform-algebra)
  - [Boundary-analytic disk algebra with doubled character space](#boundary-analytic-disk-algebra-with-doubled-character-space)
  - [Disk algebra](#disk-algebra)
  - [Natural uniform algebra](#natural-uniform-algebra)
    - [Finite-generator criterion for a natural uniform algebra](#finite-generator-criterion-for-a-natural-uniform-algebra)
- [Semisimple commutative Banach algebra](#semisimple-commutative-banach-algebra)
- [Supremum bound for a complete function-algebra norm](#supremum-bound-for-a-complete-function-algebra-norm)
- [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)
  - [Identity component of Banach-algebra invertibles](#identity-component-of-banach-algebra-invertibles)
  - [Noninvertible limits of invertibles have no one-sided inverse](#noninvertible-limits-of-invertibles-have-no-one-sided-inverse)
  - [Right inverse of an algebra element](#right-inverse-of-an-algebra-element)
  - [Left inverse of an algebra element](#left-inverse-of-an-algebra-element)
  - [Inverse norm divergence at noninvertible boundary points](#inverse-norm-divergence-at-noninvertible-boundary-points)
  - [Continuity of inversion in a Banach algebra](#continuity-of-inversion-in-a-banach-algebra)
- [Qp-Banach algebra](#qp-banach-algebra)
- [Gelfand-Mazur theorem](#gelfand-mazur-theorem)
- [Algebra norm](#algebra-norm)
  - [Renorming a bounded multiplicative semigroup](#renorming-a-bounded-multiplicative-semigroup)
    - [Simultaneous spectral-radius renorming](#simultaneous-spectral-radius-renorming)
  - [Submultiplicativity](#submultiplicativity)
  - [Continuous functions on the complex plane admit no algebra norm](#continuous-functions-on-the-complex-plane-admit-no-algebra-norm)
  - [Entire function algebra admits no complete algebra norm](#entire-function-algebra-admits-no-complete-algebra-norm)
    - [Compact-disk algebra norm on entire functions](#compact-disk-algebra-norm-on-entire-functions)
  - [Minimality of the supremum norm on C(K)](#minimality-of-the-supremum-norm-on-c-k)
- [Unitization of an algebra](#unitization-of-an-algebra)
- [Neumann series](#neumann-series)
- [Spectrum of an element](#spectrum-of-an-element)
  - [Resolvent set of a Banach algebra element](#resolvent-set-of-a-banach-algebra-element)
  - [Resolvent components in a closed unital subalgebra](#resolvent-components-in-a-closed-unital-subalgebra)
    - [Boundary inclusion of spectra in a closed unital subalgebra](#boundary-inclusion-of-spectra-in-a-closed-unital-subalgebra)
  - [Translation of the spectrum by a scalar](#translation-of-the-spectrum-by-a-scalar)
  - [Quasinilpotent element](#quasinilpotent-element)
  - [Nonzero spectra of products in opposite orders](#nonzero-spectra-of-products-in-opposite-orders)
  - [Nonemptiness of the Banach-algebra spectrum](#nonemptiness-of-the-banach-algebra-spectrum)
  - [Approximate point spectrum](#approximate-point-spectrum)
    - [Bilateral shift operator](#bilateral-shift-operator)
  - [Resolvent of an element](#resolvent-of-an-element)
    - [Resolvent Cauchy coefficient formula](#resolvent-cauchy-coefficient-formula)
    - [Resolvent identity](#resolvent-identity)
    - [Resolvent norm](#resolvent-norm)
    - [Pseudospectrum](#pseudospectrum)
    - [Riesz projection](#riesz-projection)
      - [Disconnected spectrum yields a nontrivial invariant subspace](#disconnected-spectrum-yields-a-nontrivial-invariant-subspace)
  - [Spectrum in a closed unital subalgebra](#spectrum-in-a-closed-unital-subalgebra)
    - [Connected-component permanence of subalgebra invertibility](#connected-component-permanence-of-subalgebra-invertibility)
  - [Holomorphic functional calculus](#holomorphic-functional-calculus)
    - [Logarithm from a spectral slit in a Banach algebra](#logarithm-from-a-spectral-slit-in-a-banach-algebra)
    - [Spectral idempotent from a separated spectrum](#spectral-idempotent-from-a-separated-spectrum)
    - [Banach algebra exponential](#banach-algebra-exponential)
    - [Principal cube root of a Banach-algebra element](#principal-cube-root-of-a-banach-algebra-element)
    - [Principal square root in a commutative Banach algebra](#principal-square-root-in-a-commutative-banach-algebra)
    - [Resolvent-generated commutative algebra](#resolvent-generated-commutative-algebra)
    - [Continuity and uniqueness of holomorphic functional calculus](#continuity-and-uniqueness-of-holomorphic-functional-calculus)
    - [Logarithm of an element near the identity](#logarithm-of-an-element-near-the-identity)
    - [Composition rule for holomorphic functional calculus](#composition-rule-for-holomorphic-functional-calculus)
    - [Injectivity through a holomorphic functional calculus with nonvanishing derivative](#injectivity-through-a-holomorphic-functional-calculus-with-nonvanishing-derivative)
  - [Full spectrum](#full-spectrum)
- [Character of an algebra](#character-of-an-algebra)
  - [Maximal ideals of a commutative complex unital Banach algebra are character kernels](#maximal-ideals-of-a-commutative-complex-unital-banach-algebra-are-character-kernels)
  - [Maximal ideals of a complex unital Banach algebra are character kernels](#maximal-ideals-of-a-complex-unital-banach-algebra-are-character-kernels)
  - [Characters of a C-star algebra respect the involution](#characters-of-a-c-star-algebra-respect-the-involution)
  - [Automatic continuity of characters](#automatic-continuity-of-characters)
  - [Character space of an algebra](#character-space-of-an-algebra)
    - [Maximal ideal space of a commutative Banach algebra](#maximal-ideal-space-of-a-commutative-banach-algebra)
    - [Character space of R(K)](#character-space-of-r-k)
    - [Absence of characters on an operator algebra with isomorphic complementary summands](#absence-of-characters-on-an-operator-algebra-with-isomorphic-complementary-summands)
    - [Gelfand topology](#gelfand-topology)
    - [Evaluation character](#evaluation-character)
    - [Gelfand representation](#gelfand-representation)
      - [Involution alone does not imply an isometric Gelfand transform](#involution-alone-does-not-imply-an-isometric-gelfand-transform)
      - [Spectrum equals character values in a commutative Banach algebra](#spectrum-equals-character-values-in-a-commutative-banach-algebra)
      - [Gelfand representation theorem](#gelfand-representation-theorem)
- [Banach subalgebra generated by one element](#banach-subalgebra-generated-by-one-element)
  - [Spectrum of a polynomial-generated Banach subalgebra](#spectrum-of-a-polynomial-generated-banach-subalgebra)
- [C-star algebra](#c-star-algebra)
  - [Unitization of a C-star algebra](#unitization-of-a-c-star-algebra)
    - [C-star unitization by left multiplication](#c-star-unitization-by-left-multiplication)
  - [Calkin algebra](#calkin-algebra)
  - [C-star subalgebra](#c-star-subalgebra)
  - [C-star homomorphism](#c-star-homomorphism)
    - [Injective C-star homomorphism is isometric](#injective-c-star-homomorphism-is-isometric)
  - [Spectral permanence for C-star algebras](#spectral-permanence-for-c-star-algebras)
  - [Continuous functional calculus](#continuous-functional-calculus)
    - [Nonunital continuous functional calculus](#nonunital-continuous-functional-calculus)
    - [Square-root resolvent integral in a C-star algebra](#square-root-resolvent-integral-in-a-c-star-algebra)
      - [Order preservation by the positive square root](#order-preservation-by-the-positive-square-root)
    - [Strong continuity of functional calculus through resolvents](#strong-continuity-of-functional-calculus-through-resolvents)
    - [Disconnected spectrum gives a reducing subspace](#disconnected-spectrum-gives-a-reducing-subspace)
  - [C-star identity](#c-star-identity)
  - [Commutative Gelfand--Naimark theorem](#commutative-gelfand-naimark-theorem)
  - [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)
    - [Positive cone of a C-star algebra](#positive-cone-of-a-c-star-algebra)
    - [Squaring is not order preserving in a C-star algebra](#squaring-is-not-order-preserving-in-a-c-star-algebra)
    - [Inversion reverses the order of strictly positive elements](#inversion-reverses-the-order-of-strictly-positive-elements)
    - [Congruence preserves positivity in a C-star algebra](#congruence-preserves-positivity-in-a-c-star-algebra)
    - [Positivity of adjoint products from spectral positivity](#positivity-of-adjoint-products-from-spectral-positivity)
    - [Positive square root in a C-star algebra](#positive-square-root-in-a-c-star-algebra)
    - [Spectral characterization of a positive element in a C-star algebra](#spectral-characterization-of-a-positive-element-in-a-c-star-algebra)
  - [Hermitian element of a C-star algebra](#hermitian-element-of-a-c-star-algebra)
  - [Unitary element of a C-star algebra](#unitary-element-of-a-c-star-algebra)
  - [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra)
    - [Star polynomial in one normal element](#star-polynomial-in-one-normal-element)
    - [Unital versus nonunital generation by a normal element](#unital-versus-nonunital-generation-by-a-normal-element)
    - [Real spectrum criterion for a normal C-star element](#real-spectrum-criterion-for-a-normal-c-star-element)
    - [Spectral radius norm equality for normal elements](#spectral-radius-norm-equality-for-normal-elements)
  - [Positive functional on a C-star algebra](#positive-functional-on-a-c-star-algebra)
    - [Cauchy–Schwarz inequality for positive C-star functionals](#cauchy-schwarz-inequality-for-positive-c-star-functionals)
    - [Tracial positive functional](#tracial-positive-functional)
    - [State on a C-star algebra](#state-on-a-c-star-algebra)
      - [States separate elements of a C-star algebra](#states-separate-elements-of-a-c-star-algebra)
      - [Spectral values attained by C-star states](#spectral-values-attained-by-c-star-states)
      - [Pure state on a C-star algebra](#pure-state-on-a-c-star-algebra)
  - [Borel functional calculus for a normal operator](#borel-functional-calculus-for-a-normal-operator)
    - [Spectral essential range in Borel functional calculus](#spectral-essential-range-in-borel-functional-calculus)
    - [Normal square root from Borel functional calculus](#normal-square-root-from-borel-functional-calculus)
    - [Functional calculus convergence](#functional-calculus-convergence)
  - [Partial isometry](#partial-isometry)
  - [Polar decomposition of a bounded operator](#polar-decomposition-of-a-bounded-operator)
    - [Absolute value of an operator](#absolute-value-of-an-operator)
    - [Unitary polar factor of a finite compression](#unitary-polar-factor-of-a-finite-compression)

## Semisimple Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

A [Banach algebra](banach-algebra.md) is semisimple when its [Jacobson radical](noncommutative-algebra.md#jacobson-radical) is zero. This does not assert that every [quasinilpotent element](#quasinilpotent-element) is zero. For example, the algebra of bounded operators on a [Banach space](banach-space.md) of dimension greater than one is semisimple, but contains nonzero square-zero rank-one operators. This notion also does not require the finite-dimensional direct-sum decomposition associated with a [semisimple algebra](associative-algebra.md#semisimple-algebra).

### Automatic continuity onto a semisimple Banach algebra

↑ **Parent:** [Semisimple Banach algebra](#semisimple-banach-algebra)

An [algebra homomorphism](algebra.md#algebra-homomorphism-over-a-field) onto a [semisimple Banach algebra](#semisimple-banach-algebra) is [continuous](calculus.md#continuous-function). To see the spectral mechanism, suppose $a_n\to0$ and $T(a_n)\to b$. For any $c\in B$, choose $u,v\in A$ with $T(u)=b$ and $T(v)=c$, and [set](set.md) $d=cb$, $d_n=T(va_n)$. Apply the [spectral-radius three-circle inequality](analysis.md#spectral-radius-three-circle-inequality) to $T((1-z)va_n+zvu)$. On the outer circle its [norm](functional-analysis.md#norm) tends uniformly to $\|d\|$; on the circle of radius $1/R$ its [spectral radius](analysis.md#spectral-radius) is bounded by $(1+1/R)\|va_n\|+\|vu\|/R$. Hence $r(d)^2\le\|d\|\|vu\|/R$ for every $R>1$, so $r(cb)=0$. The [unit criterion for the Jacobson radical](noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical) gives $b\in J(B)=0$, and the [closed graph theorem](functional-analysis.md#closed-graph-theorem) finishes the proof.

## Volterra convolution algebra on a finite interval

↑ **Parent:** [Banach algebra](banach-algebra.md)

Truncated [convolution](fourier-analysis.md#convolution) makes $L^1(0,1)$ a commutative nonunital [Banach algebra](banach-algebra.md). The [Tonelli theorem](measure-theory.md#tonelli-theorem) gives $\|f*g\|_1\leq\|f\|_1\|g\|_1$, and the [Fubini theorem](measure-theory.md#fubini-s-theorem) gives associativity over the integration simplex. Its [unitization](#unitization-of-an-algebra) is $\mathbb C\oplus L^1(0,1)$ with norm $|\alpha|+\|f\|_1$ and product $(\alpha,f)(\beta,g)=(\alpha\beta,\alpha g+\beta f+f*g)$. The constant function one has convolution powers $t^{n-1}/(n-1)!$, of norm $1/n!$. Thus it is a nonnilpotent [quasinilpotent element](#quasinilpotent-element) in this unitization.

## Renorming a separately continuous Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

If an associative unital [algebra](algebra.md) has a complete [norm](functional-analysis.md#norm) and separately continuous multiplication, the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) applied to $L_x(y)=xy$, for $\|x\|\leq1$, yields $\|xy\|\leq C\|x\|\|y\|$. The [operator norm](continuous-dual-space.md#operator-norm) of $L_x$ then defines an equivalent [algebra norm](#algebra-norm): $\|x\|/\|e\|\leq\|L_x\|\leq C\|x\|$, and $L_{xy}=L_xL_y$ proves [submultiplicativity](#submultiplicativity). It normalizes the identity to norm one.

## Hermitian Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

A Hermitian [Banach algebra](banach-algebra.md) is a [Banach algebra](banach-algebra.md) with an [algebra involution](associative-algebra.md#algebra-involution) for which every [Hermitian element of a star algebra](associative-algebra.md#hermitian-element-of-a-star-algebra) has real [spectrum of an element](#spectrum-of-an-element). A [closed](topology.md#closed-set) unital [star-subalgebra](associative-algebra.md#star-subalgebra) has [spectral permanence for Hermitian Banach algebras](#spectral-permanence-for-hermitian-banach-algebras). The assumption is weaker than being a [C-star algebra](#c-star-algebra) and does not require the C-star [norm](functional-analysis.md#norm) identity.

### Spectral permanence for Hermitian Banach algebras

↑ **Parent:** [Hermitian Banach algebra](#hermitian-banach-algebra)

Let $B$ be a [closed](topology.md#closed-set) [star-subalgebra](associative-algebra.md#star-subalgebra) of a unital [Hermitian Banach algebra](#hermitian-banach-algebra) $A$, containing the same identity. For Hermitian $h\in B$, the complement of $\sigma_A(h)\subseteq\mathbb R$ is [connected](geometry-and-topology.md#connected-space). The resolvent belongs to $B$ at large modulus by the [Neumann series](#neumann-series); its membership in $B$ is both open and [closed](topology.md#closed-set) in that complement, so $\sigma_B(h)=\sigma_A(h)$. If $b$ is invertible in $A$, both $bb^*$ and $b^*b$ are invertible there and [Hermitian algebra elements](associative-algebra.md#hermitian-element-of-a-star-algebra), hence invertible in $B$. Their inverses supply respectively a right and a left inverse for $b$ in $B$, proving invertibility there. Applying this to $b-\lambda1$ proves the spectrum equality.

## L1 convolution algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

With left [Haar measure](measure-theory.md#haar-measure), $(f*g)(x)=\int_G f(y)g(y^{-1}x)\,dm(y)$ makes $L^1(G)$ a [Banach algebra](banach-algebra.md), since $\|f*g\|_1\leq\|f\|_1\|g\|_1$. For an Abelian group it is commutative, and the involution is $f^*(x)=\overline{f(x^{-1})}$. Its nonzero [characters of an algebra](#character-of-an-algebra) are exactly integration against inverses of continuous unitary group characters.

// Target: geometry-and-topology.bigb

### Character space of an Abelian L1 group algebra

↑ **Parent:** [L1 convolution algebra](#l1-convolution-algebra)

For a locally compact Hausdorff Abelian group, each [continuous unitary character](topological-group.md#continuous-unitary-character) defines an [algebra character](#character-of-an-algebra) by $f\mapsto\int f(x)\chi(x)\,dx$. Conversely, if $\Phi$ is a nonzero [algebra character](#character-of-an-algebra) and $\Phi(g)\ne0$, the ratio $\Phi(T_xg)/\Phi(g)$ is independent of $g$, continuous and multiplicative. Translation [isometries](riemannian-geometry.md#isometry) bound all its integer powers, so its modulus is one. The [convolution](fourier-analysis.md#convolution) formula $f*g=\int f(x)T_xg\,dx$ recovers $\Phi(f)=\int f\chi$. The [Gelfand topology](#gelfand-topology) corresponds to the [compact-open topology](real-analysis.md#compact-open-topology) on the [Pontryagin dual group](group.md#pontryagin-dual-group); conjugating the characters gives the alternative Fourier sign convention.

## Closed subalgebra of a Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

A norm-closed [subalgebra](algebra.md#subalgebra) of a [Banach algebra](banach-algebra.md) is itself a Banach algebra with the inherited norm: completeness follows from closedness, and the submultiplicative norm bound restricts to it. A unital inclusion uses the same identity as the ambient algebra. Inverse membership may still differ between the two algebras; [spectrum in a closed unital subalgebra](#spectrum-in-a-closed-unital-subalgebra) describes that difference.

## Continuously differentiable functions on a compact interval form a Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

With complex scalars and pointwise multiplication, the [product rule](calculus.md#product-rule) gives a submultiplicative norm. For a Cauchy sequence, uniform limits $f$ of the functions and $g$ of their derivatives satisfy $f(t)-f(0)=\int_0^tg(s)\,ds$, proving $f'=g$ and completeness. Polynomials are dense in this norm: approximate $f'$ uniformly by polynomials and integrate, fixing the initial value. This also identifies the [character space of C1 on a compact interval](#character-space-of-c1-on-a-compact-interval).

### Character space of C1 on a compact interval

↑ **Parent:** [Continuously differentiable functions on a compact interval form a Banach algebra](#continuously-differentiable-functions-on-a-compact-interval-form-a-banach-algebra)

The coordinate function has spectrum $[0,1]$: outside the interval its difference from a scalar has a continuously differentiable reciprocal, and on the interval it has a zero. Every [character of an algebra](#character-of-an-algebra) therefore takes the coordinate to some $t\in[0,1]$. Polynomial density in the norm containing both function and derivative, together with [automatic continuity of characters](#automatic-continuity-of-characters), forces evaluation at $t$ on every function. The [maximal ideals](commutative-algebra.md#maximal-ideal) are exactly $\{f:f(t)=0\}$.

## Uniform algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_algebra)

A [uniform algebra](#uniform-algebra) on a [compact Hausdorff space](topology.md#compact-hausdorff-space) $K$ is a closed complex subalgebra of $C(K)$, with the [supremum norm](functional-analysis.md#supremum-norm), containing the constants and separating points. Evaluation embeds $K$ continuously and injectively in the [character space of an algebra](#character-space-of-an-algebra). The embedding is a [homeomorphism](topology.md#homeomorphism) onto a closed subset because its domain is compact and its target is Hausdorff. Extra characters need not be point evaluations on the specified $K$.

### Boundary-analytic disk algebra with doubled character space

↑ **Parent:** [Uniform algebra](#uniform-algebra)

Let $C$ consist of continuous functions on the closed unit disk whose boundary values extend to a member of the [disk algebra](#disk-algebra). The extension is unique by the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle); the extension map $T:C\to A(\overline{\mathbb D})$ is a surjective unital algebra homomorphism of norm at most one. Its kernel $I$ is the [ideal](commutative-algebra.md#ideal) of functions vanishing on the boundary. A character vanishing on $I$ factors through $T$, so it is $f\mapsto T(f)(\lambda)$ for some closed-disk point $\lambda$. For a character $\chi$ not vanishing on $I$, choose $h\in I$ with $\chi(h)\ne0$. The rule $F\mapsto\chi(hF)/\chi(h)$ extends $\chi$ to a character of all continuous functions on the disk: multiplicativity follows from $\chi(hF)\chi(hG)=\chi(h)\chi(hFG)$. It is therefore evaluation at an interior point, since its value at $h$ is nonzero. These two closed-disk families agree exactly on their boundaries. Their glued compact space maps continuously and bijectively to the Hausdorff [character space of an algebra](#character-space-of-an-algebra), giving the stated [homeomorphism](topology.md#homeomorphism). The algebra is closed because uniform convergence of boundary data gives uniform convergence of their analytic extensions.

### Disk algebra

↑ **Parent:** [Uniform algebra](#uniform-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disk_algebra)

The [disk algebra](#disk-algebra) consists of functions continuous on the closed unit disk and holomorphic in its interior, with the [supremum norm](functional-analysis.md#supremum-norm). Polynomials are dense: dilations $f_r(z)=f(rz)$ converge uniformly to $f$ as $r\uparrow1$, and each $f_r$ is uniformly approximated on the closed disk by its Taylor polynomials. A [character of an algebra](#character-of-an-algebra) is therefore determined by its value $\lambda$ at the coordinate function; boundedness gives $|\lambda|\leq1$, and polynomial approximation yields $\varphi(f)=f(\lambda)$. Consequently the [disk algebra](#disk-algebra) is a [natural uniform algebra](#natural-uniform-algebra) on the closed disk.

### Natural uniform algebra

↑ **Parent:** [Uniform algebra](#uniform-algebra)

A [uniform algebra](#uniform-algebra) on $K$ is natural if every [character of an algebra](#character-of-an-algebra) is evaluation at a point of $K$. The evaluation embedding then identifies its character space homeomorphically with $K$. A [natural uniform algebra](#natural-uniform-algebra) is characterized by the [finite-generator criterion for a natural uniform algebra](#finite-generator-criterion-for-a-natural-uniform-algebra). In particular, $C(K)$ is natural; the [disk algebra](#disk-algebra) is natural when its underlying space is the closed disk.

#### Finite-generator criterion for a natural uniform algebra

↑ **Parent:** [Natural uniform algebra](#natural-uniform-algebra)

A [uniform algebra](#uniform-algebra) is natural exactly when functions with no common zero generate the unit [ideal](commutative-algebra.md#ideal). If a generated [ideal](commutative-algebra.md#ideal) is proper, it is contained in a [maximal ideal](commutative-algebra.md#maximal-ideal). That [maximal ideal](commutative-algebra.md#maximal-ideal) is closed: the closure of a proper [ideal](commutative-algebra.md#ideal) stays proper, since an element within distance less than one of the identity is invertible by the [Neumann series](#neumann-series). The [Gelfand-Mazur theorem](#gelfand-mazur-theorem) identifies the maximal-ideal quotient with the complex numbers, yielding a [character of an algebra](#character-of-an-algebra). Naturality would make that character a common-zero evaluation, a contradiction. Conversely, the asserted unit-ideal property makes the zero sets of every finite collection in a character's kernel intersect. Compactness gives a point common to all these zero sets; applying this to $f-\varphi(f)1$ proves $\varphi(f)=f(x)$. For $C(K)$, one can directly take $g_j=\overline{f_j}/\sum_k|f_k|^2$.

## Semisimple commutative Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

A commutative [Banach algebra](banach-algebra.md) is semisimple when its [Jacobson radical](noncommutative-algebra.md#jacobson-radical) is zero. For a complex unital [Banach algebra](banach-algebra.md) this is equivalent to injectivity of the [Gelfand transform](#gelfand-representation). This condition concerns the [Jacobson radical](noncommutative-algebra.md#jacobson-radical); it does not assert a finite product decomposition as in finite-dimensional semisimple algebra theory.

## Supremum bound for a complete function-algebra norm

↑ **Parent:** [Banach algebra](banach-algebra.md)

For an algebra of complex-valued functions with a complete [algebra norm](#algebra-norm), every point value $f(t)$ belongs to the [spectrum of an element](#spectrum-of-an-element) of $f$ in the artificial [unitization](#unitization-of-an-algebra). Indeed $(h,\lambda)\mapsto h(t)+\lambda$ is an algebraic unital [character of an algebra](#character-of-an-algebra), and it vanishes on $f-f(t)1$. The [spectrum](linear-operator-theory.md#spectrum-functional-analysis) bound gives $|f(t)|\le\|f\|$ without first assuming that evaluation is continuous.

## Group of invertible elements of a Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

The invertible elements of a unital [Banach algebra](banach-algebra.md) form an open multiplicative [group](group.md). For $a\in G(A)$, every $b$ satisfying $\|a^{-1}\|\|b-a\|<1$ is invertible, because $b=a(1+a^{-1}(b-a))$ and the second factor has a [Neumann series](#neumann-series) inverse.

### Identity component of Banach-algebra invertibles

↑ **Parent:** [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)

Finite products of [Banach algebra exponentials](#banach-algebra-exponential) form a [subgroup](group.md#subgroup): inverses are $e^{-a}$ and conjugation sends $e^a$ to $e^{gag^{-1}}$. Each product is joined to the identity by $t\mapsto\prod e^{ta_i}$. The [logarithm of an element near the identity](#logarithm-of-an-element-near-the-identity) puts a [norm](functional-analysis.md#norm) neighborhood of $1$ in this [subgroup](group.md#subgroup), so its cosets are [open](topology.md#open-set) and its complement is [open](topology.md#open-set). It is therefore exactly the [identity component of a topological group](geometry-and-topology.md#identity-component), and is an [open](topology.md#open-set), [closed](topology.md#closed-set), [normal subgroup](group-theory.md#normal-subgroup). A product of exponentials need not be a single exponential in a noncommutative algebra.

### Noninvertible limits of invertibles have no one-sided inverse

↑ **Parent:** [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)

Suppose $a_n\to a$ in a unital [Banach algebra](banach-algebra.md), with each $a_n$ invertible. If $ba=1$, then $ba_n\to1$, so $ba_n$ is invertible eventually by the [Neumann series](#neumann-series). Then $b=(ba_n)a_n^{-1}$ is invertible, and $a=b^{-1}$. The analogous argument with $a_nb\to1$ treats a [right inverse of an algebra element](#right-inverse-of-an-algebra-element). Thus a noninvertible such limit admits neither type of one-sided inverse.

### Right inverse of an algebra element

↑ **Parent:** [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)

A right inverse of an element $a$ is an element $b$ with $ab=1$. A [left inverse of an algebra element](#left-inverse-of-an-algebra-element) and a [right inverse of an algebra element](#right-inverse-of-an-algebra-element), when both exist, coincide. For the [unilateral shift operator](linear-operator-theory.md#unilateral-shift-operator) $S$, $S^*S=1$ but $SS^*\ne1$, exhibiting the distinction in the [Banach algebra](banach-algebra.md) of bounded operators.

### Left inverse of an algebra element

↑ **Parent:** [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)

A left inverse of an element $a$ of a unital [associative algebra](associative-algebra.md) is an element $b$ with $ba=1$. A right inverse instead satisfies $ab=1$. If both exist, they agree: $b=b(ac)=(ba)c=c$. A one-sided inverse alone need not imply invertibility in an infinite-dimensional [Banach algebra](banach-algebra.md).

### Inverse norm divergence at noninvertible boundary points

↑ **Parent:** [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)

In a unital [Banach algebra](banach-algebra.md), if a subsequence of inverse norms remained bounded, $a=a_n[1+a_n^{-1}(a-a_n)]$ would be invertible for large subsequence indices by the [Neumann series](#neumann-series). This contradicts noninvertibility of $a$. If $A$ is a closed unital subalgebra of a larger [Banach algebra](banach-algebra.md) $B$ and the $a_n$ lie in $G(A)$, then such a limit cannot be invertible in $B$ either: [continuity of inversion in a Banach algebra](#continuity-of-inversion-in-a-banach-algebra) would make their inverses converge in $B$ to $a^{-1}$, which closedness puts in $A$.

### Continuity of inversion in a Banach algebra

↑ **Parent:** [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)

Inversion is continuous on the [group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra). The [Neumann series](#neumann-series) gives a local bound on inverse norms, while $b^{-1}-a^{-1}=b^{-1}(a-b)a^{-1}$ makes the difference tend to zero as $b\to a$.

## Qp-Banach algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

A Qp-Banach algebra is a $\mathbb Q_p$-algebra with a complete non-Archimedean submultiplicative norm satisfying $\lVert\lambda a\rVert=|\lambda|_p\lVert a\rVert$.

## Gelfand-Mazur theorem

↑ **Parent:** [Banach algebra](banach-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gelfand–Mazur_theorem)

Every complex unital Banach algebra in which every nonzero element is invertible is isometrically isomorphic to $\mathbb C$.

## Algebra norm

↑ **Parent:** [Banach algebra](banach-algebra.md)

An algebra norm is a norm satisfying $\lVert ab\rVert\leq\lVert a\rVert\lVert b\rVert$. Its completion is a [Banach algebra](banach-algebra.md) in which the original algebra embeds densely.

### Renorming a bounded multiplicative semigroup

↑ **Parent:** [Algebra norm](#algebra-norm)

Let $S$ be a bounded multiplicatively closed subset of a unital [Banach algebra](banach-algebra.md). The displayed auxiliary [norm](functional-analysis.md#norm) $p$ is equivalent to the original norm, and each left multiplication $L_s$ is a contraction for $s\in S$. Taking the [operator norm](continuous-dual-space.md#operator-norm) of the faithful left regular representation produces an equivalent [algebra norm](#algebra-norm) with $\|1\|_S=1$ and $\|s\|_S\leq1$. If $M=\max(\|1\|,\sup_S\|s\|)$, then $\|a\|/M\leq\|a\|_S\leq M\|a\|$. The auxiliary norm is itself submultiplicative, since $p(ab)\leq p(a)\|b\|\leq p(a)p(b)$, but $p(1)=M$ can exceed one. The operator norm enforces the required unital normalization.

#### Simultaneous spectral-radius renorming

↑ **Parent:** [Renorming a bounded multiplicative semigroup](#renorming-a-bounded-multiplicative-semigroup)

For a finite commuting family in a unital [Banach algebra](banach-algebra.md), divide each $x_j$ by $r(x_j)+\varepsilon/2$. The [spectral radius formula](analysis.md#spectral-radius-formula) makes each normalized element's powers bounded. Commutativity lets every product be reordered into one power of each generator, so the entire generated [semigroup](algebra.md#semigroup) is bounded. [Renorming a bounded multiplicative semigroup](#renorming-a-bounded-multiplicative-semigroup) gives the displayed bounds simultaneously. Applying this to two commuting elements proves submultiplicativity and subadditivity of their [spectral radius](analysis.md#spectral-radius).

### Submultiplicativity

↑ **Parent:** [Algebra norm](#algebra-norm)

An [algebra norm](#algebra-norm) is submultiplicative when it satisfies the displayed product inequality. Induction gives $\|a_1\cdots a_n\|\le\prod_j\|a_j\|$, and in particular $\|a^n\|\le\|a\|^n$. The [operator norm](continuous-dual-space.md#operator-norm) has this property because $\|STv\|\le\|S\|\|T\|\|v\|$. The [supremum norm](functional-analysis.md#supremum-norm) for bounded functions with pointwise multiplication is another example. This estimate supports the [Neumann series](#neumann-series) and the [spectral radius formula](analysis.md#spectral-radius-formula).

### Continuous functions on the complex plane admit no algebra norm

↑ **Parent:** [Algebra norm](#algebra-norm)

Take disjoint disks escaping to infinity and continuous cutoff functions $h_n$ supported in them and equal to one on smaller disks. The locally finite function $f=\sum_n n h_n$ is continuous. Choose nonzero $g_n$ supported in the smaller disks; then $fg_n=ng_n$. Any [algebra norm](#algebra-norm) would give $n\|g_n\|=\|fg_n\|\le\|f\|\|g_n\|$, forcing $n\le\|f\|$ for every positive integer. This is impossible even without a completeness assumption.

### Entire function algebra admits no complete algebra norm

↑ **Parent:** [Algebra norm](#algebra-norm)

The displayed formula is a submultiplicative norm on the algebra of [entire functions](complex-analysis.md#entire-function): definiteness follows from the [identity theorem](complex-analysis.md#identity-theorem). No submultiplicative norm on the whole algebra can be complete. The coordinate function $Z(z)=z$ has every complex number in its algebraic [spectrum of an element](#spectrum-of-an-element), because $Z-\lambda$ vanishes somewhere and has no entire inverse. This contradicts compactness of spectra in a [Banach algebra](banach-algebra.md).

#### Compact-disk algebra norm on entire functions

↑ **Parent:** [Entire function algebra admits no complete algebra norm](#entire-function-algebra-admits-no-complete-algebra-norm)

The displayed [supremum norm](functional-analysis.md#supremum-norm) is finite on every [entire function](complex-analysis.md#entire-function), positive on every nonzero one by the [identity theorem](complex-analysis.md#identity-theorem), and submultiplicative under pointwise multiplication. It is not complete: partial geometric sums $\sum_{j=0}^n(z/2)^j$ are Cauchy on the disk but their limit there extends meromorphically with a pole at two. More generally, no complete [algebra norm](#algebra-norm) exists on all [entire functions](complex-analysis.md#entire-function) because the coordinate function has algebraic [spectrum of an element](#spectrum-of-an-element) equal to the whole complex plane.

<h3 id="minimality-of-the-supremum-norm-on-c-k">Minimality of the supremum norm on C(K)</h3>

↑ **Parent:** [Algebra norm](#algebra-norm)

Any submultiplicative [algebra norm](#algebra-norm) on all of $C(K)$ dominates its [supremum norm](functional-analysis.md#supremum-norm), even when the new norm is incomplete. Every [evaluation character](#evaluation-character) extends continuously to the completion: the restrictions of the completion's [character space](#character-space-of-an-algebra) form a closed subset of $K$, and an omitted point would give a nonzero function annihilated by an invertible function in the completion.

## Unitization of an algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

The unitization adjoins an identity to a possibly nonunital algebra. For $C_0(X)$ it is naturally $C(X^+)$ on the one-point compactification.

The resulting algebra is a [unital algebra](associative-algebra.md#unital-algebra).

## Neumann series

↑ **Parent:** [Banach algebra](banach-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neumann_series)

If $a$ belongs to a unital [Banach algebra](banach-algebra.md) and $\lVert a\rVert<1$, then

$$
(1-a)^{-1}=\sum_{n=0}^\infty a^n.
$$

Absolute convergence and multiplication of partial sums prove the identity.

## Spectrum of an element

↑ **Parent:** [Banach algebra](banach-algebra.md)

The spectrum of $a$ in a unital complex algebra $A$ is

$$
\sigma_A(a)=\{\lambda\in\mathbb C:a-\lambda1\text{ is not invertible}\}.
$$

For a nonunital algebra it is defined in the [unitization of an algebra](#unitization-of-an-algebra).

### Resolvent set of a Banach algebra element

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

The [algebra resolvent set](#resolvent-set-of-a-banach-algebra-element) consists of those scalars for which $\lambda1-x$ is invertible in the algebra. It is [open](topology.md#open-set) by the [Neumann series](#neumann-series), and the inverse-valued map is the [resolvent of an element](#resolvent-of-an-element). A [closed](topology.md#closed-set) [subalgebra](algebra.md#subalgebra) can have a smaller [algebra resolvent set](#resolvent-set-of-a-banach-algebra-element) because an ambient inverse need not lie in it.

### Resolvent components in a closed unital subalgebra

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

For a [closed](topology.md#closed-set) [unital](associative-algebra.md#unital-algebra) [subalgebra](algebra.md#subalgebra) $B$ of a [unital](associative-algebra.md#unital-algebra) [Banach algebra](banach-algebra.md) $A$ and $x\in B$, the smaller-algebra [algebra resolvent set](#resolvent-set-of-a-banach-algebra-element) is relatively [open](topology.md#open-set) and [closed](topology.md#closed-set) in the larger one. Openness follows from the [Neumann series](#neumann-series); closedness follows from [continuity](calculus.md#continuous-function) of inversion in $A$ and [norm](functional-analysis.md#norm) closedness of $B$. Every larger-algebra resolvent component is therefore either retained whole or absorbed into the smaller-algebra [Banach algebra spectrum](#spectrum-of-an-element). The unbounded component is always retained, since inverses at large modulus are norm-convergent series in $x$.

#### Boundary inclusion of spectra in a closed unital subalgebra

↑ **Parent:** [Resolvent components in a closed unital subalgebra](#resolvent-components-in-a-closed-unital-subalgebra)

For a [closed subalgebra of a Banach algebra](#closed-subalgebra-of-a-banach-algebra) $B\subseteq A$ with common identity, the [algebra resolvent set](#resolvent-set-of-a-banach-algebra-element) $\rho_B(x)$ is [clopen](topology.md#clopen-set) in $\rho_A(x)$. A point in $\rho_A(x)$ has a small connected disc on which membership of $\rho_B(x)$ is constant, so it cannot lie in $\partial\sigma_B(x)$. Also $\sigma_A(x)\subseteq\sigma_B(x)$; a point in the interior of the former is in the interior of the latter. Together these observations prove the [boundary](topology.md#boundary-of-a-set) inclusion, without assuming a spectral-boundary theorem.

### Translation of the spectrum by a scalar

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

The identity $(x+\alpha e)-\lambda e=x-(\lambda-\alpha)e$ proves the formula directly from invertibility. In a nonzero complex unital [Banach algebra](banach-algebra.md), the [nonemptiness of the Banach-algebra spectrum](#nonemptiness-of-the-banach-algebra-spectrum) implies that if $x$ is a [quasinilpotent element](#quasinilpotent-element), then $\rho(x+e)=1$. Consequently every nonscalar element cannot simultaneously be quasinilpotent: adding the identity preserves nonscalarity while translating its spectrum.

### Quasinilpotent element

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

An element of a complex unital [Banach algebra](banach-algebra.md) is quasinilpotent if its [spectral radius](analysis.md#spectral-radius) is zero, equivalently its [spectrum of an element](#spectrum-of-an-element) is $\{0\}$. A [nilpotent element](commutative-algebra.md#nilpotent) is quasinilpotent, but the converse need not hold. The [Volterra convolution algebra on a finite interval](#volterra-convolution-algebra-on-a-finite-interval) gives powers which never vanish, yet have factorially decreasing norms, making the inverse series for $\lambda e-x$ converge for every $\lambda\ne0$.

### Nonzero spectra of products in opposite orders

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

In a unital [Banach algebra](banach-algebra.md), for $\lambda\ne0$ the existence of $R=(\lambda1-ab)^{-1}$ gives $(\lambda1-ba)^{-1}=\lambda^{-1}(1+bRa)$, as verified by multiplying on either side. Interchanging $a,b$ proves the converse. Zero may differ: for the [unilateral shift operator](linear-operator-theory.md#unilateral-shift-operator) $S$ on $\ell^2(\mathbb N_0)$, $S^*S=1$ has spectrum $\{1\}$ and $SS^*=1-P_0$ has spectrum $\{0,1\}$.

### Nonemptiness of the Banach-algebra spectrum

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

Every element of a nonzero complex unital [Banach algebra](banach-algebra.md) has a nonempty compact [spectrum of an element](#spectrum-of-an-element). If the [resolvent of an element](#resolvent-of-an-element) existed everywhere, composing it with any [bounded linear functional](topological-vector-space.md#continuous-linear-functional) would give a bounded [entire function](complex-analysis.md#entire-function) tending to zero at infinity. The [Liouville theorem](complex-analysis.md#liouville-theorem) and point separation by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) would force the resolvent to be zero, contradicting the inverse equation. Nonunital algebras are treated by [unitization](#unitization-of-an-algebra).

### Approximate point spectrum

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

The approximate point spectrum consists of the scalars $\lambda$ for which there are unit vectors $x_k$ satisfying $\lVert(T-\lambda I)x_k\rVert\to0$. Equivalently, $T-\lambda I$ is not bounded below.

This is a part of the [spectrum of a bounded operator](linear-operator-theory.md#spectrum-of-a-bounded-operator).

#### Bilateral shift operator

↑ **Parent:** [Approximate point spectrum](#approximate-point-spectrum)

The bilateral shift $(Tx)_n=x_{n+1}$ is unitary. It has empty [point spectrum](linear-operator-theory.md#point-spectrum), while its [approximate point spectrum](#approximate-point-spectrum) is the unit circle. For $|\lambda|=1$, normalized vectors with entries $\lambda^n$ on an interval of length $N$ fail to satisfy $Tx=\lambda x$ only at the two endpoints, giving residual norm $\sqrt{2/N}$.

It is the two-sided sequence case of a [shift operator](linear-operator-theory.md#shift-operator).

### Resolvent of an element

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

The resolvent is $R(\lambda,a)=(\lambda1-a)^{-1}$ on the complement of the [spectrum of an element](#spectrum-of-an-element). In a Banach algebra it is analytic there.

#### Resolvent Cauchy coefficient formula

↑ **Parent:** [Resolvent of an element](#resolvent-of-an-element)

For a complex unital [Banach algebra](banach-algebra.md) and a circle enclosing its element's [Banach algebra spectrum](#spectrum-of-an-element), the displayed identity holds for $n\geq0$. On a sufficiently large circle, expand the [Neumann series](#neumann-series) and integrate it term by term. At any resolvent point the local series $R(\lambda_0+h)=\sum_{j\geq0}(-h)^jR(\lambda_0)^{j+1}$ proves norm analyticity. Apply continuous complex linear functionals and the scalar Cauchy theorem to deform the large circle to any radius greater than the maximum spectral modulus; the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) separates points and restores the vector integral identity. Its norm bound $\|x^n\|\leq R^{n+1}\max_{|\lambda|=R}\|R(\lambda)\|$ gives the reverse inequality in the [spectral radius formula](analysis.md#spectral-radius-formula).

#### Resolvent identity

↑ **Parent:** [Resolvent of an element](#resolvent-of-an-element)

For two points $z,w$ in the resolvent set of an operator $A$,

$$
R(z,A)-R(w,A)=(w-z)R(z,A)R(w,A).
$$

In particular, the [resolvent operator](functional-analysis.md#resolvent-of-an-operator) is differentiable and $\partial_zR(z,A)=-R(z,A)^2$.

#### Resolvent norm

↑ **Parent:** [Resolvent of an element](#resolvent-of-an-element)

For a closed operator, the resolvent is operator-valued holomorphic on its resolvent set. On a Hilbert space its norm is subharmonic and therefore cannot have a strict interior maximum.

#### Pseudospectrum

↑ **Parent:** [Resolvent of an element](#resolvent-of-an-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudospectrum)

The $\epsilon$-pseudospectrum consists of spectral points together with resolvent points where $\lVert(A-zI)^{-1}\rVert>\epsilon^{-1}$. Equivalently it is described by a small lower norm.

#### Riesz projection

↑ **Parent:** [Resolvent of an element](#resolvent-of-an-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz_projection)

For a spectral subset isolated by a contour $\Gamma$ in the resolvent set,

$$
P_\Gamma=\frac1{2\pi i}\int_\Gamma(zI-A)^{-1}\,dz
$$

projects onto its spectral subspace. Norm-small perturbations preserve the rank of this projection.

##### Disconnected spectrum yields a nontrivial invariant subspace

↑ **Parent:** [Riesz projection](#riesz-projection)

For a bounded operator on a complex [Banach space](banach-space.md), partition a disconnected spectrum into two nonempty compact pieces. The [holomorphic function](complex-analysis.md#holomorphic-function) equal to one near the first piece and zero near the second defines a [Riesz projection](#riesz-projection). The [holomorphic spectral mapping theorem](mathematics.md#holomorphic-spectral-mapping-theorem) makes it neither zero nor identity. Its closed range is a proper nonzero invariant [vector subspace](vector-space.md#vector-subspace). This need not be an orthogonal projection, and the argument does not require a normal operator.

### Spectrum in a closed unital subalgebra

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

If a closed unital subalgebra $A\subseteq B$ contains $x$, then $\sigma_A(x)$ is obtained from $\sigma_B(x)$ by adjoining some bounded connected components of its complement. Membership of $(x-\lambda1)^{-1}$ in $A$ is constant on every connected component of the resolvent set, and it always holds on the unbounded component.

#### Connected-component permanence of subalgebra invertibility

↑ **Parent:** [Spectrum in a closed unital subalgebra](#spectrum-in-a-closed-unital-subalgebra)

For a closed unital subalgebra $A\subseteq B$ with common identity, its [group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra) is relatively open in $A\cap G(B)$ by the [Neumann series](#neumann-series). It is relatively closed because inversion in $B$ is continuous and $A$ is closed. Consequently each [connected component](geometry-and-topology.md#connected-component) of $A\cap G(B)$ either consists entirely of elements invertible in $A$, or entirely of elements whose inverses do not belong to $A$.

### Holomorphic functional calculus

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holomorphic_functional_calculus)

For $x$ in a unital Banach algebra and $f$ holomorphic near $\sigma(x)$, the holomorphic functional calculus defines

$$
f(x)=\frac1{2\pi i}\int_\Gamma f(z)(z1-x)^{-1}\,dz,
$$

where $\Gamma$ winds once around the spectrum. It is a continuous unital algebra homomorphism and satisfies the [spectral mapping theorem](mathematics.md#spectral-mapping-theorem) $\sigma(f(x))=f(\sigma(x))$.

#### Logarithm from a spectral slit in a Banach algebra

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

If a [compact](topology.md#compact-space) [spectrum of an element](#spectrum-of-an-element) avoids zero and zero belongs to its unbounded complementary component, choose a simple arc from zero to infinity avoiding the [Banach algebra spectrum](#spectrum-of-an-element). Its complement is a [simply connected](algebraic-topology.md#simply-connected-space) neighborhood of the [Banach algebra spectrum](#spectrum-of-an-element), admitting a [holomorphic logarithm](complex-analysis.md#holomorphic-logarithm). Apply [holomorphic functional calculus](#holomorphic-functional-calculus) to that logarithm and the [composition rule for holomorphic functional calculus](#composition-rule-for-holomorphic-functional-calculus) to the exponential to obtain the displayed identity. An invertible [matrix](vector-space.md#matrix) over the [complex numbers](complex-analysis.md#complex-number) always satisfies the hypothesis because its finite [Banach algebra spectrum](#spectrum-of-an-element) cannot separate zero from infinity.

#### Spectral idempotent from a separated spectrum

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

If a [spectrum of an element](#spectrum-of-an-element) splits into disjoint nonempty compact pieces $X,Y$, choose disjoint open neighborhoods and a [holomorphic function](complex-analysis.md#holomorphic-function) equal to one on the first and zero on the second. The [holomorphic functional calculus](#holomorphic-functional-calculus) sends it to an [idempotent](commutative-algebra.md#idempotent) with the corresponding zero/one values under every [algebra character](#character-of-an-algebra). It is neither zero nor identity: if one piece were killed, a reciprocal function on the other piece would make an originally spectral coordinate difference invertible.

#### Banach algebra exponential

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

The exponential series converges absolutely in a unital [Banach algebra](banach-algebra.md). Multiplication of absolutely convergent series gives $e^xe^{-x}=1$, and gives $e^{x+y}=e^xe^y$ when $x,y$ commute. Termwise differentiation gives $e^{tx}=1+tx+O(t^2)$ near zero. In a [C-star algebra](#c-star-algebra), if $h=h^*$ and $t$ is real, taking adjoints termwise gives $(e^{ith})^*=e^{-ith}$, so this exponential is a [Unitary element of a C-star algebra](#unitary-element-of-a-c-star-algebra) and has norm one. These facts let a norm bound on a functional recover its real values on Hermitian elements.

#### Principal cube root of a Banach-algebra element

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

If the [spectrum of an element](#spectrum-of-an-element) $x$ avoids $(-\infty,0]$, its [holomorphic functional calculus](#holomorphic-functional-calculus) value for the [principal cube root](analysis.md#principal-cube-root) is the unique $y$ with $y^3=x$ and spectrum in $\{z\ne0:|\arg z|<\pi/3\}$. For uniqueness, any other such $v$ defines a [continuous](calculus.md#continuous-function) unital [algebra homomorphism](algebra.md#algebra-homomorphism-over-a-field) $f\mapsto\Theta_v(f\circ(z\mapsto z^3))$ from the slit-plane [holomorphic functions](complex-analysis.md#holomorphic-function) to the algebra. It sends the coordinate to $x$, so [continuity and uniqueness of holomorphic functional calculus](#continuity-and-uniqueness-of-holomorphic-functional-calculus) identify it with $\Theta_x$. Applying it to the principal cube root gives $v=y$. This argument does not assume commutativity of the ambient algebra or separation by [algebra characters](#character-of-an-algebra).

#### Principal square root in a commutative Banach algebra

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

If the [spectrum of an element](#spectrum-of-an-element) $x$ lies in the open right half-plane, [holomorphic functional calculus](#holomorphic-functional-calculus) gives the displayed square root with spectrum in that half-plane. It is unique there. Two such roots $y,v$ have character values equal to the unique scalar square root with positive real part. Every [character of an algebra](#character-of-an-algebra) is therefore nonzero on $y+v$, so the character description of the spectrum makes $y+v$ invertible. From $(y-v)(y+v)=0$ one obtains $y=v$. Equal character values alone do not prove equality in a possibly nonsemisimple algebra.

#### Resolvent-generated commutative algebra

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

The closed unital algebra generated by a bounded operator and all its resolvents is commutative, because the generators commute. It has exactly the original operator spectrum at that operator: all required inverses outside that spectrum were included, and an inverse in the smaller algebra is also an operator inverse. This permits commutative-algebra [linear functional](linear-algebra.md#linear-functional) calculus without replacing the spectrum by the possibly larger spectrum of a polynomial-generated algebra.

#### Continuity and uniqueness of holomorphic functional calculus

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

Equip [holomorphic functions](complex-analysis.md#holomorphic-function) on an open spectral neighborhood with the compact-open topology. A fixed admissible contour gives a bound on $\|\Theta_x(f)\|$ by a constant times the supremum of $|f|$ on the contour, proving [continuity](calculus.md#continuous-function). The [Runge theorem](complex-analysis.md#runge-s-theorem) makes rational functions with poles outside the open set dense. A unital homomorphism sending the coordinate function to $x$ must send each inverse coordinate difference to the corresponding resolvent, so its rational values and then all its holomorphic values are forced.

#### Logarithm of an element near the identity

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

The displayed series converges absolutely in a [Banach algebra](banach-algebra.md). It is the [holomorphic functional calculus](#holomorphic-functional-calculus) value of the analytic branch $z\mapsto\log(1-z)$ on the unit disk. The [composition rule for holomorphic functional calculus](#composition-rule-for-holomorphic-functional-calculus) and $\exp(\log(1-z))=1-z$ give $\exp(\log(1-x))=1-x$. Thus every sufficiently small norm perturbation of the identity is an exponential.

#### Composition rule for holomorphic functional calculus

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

Choose a cycle $\Gamma$ surrounding $\sigma(x)$ and a cycle $\Delta$ surrounding $f(\sigma(x))$, with $f(\Gamma)$ inside the region of winding number one for $\Delta$. The algebra-homomorphism property gives

$$
(\zeta1-f(x))^{-1}=\frac1{2\pi i}\int_\Gamma\frac{(z1-x)^{-1}}{\zeta-f(z)}\,dz.
$$

Substitute this into the contour formula for $g(f(x))$, interchange integrals, and apply the [Cauchy integral formula](analysis.md#cauchy-integral-formula) to the inner $\zeta$ integral. This proves composition as an equality of algebra elements, not merely an equality on characters, which need not separate a nonsemisimple algebra.

#### Injectivity through a holomorphic functional calculus with nonvanishing derivative

↑ **Parent:** [Holomorphic functional calculus](#holomorphic-functional-calculus)

Let $x_1,x_2$ belong to a commutative unital [Banach algebra](banach-algebra.md), have the same [Gelfand transform](#gelfand-representation), and have common spectrum $K$. If $f$ is holomorphic near $K$ and $f'$ has no zero on $K$, then $f(x_1)=f(x_2)$ implies $x_1=x_2$. Apply the two-variable holomorphic functional calculus to the divided difference of $f$; its Gelfand transform never vanishes, so it is invertible.

### Full spectrum

↑ **Parent:** [Spectrum of an element](#spectrum-of-an-element)

The full spectrum of an element is its spectrum together with every bounded component of its complement. Its complement is the unbounded resolvent component, and the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle) controls a holomorphic function on each filled hole by its values on the spectral boundary.

## Character of an algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)

A character on a complex algebra is a nonzero multiplicative linear functional $\varphi:A\to\mathbb C$.

Algebra characters form the domain of the [Gelfand representation](#gelfand-representation); they are distinct from traces of group representations.

### Maximal ideals of a commutative complex unital Banach algebra are character kernels

↑ **Parent:** [Character of an algebra](#character-of-an-algebra)

In a commutative complex unital [Banach algebra](banach-algebra.md), a [maximal ideal](commutative-algebra.md#maximal-ideal) is closed: its closure remains proper, since an element within distance less than one of the identity is invertible by the [Neumann series](#neumann-series). The quotient is a complex division [Banach algebra](banach-algebra.md), hence is the complex [field](algebra.md#field) by the [Gelfand-Mazur theorem](#gelfand-mazur-theorem). Its quotient map is a [character of an algebra](#character-of-an-algebra). Conversely a nonzero multiplicative complex [linear functional](linear-algebra.md#linear-functional) has value one at the identity, is onto the complex [field](algebra.md#field), and has maximal kernel. It is automatically continuous because its value at each element belongs to that element's spectrum. The kernel determines the [algebra character](#character-of-an-algebra) uniquely since the quotient is one-dimensional.

### Maximal ideals of a complex unital Banach algebra are character kernels

↑ **Parent:** [Character of an algebra](#character-of-an-algebra)

In a commutative complex unital [Banach algebra](banach-algebra.md), a [maximal ideal](commutative-algebra.md#maximal-ideal) is closed: its closure remains proper, since an element within distance less than one of the identity is invertible by the [Neumann series](#neumann-series). The quotient is a complex division [Banach algebra](banach-algebra.md), hence is the complex field by the [Gelfand-Mazur theorem](#gelfand-mazur-theorem). Its quotient map is a [character of an algebra](#character-of-an-algebra). Conversely a nonzero multiplicative complex [linear functional](linear-algebra.md#linear-functional) has value one at the identity, is onto the complex field, and has maximal kernel. It is automatically continuous because its value at each element belongs to that element's spectrum. The kernel determines the character uniquely since the quotient is one-dimensional.

### Characters of a C-star algebra respect the involution

↑ **Parent:** [Character of an algebra](#character-of-an-algebra)

For a self-adjoint element $h$, the exponentials $\exp(ith)$ are unitary. A continuous [algebra character](#character-of-an-algebra) therefore satisfies $|\exp(it\phi(h))|\leq1$ for every real $t$, forcing $\phi(h)$ to be real. Decomposing an arbitrary element into real and imaginary self-adjoint parts proves the displayed identity. Thus every [algebra character](#character-of-an-algebra) is a star-preserving scalar homomorphism; commutativity of the whole algebra is not needed for this fact.

### Automatic continuity of characters

↑ **Parent:** [Character of an algebra](#character-of-an-algebra)

For a [character of an algebra](#character-of-an-algebra) $\varphi$ on a complex unital [Banach algebra](banach-algebra.md), $\varphi(1)=1$ and $\varphi(a)\in\sigma(a)$, so $|\varphi(a)|\leq\lVert a\rVert$ without any prior continuity assumption. Under the usual normalization $\lVert1\rVert=1$, this gives $\lVert\varphi\rVert=1$; for an unnormalized [algebra norm](#algebra-norm), only the upper bound is automatic.

### Character space of an algebra

↑ **Parent:** [Character of an algebra](#character-of-an-algebra)

The character space $\Phi_A$ is the set of all [characters](#character-of-an-algebra) on $A$.

#### Maximal ideal space of a commutative Banach algebra

↑ **Parent:** [Character space of an algebra](#character-space-of-an-algebra)

For a commutative complex unital [Banach algebra](banach-algebra.md), [maximal ideals](commutative-algebra.md#maximal-ideal) correspond bijectively to [characters of an algebra](#character-of-an-algebra) by taking kernels. Give the maximal ideal space the [Gelfand topology](#gelfand-topology) through this correspondence. It is a [compact Hausdorff space](topology.md#compact-hausdorff-space), since the characters form a weak-star closed subset of the dual unit ball, which is compact by the [Banach-Alaoglu theorem](functional-analysis.md#banach-alaoglu-theorem).

<h4 id="character-space-of-r-k">Character space of R(K)</h4>

↑ **Parent:** [Character space of an algebra](#character-space-of-an-algebra)

For a compact set $K\subset\mathbb C$, let $\mathcal R(K)$ be the uniform closure on $K$ of the rational functions with no poles on $K$. Every character of $\mathcal R(K)$ is evaluation at a unique point of $K$, so $\Phi_{\mathcal R(K)}$ is naturally homeomorphic to $K$.

#### Absence of characters on an operator algebra with isomorphic complementary summands

↑ **Parent:** [Character space of an algebra](#character-space-of-an-algebra)

If $X=Y\oplus Z$ and the Banach spaces $Y$ and $Z$ are isomorphic, then the operator algebra $\mathcal B(X)$ has no [characters](#character-of-an-algebra). The two complementary projections have unequal character values, while mutually inverse off-diagonal maps force those values to be equal.

#### Gelfand topology

↑ **Parent:** [Character space of an algebra](#character-space-of-an-algebra)

The Gelfand topology on $\Phi_A$ is the weak-star topology inherited from $A^*$, equivalently the coarsest topology making every map $\varphi\mapsto\varphi(a)$ continuous.

This is the topology on the character space used in the [Gelfand representation](#gelfand-representation).

#### Evaluation character

↑ **Parent:** [Character space of an algebra](#character-space-of-an-algebra)

For an algebra of functions on a space, evaluation at $x$ is the character $\delta_x(f)=f(x)$.

#### Gelfand representation

↑ **Parent:** [Character space of an algebra](#character-space-of-an-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gelfand_representation)

For a unital commutative complex [Banach algebra](banach-algebra.md) $A$, the [Gelfand transform](#gelfand-representation) sends $a\in A$ to the continuous function $\widehat a(\varphi)=\varphi(a)$ on its [character space of an algebra](#character-space-of-an-algebra). It is a contractive unital algebra homomorphism into $C(\Phi_A)$.

##### Involution alone does not imply an isometric Gelfand transform

↑ **Parent:** [Gelfand representation](#gelfand-representation)

The complex [dual numbers](commutative-algebra.md#dual-number) $\mathbb C[\varepsilon]/(\varepsilon^2)$, with norm $\|a+b\varepsilon\|=|a|+|b|$ and involution $a+b\varepsilon\mapsto\bar a+\bar b\varepsilon$, is a commutative unital [Banach algebra](banach-algebra.md) with an isometric involution. Its sole [character of an algebra](#character-of-an-algebra) kills $\varepsilon$, so the [Gelfand transform](#gelfand-representation) is neither injective nor isometric. The [C-star identity](#c-star-identity) excludes this example and gives the [Commutative Gelfand--Naimark theorem](#commutative-gelfand-naimark-theorem). Even preservation of the involution on characters can fail without that identity: on $\mathbb C^2$, the involution $(a,b)^*=(\bar b,\bar a)$ exchanges the two evaluation characters.

##### Spectrum equals character values in a commutative Banach algebra

↑ **Parent:** [Gelfand representation](#gelfand-representation)

For a commutative complex unital [Banach algebra](banach-algebra.md), a [character of an algebra](#character-of-an-algebra) annihilates $a-\phi(a)1$, so this element cannot be invertible. Conversely a noninvertible $a-\lambda1$ generates a proper [ideal](commutative-algebra.md#ideal), which lies in a [maximal ideal](commutative-algebra.md#maximal-ideal). The corresponding character then has value $\lambda$ at $a$. Thus the [Gelfand transform](#gelfand-representation) determines every element's spectrum even when the algebra is not semisimple.

##### Gelfand representation theorem

↑ **Parent:** [Gelfand representation](#gelfand-representation)

For a commutative complex unital [Banach algebra](banach-algebra.md), its [Gelfand transform](#gelfand-representation) is a continuous unital algebra homomorphism into the continuous functions on its compact [character space](#character-space-of-an-algebra). The values of the transform of $a$ are exactly $\sigma_A(a)$, so $\|\widehat a\|_\infty=r(a)$. Its kernel is the intersection of the kernels of the [algebra characters](#character-of-an-algebra). For a commutative [C-star algebra](#c-star-algebra), [spectral radius norm equality for normal elements](#spectral-radius-norm-equality-for-normal-elements) and the [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) upgrade this to an isometric [C-star homomorphism](#c-star-homomorphism) onto $C(\Delta(A))$.

## Banach subalgebra generated by one element

↑ **Parent:** [Banach algebra](banach-algebra.md)

The closed unital subalgebra generated by $x$ is the norm closure of the polynomials in $x$. Its character space is homeomorphic to $\sigma(x)$ through $\varphi\mapsto\varphi(x)$, and the complement of that spectrum is connected.

### Spectrum of a polynomial-generated Banach subalgebra

↑ **Parent:** [Banach subalgebra generated by one element](#banach-subalgebra-generated-by-one-element)

For $B=\overline{\mathbb C[1,x]}$ inside $A$, the displayed [set](set.md) is the [full spectrum](#full-spectrum) of $x$ in $A$. On a bounded complementary component, the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle) gives $|p(\lambda)|\le\max_{\sigma_A(x)}|p|\le\|p(x)\|$. Evaluation $p(x)\mapsto p(\lambda)$ therefore extends to a [character of an algebra](#character-of-an-algebra) on $B$, showing $\lambda\in\sigma_B(x)$. Conversely the unbounded resolvent component survives by [resolvent components in a closed unital subalgebra](#resolvent-components-in-a-closed-unital-subalgebra). In particular, if zero lies in that component, $x^{-1}$ belongs to the [norm](functional-analysis.md#norm) [closure](topology.md#closure-topology) of [polynomials](polynomial.md) in $x$.

## C-star algebra

↑ **Parent:** [Banach algebra](banach-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/C*-algebra)

A C-star algebra is a complex Banach algebra with an involution satisfying $\|a^*a\|=\|a\|^2$.

### Unitization of a C-star algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)

For a nonunital [C-star algebra](#c-star-algebra), adjoining an identity gives multiplication $(a,\lambda)(b,\mu)=(ab+\lambda b+\mu a,\lambda\mu)$ and involution $(a,\lambda)^*=(a^*,\overline\lambda)$. Its standard C-star norm extends that of $A$, with the new identity of norm one. It can be constructed by adjoining the identity operator to a faithful nondegenerate operator representation and taking the [operator norm](continuous-dual-space.md#operator-norm). The original algebra is a closed ideal. The usual [spectrum of an element](#spectrum-of-an-element) in a nonunital algebra is taken in this unitization, permitting unital spectral arguments without requiring the original algebra to contain an identity.

#### C-star unitization by left multiplication

↑ **Parent:** [Unitization of a C-star algebra](#unitization-of-a-c-star-algebra)

The left multiplication representation of a [C-star algebra](#c-star-algebra) is isometric: test $L_a$ on $a^*/\|a\|$ to get $\|L_a\|=\|a\|$. For a nonunital algebra, its closed image plus the identity operator is the algebraic [unitization](#unitization-of-an-algebra). For a formal $z=a+\lambda1$ and $b\in A$, $\|zb\|^2=\|b^*z^*zb\|\leq\|b\|\|L_{z^*z}b\|$. Thus $\|L_z\|^2\leq\|L_{z^*z}\|\leq\|L_{z^*}\|\|L_z\|$; applying the same estimate to $z^*$ proves the [algebra involution](associative-algebra.md#algebra-involution) is isometric and the [C-star identity](#c-star-identity) holds. This gives a unitization without first assuming an operator representation on a [Hilbert space](hilbert-space.md).

### Calkin algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Calkin_algebra)

For an infinite-dimensional complex [Hilbert space](hilbert-space.md), the Calkin algebra is the unital quotient of the [bounded operators](topological-vector-space.md#continuous-linear-operator) by the closed two-sided ideal of [compact operators](compact-operator.md). Its spectrum records invertibility up to compact errors. An operator is [Fredholm](functional-analysis.md#fredholm-operator) exactly when its image in this quotient is invertible.

### C-star subalgebra

↑ **Parent:** [C-star algebra](#c-star-algebra)

A C-star subalgebra is a norm-closed subalgebra closed under the involution, with the inherited [C-star identity](#c-star-identity). A unital inclusion in this context uses the same identity as the ambient [C-star algebra](#c-star-algebra). The [spectral permanence for C-star algebras](#spectral-permanence-for-c-star-algebras) says the inclusion preserves the [spectrum of an element](#spectrum-of-an-element).

### C-star homomorphism

↑ **Parent:** [C-star algebra](#c-star-algebra)

A C-star homomorphism is a complex linear multiplicative map between [C-star algebras](#c-star-algebra) that preserves the involution. Such maps are contractive; an injective one is an [isometry](riemannian-geometry.md#isometry).

#### Injective C-star homomorphism is isometric

↑ **Parent:** [C-star homomorphism](#c-star-homomorphism)

An injective [C-star homomorphism](#c-star-homomorphism) preserves norms. For unital maps, reduce to the commutative algebra generated by $1$ and $a^*a$. Its induced map on [character spaces](#character-space-of-an-algebra) has dense, hence full, image; otherwise a nonzero continuous function vanishing on that image would lie in the kernel. The [C-star identity](#c-star-identity) then gives norm preservation for $a$.

### Spectral permanence for C-star algebras

↑ **Parent:** [C-star algebra](#c-star-algebra)

If $A$ is a closed [C-star algebra](#c-star-algebra) inside a unital [C-star algebra](#c-star-algebra) $B$ and the two algebras share their identity, an element of $A$ is invertible in $A$ exactly when it is invertible in $B$. Consequently its [spectrum of an element](#spectrum-of-an-element) does not depend on which of these two algebras is used.

### Continuous functional calculus

↑ **Parent:** [C-star algebra](#c-star-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous_functional_calculus)

For a [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra) $a$ in a unital [C-star algebra](#c-star-algebra), the [Commutative Gelfand--Naimark theorem](#commutative-gelfand-naimark-theorem) identifies $C(\sigma(a))$ isometrically with the closed unital algebra generated by $a$ and $a^*$. The coordinate function maps to $a$, defining $f(a)$ for every continuous $f$ on the [spectrum of an element](#spectrum-of-an-element).

#### Nonunital continuous functional calculus

↑ **Parent:** [Continuous functional calculus](#continuous-functional-calculus)

For a [normal C-star element](#normal-element-of-a-c-star-algebra) $x$ in a nonunital algebra, take its [spectrum of an element](#spectrum-of-an-element) in the [C-star unitization](#unitization-of-a-c-star-algebra). Zero belongs to that spectrum. Continuous functions on this compact spectrum that vanish at zero form an ideal canonically identified with the displayed function algebra. Their values under the unital [continuous functional calculus](#continuous-functional-calculus) belong to the original algebra because the scalar quotient evaluates them at zero. Star-polynomial approximation with the constant term removed gives exactly the image $C^*(x)$.

#### Square-root resolvent integral in a C-star algebra

↑ **Parent:** [Continuous functional calculus](#continuous-functional-calculus)

For a [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra) $x$, the displayed improper integral converges in norm. Near zero its integrand has norm at most $t^{-1/2}$; near infinity it has norm at most $\|x\|t^{-3/2}$. The scalar identity follows by setting $t=su^2$ for $s>0$ and using $\int_0^\infty2/(1+u^2)\,du=\pi$; for $s=0$ both sides vanish. The bounds are uniform on the compact [spectrum of an element](#spectrum-of-an-element), so [continuous functional calculus](#continuous-functional-calculus) gives the operator identity.

##### Order preservation by the positive square root

↑ **Parent:** [Square-root resolvent integral in a C-star algebra](#square-root-resolvent-integral-in-a-c-star-algebra)

For [Positive elements of a C-star algebra](#positive-element-of-a-c-star-algebra) $x\leq y$, [inversion reverses the order of strictly positive elements](#inversion-reverses-the-order-of-strictly-positive-elements), so $(t1+x)^{-1}\geq(t1+y)^{-1}$ for $t>0$. Subtracting their [square-root resolvent integral in a C-star algebra](#square-root-resolvent-integral-in-a-c-star-algebra) formulas gives

$$
y^{1/2}-x^{1/2}=\frac1\pi\int_0^\infty t^{1/2}\bigl((t1+x)^{-1}-(t1+y)^{-1}\bigr)\,dt\geq0.
$$

The integrand is positive, and the positive cone is closed, so the norm limit of these integrals is positive. No commutativity of $x$ and $y$ is required. In particular, $b^2\geq a^2$ for positive $a,b$ implies $b\geq a$, even though squaring itself is not generally order preserving.

#### Strong continuity of functional calculus through resolvents

↑ **Parent:** [Continuous functional calculus](#continuous-functional-calculus)

For bounded [self-adjoint](linear-operator-theory.md#self-adjoint-operator) $a_i,a$, no uniform bound on $\|a_i\|$ is needed. The [resolvent identity](#resolvent-identity) gives $(a_i-i)^{-1}-(a-i)^{-1}=(a_i-i)^{-1}(a-a_i)(a-i)^{-1}$, and the first factor has [norm](functional-analysis.md#norm) at most one. Thus both [resolvents](functional-analysis.md#resolvent-of-an-operator) at $i$ and $-i$ converge strongly. Products preserve strong convergence for uniformly bounded nets; uniform approximation by the algebra of these [resolvent](functional-analysis.md#resolvent-of-an-operator) functions then gives the displayed statement for every continuous function vanishing at infinity.

#### Disconnected spectrum gives a reducing subspace

↑ **Parent:** [Continuous functional calculus](#continuous-functional-calculus)

For a [normal operator](hilbert-space.md#normal-operator) with disconnected [spectrum](linear-operator-theory.md#spectrum-functional-analysis) $K=K_1\sqcup K_2$, the [indicator function](measure-theory.md#indicator-function) of a nonempty proper clopen component union is continuous on $K$. The [continuous functional calculus](#continuous-functional-calculus) makes it a nonzero proper self-adjoint [linear projection](vector-space.md#projection-linear-algebra) commuting with $T,T^*$. Its range is therefore a nontrivial closed reducing subspace. No [eigenvector](linear-operator-theory.md#eigenvector) is needed.

### C-star identity

↑ **Parent:** [C-star algebra](#c-star-algebra)

The C-star identity is the norm axiom $\lVert a^*a\rVert=\lVert a\rVert^2$. It implies that the involution is isometric and that a normal element has norm equal to its spectral radius.

<h3 id="commutative-gelfand-naimark-theorem">Commutative Gelfand--Naimark theorem</h3>

↑ **Parent:** [C-star algebra](#c-star-algebra)

Every commutative unital C-star algebra $A$ is isometrically star-isomorphic to $C(\Phi_A)$ through its [Gelfand transform](#gelfand-representation), where $\Phi_A$ is its [character space of an algebra](#character-space-of-an-algebra). Thus abstract algebra elements can be treated as continuous functions on a compact Hausdorff space.

This is the isometric commutative C-star specialization of the [Gelfand representation](#gelfand-representation).

### Positive element of a C-star algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)

An element $a$ of a C-star algebra is positive when $a=b^*b$ for some $b$, equivalently when $a=a^*$ and $\sigma(a)\subseteq[0,\infty)$. Continuous functional calculus gives it a unique positive square root $a^{1/2}$.

#### Positive cone of a C-star algebra

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

The positive elements of a [C-star algebra](#c-star-algebra) form a norm-closed proper convex cone. For $p,q\geq0$ and $s=\|p\|+\|q\|$, [continuous functional calculus](#continuous-functional-calculus) gives $\|s1-p-q\|\leq s$, forcing the real spectrum of $p+q$ to be nonnegative. The same bound with one fixed upper norm bound proves norm closedness under limits; scaling by nonnegative real scalars preserves positivity. If both $h$ and $-h$ are positive, their spectra lie in $\{0\}$, and [spectral radius norm equality for normal elements](#spectral-radius-norm-equality-for-normal-elements) forces $h=0$. This cone defines the order $a\leq b$ precisely when $b-a\in A_+$.

#### Squaring is not order preserving in a C-star algebra

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

In $M_2(\mathbb C)$ take $a=\operatorname{diag}(1,2)$ and $b=\begin{pmatrix}2&1\\1&3\end{pmatrix}$. Then $a-1\geq0$ and $b-a=\begin{pmatrix}1&1\\1&1\end{pmatrix}\geq0$, but $b^2-a^2=\begin{pmatrix}4&5\\5&6\end{pmatrix}$ has [determinant](linear-algebra.md#determinant) $-1$ and a negative [eigenvalue](linear-operator-theory.md#eigenvalue). In contrast, for commuting positive elements $b^2-a^2=(b-a)(b+a)$ is positive in the commutative function algebra supplied by [continuous functional calculus](#continuous-functional-calculus). The obstruction is noncommutativity, not a failure of the scalar inequality.

#### Inversion reverses the order of strictly positive elements

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

Here strictly positive means positive and invertible. Set $k=a^{-1/2}ba^{-1/2}\geq1$ using [congruence preserves positivity in a C-star algebra](#congruence-preserves-positivity-in-a-c-star-algebra). The [continuous functional calculus](#continuous-functional-calculus) gives $k^{-1}\leq1$, since $1-t^{-1}\geq0$ for $t\geq1$. Then $a^{-1}-b^{-1}=a^{-1/2}(1-k^{-1})a^{-1/2}\geq0$. The proof works without commutativity. If $1\leq a$, functional calculus also gives $a^{-1}\leq1$.

#### Congruence preserves positivity in a C-star algebra

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

For a positive element $a$, its [positive square root in a C-star algebra](#positive-square-root-in-a-c-star-algebra) gives $c^*ac=(a^{1/2}c)^*(a^{1/2}c)$, which is positive. Applying this to $b-a$ shows that $a\leq b$ implies $c^*ac\leq c^*bc$. The map need not preserve multiplication, but it preserves order; if $c$ is invertible, the inverse congruence also preserves order.

#### Positivity of adjoint products from spectral positivity

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

Define positivity spectrally: a self-adjoint element has nonnegative spectrum. First, addition preserves it. For $p,q\geq0$ and $s=\|p\|+\|q\|$, functional calculus gives $\|s1-p-q\|\leq s$, forcing every real spectral value of $p+q$ to be nonnegative. The cone is proper because a self-adjoint element with spectrum contained in $\{0\}$ has norm zero.

For $h=a^*a$, let $h_-=\max(-h,0)$ by the [continuous functional calculus](#continuous-functional-calculus), and set $c=ah_-^{1/2}$. Then $c^*c=-h_-^2$ is nonpositive. The [nonzero spectra of products in opposite orders](#nonzero-spectra-of-products-in-opposite-orders) imply that $cc^*$ is nonpositive too. Write $c=u+iv$ with $u,v$ self-adjoint. Then $c^*c+cc^*=2(u^2+v^2)$ is positive, since self-adjoint squares have nonnegative spectrum. It is also nonpositive, hence zero. It follows that $c^*c=-cc^*$ is both positive and nonpositive, hence zero. The [C-star identity](#c-star-identity) gives $c=0$, so $h_-^2=0$ and $h_-=0$. Thus $h\geq0$, without assuming positivity of adjoint products in an earlier step.

#### Positive square root in a C-star algebra

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

Every [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra) $a$ has a unique positive element $a^{1/2}$ satisfying $(a^{1/2})^2=a$. It is obtained by applying the continuous functional calculus to $t\mapsto\sqrt t$ on $\sigma(a)\subseteq[0,\infty)$.

#### Spectral characterization of a positive element in a C-star algebra

↑ **Parent:** [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra)

An element $a$ of a C-star algebra is positive if and only if it is Hermitian and $\sigma(a)\subseteq[0,\infty)$. This characterization transfers the pointwise order on continuous functions to an abstract C-star algebra through the continuous functional calculus.

### Hermitian element of a C-star algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)

An element $x$ of a [C-star algebra](#c-star-algebra) is Hermitian when $x=x^*$. Its [spectrum](#spectrum-of-an-element) is real, its norm equals its spectral radius, and it is the difference of two [positive elements](#positive-element-of-a-c-star-algebra).

### Unitary element of a C-star algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)

An element $u$ of a unital [C-star algebra](#c-star-algebra) is unitary when $u^*u=uu^*=1$.

### Normal element of a C-star algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)

An element $x$ of a [C-star algebra](#c-star-algebra) is normal when $x^*x=xx^*$.

#### Star polynomial in one normal element

↑ **Parent:** [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra)

Since a [normal C-star element](#normal-element-of-a-c-star-algebra) commutes with its adjoint, words in those two generators can be rearranged into the displayed finite sum. Including the constant term generates the unital star algebra; omitting it generates the nonunital star algebra. Under [continuous functional calculus](#continuous-functional-calculus), such a sum is the ordinary function $\sum_{j,k}c_{jk}z^j\overline z^k$ on the spectrum. The [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) makes these functions uniformly dense.

#### Unital versus nonunital generation by a normal element

↑ **Parent:** [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra)

The unital [continuous functional calculus](#continuous-functional-calculus) has image $C^*(1,x)$, the [norm](functional-analysis.md#norm) closure of star polynomials including constants. The smallest closed star subalgebra $C^*(x)$ need not contain the ambient identity: for $x=0$ it is zero. In a nonunital algebra, apply the unital calculus in the [C-star unitization](#unitization-of-a-c-star-algebra) and retain functions vanishing at zero to recover $C^*(x)$ inside the original algebra.

#### Real spectrum criterion for a normal C-star element

↑ **Parent:** [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra)

For normal $x$, the closed unital [C-star subalgebra](#c-star-subalgebra) generated by $x,x^*$ is commutative. When the ambient spectrum is real, its complement is connected. Membership of the resolvent in this subalgebra is both open and closed on that complement, and holds at large modulus by the [Neumann series](#neumann-series). Thus the subalgebra spectrum is the same real set. Its isometric [Gelfand transform](#gelfand-representation) takes $x$ to a real-valued function and $x^*$ to its conjugate, proving equality. Normality is necessary: the nonzero matrix $\begin{pmatrix}0&1\\0&0\end{pmatrix}$ has spectrum $\{0\}$ but is not self-adjoint.

#### Spectral radius norm equality for normal elements

↑ **Parent:** [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra)

For a [Normal element of a C-star algebra](#normal-element-of-a-c-star-algebra), the [C-star identity](#c-star-identity) gives $\|a^2\|=\|a\|^2$, and iteration gives $\|a^{2^n}\|=\|a\|^{2^n}$. The [spectral radius formula](analysis.md#spectral-radius-formula) then gives $r(a)=\|a\|$. This proves the isometry of the [Gelfand transform](#gelfand-representation) for a commutative [C-star algebra](#c-star-algebra) directly from its defining norm identity.

### Positive functional on a C-star algebra

↑ **Parent:** [C-star algebra](#c-star-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_functional_on_a_C-star_algebra)

A bounded linear functional $\tau$ on a [C-star algebra](#c-star-algebra) is positive when $\tau(x)\geq0$ for every [Positive element of a C-star algebra](#positive-element-of-a-c-star-algebra). Positivity implies

$$
|\tau(y^*x)|^2\leq\tau(x^*x)\tau(y^*y)
$$

and $\|\tau\|=\tau(1)$; conversely, $\|\tau\|=\tau(1)$ implies positivity.

<h4 id="cauchy-schwarz-inequality-for-positive-c-star-functionals">Cauchy–Schwarz inequality for positive C-star functionals</h4>

↑ **Parent:** [Positive functional on a C-star algebra](#positive-functional-on-a-c-star-algebra)

Positivity of $f((x+ty)^*(x+ty))$ for every complex $t$ proves the displayed [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), including zero diagonal cases. Replacing $x,y$ by their adjoints gives $|f(xy^*)|^2\leq f(xx^*)f(yy^*)$. These two forms cannot be mixed for a general [positive functional on a C-star algebra](#positive-functional-on-a-c-star-algebra). For the state evaluating the lower-right entry of $2\times2$ matrices and $x=y=E_{12}$, $f(x^*y)=1$ but $f(xx^*)=f(yy^*)=0$, disproving the mixed form.

#### Tracial positive functional

↑ **Parent:** [Positive functional on a C-star algebra](#positive-functional-on-a-c-star-algebra)

A positive [bounded linear functional](topological-vector-space.md#continuous-linear-functional) is tracial when its value on a product is unchanged by reversing the two factors. When normalized by $\tau(1)=1$, it is a tracial state. A [vector](vector-space.md#vector) functional $\tau(a)=\langle a\Omega,\Omega\rangle$ is faithful if the [vector](vector-space.md#vector) is separating, since $\tau(a^*a)=\|a\Omega\|^2$. Its [trace](linear-algebra.md#matrix-trace) identity makes the associated [Tomita operator](functional-analysis.md#tomita-operator) isometric.

#### State on a C-star algebra

↑ **Parent:** [Positive functional on a C-star algebra](#positive-functional-on-a-c-star-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/State_on_a_C-star_algebra)

A state is a positive functional of norm one. The state space $S(A)$ is a weak-star compact convex subset of $A^*$.

##### States separate elements of a C-star algebra

↑ **Parent:** [State on a C-star algebra](#state-on-a-c-star-algebra)

Write $x=h+ik$ with both terms Hermitian. At least one is nonzero; its norm equals its [spectral radius](analysis.md#spectral-radius), so it has a nonzero spectral value. [Spectral values attained by C-star states](#spectral-values-attained-by-c-star-states) gives a state taking that nonzero value on the chosen term. Both state values on $h,k$ are real, so the corresponding complex value on $x$ cannot vanish. This also detects nonzero quasinilpotent elements, which cannot be separated by looking only at their own spectrum.

##### Spectral values attained by C-star states

↑ **Parent:** [State on a C-star algebra](#state-on-a-c-star-algebra)

On the linear span of $1,x$, define $g(a1+bx)=a+b\lambda$. Affine spectral mapping gives $|a+b\lambda|\leq\|a1+bx\|$, making this well-defined with norm one and $g(1)=1$. A norm-preserving [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) extension to the whole [C-star algebra](#c-star-algebra) remains unital; the norm characterization of a [positive functional on a C-star algebra](#positive-functional-on-a-c-star-algebra) makes it a [state on a C-star algebra](#state-on-a-c-star-algebra) attaining the spectral value.

##### Pure state on a C-star algebra

↑ **Parent:** [State on a C-star algebra](#state-on-a-c-star-algebra)

A pure state is an extreme point of the [state space](#state-on-a-c-star-algebra). The [Krein-Milman theorem](functional-analysis.md#krein-milman-theorem) guarantees pure states, and every positive element attains its norm at some pure state.

### Borel functional calculus for a normal operator

↑ **Parent:** [C-star algebra](#c-star-algebra)

For a normal operator $T$ with spectrum $K$, there is a contractive unital star-homomorphism

$$
\Psi:L^\infty(K)\longrightarrow\mathcal B(H),
\qquad
\Psi(z)=T,
$$

where $L^\infty(K)$ denotes the bounded Borel functions. It is obtained by integrating against the projection-valued spectral measure of $T$.

#### Spectral essential range in Borel functional calculus

↑ **Parent:** [Borel functional calculus for a normal operator](#borel-functional-calculus-for-a-normal-operator)

For a bounded [Borel measurable function](measure-theory.md#borel-measurable-function) $f$ and the [projection-valued measure](hilbert-space.md#projection-valued-measure) $E$ of a [normal operator](hilbert-space.md#normal-operator), the displayed set is the [spectrum of an element](#spectrum-of-an-element) of $f(T)$. Outside it, a bounded reciprocal away from a spectral-null set supplies the inverse. Inside it, unit vectors supported by the indicated arbitrarily small spectral sets make $f(T)-\lambda$ fail to be bounded below. The kernel of the calculus consists of functions satisfying $E(|f|>\varepsilon)=0$ for every $\varepsilon>0$, and its [norm](functional-analysis.md#norm) is the corresponding essential supremum. Ordinary pointwise range is insufficient: for multiplication by $t$ on $L^2[0,1]$, $\mathbf1_{\{0\}}(T)=0$ even though the function takes the value $1$.

#### Normal square root from Borel functional calculus

↑ **Parent:** [Borel functional calculus for a normal operator](#borel-functional-calculus-for-a-normal-operator)

A bounded [normal operator](hilbert-space.md#normal-operator) admits a normal square root even when no [continuous](calculus.md#continuous-function) scalar square root exists on its [Banach algebra spectrum](#spectrum-of-an-element). Choose a bounded Borel branch $s(z)=|z|^{1/2}\exp(i\operatorname{Arg}(z)/2)$, with $s(0)=0$. The [Borel functional calculus for a normal operator](#borel-functional-calculus-for-a-normal-operator) gives $S=s(T)$; multiplicativity gives $S^2=T$ and preservation of the adjoint gives $S^*S=SS^*=|s|^2(T)$. Unlike a positive square root, this square root need not be unique.

#### Functional calculus convergence

↑ **Parent:** [Borel functional calculus for a normal operator](#borel-functional-calculus-for-a-normal-operator)

Normal operators $A_n$ on approximating subspaces converge to $A$ in the functional-calculus sense when $f(A_n)$ converges weakly to $f(A)$, after the natural projection and inclusion maps, for every continuous function $f$ on a common compact spectral set.

### Partial isometry

↑ **Parent:** [C-star algebra](#c-star-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_isometry)

An operator $U$ on a Hilbert space is a partial isometry when it is isometric on $(\ker U)^\perp$. Equivalently, $U^*U$ is the orthogonal projection onto this initial space.

### Polar decomposition of a bounded operator

↑ **Parent:** [C-star algebra](#c-star-algebra)

Every bounded operator on a Hilbert space has a polar decomposition $T=U|T|$, where $|T|=(T^*T)^{1/2}$ and $U$ is a partial isometry with $\ker U=\ker T$. On $\operatorname{im}|T|$, it is defined by $U(|T|x)=Tx$.

This is the bounded-operator case of [polar decomposition](linear-operator-theory.md#polar-decomposition).

#### Absolute value of an operator

↑ **Parent:** [Polar decomposition of a bounded operator](#polar-decomposition-of-a-bounded-operator)

The absolute value of a [linear operator](vector-space.md#linear-operator) $L$ is the [positive square root of an operator](hilbert-space.md#positive-square-root-of-an-operator) $L^\dagger L$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are the [singular values](linear-algebra.md#singular-value) of $L$, its [trace](linear-algebra.md#matrix-trace) is the [trace norm](functional-analysis.md#trace-norm) of $L$, and it appears in the [polar decomposition of a bounded operator](#polar-decomposition-of-a-bounded-operator) $L=U|L|$.

#### Unitary polar factor of a finite compression

↑ **Parent:** [Polar decomposition of a bounded operator](#polar-decomposition-of-a-bounded-operator)

If $T_n=P_nAP_n^*$ is a square finite compression with [singular value decomposition](linear-algebra.md#singular-value-decomposition) $T_n=V_n\Sigma_nW_n^*$, then $U_n=V_nW_n^*$ is a unitary extension of its polar factor. When $A$ is unitary and $P_n^*P_n\to I$ strongly, $|T_n|\to I$ strongly and hence $U_nP_n\to A$ strongly.

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (97)

- [Algebra norm](#algebra-norm)
- [Automatic continuity of characters](#automatic-continuity-of-characters)
- [Banach algebra exponential](#banach-algebra-exponential)
- [Closed subalgebra of a Banach algebra](#closed-subalgebra-of-a-banach-algebra)
- [Entire function algebra admits no complete algebra norm](#entire-function-algebra-admits-no-complete-algebra-norm)
- [Gelfand representation](#gelfand-representation)
- [Gelfand representation theorem](#gelfand-representation-theorem)
- [Group of invertible elements of a Banach algebra](#group-of-invertible-elements-of-a-banach-algebra)
- [Hermitian Banach algebra](#hermitian-banach-algebra)
- [Hermitian element of a star algebra](associative-algebra.md#hermitian-element-of-a-star-algebra)
- [Injectivity through a holomorphic functional calculus with nonvanishing derivative](#injectivity-through-a-holomorphic-functional-calculus-with-nonvanishing-derivative)
- [Inverse norm divergence at noninvertible boundary points](#inverse-norm-divergence-at-noninvertible-boundary-points)
- [Involution alone does not imply an isometric Gelfand transform](#involution-alone-does-not-imply-an-isometric-gelfand-transform)
- [Johnson's continuity theorem for irreducible normed representations](module-theory.md#johnson-s-continuity-theorem-for-irreducible-normed-representations)
- [L1 convolution algebra](#l1-convolution-algebra)
- [Left inverse of an algebra element](#left-inverse-of-an-algebra-element)
- [Logarithm of an element near the identity](#logarithm-of-an-element-near-the-identity)
- [Maximal ideal space of a commutative Banach algebra](#maximal-ideal-space-of-a-commutative-banach-algebra)
- [Maximal ideals of a commutative complex unital Banach algebra are character kernels](#maximal-ideals-of-a-commutative-complex-unital-banach-algebra-are-character-kernels)
- [Maximal ideals of a complex unital Banach algebra are character kernels](#maximal-ideals-of-a-complex-unital-banach-algebra-are-character-kernels)
- [Maximal left ideal](associative-algebra.md#maximal-left-ideal)
- [Neumann series](#neumann-series)
- [Nonemptiness of the Banach-algebra spectrum](#nonemptiness-of-the-banach-algebra-spectrum)
- [Noninvertible limits of invertibles have no one-sided inverse](#noninvertible-limits-of-invertibles-have-no-one-sided-inverse)
- [Nonzero spectra of products in opposite orders](#nonzero-spectra-of-products-in-opposite-orders)
- [Normed algebra](algebra.md#normed-algebra)
- [Normed division algebra](algebra.md#normed-division-algebra)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-7.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-11.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-10.md#5/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-7.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-7.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-7.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-8.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-8.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-106.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#2/f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#2/f/iii/solution)
- [Power-decay characterization of the spectral radius](analysis.md#power-decay-characterization-of-the-spectral-radius)
- [Primitive ideal](associative-algebra.md#primitive-ideal)
- [Quasinilpotent element](#quasinilpotent-element)
- [Renorming a bounded multiplicative semigroup](#renorming-a-bounded-multiplicative-semigroup)
- [Representation of a Banach algebra](module-theory.md#representation-of-a-banach-algebra)
- [Resolvent Cauchy coefficient formula](#resolvent-cauchy-coefficient-formula)
- [Resolvent components in a closed unital subalgebra](#resolvent-components-in-a-closed-unital-subalgebra)
- [Resolvent of an operator](functional-analysis.md#resolvent-of-an-operator)
- [Right inverse of an algebra element](#right-inverse-of-an-algebra-element)
- [Scalar right action on a maximal-left-ideal quotient](associative-algebra.md#scalar-right-action-on-a-maximal-left-ideal-quotient)
- [Semisimple Banach algebra](#semisimple-banach-algebra)
- [Semisimple commutative Banach algebra](#semisimple-commutative-banach-algebra)
- [Simultaneous spectral-radius renorming](#simultaneous-spectral-radius-renorming)
- [Spectral radius formula](analysis.md#spectral-radius-formula)
- [Spectral-radius Liouville theorem](analysis.md#spectral-radius-liouville-theorem)
- [Spectral-radius maximum principle](complex-analysis.md#spectral-radius-maximum-principle)
- [Spectral-radius three-circle inequality](analysis.md#spectral-radius-three-circle-inequality)
- [Spectrum equals character values in a commutative Banach algebra](#spectrum-equals-character-values-in-a-commutative-banach-algebra)
- [Translation of the spectrum by a scalar](#translation-of-the-spectrum-by-a-scalar)
- [Volterra convolution algebra on a finite interval](#volterra-convolution-algebra-on-a-finite-interval)
