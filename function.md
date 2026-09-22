# Function

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Function_(mathematics))

A function assigns exactly one output to each input in its domain.

**Table of contents**

- [Germ (mathematics)](#germ-mathematics)
- [Nonnegative function](#nonnegative-function)
- [Commuting functions](#commuting-functions)
- [Finite modification of the identity on the real line](#finite-modification-of-the-identity-on-the-real-line)
- [Pointwise periodic self-map](#pointwise-periodic-self-map)
  - [Uniform period criterion for pointwise periodic maps](#uniform-period-criterion-for-pointwise-periodic-maps)
- [Vector-valued function](#vector-valued-function)
- [Set function](#set-function)
  - [Finite additivity of a set function](#finite-additivity-of-a-set-function)
  - [Supermodular set function](#supermodular-set-function)
  - [Submodular set function](#submodular-set-function)
- [Function collision](#function-collision)
- [Fiber of a function](#fiber-of-a-function)
  - [Factorization through a surjection](#factorization-through-a-surjection)
- [Translation of a function](#translation-of-a-function)
- [Graph of a function](#graph-of-a-function)
  - [Compact graph of a continuous map](#compact-graph-of-a-continuous-map)
  - [Closed graph of a map into a Hausdorff space](#closed-graph-of-a-map-into-a-hausdorff-space)
- [Partial function](#partial-function)
  - [Partial unary operation](#partial-unary-operation)
  - [Composition of partial functions](#composition-of-partial-functions)
- [Domain of a function](#domain-of-a-function)
  - [Domain of a partial function](#domain-of-a-partial-function)
- [Function class](#function-class)
- [Support](#support)
  - [Compact support](#compact-support)
- [Identity function](#identity-function)
- [Inverse function](#inverse-function)
  - [Right inverse](#right-inverse)
    - [Right-inverse characterization of the axiom of choice](#right-inverse-characterization-of-the-axiom-of-choice)
  - [Left inverse](#left-inverse)
- [Projection (mathematics)](#projection-mathematics)
  - [Projection map](#projection-map)
    - [Empty-set cases for Cartesian projections](#empty-set-cases-for-cartesian-projections)
- [Fixed point](#fixed-point)
- [Conjugate functions](#conjugate-functions)
- [Piecewise linear function](#piecewise-linear-function)
  - [Linear interpolation](#linear-interpolation)
- [Bounded function](#bounded-function)
  - [Unbounded function](#unbounded-function)
- [Constant function](#constant-function)
- [Real-valued function](#real-valued-function)
  - [Global maximum](#global-maximum)
  - [Positive part of a real-valued function](#positive-part-of-a-real-valued-function)
- [Bijection](#bijection)
- [Periodic function](#periodic-function)
  - [Simply periodic function](#simply-periodic-function)
  - [Cardinality of integer-periodic function spaces](#cardinality-of-integer-periodic-function-spaces)
  - [Period average](#period-average)
  - [Triangular wave](#triangular-wave)

## Germ (mathematics)

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Germ_(mathematics))

A [germ](#germ-mathematics) at a point is an [equivalence class](set-theory.md#equivalence-class) of [functions](function.md) defined on a [neighbourhood](topology.md#neighbourhood-mathematics) of the point: two representatives are equivalent if they agree on some smaller [neighbourhood](topology.md#neighbourhood-mathematics). A [germ of a holomorphic function](complex-analysis.md#germ-of-a-holomorphic-function) requires its representatives to be [holomorphic functions](complex-analysis.md#holomorphic-function); smooth and continuous germs use their corresponding classes of [functions](function.md). The [germ](#germ-mathematics) retains local behavior while forgetting the representative's values farther from the point.

## Nonnegative function

↑ **Parent:** [Function](function.md)

A real-valued function is nonnegative when all its values are at least zero. Products and nonnegative linear combinations of nonnegative functions remain nonnegative. A nonnegative partition of unity gives convex combinations, hence a convex-hull bound for a geometric basis.

## Commuting functions

↑ **Parent:** [Function](function.md)

Two self-maps $R,S:X\to X$ commute when $R\circ S=S\circ R$. Induction then gives $R^n\circ S=S\circ R^n$ and $R^n\circ S^m=S^m\circ R^n$ for all nonnegative integers $m,n$. Sharing a fixed point or invariant set does not by itself imply commutation. For rational sphere maps of degrees at least two, commutation does imply equality of their [Fatou sets](complex-dynamics.md#fatou-set) and [Julia sets](complex-dynamics.md#julia-set), by the [commuting rational maps of degree at least two have the same Julia set](complex-dynamics.md#commuting-rational-maps-of-degree-at-least-two-have-the-same-julia-set) theorem.

## Finite modification of the identity on the real line

↑ **Parent:** [Function](function.md)

A finite modification agrees with the [identity map](#identity-function) outside a finite exceptional [set](set.md). Sorting that [set](set.md) gives a unique finite record of pairs $(x,f(x))$. [Real-number pairing by separated digits](algebra.md#real-number-pairing-by-separated-digits) encodes the record in $(0,1)$, and placing length-$n$ records in disjoint intervals $(n,n+1)$ gives an [injection](algebra.md#injective-function) from all finite modifications into the real line. Conversely, changing the value at one fixed point gives a real-parameter family, so the [Cantor-Schröder-Bernstein theorem](set-theory.md#cantor-schroder-bernstein-theorem) shows this family has continuum cardinality.

## Pointwise periodic self-map

↑ **Parent:** [Function](function.md)

A pointwise periodic self-map returns each point to itself after a positive number of iterates which may depend on the point. It is a [bijection](#bijection): each finite cycle supplies predecessors; equality of two images can be undone by an iterate with an exponent one below a common multiple of the two periods. The [set](set.md) consequently decomposes into disjoint finite [permutation cycles](finite-group-theory.md#permutation-cycle). Pointwise periodicity does not imply that one iterate is the identity on an infinite [set](set.md).

### Uniform period criterion for pointwise periodic maps

↑ **Parent:** [Pointwise periodic self-map](#pointwise-periodic-self-map)

A [pointwise periodic self-map](#pointwise-periodic-self-map) has a uniform positive period exactly when its finite cycle lengths are bounded. A uniform period is divisible by every length; conversely, bounded lengths divide the [least common multiple](number-theory.md#least-common-multiple) of $1,\ldots,M$ for some bound $M$. Arbitrarily many bounded-length cycles are allowed. Every such [map](#function-class) on a [finite set](set.md#finite-set) has a uniform period. On any infinite [set](set.md) containing a countably infinite subset, cycles of unbounded finite lengths and fixed points elsewhere give a counterexample. Thus, with the usual [axiom of choice](set-theory.md#axiom-of-choice) assumption, the [sets](set.md) on which every pointwise periodic self-map has a uniform period are exactly finite [sets](set.md).

## Vector-valued function

↑ **Parent:** [Function](function.md)

A vector-valued function is a [function](function.md) with values in a [vector space](vector-space.md). For finite-dimensional real or complex target spaces, choosing a basis represents it by scalar coordinate functions; [continuity](calculus.md#continuous-function) and differentiability can then be checked coordinatewise.

## Set function

↑ **Parent:** [Function](function.md)

A real-valued set function assigns a real number to each subset of a specified ground set.

### Finite additivity of a set function

↑ **Parent:** [Set function](#set-function)

A real-valued [set function](#set-function) on an algebra of sets is finitely additive if it has the displayed property for disjoint pairs. It follows that $F(\varnothing)=0$. On a finite ambient [set](set.md), induction gives $F(A)=\sum_{x\in A}F(\{x\})$, so arbitrary signed singleton weights describe all such functions. Summing the pointwise [indicator function](measure-theory.md#indicator-function) identity for the [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) against these weights proves the same formula for $F$.

### Supermodular set function

↑ **Parent:** [Set function](#set-function)

A real-valued [set function](#set-function) is supermodular if it satisfies the displayed inequality. Its negative is a [submodular set function](#submodular-set-function). Equivalently, the gain from adding an element cannot decrease as the set grows. This is the defining property of a [convex cooperative game](game-theory.md#convex-cooperative-game), and makes [coalition](game-theory.md#coalition-game-theory) marginal allocations lie in the [core of a cooperative game](game-theory.md#core-game-theory).

### Submodular set function

↑ **Parent:** [Set function](#set-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Submodular_set_function)

A [set function](#set-function) is submodular if $f(A)+f(B)\geq f(A\cup B)+f(A\cap B)$ for every pair of subsets. [Entropy submodularity](information-theory.md#entropy-submodularity) is a fundamental example.

## Function collision

↑ **Parent:** [Function](function.md)

A function collision is a pair of distinct inputs $x\neq x'$ with $f(x)=f(x')$. An [injective function](algebra.md#injective-function) has no collisions. For a two-to-one function every nonempty [fiber](#fiber-of-a-function) has two elements and hence one unordered collision pair. Finding such a pair through an oracle is the task of [quantum collision finding](computer-science.md#quantum-collision-finding).

## Fiber of a function

↑ **Parent:** [Function](function.md)

For a [function](function.md) $f:X\to Y$ and $y\in Y$, its fiber is the [set](set.md) $f^{-1}(y)=\{x\in X:f(x)=y\}$. Fibers partition the domain after empty fibers are omitted. A function is [injective](algebra.md#injective-function) exactly when every fiber has at most one element. Quantum [hidden subgroup problem](quantum-theory.md#hidden-subgroup-problem) algorithms use functions whose fibers are [cosets](group-theory.md#coset).

### Factorization through a surjection

↑ **Parent:** [Fiber of a function](#fiber-of-a-function)

For a [surjective function](algebra.md#surjective-function) $f:B\to A$ and a function $g:B\to C$, there is a unique function $h:A\to C$ with $g=h\circ f$ if and only if $g$ is constant on each [fiber of a function](#fiber-of-a-function) of $f$. Define $h(a)$ to be the common value on $f^{-1}(a)$; it is well-defined and unique because that fiber is nonempty. This uniquely specified value requires no simultaneous arbitrary choices.

// Target: combinatorics.bigb

## Translation of a function

↑ **Parent:** [Function](function.md)

Translation shifts the argument without changing the shape of a [function](function.md). On the [real line](real-analysis.md#real-line), the displayed convention shifts a graph to the right by $h$. [Lebesgue measure](measure-theory.md#lebesgue-measure) invariance preserves every finite [Lp norm](real-analysis.md#lp-norm); its [Fourier transform](analysis.md#fourier-transform) is multiplied by $e^{-ih\xi}$.

## Graph of a function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_of_a_function)

For a [function](function.md) $f:A\to B$, its graph is the subset $\{(x,f(x)):x\in A\}$ of $A\times B$. It differs from a [graph](graph.md) in [graph theory](graph-theory.md). A solution curve of a scalar differential equation can be a graph over its independent coordinate.

### Compact graph of a continuous map

↑ **Parent:** [Graph of a function](#graph-of-a-function)

The map $x\mapsto(x,f(x))$ is continuous into the [product topology](geometry-and-topology.md#product-topology). It maps a [compact space](topology.md#compact-space) $X$ onto the [graph of a function](#graph-of-a-function) of a continuous $f$. Hence that graph is compact, whether or not the codomain is a [Hausdorff space](topology.md#hausdorff-space). Projection to $X$ is its continuous inverse.

### Closed graph of a map into a Hausdorff space

↑ **Parent:** [Graph of a function](#graph-of-a-function)

For a [continuous map](topology.md#continuous-map) $f:X\to Y$ with [Hausdorff space](topology.md#hausdorff-space) $Y$, its [graph of a function](#graph-of-a-function) is closed in the [product topology](geometry-and-topology.md#product-topology). If $y\ne f(x)$, choose disjoint neighborhoods of those two points in $Y$. Continuity supplies a neighborhood of $x$ whose image lies in the neighborhood of $f(x)$; its product with the other neighborhood misses the graph.

## Partial function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_function)

A partial function from $X$ to $Y$ assigns at most one value in $Y$ to each element of $X$; it may be undefined outside a subset of $X$.

### Partial unary operation

↑ **Parent:** [Partial function](#partial-function)

A partial unary operation on a set $A$ is a [partial function](#partial-function) with specified domain $D\subseteq A$ and values in $A$. A map preserving such operations must send each point of the source domain into the target domain and preserve its assigned value. It need not reflect whether the operation is defined.

### Composition of partial functions

↑ **Parent:** [Partial function](#partial-function)

Composition of [partial functions](#partial-function) is strict: $g(h_1(x),\ldots,h_r(x))$ is defined only if every $h_i(x)$ is defined and $g$ is defined on the resulting tuple. An argument discarded by the outer function still has to be defined. A representation in a non-strict programming language therefore needs an explicit sequencing guard.

## Domain of a function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Domain_of_a_function)

The domain of a function is the set of inputs on which it is defined.

### Domain of a partial function

↑ **Parent:** [Domain of a function](#domain-of-a-function)

For a partial function $f:X\rightharpoonup Y$, the domain is the subset $\{x\in X:f(x)\text{ is defined}\}$. Outside this subset, evaluation of $f$ is undefined.

## Function class

↑ **Parent:** [Function](function.md)

A function class is a [set](set.md) whose elements are functions, usually sharing a common domain and codomain.

## Support

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Support_(mathematics))

The support of a function is the closure of the set on which it is nonzero.

### Compact support

↑ **Parent:** [Support](#support)

A function has compact support when its [support](#support) is a [compact set](topology.md#compact-space).

## Identity function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Identity_function)

The identity function on a set $X$ maps every $x\in X$ to itself.

## Inverse function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_function)

If a function $f:X\to Y$ is bijective, its inverse function $f^{-1}:Y\to X$ is characterized by $f^{-1}(f(x))=x$ and $f(f^{-1}(y))=y$.

### Right inverse

↑ **Parent:** [Inverse function](#inverse-function)

A right inverse of a [function](function.md) $f:X\to Y$ is a function $g:Y\to X$ satisfying $f\circ g=\operatorname{id}_Y$. It forces $f$ to be a [surjective function](algebra.md#surjective-function). A [surjective linear map](vector-space.md#surjective-linear-map) onto a finite-dimensional [vector space](vector-space.md) has a linear right inverse: lift a [basis](vector-space.md#basis) of the target and extend by [linearity](vector-space.md#linearity).

#### Right-inverse characterization of the axiom of choice

↑ **Parent:** [Right inverse](#right-inverse)

The assertion that every [surjective function](algebra.md#surjective-function) has a [right inverse](#right-inverse) is equivalent to the [axiom of choice](set-theory.md#axiom-of-choice). Choice selects one member of each nonempty [fiber of a function](#fiber-of-a-function), giving a right inverse. Conversely, for a family $(X_i)_{i\in I}$ of nonempty sets, the projection from the disjoint union $\{(i,x):i\in I,\ x\in X_i\}$ onto $I$ is surjective. A right inverse selects one element from each $X_i$, giving a choice function.

### Left inverse

↑ **Parent:** [Inverse function](#inverse-function)

A left inverse of a [function](function.md) $f:X\to Y$ is a function $g:Y\to X$ satisfying $g\circ f=\operatorname{id}_X$. It forces $f$ to be [injective](algebra.md#injective-function), since equal images can be mapped back to equal original elements.

## Projection (mathematics)

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projection_(mathematics))

A [projection](#projection-mathematics) is a [function](function.md) that fixes the points in its image: applying it twice has the same effect as applying it once. A coordinate projection can be represented this way when its target is identified with a retract; a [linear projection](vector-space.md#projection-linear-algebra) additionally respects the vector-space operations.

### Projection map

↑ **Parent:** [Projection (mathematics)](#projection-mathematics)

A projection map from a Cartesian product selects specified coordinates, for example $p_j:\prod_iX_i\to X_j$ with $p_j((x_i)_i)=x_j$.

#### Empty-set cases for Cartesian projections

↑ **Parent:** [Projection map](#projection-map)

For a coordinate [projection map](#projection-map) onto $X_i$, write $X_j$ for the other factor. The map is [surjective](algebra.md#surjective-function) exactly when $X_i$ is empty or $X_j$ is nonempty. It is [injective](algebra.md#injective-function) exactly when $X_i$ is empty or $X_j$ has at most one element. In particular, a [surjection](algebra.md#surjective-function) onto an empty [Cartesian product](set-theory.md#cartesian-product) need not induce a [surjection](algebra.md#surjective-function) onto a nonempty factor.

## Fixed point

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fixed_point)

A fixed point of a function $f:X\to X$ is an element $x\in X$ satisfying $f(x)=x$.

## Conjugate functions

↑ **Parent:** [Function](function.md)

Functions $f:X\to X$ and $g:Y\to Y$ are conjugate through a [bijection](#bijection) $\sigma:X\to Y$ when $g=\sigma f\sigma^{-1}$. The bijection transports orbits and fixed points of every iterate of $f$ to the corresponding objects for $g$.

## Piecewise linear function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Piecewise_linear_function)

A piecewise-linear function is linear on each member of a finite or locally finite partition of its domain into intervals or polyhedral pieces.

### Linear interpolation

↑ **Parent:** [Piecewise linear function](#piecewise-linear-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_interpolation)

Between two prescribed values, [linear interpolation](#linear-interpolation) assigns $(1-t)f(a)+tf(b)$ at $(1-t)a+tb$, for $0\leq t\leq1$. Joining successive samples produces a [piecewise linear function](#piecewise-linear-function). For a [continuous function](calculus.md#continuous-function) on a compact interval, interpolants along grids with mesh tending to zero converge in the [uniform norm](functional-analysis.md#supremum-norm); their error is bounded by the [modulus of continuity](topological-analysis.md#modulus-of-continuity) at the mesh size.

## Bounded function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounded_function)

A real- or complex-valued function is bounded when the [moduli](complex-analysis.md#modulus) of all its values have one finite upper bound.

### Unbounded function

↑ **Parent:** [Bounded function](#bounded-function)

An unbounded function has no finite bound on the [moduli](complex-analysis.md#modulus) of its values.

## Constant function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constant_function)

A constant function has the same output for every input.

## Real-valued function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real-valued_function)

A real-valued function has codomain contained in the real numbers.

### Global maximum

↑ **Parent:** [Real-valued function](#real-valued-function)

A global maximum of a real-valued function is a value $f(x_0)$ satisfying $f(x)\leq f(x_0)$ throughout its domain.

A [global maximum](#global-maximum) is one type of [extremum of a real-valued function](mathematical-optimization.md#maximum-and-minimum); global minima reverse the inequality.

### Positive part of a real-valued function

↑ **Parent:** [Real-valued function](#real-valued-function)

The positive part of a [real-valued function](#real-valued-function) $f$ is $f_+(x)=\max(0,f(x))$. Together with the negative part $f_-(x)=\max(0,-f(x))$, it gives $f=f_+-f_-$ and $|f|=f_++f_-$.

## Bijection

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bijection)

A bijection is a function that is both injective and surjective, so every target element has exactly one preimage.

## Periodic function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Periodic_function)

A function is periodic when $f(x+T)=f(x)$ for some nonzero period $T$ and every $x$ in its domain.

### Simply periodic function

↑ **Parent:** [Periodic function](#periodic-function)

A nonconstant [meromorphic function](isolated-singularity.md#meromorphic-function) on the [complex plane](complex-analysis.md#complex-plane) is simply periodic when its group of periods is generated by one nonzero complex number. It is distinct from a doubly periodic [elliptic function](complex-analysis.md#elliptic-function), whose [period lattice](complex-analysis.md#period-lattice) has two real-linearly independent generators. Single periodicity alone imposes no algebraic addition law.

### Cardinality of integer-periodic function spaces

↑ **Parent:** [Periodic function](#periodic-function)

For fixed positive integer period $n$, integer-valued [periodic functions](#periodic-function) on $\mathbb Z$ are in [bijection](#bijection) with $\mathbb Z^n$ and hence form a [countable set](set-theory.md#countable-set). Their union over periods is a [countable union of countable sets](set-theory.md#countable-union-of-countable-sets). In contrast, period-one integer-valued [functions](function.md) on $\mathbb Q$ can prescribe arbitrary binary values on its infinitely many distinct classes modulo $\mathbb Z$. The [power set](set.md#power-set) of a countably infinite set injects into them, proving uncountability.

### Period average

↑ **Parent:** [Periodic function](#periodic-function)

For an integrable [periodic function](#periodic-function) $f$ with period $T$, its period average is $\langle f\rangle=T^{-1}\int_{t_0}^{t_0+T}f(t)\,dt$, independent of $t_0$. In particular a sinusoidal square has period average $1/2$.

### Triangular wave

↑ **Parent:** [Periodic function](#periodic-function)

A triangular wave is a continuous piecewise linear [periodic function](#periodic-function) whose slope alternates between two values. The even $2\pi$-periodic extension of $bx$ from $[0,\pi]$ is $P(s)=b|s-2k\pi|$ for $(2k-1)\pi\le s\le(2k+1)\pi$. Its [Fourier cosine series](fourier-series.md#fourier-cosine-series) contains a constant term and odd modes with coefficients proportional to the inverse square of the mode number. Such extensions describe reflection under [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition).

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (506)

- [Absolute Fourier convergence from a square-integrable derivative](fourier-series.md#absolute-fourier-convergence-from-a-square-integrable-derivative)
- [Adaptivity to an unknown covariate distribution](statistical-inference.md#adaptivity-to-an-unknown-covariate-distribution)
- [Adjoints of inverse image on power sets](category.md#adjoints-of-inverse-image-on-power-sets)
- [Affine upper envelope](topological-vector-space.md#affine-upper-envelope)
- [Analysis of Boolean functions](combinatorics.md#analysis-of-boolean-functions)
- [Axiom of global choice](set-theory.md#axiom-of-global-choice)
- [Barycenter](topological-vector-space.md#barycenter)
- [Best N-term wavelet approximation of piecewise Hölder functions](hilbert-space.md#best-n-term-wavelet-approximation-of-piecewise-holder-functions)
- [Best uniform approximation](uniform-approximation.md#best-uniform-approximation)
- [Biconjugation as closed convexification](convex-optimization.md#biconjugation-as-closed-convexification)
- [Bilinear correlation bound for the box norm](additive-combinatorics.md#bilinear-correlation-bound-for-the-box-norm)
- [Binary diagonally noncomputable function](foundations-of-mathematics.md#binary-diagonally-noncomputable-function)
- [Binary operation](algebra.md#binary-operation)
- [Boolean cube expansion from bounded differences](probability-inequality.md#boolean-cube-expansion-from-bounded-differences)
- [Boundary condition](differential-equation.md#boundary-condition)
- [Boundary trace of a function](differential-equation.md#boundary-trace-of-a-function)
- [Bounded differences property](probability-inequality.md#bounded-differences-property)
- [Bounded nonconvergent Fourier partial sums](fourier-series.md#bounded-nonconvergent-fourier-partial-sums)
- [Bounding-to-almost-disjointness inequality](set-theory.md#bounding-to-almost-disjointness-inequality)
- [Box norm](additive-combinatorics.md#box-norm)
- [Bukovský-Hechler theorem](set-theory.md#bukovsky-hechler-theorem)
- [Calculus of variations](calculus-of-variations.md)
- [Cardinality of integer-periodic function spaces](#cardinality-of-integer-periodic-function-spaces)
- [Cartan's magic formula](differential-form.md#cartan-s-magic-formula)
- [Category of finite sets](category.md#category-of-finite-sets)
- [Category of pointed sets](category.md#category-of-pointed-sets)
- [Certifiable function](probability-inequality.md#certifiable-function)
- [Choquet's theorem by strict convexity](topological-vector-space.md#choquet-s-theorem-by-strict-convexity)
- [Classifier](foundations-of-mathematics.md#classifier)
- [Closed ball](topological-analysis.md#closed-ball)
- [Closed forcing adds no short ground-valued sequences](forcing.md#closed-forcing-adds-no-short-ground-valued-sequences)
- [Coherent coinfinite injections into omega](algebra.md#coherent-coinfinite-injections-into-omega)
- [Coherent-injection Aronszajn tree](set.md#coherent-injection-aronszajn-tree)
- [Compact metrizable convex set](topological-vector-space.md#compact-metrizable-convex-set)
- [Continuous exponential functional equation](analysis.md#continuous-exponential-functional-equation)
- [Correlation function of a point process](probability-theory.md#correlation-function-of-a-point-process)
- [Countable saturation of a nonprincipal ultraproduct over omega](foundations-of-mathematics.md#countable-saturation-of-a-nonprincipal-ultraproduct-over-omega)
- [Counting lemma for octahedrally quasirandom three-uniform hypergraphs](hypergraph.md#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs)
- [Curl of a gradient](calculus.md#curl-of-a-gradient)
- [Density of bounded centered scores](statistical-model.md#density-of-bounded-centered-scores)
- [Differentiability implies continuity](analysis.md#differentiability-implies-continuity)
- [Differential operator](analysis.md#differential-operator)
- [Differentiation](calculus.md#differentiation)
- [Directed limit of elementary embeddings](foundations-of-mathematics.md#directed-limit-of-elementary-embeddings)
- [Double-coset Hecke algebra](group-theory.md#double-coset-hecke-algebra)
- [Dyadic conditional averages recover integrable functions](measure-theory.md#dyadic-conditional-averages-recover-integrable-functions)
- [Effective diagonal lemma](mathematical-logic.md#effective-diagonal-lemma)
- [Effective domain](real-analysis.md#effective-domain)
- [Empirical spectral measure](probability-theory.md#empirical-spectral-measure)
- [Equivalence of partial functions modulo finite changes](set-theory.md#equivalence-of-partial-functions-modulo-finite-changes)
- [Equivalence relation induced by a function](set-theory.md#equivalence-relation-induced-by-a-function)
- [Extreme-point criterion for the L-infinity unit ball](mathematical-optimization.md#extreme-point-criterion-for-the-l-infinity-unit-ball)
- [Failure of L2 closure of the global BV domain](inverse-problem.md#failure-of-l2-closure-of-the-global-bv-domain)
- [Fast-growing hierarchy](set-theory.md#fast-growing-hierarchy)
- [Fiber of a function](#fiber-of-a-function)
- [Finite coloring](ramsey-theory.md#finite-coloring)
- [Finite-cost optimal transport converse](mathematical-optimization.md#finite-cost-optimal-transport-converse)
- [Finite difference](finite-difference.md)
- [Finite witness array coding](foundations-of-mathematics.md#finite-witness-array-coding)
- [Four-neighbour mean expansion](finite-difference.md#four-neighbour-mean-expansion)
- [Full second-order replacement rank obstruction](set-theory.md#full-second-order-replacement-rank-obstruction)
- [Full shift](dynamical-systems.md#full-shift)
- [Function in extension](foundations-of-mathematics.md#function-in-extension)
- [Function space](functional-analysis.md#function-space)
- [Functional](calculus-of-variations.md#functional)
- [Functional equation](analysis.md#functional-equation)
- [Gaussian white noise model](stochastic-process.md#gaussian-white-noise-model)
- [Germ (mathematics)](#germ-mathematics)
- [Goodstein function](number-theory.md#goodstein-function)
- [Graph homomorphism](graph-theory.md#graph-homomorphism)
- [Graph of a function](#graph-of-a-function)
- [Haar projection](fourier-analysis.md#haar-projection)
- [Haar projection error for a Lipschitz function](fourier-analysis.md#haar-projection-error-for-a-lipschitz-function)
- [Haar scaling function](fourier-analysis.md#haar-scaling-function)
- [Hamiltonian trace functional on monic differential operators](analysis.md#hamiltonian-trace-functional-on-monic-differential-operators)
- [Hölder-Taylor remainder bound](sobolev-space.md#holder-taylor-remainder-bound)
- [Holomorphic function](complex-analysis.md#holomorphic-function)
- [Homogeneous function](real-analysis.md#homogeneous-function)
- [Image of a function](set-theory.md#image-of-a-function)
- [Infinite-dimensional Hamiltonian integrability](integrable-systems.md#infinite-dimensional-hamiltonian-integrability)
- [Infinite path through a binary tree](geometry-and-topology.md#infinite-path-through-a-binary-tree)
- [Influence-function representer](statistical-inference.md#influence-function-representer)
- [Integral kernel](functional-analysis.md#integral-kernel)
- [Integral representation](calculus.md#integral-representation)
- [Integrand](calculus.md#integrand)
- [Joint injectivity of a pair of functions](set-theory.md#joint-injectivity-of-a-pair-of-functions)
- [Kahane-Katznelson divergence theorem](fourier-series.md#kahane-katznelson-divergence-theorem)
- [Kernel support-vector coefficient from hinge activity](statistical-learning.md#kernel-support-vector-coefficient-from-hinge-activity)
- [Kuratowski ordered pair](set.md#kuratowski-ordered-pair)
- [Lambda definition of primitive recursion by pair iteration](foundations-of-mathematics.md#lambda-definition-of-primitive-recursion-by-pair-iteration)
- [Lambda representation of partial computable functions](foundations-of-mathematics.md#lambda-representation-of-partial-computable-functions)
- [Left inverse](#left-inverse)
- [Lenard-Magri recursion](symplectic-geometry.md#lenard-magri-recursion)
- [Local maximum](analysis.md#local-maximum)
- [Locally square-integrable function](measure-theory.md#locally-square-integrable-function)
- [Long chain under eventual domination](set-theory.md#long-chain-under-eventual-domination)
- [Low-pass filter of a multiresolution analysis](fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis)
- [Mollification](distribution-theory.md#mollification)
- [Multipartite hypergraph](hypergraph.md#multipartite-hypergraph)
- [Multiple integral](calculus.md#multiple-integral)
- [Nondecreasing function](calculus.md#nondecreasing-function)
- [Nonincreasing function](calculus.md#nonincreasing-function)
- [Normal ultrafilter on small subsets](set-theory.md#normal-ultrafilter-on-small-subsets)
- [Normalizing constant](continuous-probability-distribution.md#normalizing-constant)
- [Orthogonal polynomial projection kernel](functional-analysis.md#orthogonal-polynomial-projection-kernel)
- [Pair-factor correlation bound for the three-dimensional box norm](additive-combinatorics.md#pair-factor-correlation-bound-for-the-three-dimensional-box-norm)
- [Parametric equation](geometry-and-topology.md#parametric-equation)
- [Partial derivative](calculus.md#partial-derivative)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#10a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#11h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#1a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#1a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#2h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-9.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#10c/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#11c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#12c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#7/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1.md#3b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4.md#8c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#7/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#7/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1.md#9d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1.md#9d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-8.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-8.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-8.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-8.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-8.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-8.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#13b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#14f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#15e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#18f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#3b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#18g/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#19g/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#23h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#30c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-16.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-20.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#11/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-56.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#7e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#7e/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1.md#11e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1.md#11e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1.md#12d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1.md#9f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3.md#12c/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3.md#12c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3.md#3c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4.md#8d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-24.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31.md#2/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82.md#1/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4.md#5e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4.md#5e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4.md#5e/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4.md#7e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#2/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#2/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#2/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-49.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3.md#3a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3.md#3a/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3.md#9a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#8e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#3/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iv/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-8.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-8.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-8.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-8.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#13i/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-25.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-25.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#2d/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#4a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#6d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#6d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#13e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#22f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#22f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#24i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#24i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#26j/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#27k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#29j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#31a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#4h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-130.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4.md#1e/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#10e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#11e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#12e/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#3e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#3e/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#10f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#12f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#7a/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#7a/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-4.md#8d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#12g/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#14d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#17b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#17b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#13c/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#2g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#3a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#7h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#11g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#13g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#4c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#6d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-1.md#10e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-1.md#10e/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-1.md#12d/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-1.md#12d/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2.md#1a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2.md#2a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2.md#3f/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2.md#9f/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-3.md#9b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-3.md#9b/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1.md#12f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1.md#12f/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1.md#18h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1.md#6h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2.md#18h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2.md#5d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2.md#8g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3.md#11f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3.md#13f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4.md#12b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4.md#18h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4.md#2f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#13l/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#14d/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#16i/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#16i/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#16i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#25f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#27g/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#37d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#5l/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#13d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#13d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#13d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#4j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#4j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#4j/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#16i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#21g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#24f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#26g/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#38c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#3k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#3k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#16i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#19h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#1f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#22g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#23g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#29l/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1.md#10e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1.md#10e/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1.md#10e/e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1.md#12e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-2.md#4f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-3.md#10a/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-1.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2.md#15c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2.md#17a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2.md#7h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2.md#9e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3.md#13e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3.md#18h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3.md#18h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3.md#3a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-4.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#12f/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#15e/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#25j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#27h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#27h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#32a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#35b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#36c/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#40a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2.md#8b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1.md#12e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1.md#12e/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1.md#12e/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1.md#12e/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-2.md#11f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-2.md#12f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-1.md#11/11-2c/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-1.md#16c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-2.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-3.md#13g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-4.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#16j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#24g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#27l/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#30l/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#4j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#23h/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#25f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#2i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#10e/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#12j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#12j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#22h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#22h/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#23g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#26l/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3.md#31b/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#18f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#24f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#26l/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#26l/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#4i/a/solution)
- [Peano zero](calculus.md#peano-zero)
- [Penrose-Ward correspondence](general-relativity.md#penrose-ward-correspondence)
- [Period of a function](mathematics.md#period-of-a-function)
- [Periodic phase change of a scaling function](fourier-analysis.md#periodic-phase-change-of-a-scaling-function)
- [Pointed set](set.md#pointed-set)
- [Pointwise convergence of a piecewise smooth Fourier series](fourier-series.md#pointwise-convergence-of-a-piecewise-smooth-fourier-series)
- [Poisson pencil](symplectic-geometry.md#poisson-pencil)
- [Positively homogeneous function (degree one)](real-analysis.md#positively-homogeneous-function-degree-one)
- [Potential of a conservative vector field](calculus.md#potential-of-a-conservative-vector-field)
- [Preimage](set-theory.md#preimage)
- [Principal minor resolvent trace bound](functional-analysis.md#principal-minor-resolvent-trace-bound)
- [Probability density](quantum-mechanics.md#probability-density)
- [Productive set](foundations-of-mathematics.md#productive-set)
- [Progression partition with nearly constant linear phase](additive-combinatorics.md#progression-partition-with-nearly-constant-linear-phase)
- [Projection (mathematics)](#projection-mathematics)
- [Pushforward filter](set-theory.md#pushforward-filter)
- [Pushforward ultrafilter](set-theory.md#pushforward-ultrafilter)
- [Quadratic polynomial](polynomial.md#quadratic-polynomial)
- [Quadratic spline](uniform-approximation.md#quadratic-spline)
- [Quantum collision finding](computer-science.md#quantum-collision-finding)
- [Quantum spectral filtering](quantum-theory.md#quantum-spectral-filtering)
- [Qutrit linear-function identification](quantum-theory.md#qutrit-linear-function-identification)
- [Random variable](random-variable.md)
- [Reduced-denominator function unbounded on every interval](mathematics.md#reduced-denominator-function-unbounded-on-every-interval)
- [Reversible density-ratio propagation](markov-process.md#reversible-density-ratio-propagation)
- [Right inverse](#right-inverse)
- [Rule of product](combinatorics.md#rule-of-product)
- [Sampling expansion by periodic Fourier projection](fourier-analysis.md#sampling-expansion-by-periodic-fourier-projection)
- [Sections of the degree-one line bundle on the projective line](complex-geometry.md#sections-of-the-degree-one-line-bundle-on-the-projective-line)
- [Self-bounding function](probability-inequality.md#self-bounding-function)
- [Skolem expansion](mathematical-logic.md#skolem-expansion)
- [Skolem function](mathematical-logic.md#skolem-function)
- [Smoothness](analysis.md#smoothness)
- [Solution of a differential equation](differential-equation.md#solution-of-a-differential-equation)
- [Spectral Lipschitz bound from Frobenius distance](linear-operator-theory.md#spectral-lipschitz-bound-from-frobenius-distance)
- [Step-function proof of the Riemann-Lebesgue lemma](fourier-analysis.md#step-function-proof-of-the-riemann-lebesgue-lemma)
- [Strict local maximum](analysis.md#strict-local-maximum)
- [Subdifferential under scalar affine composition](convex-optimization.md#subdifferential-under-scalar-affine-composition)
- [Substructure of a first-order structure](mathematical-logic.md#substructure-of-a-first-order-structure)
- [Supporting measure lemma for affine upper envelopes](topological-vector-space.md#supporting-measure-lemma-for-affine-upper-envelopes)
- [Supremum norm](functional-analysis.md#supremum-norm)
- [Tangent line](calculus.md#tangent-line)
- [Tangential boundary derivative](differential-equation.md#tangential-boundary-derivative)
- [Taylor expansion from a periodic derivative equation](calculus.md#taylor-expansion-from-a-periodic-derivative-equation)
- [Taylor series](calculus.md#taylor-series)
- [Tensorization of entropy](probability-inequality.md#tensorization-of-entropy)
- [Threshold Choquet representation in L-infinity](topological-vector-space.md#threshold-choquet-representation-in-l-infinity)
- [Total computable diagonal over primitive recursive syntax](foundations-of-mathematics.md#total-computable-diagonal-over-primitive-recursive-syntax)
- [Translation continuity in Lp](measure-theory.md#translation-continuity-in-lp)
- [Translation of a function](#translation-of-a-function)
- [Transport cost function](mathematical-optimization.md#transport-cost-function)
- [Ultraproduct proof of the Ehrenfeucht-Mostowski theorem](foundations-of-mathematics.md#ultraproduct-proof-of-the-ehrenfeucht-mostowski-theorem)
- [Unbounded torsion obstructs uniform control of four-term progressions](additive-combinatorics.md#unbounded-torsion-obstructs-uniform-control-of-four-term-progressions)
- [Uniform approximation](uniform-approximation.md)
- [Uniform negative curvature and global maximization](real-analysis.md#uniform-negative-curvature-and-global-maximization)
- [Uniform step approximation on a compact interval](uniform-approximation.md#uniform-step-approximation-on-a-compact-interval)
- [Uniformization of a binary relation](descriptive-set-theory.md#uniformization-of-a-binary-relation)
- [Universal property of Cartesian products](set-theory.md#universal-property-of-cartesian-products)
- [Upper semicontinuity](calculus.md#upper-semicontinuity)
- [Vector-valued function](#vector-valued-function)
- [Weak gradient](distribution-theory.md#weak-gradient)
- [Weighted inner product](linear-algebra.md#weighted-inner-product)
- [Wiener algebra](fourier-series.md#wiener-algebra)
- [Wiener-Hopf kernel](differential-equation.md#wiener-hopf-kernel)
- [Zero set](polynomial.md#zero-set)
