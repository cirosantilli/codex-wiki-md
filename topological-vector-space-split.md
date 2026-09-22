# Topological vector space

↑ **Parent:** [Functional analysis](functional-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_vector_space)

A topological vector space is a [vector space](vector-space-split.md) $E$ over $\mathbb K=\mathbb R$ or $\mathbb C$, equipped with a [topology](topology-split.md) such that [vector addition](vector-addition.md) and [scalar multiplication](scalar-multiplication.md) are jointly [continuous](continuous-function.md):

$$
E\times E\longrightarrow E,\quad (x,y)\longmapsto x+y,
\qquad
\mathbb K\times E\longrightarrow E,\quad (\lambda,x)\longmapsto\lambda x.
$$

The domains carry the [product topology](product-topology.md), and the [scalar](scalar.md) field carries its usual [topology](topology-split.md). Joint [continuity](continuous-function.md) permits both inputs to vary at once. Here the definition does not impose the [Hausdorff](hausdorff-space.md) condition; we state it separately when needed. [Peter Philip, Functional Analysis, Definition 1.1 and Example 1.2](https://www.math.lmu.de/~philip/publications/lectureNotes/philipPeter_FunctionalAnalysis.pdf).

Every [normed vector space](normed-vector-space.md) is a [topological vector space](topological-vector-space-split.md): the [triangle inequality](triangle-inequality.md) gives $\|x+y\|\leq\|x\|+\|y\|$, while

$$
\|\lambda x-\lambda_0x_0\|\leq |\lambda|\,\|x-x_0\|+|\lambda-\lambda_0|\,\|x_0\|
$$

controls [scalar multiplication](scalar-multiplication.md) near any $(\lambda_0,x_0)$. More generally, a [seminorm topology](seminorm-topology.md) supplies many measurements of smallness, rather than one [norm](norm.md). Translation by any [vector](vector.md) is a [homeomorphism](homeomorphism.md), so a [neighbourhood basis](neighbourhood-basis.md) at zero determines all [neighbourhoods](neighbourhood-mathematics.md) by translation.

The compatibility matters: on a nonzero real [vector space](vector-space-split.md), the [discrete topology](discrete-space.md) makes [vector addition](vector-addition.md) [continuous](continuous-function.md), but not [scalar multiplication](scalar-multiplication.md). For $x\ne0$, the [sequence](sequence.md) of scalars $1/n$ tends to zero, whereas the [sequence](sequence.md) $x/n$ never enters the [open set](open-set.md) $\{0\}$. Thus choosing a [topology](topology-split.md) arbitrarily need not respect the [linear algebra](linear-algebra-split.md).

This framework lets [functional analysis](functional-analysis-split.md) choose the appropriate notion of [limit of a sequence](limit-of-a-sequence.md). [Norm topology](norm-topology.md) measures one global error, [weak topology](weak-topology-split.md) tests [linear functionals](linear-functional.md), and the [Fréchet space](frechet-space.md) of [smooth functions](smooth-function.md) controls every order of [derivative](derivative.md). In each case the operations forming [linear combinations](linear-combination.md) are [continuous](continuous-function.md), making approximation compatible with the underlying equations.

**Table of contents**

- [Dense subspace](dense-subspace.md)
- [Sequential continuity criterion in a metrizable vector space](sequential-continuity-criterion-in-a-metrizable-vector-space.md)
- [Bounded set in a topological vector space](bounded-set-in-a-topological-vector-space.md)
- [Strict inductive limit topology](strict-inductive-limit-topology.md)
- [Metrizable topological vector space](metrizable-topological-vector-space.md)
- [Finite-dimensional vector-space topology](finite-dimensional-vector-space-topology.md)
  - [Equivalence of norms in finite dimensions](equivalence-of-norms-in-finite-dimensions.md)
    - [Sharp comparison of l1 and l2 norms](sharp-comparison-of-l1-and-l2-norms.md)
- [Locally convex space](locally-convex-space.md)
  - [Seminorm topology](seminorm-topology.md)
    - [Separating family of seminorms](separating-family-of-seminorms.md)
  - [Compact metrizable convex set](compact-metrizable-convex-set.md)
    - [Choquet theorem](choquet-theorem.md)
      - [Threshold Choquet representation in L-infinity](threshold-choquet-representation-in-l-infinity.md)
      - [Choquet's theorem by strict convexity](choquet-s-theorem-by-strict-convexity.md)
    - [Affine upper envelope](affine-upper-envelope.md)
      - [Supporting measure lemma for affine upper envelopes](supporting-measure-lemma-for-affine-upper-envelopes.md)
    - [Barycenter](barycenter.md)
  - [Seminorm](seminorm.md)
    - [Kernel of a seminorm](kernel-of-a-seminorm.md)
    - [Coordinate seminorms](coordinate-seminorms.md)
    - [Dual seminorm](dual-seminorm.md)
  - [Fréchet space](frechet-space.md)
    - [Derivative seminorms on a compact interval](derivative-seminorms-on-a-compact-interval.md)
      - [Smooth convergence on a compact interval](smooth-convergence-on-a-compact-interval.md)
  - [Minkowski functional](minkowski-functional.md)
    - [Norm from a bounded symmetric convex neighbourhood](norm-from-a-bounded-symmetric-convex-neighbourhood.md)
  - [Separation of a point and an open convex set](separation-of-a-point-and-an-open-convex-set.md)
    - [Hahn-Banach separation theorem for two convex sets](hahn-banach-separation-theorem-for-two-convex-sets.md)
    - [Finite-dimensional separation of open convex sets](finite-dimensional-separation-of-open-convex-sets.md)
  - [Dual pair](dual-pair.md)
    - [Continuous dual of a weak topology](continuous-dual-of-a-weak-topology.md)
    - [Compact norming dual-pair criterion](compact-norming-dual-pair-criterion.md)
    - [Bipolar theorem for a dual pair](bipolar-theorem-for-a-dual-pair.md)
  - [Product of locally convex spaces](product-of-locally-convex-spaces.md)
- [Continuous linear operator](continuous-linear-operator.md)
  - [Completely continuous operator](completely-continuous-operator.md)
  - [Approximate surjectivity with geometric correction](approximate-surjectivity-with-geometric-correction.md)
  - [Absolutely p-summing operator](absolutely-p-summing-operator.md)
    - [2-summing operator](2-summing-operator.md)
      - [2-summing norm of a finite-dimensional identity](2-summing-norm-of-a-finite-dimensional-identity.md)
    - [Pietsch factorization theorem](pietsch-factorization-theorem.md)
    - [Absolutely summing operator](absolutely-summing-operator.md)
  - [Strictly singular operator](strictly-singular-operator.md)
  - [Positivity-preserving linear operator on L1](positivity-preserving-linear-operator-on-l1.md)
    - [Mean control for positive imaging operators](mean-control-for-positive-imaging-operators.md)
  - [Schur test](schur-test.md)
  - [Bounded inverse](bounded-inverse.md)
  - [Positive linear operator on continuous functions](positive-linear-operator-on-continuous-functions.md)
    - [Zero-preserving linear operator on continuous functions](zero-preserving-linear-operator-on-continuous-functions.md)
  - [Contractive linear operator](contractive-linear-operator.md)
  - [Range of a bounded linear operator](range-of-a-bounded-linear-operator.md)
  - [Extension of a bounded linear operator from a dense subspace](extension-of-a-bounded-linear-operator-from-a-dense-subspace.md)
    - [Failure of dense-subspace extension into an incomplete codomain](failure-of-dense-subspace-extension-into-an-incomplete-codomain.md)
  - [Banach space of bounded linear operators](banach-space-of-bounded-linear-operators.md)
  - [Continuous linear functional](continuous-linear-functional.md)
    - [Linear functional with closed kernel](linear-functional-with-closed-kernel.md)
    - [Point evaluation functional](point-evaluation-functional.md)
  - [Sequential continuity criterion for a linear map on a metrizable topological vector space](sequential-continuity-criterion-for-a-linear-map-on-a-metrizable-topological-vector-space.md)
  - [Isomorphism of Banach spaces](isomorphism-of-banach-spaces.md)

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Bounded set in a topological vector space](bounded-set-in-a-topological-vector-space.md)
- [Closed vector subspace](closed-vector-subspace.md)
- [Continuous dual space](continuous-dual-space-split.md)
- [Continuous linear functional](continuous-linear-functional.md)
- [Dense subspace](dense-subspace.md)
- [Dual space](dual-space.md)
- [Locally convex space](locally-convex-space.md)
- [Reflexive space](reflexive-space.md)
- [Topological vector space](topological-vector-space-split.md)
