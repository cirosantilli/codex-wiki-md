# Topological vector space

↑ **Parent:** [Functional analysis](functional-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_vector_space)

A topological vector space is a [vector space](vector-space.md) with a topology for which vector addition and scalar multiplication are continuous.

**Table of contents**

- [Dense subspace](#dense-subspace)
- [Sequential continuity criterion in a metrizable vector space](#sequential-continuity-criterion-in-a-metrizable-vector-space)
- [Bounded set in a topological vector space](#bounded-set-in-a-topological-vector-space)
- [Strict inductive limit topology](#strict-inductive-limit-topology)
- [Metrizable topological vector space](#metrizable-topological-vector-space)
- [Finite-dimensional vector-space topology](#finite-dimensional-vector-space-topology)
  - [Equivalence of norms in finite dimensions](#equivalence-of-norms-in-finite-dimensions)
    - [Sharp comparison of l1 and l2 norms](#sharp-comparison-of-l1-and-l2-norms)
- [Locally convex space](#locally-convex-space)
  - [Compact metrizable convex set](#compact-metrizable-convex-set)
    - [Choquet theorem](#choquet-theorem)
      - [Threshold Choquet representation in L-infinity](#threshold-choquet-representation-in-l-infinity)
      - [Choquet's theorem by strict convexity](#choquet-s-theorem-by-strict-convexity)
    - [Affine upper envelope](#affine-upper-envelope)
      - [Supporting measure lemma for affine upper envelopes](#supporting-measure-lemma-for-affine-upper-envelopes)
    - [Barycenter](#barycenter)
  - [Seminorm](#seminorm)
    - [Dual seminorm](#dual-seminorm)
  - [Fréchet space](#frechet-space)
  - [Minkowski functional](#minkowski-functional)
    - [Norm from a bounded symmetric convex neighbourhood](#norm-from-a-bounded-symmetric-convex-neighbourhood)
  - [Separation of a point and an open convex set](#separation-of-a-point-and-an-open-convex-set)
    - [Hahn-Banach separation theorem for two convex sets](#hahn-banach-separation-theorem-for-two-convex-sets)
    - [Finite-dimensional separation of open convex sets](#finite-dimensional-separation-of-open-convex-sets)
  - [Dual pair](#dual-pair)
    - [Continuous dual of a weak topology](#continuous-dual-of-a-weak-topology)
    - [Compact norming dual-pair criterion](#compact-norming-dual-pair-criterion)
    - [Bipolar theorem for a dual pair](#bipolar-theorem-for-a-dual-pair)
  - [Product of locally convex spaces](#product-of-locally-convex-spaces)
- [Continuous linear operator](#continuous-linear-operator)
  - [Completely continuous operator](#completely-continuous-operator)
  - [Approximate surjectivity with geometric correction](#approximate-surjectivity-with-geometric-correction)
  - [Absolutely p-summing operator](#absolutely-p-summing-operator)
    - [2-summing operator](#2-summing-operator)
      - [2-summing norm of a finite-dimensional identity](#2-summing-norm-of-a-finite-dimensional-identity)
    - [Pietsch factorization theorem](#pietsch-factorization-theorem)
    - [Absolutely summing operator](#absolutely-summing-operator)
  - [Strictly singular operator](#strictly-singular-operator)
  - [Positivity-preserving linear operator on L1](#positivity-preserving-linear-operator-on-l1)
    - [Mean control for positive imaging operators](#mean-control-for-positive-imaging-operators)
  - [Schur test](#schur-test)
  - [Bounded inverse](#bounded-inverse)
  - [Positive linear operator on continuous functions](#positive-linear-operator-on-continuous-functions)
    - [Zero-preserving linear operator on continuous functions](#zero-preserving-linear-operator-on-continuous-functions)
  - [Contractive linear operator](#contractive-linear-operator)
  - [Range of a bounded linear operator](#range-of-a-bounded-linear-operator)
  - [Extension of a bounded linear operator from a dense subspace](#extension-of-a-bounded-linear-operator-from-a-dense-subspace)
    - [Failure of dense-subspace extension into an incomplete codomain](#failure-of-dense-subspace-extension-into-an-incomplete-codomain)
  - [Banach space of bounded linear operators](#banach-space-of-bounded-linear-operators)
  - [Continuous linear functional](#continuous-linear-functional)
    - [Linear functional with closed kernel](#linear-functional-with-closed-kernel)
    - [Point evaluation functional](#point-evaluation-functional)
  - [Sequential continuity criterion for a linear map on a metrizable topological vector space](#sequential-continuity-criterion-for-a-linear-map-on-a-metrizable-topological-vector-space)
  - [Isomorphism of Banach spaces](#isomorphism-of-banach-spaces)

## Dense subspace

↑ **Parent:** [Topological vector space](topological-vector-space.md)

A dense subspace of a [topological vector space](topological-vector-space.md) $X$ is a [linear subspace](vector-space.md#vector-subspace) $D$ whose closure is all of $X$. It permits continuous operators to be determined or extended from values on $D$. For a normed space, every vector in $X$ is a limit of vectors from $D$.

## Sequential continuity criterion in a metrizable vector space

↑ **Parent:** [Topological vector space](topological-vector-space.md)

A linear map from a [metrizable space](mathematics.md#metrizable-space) carrying a vector-space topology is continuous if it takes every null sequence to a null sequence. If continuity fails, choose a point in each shrinking basic neighborhood whose image stays outside a fixed neighborhood of zero. These points converge to zero but their images do not. For a [Fréchet space](#frechet-space) described by increasing [seminorms](#seminorm) $p_j$, a discontinuous functional admits $p_j(f_j)\leq1/j$ and $|u(f_j)|\geq1$.

## Bounded set in a topological vector space

↑ **Parent:** [Topological vector space](topological-vector-space.md)

A subset $B$ of a [topological vector space](topological-vector-space.md) is bounded when every neighborhood $U$ of zero absorbs it: $B\subseteq tU$ for all sufficiently large positive $t$. In a [locally convex space](#locally-convex-space) defined by [seminorms](#seminorm) $p_\lambda$, this is equivalent to $\sup_{x\in B}p_\lambda(x)<\infty$ for every $\lambda$. In particular, a bounded subset of the [Schwartz space](fourier-analysis.md#schwartz-space) has a uniform bound for every Schwartz seminorm; it need not have uniformly bounded supports.

## Strict inductive limit topology

↑ **Parent:** [Topological vector space](topological-vector-space.md)

A strict inductive limit topology on an increasing union $E=\bigcup_nE_n$ is the finest locally convex topology compatible with the inclusions of the stages $E_n$. A linear map from $E$ is continuous exactly when each restriction to $E_n$ is continuous.

## Metrizable topological vector space

↑ **Parent:** [Topological vector space](topological-vector-space.md)

A topological vector space is metrizable when its topology is induced by a [metric](topological-analysis.md#metric). At the origin it then has a countable neighborhood basis, so continuity of a [linear map](vector-space.md#linear-map) can be tested on sequences.

## Finite-dimensional vector-space topology

↑ **Parent:** [Topological vector space](topological-vector-space.md)

Every finite-dimensional real vector space has a unique Hausdorff topology making it a topological vector space. Choosing a basis identifies it with ordinary Euclidean space; every linear map between such spaces is continuous.

### Equivalence of norms in finite dimensions

↑ **Parent:** [Finite-dimensional vector-space topology](#finite-dimensional-vector-space-topology)

On a finite-dimensional vector space over a complete valued field, any two norms induce the same topology. Choosing a basis reduces the claim to comparison with the maximum of the absolute values of the coordinates.

#### Sharp comparison of l1 and l2 norms

↑ **Parent:** [Equivalence of norms in finite dimensions](#equivalence-of-norms-in-finite-dimensions)

For $x\in\mathbb R^n$, [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) applied to $(|x_i|)$ and $(1)$ gives the upper bound. Equal absolute coordinate values attain its factor $\sqrt n$. Expanding $(\sum_i|x_i|)^2$ gives the lower bound, and a vector with only one nonzero coordinate attains its factor one. Thus both constants are optimal. These [Lp norms](real-analysis.md#lp-norm) define the same finite-dimensional topology despite having different unit balls.

## Locally convex space

↑ **Parent:** [Topological vector space](topological-vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_convex_space)

A locally convex space is a topological vector space whose topology is generated by a family of seminorms. Its continuous dual consists of the linear functionals bounded by a finite maximum of those seminorms.

### Compact metrizable convex set

↑ **Parent:** [Locally convex space](#locally-convex-space)

Here the set is a nonempty compact metrizable convex subset of a Hausdorff locally convex space. The ambient space can be infinite-dimensional. Continuous affine [functions](function.md) separate its points, and weak-star compact dual balls with separable preduals provide examples. This general setting is needed for [Choquet theorem](#choquet-theorem).

#### Choquet theorem

↑ **Parent:** [Compact metrizable convex set](#compact-metrizable-convex-set)

Every point of a compact metrizable convex subset of a Hausdorff locally convex space is the [barycenter](#barycenter) of a [Borel probability measure](measure-theory.md#borel-probability-measure) concentrated on its [extreme points](mathematical-optimization.md#extreme-point). The theorem is an existence assertion; uniqueness requires additional hypotheses such as a simplex structure.

##### Threshold Choquet representation in L-infinity

↑ **Parent:** [Choquet theorem](#choquet-theorem)

For a real [function](function.md) in the $L^\infty$ unit ball, push uniform [measure](measure-theory.md#measure) on $t\in[0,1]$ forward by the displayed sign-valued [functions](function.md). In the [weak-star topology](weak-topology.md#weak-star-topology) this is a Borel probability concentrated on the [extreme points](mathematical-optimization.md#extreme-point), and [Fubini's theorem](measure-theory.md#fubini-s-theorem) shows that its [barycenter](#barycenter) is $f$. Weak-star compactness and separability of the predual $L^1$ place the example within [Choquet theorem](#choquet-theorem).

<h5 id="choquet-s-theorem-by-strict-convexity">Choquet's theorem by strict convexity</h5>

↑ **Parent:** [Choquet theorem](#choquet-theorem)

Maximize the integral of a continuous strictly convex [function](function.md) among [probability measures](probability-theory.md#probability-measure) with a fixed [barycenter](#barycenter). The [supporting measure lemma for affine upper envelopes](#supporting-measure-lemma-for-affine-upper-envelopes) implies that the maximizing [measure](measure-theory.md#measure) has zero integral of the nonnegative envelope gap. Strict convexity makes this gap positive at every nonextreme point, so the [measure](measure-theory.md#measure) is concentrated on the extreme boundary. Metrizability makes that boundary Borel and supplies the continuous strictly convex [function](function.md).

#### Affine upper envelope

↑ **Parent:** [Compact metrizable convex set](#compact-metrizable-convex-set)

For a bounded real [function](function.md) on a compact convex set, this envelope is the infimum of its continuous affine majorants. It is finite, concave and [upper semicontinuous](calculus.md#upper-semicontinuity), and dominates the [function](function.md). For continuous [functions](function.md) it describes the maximal integral among [probability measures](probability-theory.md#probability-measure) with a specified [barycenter](#barycenter). Its homogeneity, subadditivity and affine-translation identities give the [supporting measure lemma for affine upper envelopes](#supporting-measure-lemma-for-affine-upper-envelopes).

##### Supporting measure lemma for affine upper envelopes

↑ **Parent:** [Affine upper envelope](#affine-upper-envelope)

The sublinear functional $p(g)=\mu(\overline g)$ has a linear supporting functional taking the value $p(f)$ at a specified continuous $f$, by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem). It is positive and normalized because $p$ has these values on constants. The [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) gives the probability $\nu$. Testing affine [functions](function.md) and their negatives shows that $\mu$ and $\nu$ have the same [barycenter](#barycenter).

#### Barycenter

↑ **Parent:** [Compact metrizable convex set](#compact-metrizable-convex-set)

The [barycenter](#barycenter) of a [probability measure](probability-theory.md#probability-measure) on a compact convex set is the point satisfying the displayed affine integral identities. It exists by approximating the [measure](measure-theory.md#measure) by finitely supported [measures](measure-theory.md#measure) and using compactness of their finite convex combinations. It is unique because continuous affine [functions](function.md) separate points. In a Banach-space setting it agrees with the appropriate vector integral when that integral is defined.

### Seminorm

↑ **Parent:** [Locally convex space](#locally-convex-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seminorm)

A seminorm on a [vector space](vector-space.md) is a nonnegative function $p$ satisfying $p(\lambda x)=|\lambda|p(x)$ and $p(x+y)\leq p(x)+p(y)$. Unlike a [norm](functional-analysis.md#norm), it may vanish at nonzero vectors.

#### Dual seminorm

↑ **Parent:** [Seminorm](#seminorm)

Given a bilinear pairing $\langle\cdot,\cdot\rangle$ and a [seminorm](#seminorm) $p$, its dual seminorm is

$$
p^*(y)=\sup_{p(x)\leq1}|\langle x,y\rangle|.
$$

It may be infinite when $y$ does not annihilate the kernel of $p$. Whenever it is finite, the defining inequality gives $|\langle x,y\rangle|\leq p(x)p^*(y)$.

<h3 id="frechet-space">Fréchet space</h3>

↑ **Parent:** [Locally convex space](#locally-convex-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fréchet_space)

A Fréchet space is a complete metrizable [locally convex space](#locally-convex-space). Its topology can be described by a countable family of [seminorms](#seminorm).

### Minkowski functional

↑ **Parent:** [Locally convex space](#locally-convex-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minkowski_functional)

For an absorbing convex set $U$ containing zero, its Minkowski functional is $p_U(x)=\inf\{t>0:x\in tU\}$. If $U$ is open and convex, then $p_U$ is sublinear and $U=\{x:p_U(x)<1\}$.

#### Norm from a bounded symmetric convex neighbourhood

↑ **Parent:** [Minkowski functional](#minkowski-functional)

For a bounded convex open set $U$ containing zero and invariant under $x\mapsto-x$, its [Minkowski functional](#minkowski-functional) is a [norm](functional-analysis.md#norm). Inner and outer Euclidean balls give positive finite bounds; symmetry and scaling give absolute homogeneity; convexity gives the [triangle inequality](topological-analysis.md#triangle-inequality). Openness makes $U=\{p_U<1\}$, while boundedness prevents nonzero vectors from having zero gauge.

### Separation of a point and an open convex set

↑ **Parent:** [Locally convex space](#locally-convex-space)

If $C$ is a nonempty open convex subset of a real locally convex space and $x_0\notin C$, a continuous linear functional strictly separates them: after choosing a sign, $f(c)<f(x_0)$ for every $c\in C$. Apply the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) to the [Minkowski functional](#minkowski-functional) of a translate of $C$.

#### Hahn-Banach separation theorem for two convex sets

↑ **Parent:** [Separation of a point and an open convex set](#separation-of-a-point-and-an-open-convex-set)

If $A$ and $B$ are disjoint nonempty convex subsets of a real locally convex space and $A$ is open, then some continuous linear functional $f$ satisfies

$$
f(a)<f(b)
$$

for all $a\in A$ and $b\in B$.

#### Finite-dimensional separation of open convex sets

↑ **Parent:** [Separation of a point and an open convex set](#separation-of-a-point-and-an-open-convex-set)

If finitely many open convex subsets $K_1,\ldots,K_n$ of a locally convex space have empty intersection, some continuous linear map $T:X\to\mathbb R^{n-1}$ preserves that fact: $\bigcap_iT(K_i)=\varnothing$.

### Dual pair

↑ **Parent:** [Locally convex space](#locally-convex-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_pair)

A dual pair $(E,F)$ consists of a real vector space $E$ and a vector space $F$ of linear functionals that separates the points of $E$. Its weak topology $\sigma(E,F)$ is the coarsest topology making every $f\in F$ continuous, and its continuous dual is exactly $F$.

#### Continuous dual of a weak topology

↑ **Parent:** [Dual pair](#dual-pair)

For a [separated dual pair](#dual-pair), the continuous linear functionals for its [weak topology](weak-topology.md) are exactly evaluations by members of the paired space. Continuity bounds a functional on a neighbourhood defined by finitely many evaluations; scalar rescaling makes it vanish on their common kernel. It then factors through their finite-dimensional evaluation map and is a finite linear combination of them.

#### Compact norming dual-pair criterion

↑ **Parent:** [Dual pair](#dual-pair)

Let $Z\subseteq X^*$ separate points of a Banach space $X$. If the closed unit ball of $X$ is compact for $\sigma(X,Z)$ and $Z$ has the norm inherited from $X^*$, then the evaluation map $X\to Z^*$ is an isometric isomorphism. [Goldstine theorem](functional-analysis.md#goldstine-theorem) makes its unit-ball image weak-star dense, while the assumed compactness makes that image closed.

#### Bipolar theorem for a dual pair

↑ **Parent:** [Dual pair](#dual-pair)

For $A\subseteq E$ in a [dual pair](#dual-pair) $(E,F)$, define $A^\circ=\{f\in F:f(a)\leq1\text{ for all }a\in A\}$. Then

$$
A^{\circ\circ}=\overline{\operatorname{conv}}^{\sigma(E,F)}(A\cup\{0\}).
$$

### Product of locally convex spaces

↑ **Parent:** [Locally convex space](#locally-convex-space)

The product topology on $X\times Y$ is generated by the seminorms $(x,y)\mapsto p(x)$ and $(x,y)\mapsto q(y)$. Its continuous dual is canonically $X^*\oplus Y^*$.

## Continuous linear operator

↑ **Parent:** [Topological vector space](topological-vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous_linear_operator)

A continuous linear map is a [linear map](vector-space.md#linear-map) that is continuous for the topologies on its domain and codomain. Between [normed vector spaces](functional-analysis.md#normed-vector-space), continuity is equivalent to boundedness.

### Completely continuous operator

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A [bounded linear operator](#continuous-linear-operator) between [Banach spaces](banach-space.md) is completely continuous when it maps weakly convergent sequences to norm-convergent sequences. Equivalently, it maps weakly compact sets to norm-compact sets: the [Eberlein-Šmulian theorem](weak-topology.md#eberlein-smulian-theorem) gives the forward direction, while a weakly convergent sequence together with its limit is weakly compact and gives the reverse direction. The inclusion $C(\mathbb T)\to L^2(\mathbb T)$ for finite [Lebesgue measure](measure-theory.md#lebesgue-measure) is completely continuous by pointwise convergence, the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) and the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem), but is not a [compact operator](compact-operator.md) because of the orthogonal Fourier modes.

### Approximate surjectivity with geometric correction

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

Let $T:V\to W$ be a [bounded linear operator](#continuous-linear-operator) with $V$ a [Banach space](banach-space.md). If every $y\in W$ has an approximate preimage $x$ with $\|x\|\le R\|y\|$ and $\|Tx-y\|\le k\|y\|$, where $k<1$, then every $y$ has an exact preimage with the displayed norm bound. Repeatedly correct the residual: the corrections have norms at most $Rk^j\|y\|$ and form an absolutely convergent series; its image under $T$ equals $y$. This proves surjectivity but does not provide a bounded linear right inverse.

### Absolutely p-summing operator

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

For $1\le p<\infty$, a [bounded linear operator](#continuous-linear-operator) $T:E\to F$ between [Banach spaces](banach-space.md) is absolutely p-summing if $(\sum_j\|Tx_j\|^p)^{1/p}\le C\sup_{\phi\in B_{E^*}}(\sum_j|\phi(x_j)|^p)^{1/p}$ for every finite family. The least $C$ is its p-summing norm $\pi_p(T)$. Direct substitution gives the ideal inequality $\pi_p(BTA)\le\|B\|\pi_p(T)\|A\|$ for compatible [bounded linear operators](#continuous-linear-operator).

#### 2-summing operator

↑ **Parent:** [Absolutely p-summing operator](#absolutely-p-summing-operator)

A [bounded linear operator](#continuous-linear-operator) $T:E\to F$ is 2-summing if $\sum_j\|Tx_j\|^2\le C^2\sup_{\phi\in B_{E^*}}\sum_j|\phi(x_j)|^2$ for every finite family; $\pi_2(T)$ is the least $C$. For operators between [Hilbert spaces](hilbert-space.md), this is equivalent to being a [Hilbert-Schmidt operator](compact-operator.md#hilbert-schmidt-operator), with $\pi_2(T)=\|T\|_{\mathrm{HS}}$. The upper bound follows by applying the [Hilbert-Schmidt norm](compact-operator.md#hilbert-schmidt-norm) ideal inequality to the column operator of the family; testing finite orthonormal families gives the reverse bound.

##### 2-summing norm of a finite-dimensional identity

↑ **Parent:** [2-summing operator](#2-summing-operator)

For a finite-dimensional [normed vector space](functional-analysis.md#normed-vector-space) $E$, represent a finite family by its column operator $A:\ell_2^m\to E$. Its operator norm is the family's weak square norm. Since $A=AQ$ for the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto $(\ker A)^\perp$, summing $\|Ae_j\|^2\le\|A\|^2\|Qe_j\|_2^2$ proves the upper bound $\sqrt{\dim E}$. In coordinates adapted to a maximal inscribed Euclidean or Hermitian [ellipsoid](geometry-and-topology.md#ellipsoid), the [John contact decomposition](geometry-and-topology.md#john-contact-decomposition) gives $\sum_r c_ru_ru_r^*=I$ and $\sum_rc_r=\dim E$. The vectors $\sqrt{c_r}u_r$ have total squared norm $\dim E$ and weak square norm one, giving equality. This holds over both real and complex scalars.

#### Pietsch factorization theorem

↑ **Parent:** [Absolutely p-summing operator](#absolutely-p-summing-operator)

For an [absolutely p-summing operator](#absolutely-p-summing-operator) $T:E\to F$, there is a [probability measure](probability-theory.md#probability-measure) $\mu$ on the dual unit ball with its [weak-star topology](weak-topology.md#weak-star-topology) such that $\|Tx\|\le\pi_p(T)(\int|\phi(x)|^p\,d\mu(\phi))^{1/p}$. Thus $T$ factors through the closed span of the evaluation functions in $L^p(\mu)$, with the final operator having norm at most $\pi_p(T)$. Conversely this factorization implies the summing inequality by summing under the integral. Existence of $\mu$ follows from finite-dimensional [Hahn-Banach separation theorem](functional-analysis.md#hahn-banach-separation-theorem): failure for finitely many vectors would contradict the summing inequality for a nonnegative weighted family. Compactness of probability measures then combines the finite constraints. The final operator need only be defined on the indicated closed subspace, not on all of $L^p(\mu)$.

#### Absolutely summing operator

↑ **Parent:** [Absolutely p-summing operator](#absolutely-p-summing-operator)

An absolutely summing operator is an [absolutely p-summing operator](#absolutely-p-summing-operator) with $p=1$. The identity on the infinite-dimensional [l2 sequence space](banach-space.md#l2-sequence-space) is not absolutely summing: the first $n$ coordinate vectors have sum of norms $n$, while their weak 1-norm is $\sqrt n$.

### Strictly singular operator

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A bounded linear operator is strictly singular if it is bounded below on no infinite-dimensional subspace. Equivalently, every infinite-dimensional subspace contains unit vectors with arbitrarily small images. On a [hereditarily indecomposable Banach space](banach-space.md#hereditarily-indecomposable-banach-space), an operator which is arbitrarily small on unit vectors in every finite-codimensional subspace is strictly singular: construct an infinite basic span on which its operator norm is small, then use the zero-angle property of hereditary indecomposability.

### Positivity-preserving linear operator on L1

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A bounded [linear operator](vector-space.md#linear-operator) $T:L^1(\Omega)\to L^1(\Omega)$ preserves positivity when it takes nonnegative functions to nonnegative functions. By linearity it also preserves the pointwise order: $u\le v$ implies $Tu\le Tv$. For example, integration against a nonnegative kernel preserves positivity, as does the identity operator. This is order positivity, which differs from a positive quadratic form on a [Hilbert space](hilbert-space.md).

#### Mean control for positive imaging operators

↑ **Parent:** [Positivity-preserving linear operator on L1](#positivity-preserving-linear-operator-on-l1)

On a bounded connected [Lipschitz domain](real-analysis.md#lipschitz-domain), let $u\ge0$ belong to the [BV space](inverse-problem.md#function-of-bounded-variation-on-a-domain), and let $T$ be a [positivity-preserving operator](#positivity-preserving-linear-operator-on-l1) with $T1\ne0$. Writing $u=c1+(u-c1)$, $c=u_\Omega\ge0$, the [triangle inequality](topological-analysis.md#triangle-inequality) and [Poincaré inequality for total variation](inverse-problem.md#poincare-inequality-for-total-variation) give $c\|T1\|_1\le\|Tu\|_1+\|T\|\|u-c\|_1\le\|Tu\|_1+C_\Omega\|T\|\operatorname{TV}(u)$. Thus forward-image and variation bounds control the missing constant mode, and hence the full $BV$ [norm](functional-analysis.md#norm).

### Schur test

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_test)

For a matrix with nonnegative entries, row sums at most $R$ and column sums at most $C$ imply an $\ell^2$ operator [norm](functional-analysis.md#norm) at most $\sqrt{RC}$. Indeed the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $|\sum_j A_{ij}x_j|^2\le(\sum_jA_{ij})\sum_jA_{ij}|x_j|^2$. Summing over $i$ bounds the result by $RC\sum_j|x_j|^2$. Integral kernels and positive weight functions give analogous forms. The symmetric case has equal row and column bounds.

### Bounded inverse

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

An invertible [bounded linear operator](#continuous-linear-operator) has a [bounded inverse](#bounded-inverse) when $\|u\|\le C\|Ku\|$ for all $u$.

### Positive linear operator on continuous functions

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A linear map $U:C(K,\mathbb R)\to C(K,\mathbb R)$ is positive when $f\geq0$ implies $Uf\geq0$. This is positivity for the pointwise order, not positivity of a quadratic form. On a compact space, $|Uf|\leq U|f|\leq\|f\|_\infty U1$, so $\|U\|=\|U1\|_\infty$. This makes positive maps especially useful for [uniform approximation](uniform-approximation.md).

#### Zero-preserving linear operator on continuous functions

↑ **Parent:** [Positive linear operator on continuous functions](#positive-linear-operator-on-continuous-functions)

If a linear operator on real continuous functions preserves every zero, evaluate $f-f(x)1$ at $x$. The zero-preserving hypothesis forces $Lf(x)=f(x)L1(x)$, so the operator is multiplication by the continuous function $L1$. Positivity further makes that multiplier nonnegative; linearity and zero preservation alone already give the multiplication representation.

### Contractive linear operator

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A bounded [linear operator](vector-space.md#linear-operator) between normed spaces is contractive if its operator norm is at most one. This norm property is distinct from a strict [contraction mapping](analysis.md#contraction-mapping), whose Lipschitz constant must be less than one.

### Range of a bounded linear operator

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

The [operator range](#range-of-a-bounded-linear-operator) is the [image of a linear map](vector-space.md#image-of-a-linear-map) $K$. It need not be closed in an infinite-dimensional [Hilbert space](hilbert-space.md); that failure makes the [Moore–Penrose inverse of an operator](inverse-problem.md#moore-penrose-inverse-of-an-operator) unbounded on its domain.

### Extension of a bounded linear operator from a dense subspace

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

Let $D$ be a [dense linear subspace](topology.md#dense-set) of a normed space $X$, let $Y$ be a [Banach space](banach-space.md), and let $T:D\to Y$ be linear with $\lVert Tx\rVert\leq C\lVert x\rVert$. Then $T$ has a unique bounded extension $\widetilde T:X\to Y$, defined by $\widetilde Tx=\lim_nTx_n$ for any sequence $x_n\in D$ converging to $x$, and $\lVert\widetilde T\rVert\leq C$.

#### Failure of dense-subspace extension into an incomplete codomain

↑ **Parent:** [Extension of a bounded linear operator from a dense subspace](#extension-of-a-bounded-linear-operator-from-a-dense-subspace)

Let $c_{00}$ have the $\ell^2$ norm, take $D=c_{00}\subset X=\ell^2$, and let $T:D\to c_{00}$ be the identity. It is bounded but has no continuous extension $\ell^2\to c_{00}$, because continuity and density would force the extension to be the identity on every element of $\ell^2$.

### Banach space of bounded linear operators

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

If $X$ is a normed vector space and $Y$ is a [Banach space](banach-space.md), then the bounded linear maps $\mathcal B(X,Y)$ form a Banach space under the [operator norm](continuous-dual-space.md#operator-norm). Completeness of the domain is unnecessary.

### Continuous linear functional

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A continuous linear functional is a continuous linear map from a [topological vector space](topological-vector-space.md) to its scalar field. The collection of all such functionals is the [continuous dual space](continuous-dual-space.md).

#### Linear functional with closed kernel

↑ **Parent:** [Continuous linear functional](#continuous-linear-functional)

A [linear functional](linear-algebra.md#linear-functional) on a [normed vector space](functional-analysis.md#normed-vector-space) is continuous exactly when its kernel is closed. The forward direction follows because zero is closed in the scalar field. Conversely, if $l\ne0$, choose $v$ with $l(v)=1$ and write $M=\ker l$. Closedness gives $d=\operatorname{dist}(v,M)>0$. Since $x/l(x)-v\in M$ when $l(x)\ne0$, $|l(x)|\leq\|x\|/d$. The zero functional is continuous separately. Thus the criterion does not require completeness or the [closed graph theorem](functional-analysis.md#closed-graph-theorem).

#### Point evaluation functional

↑ **Parent:** [Continuous linear functional](#continuous-linear-functional)

For a function space on a set $X$ and a point $x\in X$, the point evaluation functional is $\delta_x(f)=f(x)$. It is bounded on $C(X)$ with the [supremum norm](functional-analysis.md#supremum-norm).

### Sequential continuity criterion for a linear map on a metrizable topological vector space

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

A [linear map](vector-space.md#linear-map) from a [metrizable topological vector space](#metrizable-topological-vector-space) is continuous exactly when it maps every sequence converging to zero to a sequence converging to zero. If continuity fails, a decreasing countable neighborhood basis supplies a null sequence whose images stay outside one fixed neighborhood of zero.

### Isomorphism of Banach spaces

↑ **Parent:** [Continuous linear operator](#continuous-linear-operator)

An isomorphism of Banach spaces is a bijective bounded [linear map](vector-space.md#linear-map) whose inverse is bounded. The [bounded inverse theorem](functional-analysis.md#bounded-inverse-theorem) makes boundedness of the inverse automatic.

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Bounded set in a topological vector space](#bounded-set-in-a-topological-vector-space)
- [Closed vector subspace](vector-space.md#closed-vector-subspace)
- [Continuous linear functional](#continuous-linear-functional)
- [Dense subspace](#dense-subspace)
- [Reflexive space](functional-analysis.md#reflexive-space)
