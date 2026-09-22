# Topological analysis

↑ **Parent:** [Analysis](analysis.md)

**Table of contents**

- [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)
  - [Positive matrix eigenvector from simplex normalization](#positive-matrix-eigenvector-from-simplex-normalization)
  - [Surjectivity of a continuous bounded-displacement map](#surjectivity-of-a-continuous-bounded-displacement-map)
  - [Brouwer inward-pointing zero lemma](#brouwer-inward-pointing-zero-lemma)
  - [Polynomial root from a disk self-map](#polynomial-root-from-a-disk-self-map)
  - [Poincaré-Miranda theorem](#poincare-miranda-theorem)
    - [Clamped-map proof of planar path crossing](#clamped-map-proof-of-planar-path-crossing)
  - [Sperner's lemma](#sperner-s-lemma)
- [No-retraction theorem](#no-retraction-theorem)
- [Metric space](#metric-space)
  - [Distortion (mathematics)](#distortion-mathematics)
  - [Ball (mathematics)](#ball-mathematics)
  - [Maximum product metric](#maximum-product-metric)
    - [Closed diagonal of a metric space](#closed-diagonal-of-a-metric-space)
  - [Metric epsilon-net](#metric-epsilon-net)
  - [Uniform metric](#uniform-metric)
    - [Completeness of the continuous-map space in the uniform metric](#completeness-of-the-continuous-map-space-in-the-uniform-metric)
  - [Separated subset of a metric space](#separated-subset-of-a-metric-space)
    - [Inclusion-maximal separated set](#inclusion-maximal-separated-set)
      - [Maximal separated sets give covers](#maximal-separated-sets-give-covers)
  - [Closed ball](#closed-ball)
  - [Metric net](#metric-net)
    - [Unit sphere net from ball covering](#unit-sphere-net-from-ball-covering)
    - [Quadratic form net bound](#quadratic-form-net-bound)
    - [Volumetric bound for Euclidean metric nets](#volumetric-bound-for-euclidean-metric-nets)
  - [Metric covering number](#metric-covering-number)
    - [Metric entropy](#metric-entropy)
      - [Entropy of Lipschitz compositions](#entropy-of-lipschitz-compositions)
      - [Entropy of a smooth periodic function ball](#entropy-of-a-smooth-periodic-function-ball)
    - [Finite net](#finite-net)
      - [Random Lipschitz constant in a finite net bound](#random-lipschitz-constant-in-a-finite-net-bound)
  - [Metric path length](#metric-path-length)
  - [Geodesic metric space](#geodesic-metric-space)
    - [Metric geodesic](#metric-geodesic)
      - [Metric geodesic triangle](#metric-geodesic-triangle)
  - [Metric topology](#metric-topology)
  - [Bounded set](#bounded-set)
  - [Distance from a point to a closed set](#distance-from-a-point-to-a-closed-set)
  - [Metric](#metric)
    - [Bounded metric transform](#bounded-metric-transform)
    - [Compatible metric](#compatible-metric)
    - [Arctangent pullback metric](#arctangent-pullback-metric)
    - [Discrete metric](#discrete-metric)
    - [Pseudometric](#pseudometric)
      - [Metric quotient of a pseudometric](#metric-quotient-of-a-pseudometric)
    - [Ultrametric](#ultrametric)
  - [Compact metric space](#compact-metric-space)
    - [Complete totally bounded metric space is compact](#complete-totally-bounded-metric-space-is-compact)
    - [Totally bounded space](#totally-bounded-space)
  - [Convergence in a metric space](#convergence-in-a-metric-space)
  - [Sequential characterization of continuity in metric spaces](#sequential-characterization-of-continuity-in-metric-spaces)
  - [Sequential compactness of a compact metric space](#sequential-compactness-of-a-compact-metric-space)
  - [Normality of every metric space](#normality-of-every-metric-space)
  - [Bounded-continuous-function characterization of compact metric spaces](#bounded-continuous-function-characterization-of-compact-metric-spaces)
  - [Completeness](#completeness)
  - [Triangle inequality](#triangle-inequality)
    - [Reverse triangle inequality](#reverse-triangle-inequality)
      - [Four-point triangle inequality](#four-point-triangle-inequality)
    - [Triangle inequality for a vector-valued integral](#triangle-inequality-for-a-vector-valued-integral)
    - [Equality condition in the complex triangle inequality](#equality-condition-in-the-complex-triangle-inequality)
    - [Integral triangle inequality](#integral-triangle-inequality)
  - [Euclidean distance](#euclidean-distance)
    - [Standardized Euclidean distance](#standardized-euclidean-distance)
  - [Diameter](#diameter)
  - [Uniform continuity](#uniform-continuity)
    - [Uniformly continuous integrable dissipation tends to zero](#uniformly-continuous-integrable-dissipation-tends-to-zero)
    - [Uniformly continuous function on a totally bounded set is bounded](#uniformly-continuous-function-on-a-totally-bounded-set-is-bounded)
    - [Products of unbounded uniformly continuous functions](#products-of-unbounded-uniformly-continuous-functions)
    - [Uniformly continuous integrable functions vanish at infinity](#uniformly-continuous-integrable-functions-vanish-at-infinity)
    - [Pointwise approximation by uniformly continuous functions](#pointwise-approximation-by-uniformly-continuous-functions)
    - [Modulus of continuity](#modulus-of-continuity)
      - [Log-Lipschitz modulus](#log-lipschitz-modulus)
    - [Heine-Cantor theorem](#heine-cantor-theorem)
    - [Uniform limit theorem for uniformly continuous functions](#uniform-limit-theorem-for-uniformly-continuous-functions)
    - [Sequential criterion for uniform continuity](#sequential-criterion-for-uniform-continuity)
  - [Equivalence of metrics](#equivalence-of-metrics)
    - [Equivalent metrics need not be bi-Lipschitz equivalent](#equivalent-metrics-need-not-be-bi-lipschitz-equivalent)
    - [Equivalent codomain metrics need not preserve uniform convergence](#equivalent-codomain-metrics-need-not-preserve-uniform-convergence)
  - [Distance to a set](#distance-to-a-set)
    - [Distance between two sets](#distance-between-two-sets)
  - [Isolated point](#isolated-point)
  - [Complete metric space](#complete-metric-space)
    - [Cauchy-sequence construction of a metric completion](#cauchy-sequence-construction-of-a-metric-completion)
    - [Topological completeness](#topological-completeness)
      - [G-delta criterion for topological completeness](#g-delta-criterion-for-topological-completeness)
    - [Polish space](#polish-space)
      - [Tree on a Polish space](#tree-on-a-polish-space)
    - [Cantor's intersection theorem](#cantor-s-intersection-theorem)
    - [Baire category theorem](#baire-category-theorem)
      - [Baire avoidance of countably many affine hyperplanes](#baire-avoidance-of-countably-many-affine-hyperplanes)
      - [Local uniform Cauchy control for pointwise convergent continuous functions](#local-uniform-cauchy-control-for-pointwise-convergent-continuous-functions)
      - [Residual set](#residual-set)
      - [Comeagre subgroup completeness argument](#comeagre-subgroup-completeness-argument)
      - [Banach space has uncountable Hamel dimension](#banach-space-has-uncountable-hamel-dimension)
      - [Nowhere differentiable continuous function](#nowhere-differentiable-continuous-function)
      - [Baire space](#baire-space)
        - [Baire function](#baire-function)
          - [Baire class one function](#baire-class-one-function)
            - [Rationality indicator is not Baire class one](#rationality-indicator-is-not-baire-class-one)
      - [Closed convex absorbing set has an origin neighbourhood](#closed-convex-absorbing-set-has-an-origin-neighbourhood)
        - [Closed symmetric absorbing set without an origin neighbourhood](#closed-symmetric-absorbing-set-without-an-origin-neighbourhood)
      - [Isolated points in a countable complete metric space](#isolated-points-in-a-countable-complete-metric-space)
      - [Nowhere dense set](#nowhere-dense-set)
      - [Meagre set](#meagre-set)
        - [Luzin set](#luzin-set)
        - [Comeagre set](#comeagre-set)
        - [Lusin set](#lusin-set)
          - [Lusin set construction under CH](#lusin-set-construction-under-ch)
      - [Generic nowhere-monotone continuous function](#generic-nowhere-monotone-continuous-function)
      - [Smooth function with a pointwise vanishing derivative](#smooth-function-with-a-pointwise-vanishing-derivative)
      - [Nonpolynomial entire function has a centre with no zero Taylor coefficient](#nonpolynomial-entire-function-has-a-centre-with-no-zero-taylor-coefficient)
    - [Space of smooth functions on a compact interval](#space-of-smooth-functions-on-a-compact-interval)
      - [Completeness of the smooth-function metric](#completeness-of-the-smooth-function-metric)
      - [Generic superfactorial derivative growth at rational points](#generic-superfactorial-derivative-growth-at-rational-points)
        - [Nowhere-analytic generic smooth function](#nowhere-analytic-generic-smooth-function)
    - [Closed-subspace completeness theorem](#closed-subspace-completeness-theorem)
  - [Hausdorff distance](#hausdorff-distance)
    - [Closed singleton embedding in a Hausdorff hyperspace](#closed-singleton-embedding-in-a-hausdorff-hyperspace)
      - [Completeness is reflected by the Hausdorff hyperspace](#completeness-is-reflected-by-the-hausdorff-hyperspace)
    - [Gromov-Hausdorff distance](#gromov-hausdorff-distance)
      - [Gromov-Hausdorff topology](#gromov-hausdorff-topology)
      - [Real tree](#real-tree)
        - [Multiplicity of a point in a real tree](#multiplicity-of-a-point-in-a-real-tree)
        - [Real tree encoded by an excursion](#real-tree-encoded-by-an-excursion)
          - [Excursion coding theorem for compact real trees](#excursion-coding-theorem-for-compact-real-trees)
- [Equicontinuity](#equicontinuity)
  - [Uniformly bounded family of functions](#uniformly-bounded-family-of-functions)
  - [Pointwise bounded family of functions](#pointwise-bounded-family-of-functions)
  - [Arzelà-Ascoli theorem](#arzela-ascoli-theorem)
    - [Nonlinear ODE bounds from interior extrema](#nonlinear-ode-bounds-from-interior-extrema)
    - [Relatively compact subset](#relatively-compact-subset)
    - [Diagonal subsequence for locally uniform convergence](#diagonal-subsequence-for-locally-uniform-convergence)
      - [Escaping bump counterexample to global uniform convergence](#escaping-bump-counterexample-to-global-uniform-convergence)

## Brouwer fixed-point theorem

↑ **Parent:** [Topological analysis](topological-analysis.md)

Every continuous self-map of a closed disc has a fixed point.

### Positive matrix eigenvector from simplex normalization

↑ **Parent:** [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)

For a strictly positive real matrix $A$, the map $x\mapsto Ax/\sum_i(Ax)_i$ is a continuous self-map of the probability simplex. A [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem) fixed point satisfies $Ax=\lambda x$ with $\lambda>0$. The image lies in the interior of the simplex, so every entry of this [eigenvector](linear-operator-theory.md#eigenvector) is strictly positive. Nonnegative entries and nonzero columns alone do not imply this strict conclusion.

### Surjectivity of a continuous bounded-displacement map

↑ **Parent:** [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)

If a [continuous map](topology.md#continuous-map) $g:\mathbb R^n\to\mathbb R^n$ has $\|g(x)-x\|\leq K$, then it is onto. For a target $y$, choose $R\geq K+\|y\|$, $R>0$, and map the [unit ball](functional-analysis.md#unit-ball) to itself by $f(x)=x-(g(Rx)-y)/R$. A [fixed point](function.md#fixed-point) gives $g(Rx)=y$.

### Brouwer inward-pointing zero lemma

↑ **Parent:** [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)

Let $V$ be a finite-dimensional real inner-product space and let $F:V\to V$ be continuous. If $\langle F(x),x\rangle<0$ on the sphere $\|x\|=R$, then $F$ has a zero in the open ball. Otherwise the radial projection of $F$ gives a map of the ball that contradicts the [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem).

### Polynomial root from a disk self-map

↑ **Parent:** [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)

If a polynomial equation can be rearranged as $z=F(z)$ with a continuous $F$ mapping a closed disk into itself, Brouwer's theorem guarantees a root in that disk.

<h3 id="poincare-miranda-theorem">Poincaré-Miranda theorem</h3>

↑ **Parent:** [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré–Miranda_theorem)

If each component of a continuous map on a box has opposite weak signs on the corresponding pair of faces, the map has a zero.

#### Clamped-map proof of planar path crossing

↑ **Parent:** [Poincaré-Miranda theorem](#poincare-miranda-theorem)

Projecting a sign-corrected displacement map back to a square turns Brouwer's fixed point into a zero of the displacement, proving that paths joining opposite side pairs intersect.

<h3 id="sperner-s-lemma">Sperner's lemma</h3>

↑ **Parent:** [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sperner's_lemma)

Triangulate a triangle and label every vertex by $1$, $2$, or $3$, forbidding label $i$ on the side opposite vertex $i$. Then the number of small triangles carrying all three labels is odd, and in particular at least one such triangle exists. Counting edges whose endpoint labels are $1$ and $2$ proves the parity statement: boundary incidences are odd, while a small triangle has odd incidence exactly when it has all three labels.

## No-retraction theorem

↑ **Parent:** [Topological analysis](topological-analysis.md)

No closed disc retracts continuously onto its boundary. This is equivalent to [Brouwer fixed-point theorem](#brouwer-fixed-point-theorem) by the standard ray construction and the antipodal map.

## Metric space

↑ **Parent:** [Topological analysis](topological-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metric_space)

A metric space is a set equipped with a nonnegative symmetric distance satisfying definiteness and the triangle inequality.

### Distortion (mathematics)

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Distortion_(mathematics))

[Distortion](#distortion-mathematics) measures how a mapping changes distances or geometric quantities relative to their original values. For an injective map between metric spaces, one multiplicative measure is the product of its Lipschitz constant and the Lipschitz constant of its inverse on the image. [Subgroup distortion](geometric-group-theory.md#subgroup-distortion) instead compares intrinsic and ambient word metrics through a growth function.

### Ball (mathematics)

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ball_(mathematics))

In a [metric space](#metric-space), an open ball $B(a,r)$ consists of points whose distance from $a$ is less than $r$. The closed ball uses a nonstrict inequality. A [Euclidean ball](functional-analysis.md#euclidean-ball) uses Euclidean distance, while a [unit ball](functional-analysis.md#unit-ball) in a normed space uses its norm and radius one.

### Maximum product metric

↑ **Parent:** [Metric space](#metric-space)

The displayed metric on a product of two [metric spaces](#metric-space) satisfies its [triangle inequality](#triangle-inequality) because $\max\{a+c,b+d\}\le\max\{a,b\}+\max\{c,d\}$ for nonnegative coordinates. Its open balls are products of equal-radius balls, so it induces the [product topology](geometry-and-topology.md#product-topology).

#### Closed diagonal of a metric space

↑ **Parent:** [Maximum product metric](#maximum-product-metric)

For a [metric space](#metric-space) with the same metric on both factors, the diagonal is a [closed subset](topology.md#closed-set) of its product. At an off-diagonal point $(x,y)$ let $\delta=d(x,y)>0$. A maximum-metric ball of radius $\delta/3$ misses the diagonal, since a common coordinate $z$ would give $d(x,y)\le d(x,z)+d(z,y)<2\delta/3$. Equality of underlying sets without equality or compatibility of the metrics is a different assertion.

### Metric epsilon-net

↑ **Parent:** [Metric space](#metric-space)

An [epsilon-net](#metric-epsilon-net) in a [metric space](#metric-space) is a set within distance $\varepsilon$ of every point. A maximal $\varepsilon$-separated set is an [epsilon-net](#metric-epsilon-net): any uncovered point could be added. On the [unit sphere](topology.md#unit-sphere) of $\mathbb R^k$, disjoint [Euclidean balls](functional-analysis.md#euclidean-ball) of radius $\varepsilon/2$ around separated points lie in the ball of radius $1+\varepsilon/2$. Comparing [Lebesgue measures](measure-theory.md#lebesgue-measure) gives a net of [cardinality](set-theory.md#cardinality) at most $(1+2/\varepsilon)^k$.

### Uniform metric

↑ **Parent:** [Metric space](#metric-space)

The supremum of pointwise distances defines a metric on maps when it is finite, for example if the target [metric space](#metric-space) is bounded. Convergence in this metric is [uniform convergence](real-analysis.md#uniform-convergence). If the target is complete, Cauchy sequences have pointwise limits and the Cauchy estimate makes convergence uniform.

#### Completeness of the continuous-map space in the uniform metric

↑ **Parent:** [Uniform metric](#uniform-metric)

A Cauchy sequence in the [uniform metric](#uniform-metric) has a pointwise limit in the complete target, and the common Cauchy bound makes convergence uniform. The triangle inequality with one fixed continuous approximant shows that the limit is continuous. Thus the space of all continuous maps into a bounded [complete metric space](#complete-metric-space) is complete, with no compactness assumption on the domain.

### Separated subset of a metric space

↑ **Parent:** [Metric space](#metric-space)

A subset is $r$-separated if distinct points have distance at least $r$. Such a subset is a packing by points; small balls around them have disjoint interiors at suitable radius. A large [separated set](#separated-subset-of-a-metric-space) supplies many distinguishable alternatives in statistical lower-bound arguments.

#### Inclusion-maximal separated set

↑ **Parent:** [Separated subset of a metric space](#separated-subset-of-a-metric-space)

An inclusion-maximal [separated set](#separated-subset-of-a-metric-space) is one to which no further point of the ambient [metric space](#metric-space) can be added while keeping the same separation. It need not have the largest possible cardinality. In a finite space it can be obtained by repeatedly adding an admissible point.

##### Maximal separated sets give covers

↑ **Parent:** [Inclusion-maximal separated set](#inclusion-maximal-separated-set)

If an [inclusion-maximal separated set](#inclusion-maximal-separated-set) has separation at least $r$, every point of the ambient [metric space](#metric-space) is at distance strictly less than $r$ from a selected point. Otherwise that point could be added. Thus upper bounds on the sizes or measures of radius-$r$ balls give lower bounds on the size of the [separated set](#separated-subset-of-a-metric-space).

### Closed ball

↑ **Parent:** [Metric space](#metric-space)

In a [metric space](#metric-space) $(M,d)$, the closed ball centred at $x$ of radius $r\geq0$ is $\{y\in M:d(x,y)\leq r\}$. It is a [closed set](topology.md#closed-set), since the distance to $x$ is a [continuous](calculus.md#continuous-function) [function](function.md). Its boundary need not be the whole corresponding distance sphere in an arbitrary [metric space](#metric-space).

### Metric net

↑ **Parent:** [Metric space](#metric-space)

An $\varepsilon$-net of a [metric space](#metric-space) $(T,d)$ is a subset $U\subseteq T$ such that every $x\in T$ has $d(x,u)\leq\varepsilon$ for some $u\in U$. Its least possible finite size is the [metric covering number](#metric-covering-number) with closed balls. A maximal set with pairwise distances greater than $\varepsilon$ is an $\varepsilon$-net.

#### Unit sphere net from ball covering

↑ **Parent:** [Metric net](#metric-net)

A cover of the [unit ball](functional-analysis.md#unit-ball) by balls of radius $\delta/2$ gives a radius-$\delta$ [metric net](#metric-net) on the [unit sphere](topology.md#unit-sphere): discard balls missing the sphere and choose a sphere point in each remaining ball. Every sphere point lies within $\delta$ of the selected point in its ball. The argument keeps the number of balls and ensures that the selected points have unit length, regardless of the initial covering centers.

#### Quadratic form net bound

↑ **Parent:** [Metric net](#metric-net)

For a [symmetric matrix](linear-algebra.md#symmetric-matrix) $H$ and an $\eta$-[metric net](#metric-net) $U$ of the [unit sphere](topology.md#unit-sphere), with $0<\eta<1/2$, approximate a maximizing unit vector $x$ by $u\in U$. Expanding $x^\top Hx-u^\top Hu=(x-u)^\top Hx+u^\top H(x-u)$ bounds its absolute value by $2\eta\|H\|_{\mathrm{op}}$. Rearrangement proves the bound. The [volumetric bound for Euclidean metric nets](#volumetric-bound-for-euclidean-metric-nets) limits the number of needed directions, allowing a [union bound](probability-inequality.md#boole-s-inequality) to control a random matrix.

#### Volumetric bound for Euclidean metric nets

↑ **Parent:** [Metric net](#metric-net)

A subset of the radius-$R$ [Euclidean ball](functional-analysis.md#euclidean-ball) admits an $\varepsilon$-[metric net](#metric-net) of size at most $(1+2R/\varepsilon)^n$. Take a maximal separated set: its disjoint radius-$\varepsilon/2$ [Euclidean balls](functional-analysis.md#euclidean-ball) lie in the radius-$(R+\varepsilon/2)$ ball. Comparing [Lebesgue measures](measure-theory.md#lebesgue-measure) gives the estimate. In particular, the [unit sphere](topology.md#unit-sphere) admits a net of radius one with at most $3^n$ points.

### Metric covering number

↑ **Parent:** [Metric space](#metric-space)

For a [metric space](#metric-space) or [pseudometric](#pseudometric) space $(T,d)$, this is the minimum number of balls of radius $\varepsilon>0$, with centers in $T$, needed to cover $T$. The displayed grid bound uses closed balls. For open balls, replacing the radius by a fixed constant factor gives the same entropy estimates. For $T=[0,1]$ and $d(s,t)=c|s-t|^H$, a uniform grid gives $N(\varepsilon,T,d)\leq1+\lceil(c/\varepsilon)^{1/H}\rceil$. These polynomial growth bounds make the [Dudley entropy integral](stochastic-process.md#dudley-entropy-integral) finite.

#### Metric entropy

↑ **Parent:** [Metric covering number](#metric-covering-number)

For a subset $E$ of a [metric space](#metric-space), its metric entropy at resolution $\varepsilon$ is the logarithm of the least number of radius-$\varepsilon$ balls covering $E$, with value infinity when no finite cover exists. It quantifies how many choices are needed to approximate an element at that resolution. If points are pairwise more than $2\varepsilon$ apart, each covering ball contains at most one, giving a lower bound by their logarithmic cardinality. The logarithm base changes only a constant factor. This approximation entropy differs from [Kolmogorov-Sinai entropy](measure-theory.md#kolmogorov-sinai-entropy) of a dynamical system.

##### Entropy of Lipschitz compositions

↑ **Parent:** [Metric entropy](#metric-entropy)

Suppose outer functions in a family $B$ obey $|f(x)-f(y)|\le L\max_j|x_j-y_j|$, and compose them with $m$ inner functions drawn from $E$. Approximate the outer function within $\varepsilon/2$ and each inner function within $\varepsilon/(2L)$. The triangle inequality bounds the composed error by $\varepsilon$. Multiplying the numbers of possible net choices and taking logarithms gives the stated inequality. A uniform bound on first partial derivatives supplies $L=m$ for the $C^p$ unit ball, so the exponent of a common entropy bound for the outer and inner classes is retained under [function composition](algebra.md#function-composition).

##### Entropy of a smooth periodic function ball

↑ **Parent:** [Metric entropy](#metric-entropy)

For the unit ball of $C^p(\mathbb T^n)$ measured in the uniform metric, $c\varepsilon^{-n/p}\le H(\varepsilon)\le C\varepsilon^{-n/p}\log(1/\varepsilon)$. The lower bound uses disjoint [bump functions](analysis.md#bump-function) of spatial scale $h$, height proportional to $h^p$ and independently chosen zero/one coefficients: there are $\exp(c h^{-n})$ functions separated at scale $h^p$. For the upper bound, [Multivariable Jackson approximation](uniform-approximation.md#multivariable-jackson-approximation) gives a [trigonometric polynomial](fourier-series.md#trigonometric-polynomial) of degree $O(\varepsilon^{-1/p})$. Its $O(\varepsilon^{-n/p})$ coefficients are bounded and can be rounded with coefficient accuracy proportional to $\varepsilon$ divided by the coefficient count. Counting those rounded coefficient arrays supplies the logarithmic factor. The continuous-function unit ball without derivative bounds has infinite entropy for $\varepsilon<1/2$, by an infinite sequence of disjoint height-one bumps.

#### Finite net

↑ **Parent:** [Metric covering number](#metric-covering-number)

An $\varepsilon$-net of a [metric space](#metric-space) is a set $G$ such that every point lies within distance $\varepsilon$ of a point of $G$. A Cartesian grid of coordinate spacing $\eta$ is a finite $\sqrt d\,\eta$-net of a bounded cube in the [Euclidean norm](functional-analysis.md#euclidean-norm). A [Lipschitz bound](real-analysis.md#lipschitz-bound) transfers control on the grid to control over the whole cube.

##### Random Lipschitz constant in a finite net bound

↑ **Parent:** [Finite net](#finite-net)

Suppose $|Z(u)-Z(v)|\leq L\|u-v\|$ with a random finite $L$. On $L\leq\ell$, a [finite net](#finite-net) with radius $\eta$ bounds the full [supremum](real-analysis.md#supremum) by the grid maximum plus $\ell\eta$. The [Markov inequality](probability-inequality.md#markov-inequality) controls the exceptional event using $\mathbb EL$, and a [union bound](probability-inequality.md#boole-s-inequality) controls the grid maximum. Choosing the net spacing balances these two costs.

### Metric path length

↑ **Parent:** [Metric space](#metric-space)

For a [continuous path](geometry-and-topology.md#continuous-path) $\gamma:[a,b]\to X$ in a [metric space](#metric-space), take the [supremum](real-analysis.md#supremum) over finite partitions $a=t_0<\cdots<t_n=b$ of $\sum_{i=1}^n d(\gamma(t_i),\gamma(t_{i-1}))$. This definition allows $+\infty$ and needs no [derivative](calculus.md#derivative). A [metric geodesic](#metric-geodesic) parametrized on $[a,b]$ has length $b-a$. In a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), it agrees with the usual [arc length](riemannian-geometry.md#arc-length) integral for a [smooth](analysis.md#smooth-function) curve.

### Geodesic metric space

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic_metric_space)

A [metric space](#metric-space) in which every two points are joined by a [metric geodesic](#metric-geodesic) segment. Equivalently, they admit a [continuous path](geometry-and-topology.md#continuous-path) whose [metric path length](#metric-path-length) equals their distance. In this general setting no [Riemannian metric](differential-geometry.md#riemannian-metric) or [covariant derivative](general-relativity.md#covariant-derivative) is required.

#### Metric geodesic

↑ **Parent:** [Geodesic metric space](#geodesic-metric-space)

A unit-speed metric geodesic in a [metric space](#metric-space) is an [isometric embedding](riemannian-geometry.md#isometric-embedding) $\gamma:I\to X$ of a [real interval](real-analysis.md#interval-mathematics). Every restricted segment realizes the distance between its endpoints. A one-point interval permits a constant segment. In a unit-edge graph, shortest edge paths parametrized by [metric path length](#metric-path-length) are metric geodesics; no smooth structure is required. This is stronger than the differential definition of a [geodesic](riemannian-geometry.md#geodesic) in a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), which need only minimize locally: on a unit circle, an arc of angle $3\pi/2$ is a Riemannian geodesic but its endpoint distance is only $\pi/2$.

##### Metric geodesic triangle

↑ **Parent:** [Metric geodesic](#metric-geodesic)

A metric geodesic triangle consists of three points of a [geodesic metric space](#geodesic-metric-space) and a chosen [metric geodesic](#metric-geodesic) segment between each pair. Multiple choices are allowed, and coincident vertices give degenerate triangles. A [Gromov-hyperbolic metric space](geometric-group-theory.md#hyperbolic-metric-space) has a uniform bound on the distance from each side to the other two sides for every such choice. This definition applies to [Cayley graphs](geometric-group-theory.md#cayley-graph) and trees without tangent vectors or curvature assumptions; it does not invoke the surface angle formula for a [geodesic triangle](riemannian-geometry.md#geodesic-triangle).

### Metric topology

↑ **Parent:** [Metric space](#metric-space)

The metric topology consists of the sets $U$ such that every $x\in U$ contains some open ball $B(x,r)$ lying in $U$.

### Bounded set

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounded_set)

A subset $A$ of a [metric space](#metric-space) is bounded if it lies in some finite-radius ball: there are $x$ and $R<\infty$ such that $d(x,a)\leq R$ for every $a\in A$.

### Distance from a point to a closed set

↑ **Parent:** [Metric space](#metric-space)

For a point $x$ and a nonempty [closed set](topology.md#closed-set) $A$ in a [metric space](#metric-space), the distance

$$
d(x,A)=\inf_{a\in A}d(x,a)
$$

is a continuous function of $x$. It vanishes exactly on $A$.

### Metric

↑ **Parent:** [Metric space](#metric-space)

A metric on a [set](set.md) $X$ is a function $d:X\times X\to[0,\infty)$ that is symmetric, satisfies the [triangle inequality](#triangle-inequality), and obeys $d(x,y)=0$ exactly when $x=y$.

A metric equips its underlying [set](set.md) with a [metric space](#metric-space) structure; the distance function and the space carrying it are distinct concepts.

#### Bounded metric transform

↑ **Parent:** [Metric](#metric)

The increasing function $\phi(s)=s/(1+s)$ is subadditive on nonnegative arguments: each summand $b/(1+b)$ and $c/(1+c)$ is at least its numerator divided by $1+b+c$. Thus $\phi\circ d$ is a [metric](#metric) whenever $d$ is. It is bounded and induces the same topology because $\phi$ and its inverse near zero preserve convergence to zero.

#### Compatible metric

↑ **Parent:** [Metric](#metric)

A [metric](#metric) is compatible with a given topology when its open balls generate exactly that topology. [Compatible metrics](#compatible-metric) on a compact [topological space](topology.md#topological-space) are uniformly equivalent: the identity maps between the resulting compact [metric spaces](#metric-space) are [uniformly continuous](#uniform-continuity). Consequently they define the same [proximality](dynamical-systems.md#proximality) and the same asymptotic-pair relation for a fixed [continuous map](topology.md#continuous-map).

#### Arctangent pullback metric

↑ **Parent:** [Metric](#metric)

This [metric](#metric) identifies $\mathbb R$ isometrically with the open interval $(-\pi/2,\pi/2)$ in the usual real distance. It induces the usual topology but is incomplete: the integer sequence has transformed limit $\pi/2$ outside that interval. This illustrates that completeness depends on the [metric](#metric), not solely on its topology.

#### Discrete metric

↑ **Parent:** [Metric](#metric)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_metric)

The discrete metric sets $d(x,x)=0$ and $d(x,y)=1$ for distinct points. It induces the [discrete topology](topology.md#discrete-space), and its Cauchy sequences are exactly the eventually constant sequences.

#### Pseudometric

↑ **Parent:** [Metric](#metric)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudometric)

A pseudometric satisfies the axioms of a [metric](#metric) except that distinct points may have distance zero.

##### Metric quotient of a pseudometric

↑ **Parent:** [Pseudometric](#pseudometric)

Zero distance in a [pseudometric](#pseudometric) defines an [equivalence relation](set-theory.md#equivalence-relation): the triangle inequality proves transitivity. If $x$ and $x'$ have zero distance, as do $y$ and $y'$, the triangle inequality in both directions gives $d(x,y)=d(x',y')$. Thus distance descends to the quotient and becomes a [metric](#metric), since zero quotient distance means the classes coincide.

#### Ultrametric

↑ **Parent:** [Metric](#metric)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultrametric)

An ultrametric is a [metric](#metric) satisfying the strong triangle inequality

$$
d(x,z)\leq\max\{d(x,y),d(y,z)\}.
$$

### Compact metric space

↑ **Parent:** [Metric space](#metric-space)

A compact metric space is a [metric space](#metric-space) that is [compact](topology.md#compact-space). Equivalently, it is [complete](#completeness) and [totally bounded](#totally-bounded-space).

#### Complete totally bounded metric space is compact

↑ **Parent:** [Compact metric space](#compact-metric-space)

A metric space is compact exactly when it is both [complete](#completeness) and [totally bounded](#totally-bounded-space). For the nontrivial direction, successively choose a point from a nested sequence of finite $2^{-n}$-nets; a diagonal construction gives a Cauchy subsequence of every sequence, and completeness gives its limit.

#### Totally bounded space

↑ **Parent:** [Compact metric space](#compact-metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Totally_bounded_space)

A [metric space](#metric-space) is totally bounded when, for every $\varepsilon>0$, it is covered by finitely many open balls of radius $\varepsilon$.

A [metric space](#metric-space) is totally bounded when, for every $\varepsilon>0$, finitely many open balls of radius $\varepsilon$ cover it. Equivalently it has a finite $\varepsilon$-net at every positive scale.

### Convergence in a metric space

↑ **Parent:** [Metric space](#metric-space)

A sequence $(x_n)$ converges to $x$ in a metric space when $d(x_n,x)\to0$, equivalently when every neighbourhood of $x$ contains all sufficiently late terms.

### Sequential characterization of continuity in metric spaces

↑ **Parent:** [Metric space](#metric-space)

A map between metric spaces is continuous exactly when $x_n\to x$ always implies $f(x_n)\to f(x)$. If an inverse image of an open set were not open, points outside it could be chosen within distance $1/n$ of a point inside it, proving the converse by contradiction.

### Sequential compactness of a compact metric space

↑ **Parent:** [Metric space](#metric-space)

Every sequence in a compact metric space has a convergent subsequence. Conversely, sequential compactness and compactness are equivalent for metric spaces.

### Normality of every metric space

↑ **Parent:** [Metric space](#metric-space)

Every metric space is normal. For disjoint closed sets $A,B$, the function

$$
x\longmapsto\frac{d(x,A)}{d(x,A)+d(x,B)}
$$

is continuous, equals zero on $A$, and equals one on $B$; inverse images of disjoint neighbourhoods of zero and one separate the sets.

### Bounded-continuous-function characterization of compact metric spaces

↑ **Parent:** [Metric space](#metric-space)

A metric space $X$ is compact exactly when every continuous function $X\to\mathbb R$ is bounded. For the converse, a noncompact metric space contains a closed discrete sequence; the unbounded function assigning its $n$th point the value $n$ extends to $X$ by the Tietze extension theorem.

### Completeness

↑ **Parent:** [Metric space](#metric-space)

A metric space is complete when every [Cauchy sequence](real-analysis.md#cauchy-sequence) converges to a point of the space.

### Triangle inequality

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangle_inequality)

A metric satisfies $d(x,z)\leq d(x,y)+d(y,z)$. A norm satisfies the corresponding inequality $\|u+v\|\leq\|u\|+\|v\|$.

#### Reverse triangle inequality

↑ **Parent:** [Triangle inequality](#triangle-inequality)

In a [metric space](#metric-space), applying the [triangle inequality](#triangle-inequality) in both directions gives $|d(x,z)-d(y,z)|\leq d(x,y)$. In a [normed vector space](functional-analysis.md#normed-vector-space), its corresponding form is $|\|x\|-\|y\||\leq\|x-y\|$. In particular, distance to a fixed point is a [Lipschitz continuous](real-analysis.md#lipschitz-continuity) real function.

##### Four-point triangle inequality

↑ **Parent:** [Reverse triangle inequality](#reverse-triangle-inequality)

For four points $x_1,x_2,y_1,y_2$ in a [metric space](#metric-space),

$$
d(x_1,y_1)-d(x_1,y_2)\leq d(y_1,y_2)\leq d(x_2,y_1)+d(x_2,y_2).
$$

Both steps follow from the [triangle inequality](#triangle-inequality). The first also holds with an absolute value around the difference, by the [reverse triangle inequality](#reverse-triangle-inequality). This transports a difference of distances measured from one point into a sum measured from another.

#### Triangle inequality for a vector-valued integral

↑ **Parent:** [Triangle inequality](#triangle-inequality)

For an integrable function $f$ with values in a finite-dimensional normed vector space,

$$
\left\|\int f\right\|\leq\int\|f\|.
$$

For the Euclidean norm, pair the integral with a unit vector in its direction and apply the Cauchy-Schwarz inequality pointwise.

#### Equality condition in the complex triangle inequality

↑ **Parent:** [Triangle inequality](#triangle-inequality)

For nonzero [complex numbers](complex-analysis.md#complex-number) $x,y$, equality $|x+y|=|x|+|y|$ holds exactly when $x/y$ is a positive real number, equivalently when the two numbers have the same [complex argument](complex-analysis.md#argument-complex-analysis) modulo $2\pi$.

#### Integral triangle inequality

↑ **Parent:** [Triangle inequality](#triangle-inequality)

For every integrable real or complex function,

$$
\left|\int f\,d\mu\right|\leq\int|f|\,d\mu.
$$

### Euclidean distance

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_distance)

The Euclidean distance between $x,y\in\mathbb R^d$ is

$$
\|x-y\|_2=\sqrt{\sum_{i=1}^d(x_i-y_i)^2}.
$$

#### Standardized Euclidean distance

↑ **Parent:** [Euclidean distance](#euclidean-distance)

With fixed positive scale estimates $s_j$, this is [Euclidean distance](#euclidean-distance) in standardized coordinates. It removes marginal units but ignores correlations. Small estimated [variances](variance.md) can greatly amplify measurement noise; a zero scale must be handled separately.

### Diameter

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diameter)

The diameter of a subset $S$ of a metric space is

$$
\operatorname{diam}(S)=\sup\{d(x,y):x,y\in S\}.
$$

The diameter of a nonempty subset $S$ of a [metric space](#metric-space) is $\operatorname{diam}(S)=\sup\{d(x,y):x,y\in S\}$. For a Euclidean circle it is the longest chord length; the same definition applies to arbitrary metric subsets.

### Uniform continuity

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_continuity)

Uniform continuity requires one input tolerance to work at every point of the domain for a chosen output tolerance.

#### Uniformly continuous integrable dissipation tends to zero

↑ **Parent:** [Uniform continuity](#uniform-continuity)

Suppose $d$ is nonnegative, integrable and [uniformly continuous](#uniform-continuity) on the positive half-line. If $d(t_n)\geq\epsilon>0$ at times tending to infinity, [uniform continuity](#uniform-continuity) supplies intervals of one fixed positive length around those times on which $d\geq\epsilon/2$. An infinite disjoint subsequence of these intervals contradicts integrability. Thus the displayed implication holds. Mere smoothness at every finite time is insufficient: smooth peaks of shrinking widths can have finite integral and heights bounded away from zero.

#### Uniformly continuous function on a totally bounded set is bounded

↑ **Parent:** [Uniform continuity](#uniform-continuity)

Choose the [uniform continuity](#uniform-continuity) input tolerance corresponding to output tolerance one. A [totally bounded](#totally-bounded-space) domain is covered by finitely many balls of smaller radius centred in the domain. Every function value differs by less than one from the value at one of their finitely many centres. Taking the largest centre value bounds the whole function. Compactness or closedness of the domain is unnecessary.

#### Products of unbounded uniformly continuous functions

↑ **Parent:** [Uniform continuity](#uniform-continuity)

A product of two [uniformly continuous](#uniform-continuity) functions need not have [uniform continuity](#uniform-continuity) on an unbounded domain. The functions $f(x)=g(x)=x$ give the counterexample $x^2$, since inputs $n$ and $n+1/n$ approach each other while their squared values remain separated. For bounded factors the estimate $|f(x)g(x)-f(y)g(y)|\le\|f\|_\infty|g(x)-g(y)|+\|g\|_\infty|f(x)-f(y)|$ restores uniform continuity.

#### Uniformly continuous integrable functions vanish at infinity

↑ **Parent:** [Uniform continuity](#uniform-continuity)

If a [uniformly continuous function](calculus.md#uniformly-continuous-function) $u:\mathbb R^d\to\mathbb R$ belongs to [Lp space](measure-theory.md#lp-space) for some $1\leq p<\infty$, then $u(x)\to0$ as $|x|\to\infty$. Otherwise choose points escaping to infinity with $|u(x_j)|\geq2\theta>0$. [Uniform continuity](#uniform-continuity) gives one radius $\rho>0$ on which $|u|\geq\theta$ around every $x_j$. Extract disjoint such balls. Their contributions to $\int|u|^p$ are each at least $\theta^p|B_\rho|$, a contradiction. The finite-$p$ condition is essential: the constant function one lies in $W^{1,\infty}$ and does not vanish at infinity.

#### Pointwise approximation by uniformly continuous functions

↑ **Parent:** [Uniform continuity](#uniform-continuity)

Every continuous $f:\mathbb R\to\mathbb R$ can be approximated with [pointwise convergence](real-analysis.md#pointwise-convergence) by [uniformly continuous](#uniform-continuity) functions. Set $c_n(x)=\max(-n,\min(x,n))$ and $f_n=f\circ c_n$. The map $c_n$ is [Lipschitz continuous](real-analysis.md#lipschitz-continuity) with constant one and $f|_{[-n,n]}$ is [uniformly continuous](#uniform-continuity) by the [Heine-Cantor theorem](#heine-cantor-theorem), so $f_n$ is [uniformly continuous](#uniform-continuity) on the whole line. On every fixed bounded interval, $f_n=f$ eventually.

#### Modulus of continuity

↑ **Parent:** [Uniform continuity](#uniform-continuity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modulus_of_continuity)

The modulus of continuity of a function $f$ is

$$
\omega(f,\delta)=\sup\{|f(x)-f(y)|:d(x,y)\leq\delta\}.
$$

It quantifies [uniform continuity](#uniform-continuity) by recording the largest oscillation of $f$ across pairs of points at distance at most $\delta$.

##### Log-Lipschitz modulus

↑ **Parent:** [Modulus of continuity](#modulus-of-continuity)

Set $\mu(0)=0$ and extend $\mu(r)=1$ for $r\geq1$. This positive, nondecreasing [modulus of continuity](#modulus-of-continuity) is weaker than a linear [Lipschitz continuity](real-analysis.md#lipschitz-continuity) bound but still has $\int_0^1dr/\mu(r)=\infty$. At small distances it is equivalent to $r\log(1/r)$. A signed $r\log r$ cannot be an upper modulus at distances less than one. The [planar vorticity velocity kernel](fluid-mechanics.md#planar-vorticity-velocity-kernel) maps $L^1\cap L^\infty$ into velocity fields with this modulus.

#### Heine-Cantor theorem

↑ **Parent:** [Uniform continuity](#uniform-continuity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heine–Cantor_theorem)

Every continuous map from a compact metric space to a metric space is uniformly continuous.

#### Uniform limit theorem for uniformly continuous functions

↑ **Parent:** [Uniform continuity](#uniform-continuity)

A uniform limit of uniformly continuous maps between metric spaces is uniformly continuous. Approximate the limit at both endpoints by one fixed member of the sequence and use its uniform continuity between them.

#### Sequential criterion for uniform continuity

↑ **Parent:** [Uniform continuity](#uniform-continuity)

A function between metric spaces is uniformly continuous exactly when $d(x_n,y_n)\to0$ implies $d(f(x_n),f(y_n))\to0$ for every two sequences $(x_n)$ and $(y_n)$. Failure of uniform continuity supplies pairs with input distance below $1/n$ but output distance bounded below.

### Equivalence of metrics

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivalence_of_metrics)

Two metrics are equivalent when they induce the same topology. Global two-sided constant bounds imply equivalence, but equivalence alone need not supply such bounds.

#### Equivalent metrics need not be bi-Lipschitz equivalent

↑ **Parent:** [Equivalence of metrics](#equivalence-of-metrics)

On $\mathbb R$, the usual metric and $|\arctan x-\arctan y|$ induce the same topology, but their ratio along $(0,n)$ tends to zero. Thus no positive global lower comparison constant exists.

#### Equivalent codomain metrics need not preserve uniform convergence

↑ **Parent:** [Equivalence of metrics](#equivalence-of-metrics)

Topological equivalence does not determine uniform convergence. For the usual and arctangent metrics on $\mathbb R$, maps that change the value $n$ to $2n$ at a single domain point have arctangent sup-error tending to zero while their usual sup-error diverges.

### Distance to a set

↑ **Parent:** [Metric space](#metric-space)

For a metric space, $d(x,S)=\inf_{s\in S}d(x,s)$ is $1$-Lipschitz and vanishes on the closure of $S$.

#### Distance between two sets

↑ **Parent:** [Distance to a set](#distance-to-a-set)

The set distance is the infimum of pairwise [metric](#metric) distances. Two nonempty disjoint [compact sets](topology.md#compact-space) have positive set distance: continuity attains the minimum on their [Cartesian product](set-theory.md#cartesian-product), and a zero minimum would give a common point. Disjoint closed sets without compactness need not have positive separation.

### Isolated point

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isolated_point)

A point $x$ of a metric space is isolated when some open ball about $x$ contains no other point of the space, equivalently when the singleton $\{x\}$ is open.

### Complete metric space

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_metric_space)

A metric space is complete when every Cauchy sequence converges to a point of the space.

#### Cauchy-sequence construction of a metric completion

↑ **Parent:** [Complete metric space](#complete-metric-space)

For two [Cauchy sequences](real-analysis.md#cauchy-sequence), $|d(x_n,y_n)-d(x_m,y_m)|\leq d(x_n,x_m)+d(y_n,y_m)$, so the displayed limit exists. It defines a [pseudometric](#pseudometric) on the Cauchy sequences, and its [metric quotient](#metric-quotient-of-a-pseudometric) identifies sequences whose mutual distance tends to zero. Constant sequences embed the original [metric space](#metric-space) isometrically. Their image is dense, because the class of $(x_n)$ is approached by the constant classes of $x_n$. The quotient is complete: from a Cauchy sequence of its points select a subsequence whose successive distances are below $2^{-j}$ and choose original-space points within $2^{-j}$ of these subsequence points. Those original-space points form a Cauchy sequence and its class is the limit of the subsequence, hence of the whole sequence. The original embedding is onto exactly when the original space is complete.

#### Topological completeness

↑ **Parent:** [Complete metric space](#complete-metric-space)

A metrizable space is topologically complete when some [metric](#metric) inducing its topology is complete. The given [metric](#metric) need not be complete: the open interval $(0,1)$ is an example. A [Polish space](#polish-space) additionally requires separability.

##### G-delta criterion for topological completeness

↑ **Parent:** [Topological completeness](#topological-completeness)

A subspace of a complete [metric space](#metric-space) admits a compatible complete [metric](#metric) if and only if it is a [G-delta set](topology.md#g-delta-set). For the reverse direction, adjoining the coordinates $1/d(x,X\setminus U_n)$ to the ambient [metric](#metric) prevents Cauchy sequences from approaching any excluded closed boundary. For the forward direction, small-diameter relative open covers in a compatible complete [metric](#metric) produce the ambient open sets.

#### Polish space

↑ **Parent:** [Complete metric space](#complete-metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polish_space)

A Polish space is a [topological space](topology.md#topological-space) whose topology can be induced by a complete separable metric. The completeness requirement concerns some compatible metric; it need not hold for every metric inducing the topology. Euclidean spaces are examples.

##### Tree on a Polish space

↑ **Parent:** [Polish space](#polish-space)

A tree on $P$ is a subset of $\bigcup_{n\geq0}P^n$ closed under initial segments. It is closed when each finite level is closed in the corresponding product topology, and well-founded when it has no infinite branch. A countable-basis approximation tree, with nested sets of shrinking diameter, reduces a closed well-founded tree on a [Polish space](#polish-space) to a countable well-founded tree and bounds its height by a countable ordinal.

<h4 id="cantor-s-intersection-theorem">Cantor's intersection theorem</h4>

↑ **Parent:** [Complete metric space](#complete-metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor's_intersection_theorem)

A metric space is complete if and only if every decreasing sequence of nonempty closed sets whose diameters tend to zero has nonempty intersection. In that case the intersection contains exactly one point.

#### Baire category theorem

↑ **Parent:** [Complete metric space](#complete-metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baire_category_theorem)

Every complete metric space is a Baire space: every countable intersection of open dense subsets is dense. Equivalently, no nonempty open subset is a countable union of nowhere-dense subsets.

To prove the dense-intersection form, let $V$ be nonempty and open and let $G_1,G_2,\ldots$ be open dense sets. Successively choose closed balls

$$
\overline B(x_n,r_n)\subset B(x_{n-1},r_{n-1})\cap G_n,
\qquad 0<r_n<2^{-n},
$$

starting with a ball contained in $V\cap G_1$. The centres form a Cauchy sequence. Its limit belongs to every closed ball, and hence to $V\cap\bigcap_nG_n$.

##### Baire avoidance of countably many affine hyperplanes

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

Every proper [affine hyperplane](vector-space.md#affine-hyperplane) in $\mathbb R^n$ is closed and has empty interior: a small displacement along its nonzero normal vector leaves it. The [Baire category theorem](#baire-category-theorem) therefore makes the complement of a countable collection of such hyperplanes dense. In particular, avoiding the hyperplanes $\sum_{j=1}^n k_jx_j=k_{n+1}$ for nonzero integer tuples yields a vector for which $1,x_1,\ldots,x_n$ are linearly independent over $\mathbb Q$. Tuples with all the first $n$ entries zero define an empty forbidden set.

##### Local uniform Cauchy control for pointwise convergent continuous functions

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

Suppose [continuous functions](calculus.md#continuous-function) $f_n:\mathbb R\to\mathbb R$ converge [pointwise](real-analysis.md#pointwise-convergence) to $f$. For each $\epsilon>0$, some nonempty [open interval](topology.md#open-interval) $I$ and integer $N$ satisfy $|f_n(x)-f(x)|\leq\epsilon$ for every $x\in I$ and $n\geq N$. Indeed the [closed sets](topology.md#closed-set) $Q_N=\bigcap_{n,m\geq N}\{|f_n-f_m|\leq\epsilon\}$ cover $\mathbb R$. The [Baire category theorem](#baire-category-theorem) gives an interval inside one $Q_N$, and passing $m\to\infty$ proves the assertion. The interval may depend on $\epsilon$; this does not assert [uniform convergence](real-analysis.md#uniform-convergence) on one fixed interval.

##### Residual set

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

A set containing a countable intersection of open dense subsets. The intersection itself is also called a residual set. In a [Baire space](#baire-space) it is dense. This topological notion of genericity does not by itself assert full measure.

##### Comeagre subgroup completeness argument

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

A dense additive subgroup of a complete metrizable topological group cannot be proper if it is [comeagre](#comeagre-set). Every translate is comeagre and meets the subgroup, so every translating element is a difference of two subgroup elements. Applied to a [topologically complete](#topological-completeness) normed space inside its completion, this proves that its original norm is complete.

##### Banach space has uncountable Hamel dimension

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

No infinite-dimensional [Banach space](banach-space.md) has a countable [Hamel basis](vector-space.md#basis). If $(e_n)$ were such a basis, the space would be the countable union of the finite-dimensional subspaces $\operatorname{span}(e_1,\ldots,e_n)$. Each is closed and has empty interior, contradicting the [Baire category theorem](#baire-category-theorem).

##### Nowhere differentiable continuous function

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

A nowhere differentiable continuous function is continuous at every point and has no finite derivative anywhere. A Baire-category argument shows that such functions form a dense subset of $C([0,1])$ in the [uniform norm](functional-analysis.md#supremum-norm).

##### Baire space

↑ **Parent:** [Baire category theorem](#baire-category-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baire_space)

A Baire space is a topological space in which every countable intersection of open dense sets is dense, equivalently one in which no nonempty open set is a countable union of nowhere-dense sets. Every compact Hausdorff space and every complete metric space is a Baire space.

###### Baire function

↑ **Parent:** [Baire space](#baire-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baire_function)

A Baire function belongs to the smallest hierarchy of real-valued functions containing the continuous functions and closed under pointwise sequential limits.

###### Baire class one function

↑ **Parent:** [Baire function](#baire-function)

A Baire class one function is a pointwise limit of [continuous functions](calculus.md#continuous-function). On a complete metric domain, its set of discontinuities is meagre; in particular, it has a point of continuity on every nonempty perfect closed subset.

###### Rationality indicator is not Baire class one

↑ **Parent:** [Baire class one function](#baire-class-one-function)

The indicator of the [rational numbers](number-theory.md#rational-number) in the [real numbers](arithmetic.md#real-number) is discontinuous everywhere because both the rationals and irrationals are dense. The discontinuity theorem for [Baire class one functions](#baire-class-one-function) therefore shows that it is not Baire class one.

##### Closed convex absorbing set has an origin neighbourhood

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

Let $S$ be a nonempty closed, convex, symmetric subset of a Banach space and suppose $\bigcup_{n\geq1}nS=X$. Baire's theorem puts a ball $B(x,r)$ inside some $nS$. Symmetry also puts $B(-x,r)$ there, and convexity puts the midpoint of $x+z$ and $-x+z$, namely $z$, in $nS$ whenever $\|z\|<r$. Hence $B(0,r/n)\subset S$.

###### Closed symmetric absorbing set without an origin neighbourhood

↑ **Parent:** [Closed convex absorbing set has an origin neighbourhood](#closed-convex-absorbing-set-has-an-origin-neighbourhood)

Convexity is essential. In $\mathbb R$, let

$$
S=\{0\}\cup\bigcup_{k\geq0}
\{x:4^{-k}\leq|x|\leq2\cdot4^{-k}\}.
$$

This set is closed, symmetric, and has gaps arbitrarily near zero. Given $x\ne0$, choose $k$ so small-scale that the interval  
$[|x|/(2\cdot4^{-k}),|x|/4^{-k}]$ has length at least one; it contains an integer $n$, and then $x/n\in S$. Thus $\bigcup_n nS=\mathbb R$, although $S$ is not a neighbourhood of zero.

##### Isolated points in a countable complete metric space

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

Every nonempty countable complete metric space has an [isolated point](#isolated-point). Otherwise it is the countable union of its singleton subsets, each of which is nowhere dense, contradicting the [Baire category theorem](#baire-category-theorem).

If such a space has infinitely many points, it has infinitely many isolated points. Indeed, after deleting any finite collection of isolated points, the remaining set is closed, complete, countable, and nonempty. It therefore has a point isolated in the remaining space; because the deleted set is finite, that point is also isolated in the original space.

##### Nowhere dense set

↑ **Parent:** [Baire category theorem](#baire-category-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nowhere_dense_set)

A subset $A$ of a topological space is nowhere dense when the interior of its closure is empty. Equivalently, every nonempty open set contains a nonempty open subset disjoint from $A$.

##### Meagre set

↑ **Parent:** [Baire category theorem](#baire-category-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Meagre_set)

A meagre, or first-category, set is a countable union of [nowhere dense sets](#nowhere-dense-set).

###### Luzin set

↑ **Parent:** [Meagre set](#meagre-set)

An uncountable [subset](set.md#subset) of the [real numbers](arithmetic.md#real-number) with countable intersection with every [meagre set](#meagre-set). This is the category counterpart of a [Sierpiński set](measure-theory.md#sierpinski-set).

###### Comeagre set

↑ **Parent:** [Meagre set](#meagre-set)

The complement of a comeagre set is a [meagre set](#meagre-set), a countable union of nowhere dense sets. A dense [G-delta set](topology.md#g-delta-set) is comeagre. The [Baire category theorem](#baire-category-theorem) ensures that two comeagre subsets of a nonempty complete [metric](#metric) space cannot be disjoint.

###### Lusin set

↑ **Parent:** [Meagre set](#meagre-set)

A Lusin set is an uncountable [subset](set.md#subset) $A$ of the [real numbers](arithmetic.md#real-number) such that $A\cap M$ is countable for every [meagre set](#meagre-set) $M$. Every meagre subset has a meagre $F_\sigma$ cover, so testing those covers suffices. The [Lusin set construction under CH](#lusin-set-construction-under-ch) gives an example. A Lusin set has no uncountable meagre subset of itself.

###### Lusin set construction under CH

↑ **Parent:** [Lusin set](#lusin-set)

Under the [Continuum hypothesis](set-theory.md#continuum-hypothesis), enumerate the meagre $F_\sigma$ covers by $\omega_1$. At stage $\alpha$ choose a new real outside all earlier covers and the previous choices. The excluded union is meagre, so the [Baire category theorem](#baire-category-theorem) makes the choice possible. Each cover then contains only countably many selected points. Arbitrary [meagre sets](#meagre-set) need not themselves have only continuum many possible choices; the coded covers are what is enumerated.

##### Generic nowhere-monotone continuous function

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

In $C([0,1])$ with the uniform norm, the continuous functions that are monotone on some interval of positive length form a [meagre set](#meagre-set). Indeed, it is enough to use intervals with rational endpoints. For each such interval, the nondecreasing and nonincreasing functions form closed sets with empty interior: a sufficiently small local triangular perturbation breaks the relevant inequality. The [Baire category theorem](#baire-category-theorem) therefore shows that a dense set of continuous functions is monotone on no nontrivial interval.

##### Smooth function with a pointwise vanishing derivative

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

Let $f\in C^\infty(\mathbb R)$ and suppose that for every $x$ there is an $n=n(x)\geq0$ such that $f^{(n)}(x)=0$. Then $f$ is a polynomial.

##### Nonpolynomial entire function has a centre with no zero Taylor coefficient

↑ **Parent:** [Baire category theorem](#baire-category-theorem)

If an [entire function](complex-analysis.md#entire-function) $f$ is not a [polynomial](polynomial.md), then there is a point $z_0\in\mathbb C$ for which $f^{(n)}(z_0)\ne0$ for every nonnegative integer $n$. Consequently every coefficient in the [Taylor series](calculus.md#taylor-series) of $f$ about $z_0$ is nonzero.

For each $n$, the function $f^{(n)}$ is not identically zero, since otherwise $f$ would be a polynomial. Its zero set is closed and has empty interior by the [identity theorem](complex-analysis.md#identity-theorem), hence is a [nowhere dense set](#nowhere-dense-set). The [Baire category theorem](#baire-category-theorem) says that the [complete metric space](#complete-metric-space) $\mathbb C$ cannot be the union of these countably many zero sets.

Set $S_n=\{x:f^{(n)}(x)=0\}$ and $E_n=\operatorname{int}S_n$. The sets $S_n$ are closed, $E_n\subset E_{n+1}$, and Baire's theorem on each interval shows that $\Omega=\bigcup_nE_n$ is dense. On every connected component of $\Omega$, compactness and the increasing cover by the $E_n$ show that one derivative vanishes locally with a uniform finite order, so $f$ agrees there with one polynomial.

If $F=\mathbb R\setminus\Omega$ were nonempty, it would be closed and have no isolated points: polynomial pieces on both sides of an isolated point would have matching derivatives of every order and hence join into one polynomial piece. Applying Baire's theorem to the cover $F=\bigcup_n(F\cap S_n)$ gives an interval $U$ and an index $k$ for which $F\cap U$ is nonempty and contained in $S_k$. Because $F$ has no isolated points, difference quotients show that every derivative of order at least $k$ vanishes on $F\cap U$. Each polynomial component of $\Omega$ meeting $U$ has an endpoint in $F\cap U$, so its degree is less than $k$. Thus $f^{(k)}=0$ throughout $U$, contradicting $F\cap U\ne\varnothing$. Hence $\Omega=\mathbb R$, and its sole connected component carries one polynomial.

#### Space of smooth functions on a compact interval

↑ **Parent:** [Complete metric space](#complete-metric-space)

The space $C^\infty([0,1])$ becomes a complete metric space under

$$
d(f,g)=\sum_{r=0}^\infty2^{-r}
\min\{1,\|f^{(r)}-g^{(r)}\|_\infty\}.
$$

Convergence in this metric is exactly uniform convergence of every derivative separately.

##### Completeness of the smooth-function metric

↑ **Parent:** [Space of smooth functions on a compact interval](#space-of-smooth-functions-on-a-compact-interval)

If $(f_n)$ is Cauchy in the smooth-function metric, each derivative sequence $(f_n^{(r)})$ converges uniformly to a continuous function $g_r$. Passing to the limit in

$$
f_n^{(r)}(x)-f_n^{(r)}(0)=\int_0^x f_n^{(r+1)}(t)\,dt
$$

shows that $g_r'=g_{r+1}$. Hence $g_0$ is smooth and $f_n\to g_0$ in the metric.

##### Generic superfactorial derivative growth at rational points

↑ **Parent:** [Space of smooth functions on a compact interval](#space-of-smooth-functions-on-a-compact-interval)

Outside a [meagre set](#meagre-set) in $C^\infty([0,1])$, every rational $q\in(0,1)$ and every positive integer $M$ admit $m\geq M$ such that

$$
|f^{(m)}(q)|>m!m^m.
$$

For fixed $q,M$, the union over $m\geq M$ of these strict-inequality sets is open. It is dense because a perturbation $\delta\cos(K(x-q)-m\pi/2)$ can make the $m$th derivative arbitrarily large while keeping any prescribed finite collection of lower derivatives arbitrarily small. The [Baire category theorem](#baire-category-theorem) applied over the countable pairs $(q,M)$ gives the claim.

###### Nowhere-analytic generic smooth function

↑ **Parent:** [Generic superfactorial derivative growth at rational points](#generic-superfactorial-derivative-growth-at-rational-points)

The generic derivative bound implies that at every rational $q\in(0,1)$,

$$
\limsup_m\left|\frac{f^{(m)}(q)}{m!}\right|^{1/m}=\infty.
$$

The [Cauchy-Hadamard theorem](real-analysis.md#cauchy-hadamard-theorem) therefore gives radius zero to the Taylor series at every such $q$. If a Taylor series represented $f$ on a neighborhood of any point, that neighborhood would contain a rational point at which $f$ was real analytic, a contradiction.

#### Closed-subspace completeness theorem

↑ **Parent:** [Complete metric space](#complete-metric-space)

A closed subspace of a complete metric space is complete. A Cauchy sequence in the subspace converges in the ambient space, and closedness keeps its limit in the subspace.

### Hausdorff distance

↑ **Parent:** [Metric space](#metric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hausdorff_distance)

For nonempty bounded subsets of a metric space,

$$
d_H(A,B)=\max\left\{
\sup_{a\in A}d(a,B),
\sup_{b\in B}d(b,A)
\right\}.
$$

This is a metric on the nonempty closed bounded subsets. Without closedness it is only a pseudometric: a set and its closure have distance zero.

#### Closed singleton embedding in a Hausdorff hyperspace

↑ **Parent:** [Hausdorff distance](#hausdorff-distance)

The map $x\mapsto\{x\}$ is an isometry into the hyperspace of nonempty closed bounded subsets. Its image is closed because a Hausdorff limit of singletons has diameter zero and is therefore a singleton.

##### Completeness is reflected by the Hausdorff hyperspace

↑ **Parent:** [Closed singleton embedding in a Hausdorff hyperspace](#closed-singleton-embedding-in-a-hausdorff-hyperspace)

If the Hausdorff hyperspace is complete, its closed subspace of singletons is complete. Since that subspace is isometric to the original metric space, the original space is complete as well.

#### Gromov-Hausdorff distance

↑ **Parent:** [Hausdorff distance](#hausdorff-distance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gromov-Hausdorff_distance)

For [compact metric spaces](#compact-metric-space) $X$ and $Y$, the Gromov-Hausdorff distance is

$$
d_{GH}(X,Y)=\inf_{Z,\varphi,\psi}d_H^Z(\varphi(X),\psi(Y)),
$$

where the [infimum](real-analysis.md#infimum) runs over all [metric spaces](#metric-space) $Z$ and all [isometric embeddings](riemannian-geometry.md#isometric-embedding) $\varphi:X\to Z$ and $\psi:Y\to Z$. It measures how closely the two spaces can be placed inside one ambient [metric space](#metric-space).

##### Gromov-Hausdorff topology

↑ **Parent:** [Gromov-Hausdorff distance](#gromov-hausdorff-distance)

The Gromov-Hausdorff topology on isometry classes of [compact metric spaces](#compact-metric-space) is the topology induced by the [Gromov-Hausdorff distance](#gromov-hausdorff-distance).

##### Real tree

↑ **Parent:** [Gromov-Hausdorff distance](#gromov-hausdorff-distance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real_tree)

A real tree is a [metric space](#metric-space) $(T,d)$ in which every pair $a,b\in T$ is joined by a unique arc and that arc is [isometric](riemannian-geometry.md#isometry) to the [real interval](real-analysis.md#interval-mathematics) $[0,d(a,b)]$. Equivalently, it is a [geodesic metric space](#geodesic-metric-space) with no nontrivial simple loops.

###### Multiplicity of a point in a real tree

↑ **Parent:** [Real tree](#real-tree)

The multiplicity of $a$ in a [real tree](#real-tree) $T$ is the number of [connected components](geometry-and-topology.md#connected-component) of $T\setminus\{a\}$. A point of multiplicity one is a leaf, one of multiplicity two lies in the interior of an unbranched arc, and one of multiplicity at least three is a branch point.

###### Real tree encoded by an excursion

↑ **Parent:** [Real tree](#real-tree)

Let $g:[0,1]\to\mathbb R_+$ be [continuous](calculus.md#continuous-function) with $g(0)=g(1)=0$, and set

$$
m_g(s,t)=\inf_{r\in[s\wedge t,s\vee t]}g(r),\qquad
d_g(s,t)=g(s)+g(t)-2m_g(s,t).
$$

The function $d_g$ is a [pseudometric](#pseudometric). Its metric quotient

$$
T_g=[0,1]/\{d_g=0\}
$$

is the real tree encoded by $g$.

###### Excursion coding theorem for compact real trees

↑ **Parent:** [Real tree encoded by an excursion](#real-tree-encoded-by-an-excursion)

Every compact [real tree](#real-tree) is [isometric](riemannian-geometry.md#isometry) to a [real tree encoded by an excursion](#real-tree-encoded-by-an-excursion). One construction takes finite subtrees spanning successively finer finite nets, performs depth-first contour traversals of those subtrees, and chooses compatible time parameterizations. The contour functions have a uniformly convergent subsequence, and continuity of excursion coding in the [Gromov-Hausdorff distance](#gromov-hausdorff-distance) identifies the limiting coded tree with the original tree.

## Equicontinuity

↑ **Parent:** [Topological analysis](topological-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equicontinuity)

A family $\mathcal F$ of maps between metric spaces is equicontinuous when, near each point, one input tolerance controls the output variation uniformly for every $f\in\mathcal F$. Uniform equicontinuity uses one input tolerance over the whole domain.

A family $\mathcal F$ of maps between [metric spaces](#metric-space) is equicontinuous at $x$ when, for every $\varepsilon>0$, one $\delta>0$ works for all $f\in\mathcal F$: $d(x,y)<\delta$ implies $d(f(x),f(y))<\varepsilon$.

### Uniformly bounded family of functions

↑ **Parent:** [Equicontinuity](#equicontinuity)

A family $\mathcal F$ of scalar-valued functions is uniformly bounded when one constant $M$ satisfies $|f(x)|\leq M$ for every $f\in\mathcal F$ and every point $x$ in their common domain.

### Pointwise bounded family of functions

↑ **Parent:** [Equicontinuity](#equicontinuity)

A family $\mathcal F$ of scalar-valued functions on $X$ is pointwise bounded when $\sup_{f\in\mathcal F}|f(x)|<\infty$ for every fixed $x\in X$; the bound may depend on $x$.

<h3 id="arzela-ascoli-theorem">Arzelà-Ascoli theorem</h3>

↑ **Parent:** [Equicontinuity](#equicontinuity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arzelà–Ascoli_theorem)

For a compact Hausdorff space $K$, a subset of $C(K)$ is relatively compact in the uniform norm exactly when it is [equicontinuous](#equicontinuity) and pointwise bounded. On a compact metric space, this says that every uniformly bounded equicontinuous sequence has a uniformly convergent subsequence.

#### Nonlinear ODE bounds from interior extrema

↑ **Parent:** [Arzelà-Ascoli theorem](#arzela-ascoli-theorem)

If a thrice differentiable solution has both endpoint values and both endpoint first derivatives bounded in modulus by $N$, it obeys $|f|\leq N$ and $|f'|\leq N$ throughout the interval. A positive interior maximum of $f$ would give $f''=f>0$, and a negative interior minimum would give $f''=f<0$, both impossible. For $w=f'$, differentiation gives $w''=w+2ww'$, so the same argument applies at an extremum of $w$. The resulting uniform bound and Lipschitz constant imply total boundedness of the solution family by the [Arzelà-Ascoli theorem](#arzela-ascoli-theorem).

#### Relatively compact subset

↑ **Parent:** [Arzelà-Ascoli theorem](#arzela-ascoli-theorem)

A subset of a topological space is relatively compact when its closure is compact.

#### Diagonal subsequence for locally uniform convergence

↑ **Parent:** [Arzelà-Ascoli theorem](#arzela-ascoli-theorem)

If successive subsequences converge uniformly on an exhaustion $K_1\subset K_2\subset\cdots$, the diagonal sequence converges uniformly on every fixed $K_m$, hence locally uniformly on their union.

##### Escaping bump counterexample to global uniform convergence

↑ **Parent:** [Diagonal subsequence for locally uniform convergence](#diagonal-subsequence-for-locally-uniform-convergence)

For a compactly supported nonzero function $\psi$, the translates $f_n(x)=\psi(x-n)$ converge uniformly to zero on every compact subset of $\mathbb R$, while $\lVert f_n\rVert_\infty=\lVert\psi\rVert_\infty$ prevents uniform convergence on all of $\mathbb R$.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
