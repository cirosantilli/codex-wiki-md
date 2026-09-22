# Weak topology

↑ **Parent:** [Functional analysis](functional-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_topology)

The weak topology $\sigma(X,X^*)$ on a normed space $X$ is the coarsest topology making every member of $X^*$ continuous. A net converges weakly exactly when every bounded linear functional converges on it.

**Table of contents**

- [Original and weak continuity of linear maps between Fréchet spaces](#original-and-weak-continuity-of-linear-maps-between-frechet-spaces)
- [Countable separating family metrizes a weakly compact set](#countable-separating-family-metrizes-a-weakly-compact-set)
- [Weakly bounded set](#weakly-bounded-set)
- [Weak and norm Borel sigma-algebras in a separable Banach space](#weak-and-norm-borel-sigma-algebras-in-a-separable-banach-space)
- [Weak convergence](#weak-convergence)
  - [Concentration prevents weak compactness in L1](#concentration-prevents-weak-compactness-in-l1)
  - [Radon-Riesz property](#radon-riesz-property)
- [Finite-dimensional weak and norm topologies coincide](#finite-dimensional-weak-and-norm-topologies-coincide)
- [Weakly convergent sequence is bounded](#weakly-convergent-sequence-is-bounded)
- [Metrization of the weak topology on a bounded set](#metrization-of-the-weak-topology-on-a-bounded-set)
  - [Weak-ball metrizability requires a norm-separable dual](#weak-ball-metrizability-requires-a-norm-separable-dual)
- [Weak closure](#weak-closure)
- [Weakly null sequence](#weakly-null-sequence)
  - [Standard unit vectors are weakly null in lp](#standard-unit-vectors-are-weakly-null-in-lp)
  - [Weak convergence of bounded disjointly supported sequences in lp](#weak-convergence-of-bounded-disjointly-supported-sequences-in-lp)
- [Weakly Cauchy sequence](#weakly-cauchy-sequence)
- [Weak closure of the unit sphere](#weak-closure-of-the-unit-sphere)
- [Weak-star topology](#weak-star-topology)
  - [Weak-star fixed point theorem for an adjoint operator](#weak-star-fixed-point-theorem-for-an-adjoint-operator)
  - [Weak-star separability of the entire dual](#weak-star-separability-of-the-entire-dual)
  - [Weak-star open dual ball category obstruction](#weak-star-open-dual-ball-category-obstruction)
  - [Weak-star topology on an entire infinite-dimensional Banach dual is not metrizable](#weak-star-topology-on-an-entire-infinite-dimensional-banach-dual-is-not-metrizable)
  - [Continuous dual of a weak-star topology](#continuous-dual-of-a-weak-star-topology)
  - [Failure of weak-star convergence to commute with squaring](#failure-of-weak-star-convergence-to-commute-with-squaring)
  - [Weak-star metrizability of the dual ball](#weak-star-metrizability-of-the-dual-ball)
    - [Weak-star metrizability criterion for a dual ball](#weak-star-metrizability-criterion-for-a-dual-ball)
  - [Grothendieck space](#grothendieck-space)
  - [Szlenk derivation](#szlenk-derivation)
    - [One-step Szlenk derivation for a separable dual](#one-step-szlenk-derivation-for-a-separable-dual)
- [Weakly compact set](#weakly-compact-set)
  - [Discontinuous pointwise limit obstruction to weak compactness](#discontinuous-pointwise-limit-obstruction-to-weak-compactness)
  - [Weakly compact subsets of l-infinity are norm separable](#weakly-compact-subsets-of-l-infinity-are-norm-separable)
  - [Weakly compact set is norm bounded](#weakly-compact-set-is-norm-bounded)
  - [Weakly sequentially compact set](#weakly-sequentially-compact-set)
    - [Eberlein-Šmulian theorem](#eberlein-smulian-theorem)
  - [Krein-Šmulian theorem](#krein-smulian-theorem)
- [Szlenk index](#szlenk-index)

<h2 id="original-and-weak-continuity-of-linear-maps-between-frechet-spaces">Original and weak continuity of linear maps between Fréchet spaces</h2>

↑ **Parent:** [Weak topology](weak-topology.md)

For [Fréchet spaces](topological-vector-space.md#frechet-space), the two continuity conditions for a [linear map](vector-space.md#linear-map) are equivalent. Original continuity makes every target [continuous linear functional](topological-vector-space.md#continuous-linear-functional) compose to a source [continuous linear functional](topological-vector-space.md#continuous-linear-functional), proving weak continuity. Conversely, weak continuity makes these compositions continuous in the original source [topology](topology.md). They separate target points, so limits in the [graph of a linear operator](functional-analysis.md#graph-of-a-linear-operator) remain in the graph. The [closed graph theorem for Fréchet spaces](functional-analysis.md#closed-graph-theorem-for-frechet-spaces) finishes the proof.

Without the hypotheses, equal [continuous dual spaces](continuous-dual-space.md) do not imply equal [topologies](topology.md). The identity from an infinite-dimensional [Hilbert space](hilbert-space.md) with its [weak topology](weak-topology.md) to its norm [topology](topology.md) is weak-to-weak continuous but not continuous in those original [topologies](topology.md).

## Countable separating family metrizes a weakly compact set

↑ **Parent:** [Weak topology](weak-topology.md)

If a countable family in $X^*$ separates points of $X$, the displayed metric induces the [weak topology](weak-topology.md) on every [weakly compact set](#weakly-compact-set) $K$. The coordinate map into the countable product of scalar lines is continuous and injective; a continuous injection from a compact space into a Hausdorff space is a homeomorphism onto its image. Equivalently, uniform convergence of the metric series makes the identity from weak $K$ to metric $K$ continuous. Compactness is essential: point separation alone need not generate the weak topology on an arbitrary bounded set.

## Weakly bounded set

↑ **Parent:** [Weak topology](weak-topology.md)

A subset $D$ of a [normed vector space](functional-analysis.md#normed-vector-space) is weakly bounded when $\sup_{x\in D}|f(x)|<\infty$ for every $f\in X^*$. It is norm bounded: its [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual) is a pointwise bounded family of functionals on the complete [continuous dual space](continuous-dual-space.md), so the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) applies. The converse is immediate. A [weakly compact set](#weakly-compact-set) is weakly bounded because each scalar evaluation has compact image.

## Weak and norm Borel sigma-algebras in a separable Banach space

↑ **Parent:** [Weak topology](weak-topology.md)

The [weak topology](weak-topology.md) and [norm topology](functional-analysis.md#norm-topology) of a [separable Banach space](banach-space.md#separable-banach-space) generate the same [Borel sigma-algebra](measure-theory.md#borel-sigma-algebra). A [countable norming family](functional-analysis.md#countable-norming-family) makes every norm ball weakly Borel measurable, and separability makes every norm-open set a countable union of such balls. The reverse inclusion follows because the [weak topology](weak-topology.md) is coarser.

## Weak convergence

↑ **Parent:** [Weak topology](weak-topology.md)

A sequence $x_n$ converges weakly to $x$ when $f(x_n)\to f(x)$ for every $f$ in the [continuous dual space](continuous-dual-space.md) $X^*$.

### Concentration prevents weak compactness in L1

↑ **Parent:** [Weak convergence](#weak-convergence)

The nonnegative [Lp space](measure-theory.md#lp-space) functions $f_j$ have $L^1$ norm one. Any weak limit tested against indicators supported outside the origin must vanish almost everywhere. Testing against the constant bounded function one would nevertheless require integral one. This contradiction applies to every subnet whose indices tend to infinity, so the $L^1$ unit ball is not weakly compact. The abstract [Banach-Alaoglu theorem](functional-analysis.md#banach-alaoglu-theorem) remains valid: weak compactness of the $L^1$ unit ball is a different assertion from weak-star compactness of a dual ball.

### Radon-Riesz property

↑ **Parent:** [Weak convergence](#weak-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radon–Riesz_property)

A [normed vector space](functional-analysis.md#normed-vector-space) has the Radon-Riesz property when [weak convergence](#weak-convergence) $u_k\rightharpoonup u$ together with $\|u_k\|\to\|u\|$ implies [strong convergence](functional-analysis.md#norm-convergence) $u_k\to u$. The Hilbert-space case is the [Radon-Riesz theorem](hilbert-space.md#radon-riesz-theorem). The condition prevents norm from remaining in weakly invisible directions.

## Finite-dimensional weak and norm topologies coincide

↑ **Parent:** [Weak topology](weak-topology.md)

On a [finite-dimensional vector space](vector-space.md#finite-dimensional-vector-space) equipped with a [norm](functional-analysis.md#norm), the [weak topology](weak-topology.md) and [norm topology](functional-analysis.md#norm-topology) coincide. The weak topology is no finer because every element of the dual is norm-continuous. Conversely, finitely many coordinate functionals in a basis control the norm, so every sufficiently small basic weak neighbourhood lies in a prescribed norm ball.

## Weakly convergent sequence is bounded

↑ **Parent:** [Weak topology](weak-topology.md)

Every [weakly convergent](#weak-convergence) sequence in a [normed vector space](functional-analysis.md#normed-vector-space) is a [bounded sequence](real-analysis.md#bounded-sequence). Apply the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) on the Banach space $X^*$ to the evaluation maps $Jx_n:f\mapsto f(x_n)$. They are pointwise bounded, while the [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual) gives $\lVert Jx_n\rVert=\lVert x_n\rVert$.

## Metrization of the weak topology on a bounded set

↑ **Parent:** [Weak topology](weak-topology.md)

Let $X^*$ have a norm-dense sequence $(\phi_m)$, and let $B\subset X$ be norm-bounded. Then

$$
d(x,y)=\sum_{m=1}^{\infty}2^{-m}
\frac{|\phi_m(x-y)|}{1+|\phi_m(x-y)|}
$$

is a metric on $B$ that induces its weak topology. Density lets convergence against the $\phi_m$ extend uniformly on $B-B$ to convergence against every $\phi\in X^*$.

### Weak-ball metrizability requires a norm-separable dual

↑ **Parent:** [Metrization of the weak topology on a bounded set](#metrization-of-the-weak-topology-on-a-bounded-set)

If the relative [weak topology](weak-topology.md) on the unit ball of a [normed vector space](functional-analysis.md#normed-vector-space) is first countable at zero, choose a countable collection of finite families of [continuous linear functionals](topological-vector-space.md#continuous-linear-functional) defining a local base. For any $f\in E'$ and $\epsilon>0$, one family $F$ has common kernel $M$ on which $\|f|_M\|\leq\epsilon$. Extend that restriction to $h\in E'$ with $\|h\|\leq\epsilon$ using the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem). Then $f-h$ vanishes on $M$, so it belongs to $\operatorname{span}F$ by finite-dimensional factorization. Consequently the countable union of these families has norm-dense linear span in $E'$. The converse is the [metrization of the weak topology on a bounded set](#metrization-of-the-weak-topology-on-a-bounded-set) construction from a norm-dense sequence in $E'$. In particular, separability of $E$ alone does not suffice: $\ell^1$ has nonseparable dual $\ell^\infty$.

## Weak closure

↑ **Parent:** [Weak topology](weak-topology.md)

The weak closure $\overline K^w$ of $K$ is its closure in the [weak topology](weak-topology.md). Thus $x\in\overline K^w$ exactly when every weak neighbourhood of $x$ meets $K$.

## Weakly null sequence

↑ **Parent:** [Weak topology](weak-topology.md)

A sequence $(x_n)$ is weakly null when $f(x_n)\to0$ for every member $f$ of the [continuous dual space](continuous-dual-space.md). It may remain bounded away from zero in norm.

### Standard unit vectors are weakly null in lp

↑ **Parent:** [Weakly null sequence](#weakly-null-sequence)

For $1<p<\infty$, identify $(\ell^p)^*$ with $\ell^q$. If $y=(y_j)\in\ell^q$, then

$$
\langle y,e_n\rangle=y_n\longrightarrow0.
$$

Thus the standard unit vectors converge weakly to zero in $\ell^p$, although $\|e_n\|_p=1$ for every $n$.

### Weak convergence of bounded disjointly supported sequences in lp

↑ **Parent:** [Weakly null sequence](#weakly-null-sequence)

Let $1<p<\infty$. Every norm-bounded sequence in $\ell^p$ whose terms have pairwise disjoint supports converges weakly to zero. Indeed, the average of $N$ distinct terms has norm $O(N^{1/p-1})$, so [Mazur theorem](hilbert-space.md#mazur-theorem) gives weak convergence through its convex-combination criterion.

## Weakly Cauchy sequence

↑ **Parent:** [Weak topology](weak-topology.md)

A sequence $(x_n)$ is weakly Cauchy when $(f(x_n))$ is a [Cauchy sequence](real-analysis.md#cauchy-sequence) for every continuous linear functional $f$. Its consecutive differences form a [weakly null sequence](#weakly-null-sequence).

## Weak closure of the unit sphere

↑ **Parent:** [Weak topology](weak-topology.md)

In an infinite-dimensional normed space, the weak closure of the unit sphere is the closed unit ball. Every basic weak neighbourhood imposes only finitely many linear conditions, whose common kernel contains a nonzero direction that can move any interior point onto the sphere.

## Weak-star topology

↑ **Parent:** [Weak topology](weak-topology.md)

The weak-star topology $\sigma(X^*,X)$ is pointwise convergence of functionals on $X$. If $X$ is nonreflexive, it is strictly weaker than the weak topology $\sigma(X^*,X^{**})$ on $X^*$.

### Weak-star fixed point theorem for an adjoint operator

↑ **Parent:** [Weak-star topology](#weak-star-topology)

If $T=S^*$ for a [bounded operator](topological-vector-space.md#continuous-linear-operator) on a separable [Banach space](banach-space.md), and $C$ is a nonempty weak-star closed convex subset of the dual [unit ball](functional-analysis.md#unit-ball) with $T(C)\subseteq C$, then $T$ has a fixed point in $C$. The [Cesaro averages](real-analysis.md#cesaro-mean) of the orbit remain in $C$, and $T$ minus the identity sends those averages to [vectors](vector-space.md#vector) of [norm](functional-analysis.md#norm) at most $2/n$. Weak-star [compactness](topology.md#compact-space) supplies a cluster point, and the adjoint action is weak-star continuous. The corresponding assertion with only weak closedness is false for the right shift on the probability simplex in $\ell^1$, the dual of $c_0$.

### Weak-star separability of the entire dual

↑ **Parent:** [Weak-star topology](#weak-star-topology)

The continuous dual of a separable [Banach space](banach-space.md) is separable in its [weak-star topology](#weak-star-topology), even when it is not norm separable. [Banach-Alaoglu theorem](functional-analysis.md#banach-alaoglu-theorem) and [weak-star metrizability of the dual ball](#weak-star-metrizability-of-the-dual-ball) make the dual unit ball a separable compact metric space. The countable union of positive integer multiples of a countable dense subset of that ball is dense in the whole dual. This does not imply global weak-star metrizability.

### Weak-star open dual ball category obstruction

↑ **Parent:** [Weak-star topology](#weak-star-topology)

For an infinite-dimensional normed space, the weak-star open unit ball of its dual is not a [Baire space](topological-analysis.md#baire-space). The smaller closed norm balls are weak-star closed and have empty relative interior: a nonzero functional annihilating any finitely many tested vectors can move the norm beyond the smaller radius while remaining below one. Their countable union is the open norm ball. Thus this topology is not [topologically complete](topological-analysis.md#topological-completeness), regardless of separability.

### Weak-star topology on an entire infinite-dimensional Banach dual is not metrizable

↑ **Parent:** [Weak-star topology](#weak-star-topology)

A countable local base at zero would give countably many finite sets of evaluation vectors. Any other evaluation must lie in the span of one of those finite sets: otherwise a bounded functional vanishing on that set but not on the evaluation vector, supplied by [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem), contradicts inclusion of neighbourhoods after scalar rescaling. Thus the predual has countable Hamel dimension, impossible for an infinite-dimensional [Banach space](banach-space.md) by the [Baire category theorem](topological-analysis.md#baire-category-theorem). This concerns the entire dual, unlike [weak-star metrizability of the dual ball](#weak-star-metrizability-of-the-dual-ball).

### Continuous dual of a weak-star topology

↑ **Parent:** [Weak-star topology](#weak-star-topology)

A [linear functional](linear-algebra.md#linear-functional) on $X^*$ is continuous for the [weak-star topology](#weak-star-topology) exactly when it is evaluation at an element of $X$. Continuity makes it vanish on the common kernel of finitely many evaluations, so it is a linear combination of those evaluations. The [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual) identifies this dual with $X$.

### Failure of weak-star convergence to commute with squaring

↑ **Parent:** [Weak-star topology](#weak-star-topology)

In $L^\infty(\mathbb R)=(L^1(\mathbb R))^*$, the sequence $f_n(x)=\sin(nx)$ converges weak-star to zero by the [Riemann-Lebesgue lemma](fourier-analysis.md#riemann-lebesgue-lemma), while $f_n^2$ converges weak-star to the constant $1/2$. Nonlinear pointwise operations therefore need not preserve weak-star limits.

### Weak-star metrizability of the dual ball

↑ **Parent:** [Weak-star topology](#weak-star-topology)

If $X$ is separable, the weak-star topology on $B_{X^*}$ is metrizable. For a dense sequence $(x_n)$ in $B_X$, a compatible metric is obtained by summing bounded multiples of $2^{-n}|f(x_n)-g(x_n)|$.

#### Weak-star metrizability criterion for a dual ball

↑ **Parent:** [Weak-star metrizability of the dual ball](#weak-star-metrizability-of-the-dual-ball)

The dual unit ball $B_{X^*}$ is weak-star metrizable if and only if $X$ is separable. For the converse direction, [Banach-Alaoglu theorem](functional-analysis.md#banach-alaoglu-theorem) makes a metrizable dual ball a compact metric space, and the evaluation map embeds $X$ isometrically into the separable space $C(B_{X^*})$.

### Grothendieck space

↑ **Parent:** [Weak-star topology](#weak-star-topology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grothendieck_space)

A Banach space $X$ is a Grothendieck space when every weak-star convergent sequence in $X^*$ is weakly convergent. Every [reflexive Banach space](functional-analysis.md#reflexive-banach-space) has this property, and every separable Grothendieck space is reflexive.

### Szlenk derivation

↑ **Parent:** [Weak-star topology](#weak-star-topology)

For a weak-star compact set $K\subseteq X^*$, its Szlenk derivation at scale $\varepsilon>0$ is

$$
K'_\varepsilon=\{f\in K:\operatorname{diam}(U\cap K)>\varepsilon\text{ for every weak-star neighbourhood }U\text{ of }f\}.
$$

It removes points having a relatively weak-star open neighbourhood of norm diameter at most $\varepsilon$.

Transfinite iteration of this operation defines the [Szlenk index](#szlenk-index); one derivation step is not itself the index.

#### One-step Szlenk derivation for a separable dual

↑ **Parent:** [Szlenk derivation](#szlenk-derivation)

If $X^*$ is separable and $K$ is a nonempty weak-star closed subset of $B_{X^*}$, then $K'_\varepsilon$ is a proper subset of $K$ for every $\varepsilon>0$. Metrizability produces sequences witnessing membership in the derivative, while a Baire-category argument applied to a universal weakly null sequence yields the strict inclusion.

## Weakly compact set

↑ **Parent:** [Weak topology](weak-topology.md)

A subset of a Banach space is weakly compact when it is compact in the [weak topology](weak-topology.md); it is relatively weakly compact when its weak closure is weakly compact.

### Discontinuous pointwise limit obstruction to weak compactness

↑ **Parent:** [Weakly compact set](#weakly-compact-set)

A bounded sequence in the [space of continuous functions on a compact space](functional-analysis.md#space-of-continuous-functions-on-a-compact-space) that has a discontinuous pointwise limit cannot lie in a weakly compact set. Compactness would give a weakly convergent subnet, and continuous point-evaluation functionals would identify its continuous limit with the prescribed pointwise limit. No assumption of sequential compactness is needed.

### Weakly compact subsets of l-infinity are norm separable

↑ **Parent:** [Weakly compact set](#weakly-compact-set)

Coordinate evaluations on the [l-infinity sequence space](banach-space.md#l-infinity-sequence-space) form a countable separating family, so a [weakly compact set](#weakly-compact-set) $K$ is metrizable by [countable separating family metrizes a weakly compact set](#countable-separating-family-metrizes-a-weakly-compact-set). Choose a countable weakly dense subset $D$. Then $K$ lies in the weak closure of $\operatorname{conv}D$, which equals its norm closure by [Mazur theorem](hilbert-space.md#mazur-theorem). Rational convex combinations make that norm closure separable, and every subset of a separable metric space is separable. The weakly dense subset itself need not be norm dense in a nonconvex $K$.

### Weakly compact set is norm bounded

↑ **Parent:** [Weakly compact set](#weakly-compact-set)

Every [weakly compact set](#weakly-compact-set) in a [normed vector space](functional-analysis.md#normed-vector-space) is norm bounded, even if the space is incomplete. Its [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual) is pointwise bounded on the [continuous dual space](continuous-dual-space.md); the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) on that Banach dual gives the norm bound.

### Weakly sequentially compact set

↑ **Parent:** [Weakly compact set](#weakly-compact-set)

A set is weakly sequentially compact when every sequence in it has a subsequence that converges weakly to a point of the set.

<h4 id="eberlein-smulian-theorem">Eberlein-Šmulian theorem</h4>

↑ **Parent:** [Weakly sequentially compact set](#weakly-sequentially-compact-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eberlein–Šmulian_theorem)

For a subset of a Banach space, relative weak compactness is equivalent to every sequence having a weakly convergent subsequence. In particular, weak compactness and weak sequential compactness coincide.

<h3 id="krein-smulian-theorem">Krein-Šmulian theorem</h3>

↑ **Parent:** [Weakly compact set](#weakly-compact-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krein–Smulian_theorem)

The closed convex hull of a weakly compact subset of a Banach space is weakly compact.

The other standard formulation says that a convex subset $C$ of a Banach-space dual is weak-star closed if its intersection with every norm-closed ball is weak-star closed.

## Szlenk index

↑ **Parent:** [Weak topology](weak-topology.md)

The Szlenk index measures how many transfinite [Szlenk derivations](#szlenk-derivation) are needed to empty the dual unit ball at each positive norm-diameter scale. At a successor ordinal take another derivation; at a limit ordinal intersect the previous sets. Taking the supremum of the emptying ordinals over the positive scales gives an ordinal invariant of the Banach space.

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (34)

- [Closed convex hull](mathematical-optimization.md#closed-convex-hull)
- [Continuous dual of a weak topology](topological-vector-space.md#continuous-dual-of-a-weak-topology)
- [Countable separating family metrizes a weakly compact set](#countable-separating-family-metrizes-a-weakly-compact-set)
- [Finite-dimensional weak and norm topologies coincide](#finite-dimensional-weak-and-norm-topologies-coincide)
- [Original and weak continuity of linear maps between Fréchet spaces](#original-and-weak-continuity-of-linear-maps-between-frechet-spaces)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#2/solution)
- [5](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#5)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#22h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-106.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-106.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-106.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#3/solution)
- [Weak and norm Borel sigma-algebras in a separable Banach space](#weak-and-norm-borel-sigma-algebras-in-a-separable-banach-space)
- [Weak-ball metrizability requires a norm-separable dual](#weak-ball-metrizability-requires-a-norm-separable-dual)
- [Weak closure](#weak-closure)
- [Weak compactness characterization of reflexivity](functional-analysis.md#weak-compactness-characterization-of-reflexivity)
- [Weak compactness of an operator and its adjoint](functional-analysis.md#weak-compactness-of-an-operator-and-its-adjoint)
- [Weak topology of a CW complex](algebraic-topology.md#weak-topology-of-a-cw-complex)
- [Weakly compact set](#weakly-compact-set)
