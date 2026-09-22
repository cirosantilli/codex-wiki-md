# Function

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Function_(mathematics))

A [function](function.md) $f:X\to Y$ assigns exactly one [output](theoretical-computer-science.md#output-computing) in the specified [codomain](#codomain) $Y$ to each [input](theoretical-computer-science.md#input-computer-science) in its [domain of a function](#domain-of-a-function) $X$. Its rule may be a formula, a finite table, or another unambiguous assignment. The outputs actually reached form its [image of a function](set-theory.md#image-of-a-function) $f(X)\subseteq Y$. A [codomain](#codomain) states where outputs are allowed; the [image of a function](set-theory.md#image-of-a-function) records where they actually land. Oscar Levin's introduction makes this distinction explicit. [Levin, Discrete Mathematics: An Open Introduction, Functions](https://discrete.openmathbooks.org/preview/sec_intro-functions.html).

For example, $f:\mathbb R\to\mathbb R$, $f(x)=x^2$, has the entire [real line](real-analysis.md#real-line) as its [domain of a function](#domain-of-a-function) and [codomain](#codomain), but its [image of a function](set-theory.md#image-of-a-function) is $[0,\infty)$. Both $-2$ and $2$ give the output $4$: several inputs sharing an output is permitted. Assigning two distinct outputs to one input is not permitted. A [partial function](#partial-function) can be undefined at some elements of a larger specified source [set](set.md); an ordinary [function](function.md) on $X$ must be defined at every element of $X$.

Three properties describe how a [function](function.md) uses its target. An [injective function](algebra.md#injective-function) never sends distinct inputs to the same output. A [surjective function](algebra.md#surjective-function) reaches every member of its specified [codomain](#codomain). A [bijection](#bijection) does both, pairing each source element with exactly one target element. These are different requirements, as finite arrow diagrams show.

<a id="image-injective-surjective-and-bijective-functions-have-different-output-patterns"></a>
![](function-injection-surjection-bijection.png)

**[Figure 1](#image-injective-surjective-and-bijective-functions-have-different-output-patterns). Injective, surjective and bijective functions have different output patterns**. Every source element has exactly one outgoing arrow. Left: an [injective function](algebra.md#injective-function) from three elements to four leaves one target unused. Middle: a [surjective function](algebra.md#surjective-function) from four elements to three reaches every target but merges two inputs. Right: a [bijection](#bijection) pairs three source elements with three targets, allowing every arrow to be reversed uniquely.

The chosen [codomain](#codomain) matters even when the formula does not change. The [function](function.md) $x\mapsto x^2$ from $\mathbb R$ to $\mathbb R$ is not [surjective](algebra.md#surjective-function), whereas the same rule from $\mathbb R$ to $[0,\infty)$ is [surjective](algebra.md#surjective-function). Both fail [injectivity](algebra.md#injective-function). Further restricting the [domain of a function](#domain-of-a-function) to $[0,\infty)$ makes it a [bijection](#bijection) onto $[0,\infty)$, with [square root](algebra.md#square-root) as its [inverse function](#inverse-function).

[Functions](function.md) make transformations composable: if $f:X\to Y$ and $g:Y\to Z$, their [function composition](#function-composition) is $(g\circ f)(x)=g(f(x))$. Identifying each intermediate [codomain](#codomain) prevents attempting to feed an output into a rule that is not defined there. When a transformation is a [bijection](#bijection), an [inverse function](#inverse-function) recovers the original input without ambiguity. This is useful whenever information must be transported or a calculation reversed.

**Table of contents**

- [Integer-valued function](#integer-valued-function)
- [Unimodal function](#unimodal-function)
- [Scalar-valued function](#scalar-valued-function)
- [Implicit function](#implicit-function)
- [Function evaluation](#function-evaluation)
- [Function input](#function-input)
- [Function output](#function-output)
- [Quotient of functions](#quotient-of-functions)
- [Codomain](#codomain)
- [Self-map](#self-map)
  - [Idempotent function](#idempotent-function)
    - [Idempotent matrix](#idempotent-matrix)
- [Function composition](#function-composition)
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
  - [Preserve the domain when simplifying a function](#preserve-the-domain-when-simplifying-a-function)
  - [Domain of a partial function](#domain-of-a-partial-function)
- [Restriction (mathematics)](#restriction-mathematics)
- [Function class](#function-class)
- [Support](#support)
  - [Compact support](#compact-support)
- [Identity function](#identity-function)
- [Inverse function](#inverse-function)
  - [Horizontal line test](#horizontal-line-test)
  - [Inverse function rule](#inverse-function-rule)
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
- [Nonconstant function](#nonconstant-function)
- [Real-valued function](#real-valued-function)
  - [Global maximum](#global-maximum)
  - [Positive part of a real-valued function](#positive-part-of-a-real-valued-function)
  - [Negative part of a real-valued function](#negative-part-of-a-real-valued-function)
- [Bijection](#bijection)
- [Periodic function](#periodic-function)
  - [Periodic extension](#periodic-extension)
  - [Fundamental period of a function](#fundamental-period-of-a-function)
    - [Continuous periodic functions have a least positive period](#continuous-periodic-functions-have-a-least-positive-period)
    - [Periodic function without a least positive period](#periodic-function-without-a-least-positive-period)
  - [Period group of a function](#period-group-of-a-function)
  - [Simply periodic function](#simply-periodic-function)
  - [Cardinality of integer-periodic function spaces](#cardinality-of-integer-periodic-function-spaces)
  - [Period average](#period-average)
  - [Triangular wave](#triangular-wave)
    - [Fourier cosine series of a triangular wave](#fourier-cosine-series-of-a-triangular-wave)

## Integer-valued function

↑ **Parent:** [Function](function.md)

## Unimodal function

↑ **Parent:** [Function](function.md)

## Scalar-valued function

↑ **Parent:** [Function](function.md)

A [scalar-valued function](#scalar-valued-function) is a [function](function.md) whose [codomain](#codomain) is a [field](algebra.md#field), typically the [real numbers](arithmetic.md#real-number) or [complex numbers](complex-analysis.md#complex-number). Its output is a single [scalar](vector-space.md#scalar), while its input can belong to an arbitrary [set](set.md). For example, the square of the [norm](normed-vector-space.md#norm) of a [vector](vector-space.md#vector) is real-valued. In a relativistic application, being scalar-valued alone does not establish [Lorentz invariance](special-relativity.md#lorentz-invariance): the transformation of the input and of the complete quantity must also be specified.

## Implicit function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_function)

An [implicit function](#implicit-function) is a [function](function.md) specified through a relation between its input and output, rather than an explicit output formula. Locally, an [equation](algebra.md#equation) $F(x,y)=0$ may specify $y=g(x)$ if one output $y$ is selected for each input $x$ in a suitable domain. Different branches can define different [functions](function.md); the relation itself need not give a unique output globally. For example, $x^2+y^2=1$ gives the two branches $y=\pm\sqrt{1-x^2}$ on $-1<x<1$.

The [implicit function theorem](multivariable-calculus.md#implicit-function-theorem) gives sufficient conditions for a unique local differentiable branch, while [implicit differentiation](multivariable-calculus.md#implicit-differentiation) computes its [derivative](calculus.md#derivative) by the [chain rule](calculus.md#chain-rule). If $F$ is continuously differentiable and $F_y\ne0$, that [derivative](calculus.md#derivative) is $g'(x)=-F_x/F_y$ along the branch.

## Function evaluation

↑ **Parent:** [Function](function.md)

[Function evaluation](#function-evaluation) determines the [function output](#function-output) $f(x)$ for a specified [function input](#function-input) $x$ in the [domain of a function](#domain-of-a-function). [Numerical integration](numerical-integration.md) uses these values at selected [quadrature nodes](numerical-integration.md#quadrature-node).

## Function input

↑ **Parent:** [Function](function.md)

A [function input](#function-input) to a [function](function.md) $f:X\to Y$ is an element $x$ of its [domain of a function](#domain-of-a-function) $X$, also called its argument. The corresponding [function output](#function-output) is $f(x)$.

## Function output

↑ **Parent:** [Function](function.md)

A [function output](#function-output) is the value $f(x)$ assigned by a [function](function.md) $f:X\to Y$ to a [function input](#function-input) $x$. It belongs to the [codomain](#codomain) $Y$; all such [function outputs](#function-output) together form the [image of a function](set-theory.md#image-of-a-function) $f(X)$.

## Quotient of functions

↑ **Parent:** [Function](function.md)

For [functions](function.md) $f$ and $g$ taking values in the same [field](algebra.md#field), their [quotient of functions](#quotient-of-functions) is defined by $(f/g)(x)=f(x)/g(x)$ on the common [domain of a function](#domain-of-a-function) restricted to points where $g(x)\ne0$. Thus $f(x)=1$ and $g(x)=x$ on the [real line](real-analysis.md#real-line) give a [quotient of functions](#quotient-of-functions) defined only for $x\ne0$.

## Codomain

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Codomain)

The [codomain](#codomain) of a [function](function.md) is its specified target [set](set.md). The [image of a function](set-theory.md#image-of-a-function) is a [subset](set.md#subset) of the [codomain](#codomain), and equals it precisely for a [surjective function](algebra.md#surjective-function). Changing a [codomain](#codomain) can change whether the same input-output rule is [surjective](algebra.md#surjective-function), as the [quadratic function](polynomial.md#quadratic-function) examples under [function](function.md) show.

## Self-map

↑ **Parent:** [Function](function.md)

A [self-map](#self-map) is a [function](function.md) whose [domain of a function](#domain-of-a-function) and [codomain](#codomain) are the same [set](set.md). It need not be a [bijection](#bijection): a [constant function](#constant-function) on a two-element [set](set.md) is a [self-map](#self-map) that merges its [inputs](theoretical-computer-science.md#input-computer-science). [Self-maps](#self-map) can always be composed with one another, and all [self-maps](#self-map) of a specified [set](set.md) form its [full transformation monoid](algebraic-operation.md#full-transformation-monoid).

### Idempotent function

↑ **Parent:** [Self-map](#self-map)

A [self-map](#self-map) $f:X\to X$ is idempotent if its [function composition](#function-composition) with itself leaves it unchanged: $f(f(x))=f(x)$ for every $x$. Equivalently, every element of its [image of a function](set-theory.md#image-of-a-function) is a [fixed point](#fixed-point). For example, the [function](function.md) on $\{a,b,c\}$ sending $a$ to $b$, $b$ to $b$, and $c$ to $c$ is idempotent. A second application makes no further change.

#### Idempotent matrix

↑ **Parent:** [Idempotent function](#idempotent-function)

## Function composition

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Function_composition)

For [functions](function.md) $f:X\to Y$ and $g:Y\to Z$, their [function composition](#function-composition) is $g\circ f:X\to Z$, defined by $(g\circ f)(x)=g(f(x))$. The rightmost [function](function.md) is applied first. Matching the intermediate [codomain](#codomain) and [domain of a function](#domain-of-a-function) makes the expression well-defined.

For [self-maps](#self-map) of the [real numbers](arithmetic.md#real-number), take $f(x)=x+1$ and $g(x)=2x$. Then $(g\circ f)(x)=2x+2$, whereas $(f\circ g)(x)=2x+1$. Thus [function composition](#function-composition) need not be [commutative](algebraic-operation.md#commutativity). It does have the [associative property](algebraic-operation.md#associative-property): both $(h\circ g)\circ f$ and $h\circ(g\circ f)$ evaluate to $h(g(f(x)))$ whenever each intermediate [codomain](#codomain) matches the next [domain of a function](#domain-of-a-function). The [identity function](#identity-function) leaves composition unchanged, making [self-maps](#self-map) particularly useful as a [monoid](algebraic-operation.md#monoid) of transformations.

## Germ (mathematics)

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Germ_(mathematics))

A [germ](#germ-mathematics) at a point is an [equivalence class](set-theory.md#equivalence-class) of [functions](function.md) defined on a [neighbourhood](topology.md#neighbourhood-mathematics) of the point: two representatives are equivalent if they agree on some smaller [neighbourhood](topology.md#neighbourhood-mathematics). A [germ of a holomorphic function](riemann-surfaces.md#germ-of-a-holomorphic-function) requires its representatives to be [holomorphic functions](holomorphic-function.md); smooth and continuous germs use their corresponding classes of [functions](function.md). The [germ](#germ-mathematics) retains local behavior while forgetting the representative's values farther from the point.

## Nonnegative function

↑ **Parent:** [Function](function.md)

A real-valued function is nonnegative when all its values are at least zero. Products and nonnegative linear combinations of nonnegative functions remain nonnegative. A nonnegative partition of unity gives convex combinations, hence a convex-hull bound for a geometric basis.

## Commuting functions

↑ **Parent:** [Function](function.md)

Two self-maps $R,S:X\to X$ commute when $R\circ S=S\circ R$. Induction then gives $R^n\circ S=S\circ R^n$ and $R^n\circ S^m=S^m\circ R^n$ for all nonnegative integers $m,n$. Sharing a fixed point or invariant set does not by itself imply commutation. For rational sphere maps of degrees at least two, commutation does imply equality of their [Fatou sets](complex-dynamics.md#fatou-set) and [Julia sets](complex-dynamics.md#julia-set), by the [commuting rational maps of degree at least two have the same Julia set](complex-dynamics.md#commuting-rational-maps-of-degree-at-least-two-have-the-same-julia-set) theorem.

## Finite modification of the identity on the real line

↑ **Parent:** [Function](function.md)

A finite modification agrees with the [identity map](#identity-function) outside a finite exceptional [set](set.md). Sorting that [set](set.md) gives a unique finite record of pairs $(x,f(x))$. [Real-number pairing by separated digits](algebra.md#real-number-pairing-by-separated-digits) encodes the record in $(0,1)$, and placing length-$n$ records in disjoint intervals $(n,n+1)$ gives an [injection](algebra.md#injective-function) from all finite modifications into the real line. Conversely, changing the value at one fixed point gives a real-parameter family, so the [Cantor-Schröder-Bernstein theorem](cardinal-number.md#cantor-schroder-bernstein-theorem) shows this family has continuum cardinality.

## Pointwise periodic self-map

↑ **Parent:** [Function](function.md)

A pointwise periodic self-map returns each point to itself after a positive number of iterates which may depend on the point. It is a [bijection](#bijection): each finite cycle supplies predecessors; equality of two images can be undone by an iterate with an exponent one below a common multiple of the two periods. The [set](set.md) consequently decomposes into disjoint finite [permutation cycles](finite-group-theory.md#permutation-cycle). Pointwise periodicity does not imply that one iterate is the identity on an infinite [set](set.md).

### Uniform period criterion for pointwise periodic maps

↑ **Parent:** [Pointwise periodic self-map](#pointwise-periodic-self-map)

A [pointwise periodic self-map](#pointwise-periodic-self-map) has a uniform positive period exactly when its finite cycle lengths are bounded. A uniform period is divisible by every length; conversely, bounded lengths divide the [least common multiple](divisibility.md#least-common-multiple) of $1,\ldots,M$ for some bound $M$. Arbitrarily many bounded-length cycles are allowed. Every such [map](#function-class) on a [finite set](set.md#finite-set) has a uniform period. On any infinite [set](set.md) containing a countably infinite subset, cycles of unbounded finite lengths and fixed points elsewhere give a counterexample. Thus, with the usual [axiom of choice](set-theory.md#axiom-of-choice) assumption, the [sets](set.md) on which every pointwise periodic self-map has a uniform period are exactly finite [sets](set.md).

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

A function collision is a pair of distinct inputs $x\neq x'$ with $f(x)=f(x')$. An [injective function](algebra.md#injective-function) has no collisions. For a two-to-one function every nonempty [fiber](#fiber-of-a-function) has two elements and hence one unordered collision pair. Finding such a pair through an oracle is the task of [quantum collision finding](theoretical-computer-science.md#quantum-collision-finding).

In the finite example under [image and preimage of a function](set-theory.md#image-and-preimage-of-a-function), the pair $\{a,b\}$ is a [function collision](#function-collision): both inputs give zero. The [function](function.md) retains their shared output but loses the distinction between them. If a [finite set](set.md#finite-set) has more inputs than the number of available outputs, the [pigeonhole principle](combinatorics.md#pigeonhole-principle) forces a [function collision](#function-collision). Equal source and target [cardinalities](cardinal-number.md#cardinality) alone do not prevent one.

For a finite [function](function.md), let $m_y$ be the [cardinality](cardinal-number.md#cardinality) of its [fiber of a function](#fiber-of-a-function) over $y$. The number of unordered [function collisions](#function-collision) is $\sum_y\binom{m_y}{2}$, because each pair must lie in one common [fiber](#fiber-of-a-function). The example's nonempty fiber sizes are $2,1,1$, giving exactly one collision pair.

## Fiber of a function

↑ **Parent:** [Function](function.md)

For a [function](function.md) $f:X\to Y$ and $y\in Y$, its [fiber of a function](#fiber-of-a-function) over $y$ is the [set](set.md) of all inputs producing that one output:

$$
f^{-1}(y)=f^{-1}(\{y\})=\{x\in X:f(x)=y\}.
$$

Here $f^{-1}(y)$ is shorthand for a [preimage](set-theory.md#preimage) of a [singleton set](set.md#singleton-mathematics), rather than a claim that an [inverse function](#inverse-function) exists. A fiber can contain several inputs or be empty. It describes exactly which distinctions the [function](function.md) forgets.

For the finite [function](function.md) under [image and preimage of a function](set-theory.md#image-and-preimage-of-a-function), the fibers over $0,1,2,3$ are $\{a,b\}$, $\{c\}$, $\{d\}$ and the [empty set](set.md#empty-set), respectively. The nonempty fibers form a [partition of a set](set.md#partition-of-a-set): they are disjoint [sets](set.md) whose [union](set.md#set-union) is the [domain of a function](#domain-of-a-function). Every input belongs to the fiber over its unique output, and two fibers with distinct output labels cannot share an input. A [function](function.md) is [injective](algebra.md#injective-function) exactly when every fiber has at most one member; it is [surjective](algebra.md#surjective-function) exactly when every member of its specified [codomain](#codomain) has a nonempty fiber.

<a id="image-a-preimage-collects-complete-fibers-the-outputs-0-2-select-the-fibers-a-b-and-d"></a>
![](function-image-preimage-subset-flow.png)

**[Figure 2](#image-a-preimage-collects-complete-fibers-the-outputs-0-2-select-the-fibers-a-b-and-d). A preimage collects complete fibers: the outputs $\{0,2\}$ select the fibers $\{a,b\}$ and $\{d\}$**.

More generally, $f^{-1}(U)$ is the [union](set.md#set-union) of the fibers over all $y\in U$. The relation $x\sim x'$ defined by $f(x)=f(x')$ is an [equivalence relation](set-theory.md#equivalence-relation), and its [equivalence classes](set-theory.md#equivalence-class) are precisely the nonempty fibers. The resulting [quotient set](set-theory.md#quotient-set) is naturally in [bijection](#bijection) with the [image of a function](set-theory.md#image-of-a-function). This links an input partition to the output values actually reached, without choosing one representative from each class.

Fibers are useful when an output is known but the input is not uniquely determined. A [solution set](set.md#solution-set) $g^{-1}(\{0\})$ is one fiber, and [factorization through a surjection](#factorization-through-a-surjection) explains when another [function](function.md) depends only on the retained output. Quantum [hidden subgroup problem](quantum-fourier-transform.md#hidden-subgroup-problem) algorithms use [functions](function.md) whose fibers are [cosets](group-theory.md#coset), giving the same idea a structured form in [group theory](group-theory.md).

### Factorization through a surjection

↑ **Parent:** [Fiber of a function](#fiber-of-a-function)

For a [surjective function](algebra.md#surjective-function) $f:B\to A$ and a function $g:B\to C$, there is a unique function $h:A\to C$ with $g=h\circ f$ if and only if $g$ is constant on each [fiber of a function](#fiber-of-a-function) of $f$. Define $h(a)$ to be the common value on $f^{-1}(a)$; it is well-defined and unique because that fiber is nonempty. This uniquely specified value requires no simultaneous arbitrary choices.

For a concrete example, restrict the [codomain](#codomain) of the finite [function](function.md) above to its [image of a function](set-theory.md#image-of-a-function) $I=\{0,1,2\}$, making $f:A\to I$ [surjective](algebra.md#surjective-function). Define $g(a)=g(b)=5$, $g(c)=7$ and $g(d)=9$. Then $h(y)=2y+5$ on $I$ gives $g=h\circ f$: knowing the output of $f$ is enough to compute $g$. If instead $g(a)\ne g(b)$, no such $h$ can exist, because $h(f(a))=h(f(b))$ must be the same value.

The [surjectivity](algebra.md#surjective-function) assumption supplies uniqueness on the full target. If the original unused target value three were retained, the factorization would impose no condition on $h(3)$, and different extensions could agree on every actual input. Thus [factorization through a surjection](#factorization-through-a-surjection) formalizes when a compressed description retains all information needed for a later calculation.

// Target: combinatorics.bigb

## Translation of a function

↑ **Parent:** [Function](function.md)

Translation shifts the argument without changing the shape of a [function](function.md). On the [real line](real-analysis.md#real-line), the displayed convention shifts a graph to the right by $h$. [Lebesgue measure](measure-theory.md#lebesgue-measure) invariance preserves every finite [Lp norm](real-analysis.md#lp-norm); its [Fourier transform](fourier-transform.md) is multiplied by $e^{-ih\xi}$.

## Graph of a function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_of_a_function)

For a [function](function.md) $f:A\to B$, its graph is the subset $\{(x,f(x)):x\in A\}$ of $A\times B$. It differs from a [graph](graph.md) in [graph theory](graph-theory.md). A solution curve of a scalar differential equation can be a graph over its independent coordinate.

### Compact graph of a continuous map

↑ **Parent:** [Graph of a function](#graph-of-a-function)

The map $x\mapsto(x,f(x))$ is continuous into the [product topology](geometry-and-topology.md#product-topology). It maps a [compact space](topology.md#compact-space) $X$ onto the [graph of a function](#graph-of-a-function) of a continuous $f$. Hence that graph is compact, whether or not the [codomain](#codomain) is a [Hausdorff space](topology.md#hausdorff-space). Projection to $X$ is its continuous inverse.

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

### Preserve the domain when simplifying a function

↑ **Parent:** [Domain of a function](#domain-of-a-function)

An algebraic simplification proves equality only where both original and transformed expressions are defined. If a cancelled factor vanishes at a point, the simplified expression may instead describe an extension to that point. For example,

$$
\frac1{1+\tan x}=\frac{\cos x}{\cos x+\sin x}
$$

holds only when $\cos x\ne0$ and $\cos x+\sin x\ne0$. The right side is zero at $x=\pi/2+k\pi$, but the left side is undefined there. A graph of the original [function](function.md) must retain those holes. The extension may be useful, but it is a different [function](function.md) with a larger [domain of a function](#domain-of-a-function).

### Domain of a partial function

↑ **Parent:** [Domain of a function](#domain-of-a-function)

For a partial function $f:X\rightharpoonup Y$, the domain is the subset $\{x\in X:f(x)\text{ is defined}\}$. Outside this subset, evaluation of $f$ is undefined.

## Restriction (mathematics)

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Restriction_(mathematics))

For a [function](function.md) $f:X\to Y$ and a [subset](set.md#subset) $A\subseteq X$, its [restriction](#restriction-mathematics) $f|_A$ keeps the same values but allows only inputs in $A$. Restricting the [domain of a function](#domain-of-a-function) can remove collisions and permit an [inverse function](#inverse-function), as the nonnegative [quadratic function](polynomial.md#quadratic-function) example shows. This changes the allowed inputs; it is different from keeping the inputs and changing the [codomain](#codomain).

## Function class

↑ **Parent:** [Function](function.md)

A [function class](#function-class) is a [set](set.md) whose elements are [functions](function.md), usually sharing a common [domain of a function](#domain-of-a-function) and [codomain](#codomain).

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

The [identity function](#identity-function) on a [set](set.md) $X$ maps each $x\in X$ to itself: $\operatorname{id}_X(x)=x$. It changes no information. For every [function](function.md) $f:X\to Y$, [function composition](#function-composition) satisfies $f\circ\operatorname{id}_X=f$ and $\operatorname{id}_Y\circ f=f$. The subscripts specify the appropriate source or target [set](set.md). An [inverse function](#inverse-function) reverses a [bijection](#bijection) exactly when the two possible compositions are these [identity functions](#identity-function).

## Inverse function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_function)

An [inverse function](#inverse-function) reverses a [bijection](#bijection). For $f:X\to Y$, it is a [function](function.md) $g:Y\to X$ satisfying

$$
g\circ f=\operatorname{id}_X,\qquad f\circ g=\operatorname{id}_Y.
$$

Equivalently, $g(f(x))=x$ for all $x\in X$ and $f(g(y))=y$ for all $y\in Y$. We write $g=f^{-1}$. The superscript denotes reversal through [function composition](#function-composition); it does not mean the pointwise [multiplicative inverse](arithmetic.md#multiplicative-inverse) $1/f(x)$. The [preimage](set-theory.md#preimage) notation $f^{-1}(B)$ for a [set](set.md) $B$ is also distinct: a [preimage](set-theory.md#preimage) exists even when no [inverse function](#inverse-function) exists.

For a computed example, let $f:\mathbb R\to\mathbb R$ be $f(x)=2x+1$. Solving $y=2x+1$ for $x$ gives $g(y)=(y-1)/2$. Thus $f(1)=3$ and $g(3)=1$; direct substitution gives $g(f(x))=x$ and $f(g(y))=y$ throughout the [real line](real-analysis.md#real-line). In contrast, $1/f(3)=1/7$, which does not undo $f(1)=3$.

Why must $f$ be a [bijection](#bijection)? If $f(x_1)=f(x_2)$, applying $g$ gives $x_1=x_2$, proving [injectivity](algebra.md#injective-function). For any $y\in Y$, the equation $f(g(y))=y$ supplies a source element, proving [surjectivity](algebra.md#surjective-function). Conversely, a [bijection](#bijection) supplies exactly one predecessor for each $y$, defining a unique [inverse function](#inverse-function). A [left inverse](#left-inverse) or [right inverse](#right-inverse) requires only one of the two composition identities.

For $f(x)=x^2$ on the [real line](real-analysis.md#real-line), the equation $f(x)=4$ has two solutions, $x=\pm2$, so its arrows cannot be reversed as one [function](function.md) on all inputs. The [restriction](#restriction-mathematics) to $[0,\infty)$ removes that ambiguity. As a [bijection](#bijection) from $[0,\infty)$ onto $[0,\infty)$, it has [inverse function](#inverse-function) $g(y)=\sqrt y$. The identity $\sqrt{x^2}=|x|$ explains why $\sqrt{x^2}=x$ works on the restricted [domain of a function](#domain-of-a-function) but fails for negative $x$. [OpenStax, inverse functions and domain restrictions](https://openstax.org/books/calculus-volume-1/pages/1-4-inverse-functions).

<a id="image-an-inverse-function-swaps-the-input-and-output-coordinates"></a>
![](inverse-function-reflection.png)

**[Figure 3](#image-an-inverse-function-swaps-the-input-and-output-coordinates). An inverse function swaps the input and output coordinates**. Left: the [function graphs](#graph-of-a-function) of $f(x)=2x+1$ and its [inverse function](#inverse-function) $g(x)=(x-1)/2$ are reflections across the [line](euclidean-geometry.md#straight-line) $y=x$; the points $(1,3)$ and $(3,1)$ correspond. Right: the nonnegative [restriction](#restriction-mathematics) $x\mapsto x^2$ and the [square root](algebra.md#square-root) have the same reflection relation. Their displayed portions lie in the first [quadrant](linear-algebra.md#quadrant-plane-geometry) or on its [boundary](topology.md#boundary-of-a-set).

More generally, $(a,b)$ lies on the [graph of a function](#graph-of-a-function) $f$ precisely when $(b,a)$ lies on the [graph of a function](#graph-of-a-function) of its [inverse function](#inverse-function). This coordinate swap explains the geometric reflection and the [horizontal line test](#horizontal-line-test). It also explains why inverse sensitivity is reciprocal locally: the [inverse function rule](#inverse-function-rule) divides by the original [derivative](calculus.md#derivative) at the corresponding input, when that [derivative](calculus.md#derivative) is nonzero.

### Horizontal line test

↑ **Parent:** [Inverse function](#inverse-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horizontal_line_test)

For a real-valued [function](function.md) drawn in the plane, the [horizontal line test](#horizontal-line-test) asks whether every horizontal [line](euclidean-geometry.md#straight-line) intersects its [function graph](#graph-of-a-function) at most once. This is exactly [injectivity](algebra.md#injective-function), since two intersections at the same height mean two inputs have the same output. A missing height is compatible with [injectivity](algebra.md#injective-function), so an [inverse function](#inverse-function) is then defined on the [image of a function](set-theory.md#image-of-a-function); it is an inverse on the entire specified [codomain](#codomain) only when [surjectivity](algebra.md#surjective-function) also holds.

### Inverse function rule

↑ **Parent:** [Inverse function](#inverse-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_function_rule)

Suppose $f$ is [continuously differentiable](multivariable-calculus.md#continuously-differentiable-function) near $a$ with $f'(a)\ne0$. It has a local [inverse function](#inverse-function) $g$ near $b=f(a)$, and

$$
g'(b)=\frac1{f'(a)}=\frac1{f'(g(b))}.
$$

The [chain rule](calculus.md#chain-rule) applied to $g(f(x))=x$ gives the formula. The nonzero [derivative](calculus.md#derivative) condition also ensures local invertibility; it does not assert a global [inverse function](#inverse-function) on an arbitrary larger [domain of a function](#domain-of-a-function). For $f(x)=x^2$ at $a=2$, the corresponding output is $b=4$, and the [square root](algebra.md#square-root)'s [derivative](calculus.md#derivative) there is $1/4$. At $a=0$, this division is unavailable: the nonnegative restriction still has a [square root](algebra.md#square-root) inverse, but its finite [derivative](calculus.md#derivative) at zero does not exist. [OpenStax, the inverse function rule and corresponding evaluation points](https://openstax.org/books/calculus-volume-1/pages/3-7-derivatives-of-inverse-functions).

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

Between two prescribed values, [linear interpolation](#linear-interpolation) assigns $(1-t)f(a)+tf(b)$ at $(1-t)a+tb$, for $0\leq t\leq1$. Joining successive samples produces a [piecewise linear function](#piecewise-linear-function). For a [continuous function](calculus.md#continuous-function) on a compact interval, interpolants along grids with mesh tending to zero converge in the [uniform norm](normed-vector-space.md#supremum-norm); their error is bounded by the [modulus of continuity](topological-analysis.md#modulus-of-continuity) at the mesh size.

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

On a nonempty [domain of a function](#domain-of-a-function) $X$, a constant [function](function.md) $f:X\to Y$ has one fixed value $c$ in its [codomain](#codomain):

$$
\boxed{f(x)=c\qquad\text{for every }x\in X.}
$$

For example, $f(x)=2$ on the [real line](real-analysis.md#real-line) is a horizontal graph. Its [image of a function](set-theory.md#image-of-a-function) is the [singleton](set.md#singleton-mathematics) $\{2\}$ even though its [domain of a function](#domain-of-a-function) has infinitely many inputs. A [constant function](#constant-function) from the [real line](real-analysis.md#real-line) to the [real numbers](arithmetic.md#real-number) has [derivative](calculus.md#derivative) zero and every nonzero real [period of a function](mathematics.md#period-of-a-function); there is no smallest positive [period](mathematics.md#period-of-a-function). It supplies a reference level from which variation can be measured.

A constant map between [vector spaces](vector-space.md) is a [linear map](vector-space.md#linear-map) only when its value is the [zero vector](vector-space.md#zero-vector), since a [linear map](vector-space.md#linear-map) must preserve zero. A nonzero constant map is still an [affine map](geometry-and-topology.md#affine-map). In a [Fourier series](fourier-series.md), the constant term records the [period average](#period-average), while the other terms describe oscillation around that level.

## Nonconstant function

↑ **Parent:** [Function](function.md)

A [function](function.md) is nonconstant when two inputs in its [domain of a function](#domain-of-a-function) have different outputs. For example, $f(x)=x^2$ on the [real line](real-analysis.md#real-line) is nonconstant, whereas the same rule restricted to $\{-1,1\}$ is a [constant function](#constant-function).

## Real-valued function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real-valued_function)

A [real-valued function](#real-valued-function) has [codomain](#codomain) contained in the [real numbers](arithmetic.md#real-number).

### Global maximum

↑ **Parent:** [Real-valued function](#real-valued-function)

A global maximum of a real-valued function is a value $f(x_0)$ satisfying $f(x)\leq f(x_0)$ throughout its domain.

A [global maximum](#global-maximum) is one type of [extremum of a real-valued function](mathematical-optimization.md#maximum-and-minimum); global minima reverse the inequality.

### Positive part of a real-valued function

↑ **Parent:** [Real-valued function](#real-valued-function)

The [positive part](#positive-part-of-a-real-valued-function) of a [real-valued function](#real-valued-function) $f$ is $f_+(x)=\max(0,f(x))$. Together with its [negative part](#negative-part-of-a-real-valued-function), it gives $f=f_+-f_-$ and $|f|=f_++f_-$.

### Negative part of a real-valued function

↑ **Parent:** [Real-valued function](#real-valued-function)

The [negative part](#negative-part-of-a-real-valued-function) of a [real-valued function](#real-valued-function) $f$ is the nonnegative [function](function.md) $f_-(x)=\max(0,-f(x))$. It records the magnitude of the negative values, rather than retaining their sign: if $f(x)=-3$, then $f_-(x)=3$. Together with the [positive part](#positive-part-of-a-real-valued-function), it gives $f=f_+-f_-$ and $|f|=f_++f_-$. This decomposition defines the [Lebesgue integral](measure-theory.md#lebesgue-integral) of a signed [function](function.md) and makes the [integrability](measure-theory.md#integrability) condition explicit.

## Bijection

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bijection)

A [bijection](#bijection) $f:X\to Y$ is a [function](function.md) that is both [injective](algebra.md#injective-function) and [surjective](algebra.md#surjective-function): each element of its [codomain](#codomain) is the output of exactly one element of its [domain of a function](#domain-of-a-function). The two requirements exclude unused targets and merged inputs respectively. The finite example $f(A)=1$, $f(B)=2$, $f(C)=3$ is a [bijection](#bijection) from $\{A,B,C\}$ to $\{1,2,3\}$, whereas adding an unused target $4$ makes that same rule fail [surjectivity](algebra.md#surjective-function).

A [bijection](#bijection) gives an [inverse function](#inverse-function) by reversing every pairing. Conversely, a two-sided [inverse function](#inverse-function) implies a [bijection](#bijection), as the proof under [inverse function](#inverse-function) shows. This is useful for transporting structures without losing or identifying elements. It also defines equality of [cardinality](cardinal-number.md#cardinality): two [sets](set.md) have equal [cardinality](cardinal-number.md#cardinality) exactly when a [bijection](#bijection) pairs them. An infinite example is $n\mapsto2n$ from the [integers](integer.md) to the even [integers](integer.md), with inverse $m\mapsto m/2$ on that specified [codomain](#codomain). A proper [subset](set.md#subset) can therefore have the same [cardinality](cardinal-number.md#cardinality) as an infinite [set](set.md). [Levin, functions: injections, surjections and bijections](https://discrete.openmathbooks.org/preview/sec_intro-functions.html).

## Periodic function

↑ **Parent:** [Function](function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Periodic_function)

A periodic [function](function.md) repeats exactly after a nonzero shift of its input. For $f:\mathbb R\to Y$, a positive [period of a function](mathematics.md#period-of-a-function) $T$ satisfies

$$
\boxed{f(x+T)=f(x)\qquad\text{for every }x\in\mathbb R.}
$$

One interval of length $T$ therefore determines the whole [function](function.md). For another [domain of a function](#domain-of-a-function) $D$, a period must also preserve the domain, $D+T=D$; equality only where two domains happen to overlap is weaker. Periodicity is an exact [translation of a function](#translation-of-a-function) symmetry, rather than merely two similar-looking pieces of its graph.

The [sine](geometry-and-topology.md#sine) $\sin(2\pi x)$ has [fundamental period](#fundamental-period-of-a-function) one. The [function](function.md) $\sin^2(2\pi x)$ repeats after half a unit: the [sine](geometry-and-topology.md#sine) changes sign under that shift, but squaring removes the sign. The mixed [function](function.md) $g(x)=2+\sin(2\pi x)+\tfrac12\cos(4\pi x)$ again has [fundamental period](#fundamental-period-of-a-function) one. All positive integer multiples of a [period](mathematics.md#period-of-a-function) are periods, so specifying one period need not identify the shortest repetition.

<a id="image-mixed-harmonics-a-squared-sine-and-a-constant-have-different-sets-of-periods"></a>
![](periodic-functions-repetition-and-fundamental-period.png)

**[Figure 4](#image-mixed-harmonics-a-squared-sine-and-a-constant-have-different-sets-of-periods). Mixed harmonics, a squared sine, and a constant have different sets of periods**.

If the input is time and $T_0$ is the [fundamental period](#fundamental-period-of-a-function), the [frequency](wave.md#frequency) is $1/T_0$ and the [angular frequency](lagrangian-mechanics.md#angular-frequency) is $2\pi/T_0$. Repetition lets a [Fourier series](fourier-series.md) describe a cycle using [sines](geometry-and-topology.md#sine) and [cosines](geometry-and-topology.md#cosine); the [period average](#period-average) separates the reference level from the oscillating terms. Strang develops this representation and its [Fourier coefficients](fourier-series.md#fourier-coefficient) in §4.1 of [Computational Science and Engineering by Gilbert Strang](mathematics-bibliography.md#computational-science-and-engineering-by-gilbert-strang).[§4.1; pp. 317](mathematics-bibliography.md#computational-science-and-engineering-by-gilbert-strang/fourier-series-for-periodic-functions)

This connection grew out of a physical problem. In his 1822 book [Théorie analytique de la chaleur by Joseph Fourier](mathematics-bibliography.md#theorie-analytique-de-la-chaleur-by-joseph-fourier), [Joseph Fourier](mathematics.md#joseph-fourier) used [periodic functions](#periodic-function) to extend profiles beyond their initial interval while treating [heat conduction](heat.md#thermal-conduction). Chapter III, §§233–234 combines [even functions](calculus.md#even-function) and [odd functions](calculus.md#odd-function) into sine–cosine expansions and rescales their period.[§§233–234; equation (p)](mathematics-bibliography.md#theorie-analytique-de-la-chaleur-by-joseph-fourier/propagation-de-la-chaleur-dans-un-solide-rectangle-infini) A modern [Fourier series](fourier-series.md) interpretation still requires the appropriate convergence conditions.

A [constant function](#constant-function) has every real shift as a period and no [fundamental period](#fundamental-period-of-a-function). Without [continuity](calculus.md#continuous-function), even a [nonconstant](#nonconstant-function) [periodic function](#periodic-function) can lack a smallest positive period; [periodic function without a least positive period](#periodic-function-without-a-least-positive-period) gives a concrete example. The [period group of a function](#period-group-of-a-function) organizes all these possibilities.

### Periodic extension

↑ **Parent:** [Periodic function](#periodic-function)

For $T>0$, values of a [function](function.md) $f$ on a half-open interval $[a,a+T)$ determine its periodic extension to the [real line](real-analysis.md#real-line): choose the unique [integer](integer.md) $k$ with $x-kT\in[a,a+T)$ and set $F(x)=f(x-kT)$. The resulting [periodic function](#periodic-function) has [period](mathematics.md#period-of-a-function) $T$. If the endpoint limits of $f$ differ, the extension has a [jump discontinuity](calculus.md#jump-discontinuity) at every period boundary. Under the usual piecewise-smooth convergence hypotheses, its [Fourier series](fourier-series.md) takes the average of the two one-sided limits there; an assigned value at an isolated endpoint does not change the [Fourier coefficients](fourier-series.md#fourier-coefficient).

### Fundamental period of a function

↑ **Parent:** [Periodic function](#periodic-function)

The fundamental period is the least positive [period of a function](mathematics.md#period-of-a-function), when one exists. For $f(x)=\sin(2\pi x)$ it is one; for $f(x)=\sin^2(2\pi x)$ it is $1/2$. A [periodic function](#periodic-function) need not have a fundamental period: a [constant function](#constant-function) has every positive period, and [periodic function without a least positive period](#periodic-function-without-a-least-positive-period) is a [nonconstant](#nonconstant-function) exception. Every [nonconstant](#nonconstant-function) [real-valued function](#real-valued-function) that is [continuous](calculus.md#continuous-function) and [periodic](#periodic-function) on the [real line](real-analysis.md#real-line) does have a least positive period.

#### Continuous periodic functions have a least positive period

↑ **Parent:** [Fundamental period of a function](#fundamental-period-of-a-function)

For a real-valued [continuous function](calculus.md#continuous-function), the [period group of a function](#period-group-of-a-function) is a [closed subgroup](topological-group.md#closed-subgroup): if periods $T_n$ tend to $T$, [continuity](calculus.md#continuous-function) passes $f(x+T_n)=f(x)$ to the limit. If positive periods could tend to zero, integer multiples of those periods would approach any prescribed displacement $y-x$, forcing $f(y)=f(x)$. A [nonconstant function](#nonconstant-function) therefore has a positive lower bound for its positive periods. Their [infimum](real-analysis.md#infimum) $T_0$ is itself a period by closedness. Subtracting an integer multiple of $T_0$ from any other period leaves a period in $[0,T_0)$, which must be zero. This proves the stated structure without assuming [differentiability](analysis.md#differentiability).

#### Periodic function without a least positive period

↑ **Parent:** [Fundamental period of a function](#fundamental-period-of-a-function)

Define the [indicator function](measure-theory.md#indicator-function) of the [rational numbers](number-theory.md#rational-number) on the [real line](real-analysis.md#real-line) by $f(x)=1$ for rational $x$ and $f(x)=0$ otherwise. Every rational shift preserves rationality and irrationality, so every nonzero rational number is a [period of a function](mathematics.md#period-of-a-function). Conversely, an irrational shift sends $x=0$ from value one to value zero, so it is not a period. The [period group of a function](#period-group-of-a-function) is exactly $\mathbb Q$, and the positive periods $1/n$ approach zero without a smallest one. The [function](function.md) is [nonconstant](#nonconstant-function) and discontinuous everywhere; this is why [continuity](calculus.md#continuous-function) matters in [continuous periodic functions have a least positive period](#continuous-periodic-functions-have-a-least-positive-period).

### Period group of a function

↑ **Parent:** [Periodic function](#periodic-function)

Include zero when forming this [set](set.md), even though a [period of a function](mathematics.md#period-of-a-function) is normally required to be nonzero. For $f:\mathbb R\to Y$, $\operatorname{Per}(f)$ is a [subgroup](group.md#subgroup) of the [additive group](group.md#additive-group) of the [real numbers](arithmetic.md#real-number): composing two preserving shifts adds them, and reversing a preserving shift negates it. A [constant function](#constant-function) has period group $\mathbb R$. A [nonconstant](#nonconstant-function) [continuous](calculus.md#continuous-function) [real-valued function](#real-valued-function) that is [periodic](#periodic-function) has period group $T_0\mathbb Z$, where $T_0$ is its [fundamental period](#fundamental-period-of-a-function).

### Simply periodic function

↑ **Parent:** [Periodic function](#periodic-function)

A nonconstant [meromorphic function](isolated-singularity.md#meromorphic-function) on the [complex plane](complex-analysis.md#complex-plane) is simply periodic when its group of periods is generated by one nonzero complex number. It is distinct from a doubly periodic [elliptic function](complex-analysis.md#elliptic-function), whose [period lattice](complex-analysis.md#period-lattice) has two real-linearly independent generators. Single periodicity alone imposes no algebraic addition law.

### Cardinality of integer-periodic function spaces

↑ **Parent:** [Periodic function](#periodic-function)

For fixed positive integer period $n$, integer-valued [periodic functions](#periodic-function) on $\mathbb Z$ are in [bijection](#bijection) with $\mathbb Z^n$ and hence form a [countable set](cardinal-number.md#countable-set). Their union over periods is a [countable union of countable sets](cardinal-number.md#countable-union-of-countable-sets). In contrast, period-one integer-valued [functions](function.md) on $\mathbb Q$ can prescribe arbitrary binary values on its infinitely many distinct classes modulo $\mathbb Z$. The [power set](set.md#power-set) of a countably infinite set injects into them, proving uncountability.

### Period average

↑ **Parent:** [Periodic function](#periodic-function)

The period average extracts the reference level of an [integrable function](measure-theory.md#lebesgue-integrable-function) that repeats. For a real- or complex-valued [periodic function](#periodic-function) $f$ with positive [period of a function](mathematics.md#period-of-a-function) $T$, assume $f$ is [Lebesgue integrable](measure-theory.md#lebesgue-integrable-function) on every bounded interval. Its average is

$$
\boxed{\langle f\rangle=\frac1T\int_a^{a+T}f(t)\,dt.}
$$

The answer is independent of the starting point $a$. Splitting a shifted interval at the old endpoint and using $f(t+T)=f(t)$ moves its extra piece back into the missing piece. The interval length must be a [period](mathematics.md#period-of-a-function); an arbitrary window can give a different average.

For $g(t)=2+\sin(2\pi t)+\tfrac12\cos(4\pi t)$, every length-one window has average $2$: both oscillating [integrals](integral.md) vanish over that window. A half-unit window instead has average $2+(2/\pi)\cos(2\pi a)$, which depends on its start. Thus a short sample of an oscillation can bias an estimate of its reference level even when the full-cycle average is known exactly.

<a id="image-a-full-period-average-is-independent-of-its-starting-point-while-a-shorter-window-is-not"></a>
![](period-average-full-and-partial-windows.png)

**[Figure 5](#image-a-full-period-average-is-independent-of-its-starting-point-while-a-shorter-window-is-not). A full-period average is independent of its starting point, while a shorter window is not**.

In the complex [Fourier series](fourier-series.md) convention with basis $e^{2\pi int/T}$, the zero-frequency [Fourier coefficient](fourier-series.md#fourier-coefficient) is $c_0=\langle f\rangle$. This assertion defines the coefficient even when an additional convergence theorem is needed to reconstruct $f$ from its series. Strang's §4.1 explicitly identifies that constant coefficient with the average.[§4.1; pp. 317](mathematics-bibliography.md#computational-science-and-engineering-by-gilbert-strang/fourier-series-for-periodic-functions)

Averaging a square measures something different from averaging its original [function](function.md). For the illustrated $g$, [orthogonality](inner-product.md#orthogonal-vectors) of the trigonometric terms gives $\langle g^2\rangle=4+1/2+1/8=37/8$, whereas $\langle g\rangle^2=4$. Its [root mean square](analysis.md#root-mean-square) is therefore $\sqrt{37/8}$. Similarly, the [period average](#period-average) of $\sin^2$ is $1/2$. A zero mean need not imply a zero mean square.

### Triangular wave

↑ **Parent:** [Periodic function](#periodic-function)

A triangular wave is a continuous piecewise linear [periodic function](#periodic-function) whose slope alternates between two values. The even $2\pi$-periodic extension of $bx$ from $[0,\pi]$ is $P(s)=b|s-2k\pi|$ for $(2k-1)\pi\le s\le(2k+1)\pi$. Its [Fourier cosine series](fourier-series.md#fourier-cosine-series) contains a constant term and odd modes with coefficients proportional to the inverse square of the mode number. Such extensions describe reflection under [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition).

#### Fourier cosine series of a triangular wave

↑ **Parent:** [Triangular wave](#triangular-wave)

The period-two extension of $1-|x|$ on $[-1,1]$ is even. Its [Fourier cosine series](fourier-series.md#fourier-cosine-series) has $a_0=1$ and $a_n=2\int_0^1(1-x)\cos(n\pi x)dx=2[1-(-1)^n]/(n^2\pi^2)$ by [integration by parts](calculus.md#integration-by-parts). This proves the displayed series, with only odd nonconstant harmonics. Continuity and piecewise smoothness give pointwise equality through the [Dirichlet-Jordan convergence theorem](fourier-series.md#dirichlet-jordan-convergence-theorem); the summable coefficient magnitudes also imply [uniform convergence](sequence-and-series.md#uniform-convergence) by the [Weierstrass M-test](probability-and-statistics.md#weierstrass-m-test). At $x=0$, it gives $\sum_{m\geq0}(2m+1)^{-2}=\pi^2/8$.

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (944)

- [Abelianization of the square symmetry group](group-theory.md#abelianization-of-the-square-symmetry-group)
- [Absolute Fourier convergence from a square-integrable derivative](fourier-series.md#absolute-fourier-convergence-from-a-square-integrable-derivative)
- [Abstraction function](computer-science.md#abstraction-function)
- [Adaptivity to an unknown covariate distribution](statistical-inference.md#adaptivity-to-an-unknown-covariate-distribution)
- [Additive constant](integral.md#additive-constant)
- [Adjoints of inverse image on power sets](category.md#adjoints-of-inverse-image-on-power-sets)
- [Affine upper envelope](topological-vector-space.md#affine-upper-envelope)
- [Aliasing of discrete Fourier modes](discrete-fourier-transform.md#aliasing-of-discrete-fourier-modes)
- [Analysis of Boolean functions](analysis-of-boolean-functions.md)
- [Analyticity](sequence-and-series.md#analyticity)
- [Antiderivative](integral.md#antiderivative)
- [Antiderivatives on disconnected domains](integral.md#antiderivatives-on-disconnected-domains)
- [Arithmetic function](arithmetic-function.md)
- [Asymptotic analysis](real-analysis.md#asymptotic-analysis)
- [Asymptotic equivalence](real-analysis.md#asymptotic-equivalence)
- [Asymptotic expansion](asymptotic-expansion.md)
- [Asymptotic power series](asymptotic-expansion.md#asymptotic-power-series)
- [Asymptotic sequence](asymptotic-expansion.md#asymptotic-sequence)
- [Average value of a function](integral.md#average-value-of-a-function)
- [Axiom of global choice](set-theory.md#axiom-of-global-choice)
- [Barycenter](topological-vector-space.md#barycenter)
- [Bernoulli corrections for polynomial sums](bernoulli-number.md#bernoulli-corrections-for-polynomial-sums)
- [Best N-term wavelet approximation of piecewise Hölder functions](hilbert-space.md#best-n-term-wavelet-approximation-of-piecewise-holder-functions)
- [Best uniform approximation](uniform-approximation.md#best-uniform-approximation)
- [Biconjugation as closed convexification](convex-optimization.md#biconjugation-as-closed-convexification)
- [Big O notation](real-analysis.md#big-o-notation)
- [Bijection](#bijection)
- [Bilinear correlation bound for the box norm](additive-combinatorics.md#bilinear-correlation-bound-for-the-box-norm)
- [Binary diagonally noncomputable function](computability-theory.md#binary-diagonally-noncomputable-function)
- [Binary operation](algebraic-operation.md#binary-operation)
- [Bisection error bound](numerical-analysis.md#bisection-error-bound)
- [Bisection stopping criterion](numerical-analysis.md#bisection-stopping-criterion)
- [Bohr-Mollerup theorem](complex-analysis.md#bohr-mollerup-theorem)
- [Boolean cube expansion from bounded differences](probability-inequality.md#boolean-cube-expansion-from-bounded-differences)
- [Boundary condition](differential-equation.md#boundary-condition)
- [Boundary convergence of a power series](sequence-and-series.md#boundary-convergence-of-a-power-series)
- [Boundary trace of a function](boundary-value-problem.md#boundary-trace-of-a-function)
- [Bounded differences property](probability-inequality.md#bounded-differences-property)
- [Bounded nonconvergent Fourier partial sums](fourier-series.md#bounded-nonconvergent-fourier-partial-sums)
- [Bounding-to-almost-disjointness inequality](set-theory.md#bounding-to-almost-disjointness-inequality)
- [Box norm](additive-combinatorics.md#box-norm)
- [Bracketing method](numerical-analysis.md#bracketing-method)
- [Brent cycle-finding algorithm](algorithm.md#brent-cycle-finding-algorithm)
- [Bukovský-Hechler theorem](cardinal-number.md#bukovsky-hechler-theorem)
- [Calculus](calculus.md)
- [Calculus of variations](calculus-of-variations.md)
- [Canonical projection of a quotient set](set-theory.md#canonical-projection-of-a-quotient-set)
- [Cantor's theorem](set.md#cantor-s-theorem)
- [Cantor-Schröder-Bernstein theorem](cardinal-number.md#cantor-schroder-bernstein-theorem)
- [Cardinality of integer-periodic function spaces](#cardinality-of-integer-periodic-function-spaces)
- [Cartan's magic formula](differential-form.md#cartan-s-magic-formula)
- [Category](category.md)
- [Category of finite sets](category.md#category-of-finite-sets)
- [Category of pointed sets](category.md#category-of-pointed-sets)
- [Category of topological manifolds](topological-manifold.md#category-of-topological-manifolds)
- [Cauchy-Hadamard theorem](sequence-and-series.md#cauchy-hadamard-theorem)
- [Cauchy principal value](complex-analysis.md#cauchy-principal-value)
- [Cauchy's functional equation](analysis.md#cauchy-s-functional-equation)
- [Causal extension by zero](integral-transform.md#causal-extension-by-zero)
- [Cellular automaton](computer-science.md#cellular-automaton)
- [Certifiable function](probability-inequality.md#certifiable-function)
- [Chain rule](calculus.md#chain-rule)
- [Change of variables formula](multivariable-calculus.md#change-of-variables-formula)
- [Chebyshev polynomial](numerical-analysis.md#chebyshev-polynomial)
- [Choquet's theorem by strict convexity](topological-vector-space.md#choquet-s-theorem-by-strict-convexity)
- [Classifier](foundations-of-mathematics.md#classifier)
- [Closed ball](topological-analysis.md#closed-ball)
- [Closed forcing adds no short ground-valued sequences](forcing.md#closed-forcing-adds-no-short-ground-valued-sequences)
- [Closed-form expression](algebra.md#closed-form-expression)
- [Closest point on a plane](geometry-and-topology.md#closest-point-on-a-plane)
- [Codomain](#codomain)
- [Coherent coinfinite injections into omega](algebra.md#coherent-coinfinite-injections-into-omega)
- [Coherent-injection Aronszajn tree](set.md#coherent-injection-aronszajn-tree)
- [Colour-preserving symmetry group](group-action.md#colour-preserving-symmetry-group)
- [Compact metrizable convex set](topological-vector-space.md#compact-metrizable-convex-set)
- [Compilation arithmetic example](programming-language.md#compilation-arithmetic-example)
- [Complex analysis](complex-analysis.md)
- [Complex differentiability](holomorphic-function.md#complex-differentiability)
- [Composite midpoint quadrature rule](numerical-analysis.md#composite-midpoint-quadrature-rule)
- [Conditional entropy](information-theory.md#conditional-entropy)
- [Conformal automorphism of the upper half-plane](complex-analysis.md#conformal-automorphism-of-the-upper-half-plane)
- [Constant function](#constant-function)
- [Continuity into a product space](geometry-and-topology.md#continuity-into-a-product-space)
- [Continuous exponential functional equation](analysis.md#continuous-exponential-functional-equation)
- [Continuous function](calculus.md#continuous-function)
- [Continuous map](topology.md#continuous-map)
- [Continuous maps from an infinite cofinite space to a Hausdorff space are constant](topology.md#continuous-maps-from-an-infinite-cofinite-space-to-a-hausdorff-space-are-constant)
- [Contour plot](topology.md#contour-plot)
- [Control-point influence on a curve](computer-aided-geometric-design.md#control-point-influence-on-a-curve)
- [Convergence in a product space](geometry-and-topology.md#convergence-in-a-product-space)
- [Convex conjugate](convex-optimization.md#convex-conjugate)
- [Convex function](real-analysis.md#convex-function)
- [Convolution](fourier-analysis.md#convolution)
- [Convolution kernel](fourier-analysis.md#convolution-kernel)
- [Convolution theorem for Laplace transforms](integral-transform.md#convolution-theorem-for-laplace-transforms)
- [Conway Game of Life](computer-science.md#conway-game-of-life)
- [Correlation function of a point process](probability-theory.md#correlation-function-of-a-point-process)
- [Countable saturation of a nonprincipal ultraproduct over omega](model-theory.md#countable-saturation-of-a-nonprincipal-ultraproduct-over-omega)
- [Counting lemma for octahedrally quasirandom three-uniform hypergraphs](hypergraph.md#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs)
- [Counting measure](measure.md#counting-measure)
- [Critical point](analysis.md#critical-point)
- [Cubic exactness of Simpson's rule](numerical-integration.md#cubic-exactness-of-simpson-s-rule)
- [Curl of a gradient](multivariable-calculus.md#curl-of-a-gradient)
- [Decay of a nonnegative uniformly continuous integrable function](calculus.md#decay-of-a-nonnegative-uniformly-continuous-integrable-function)
- [Decoupled coefficients of orthogonal polynomial projections](orthogonal-polynomial.md#decoupled-coefficients-of-orthogonal-polynomial-projections)
- [Definite integral](integral.md#definite-integral)
- [Delay differential equation](differential-equation.md#delay-differential-equation)
- [Density of bounded centered scores](statistical-model.md#density-of-bounded-centered-scores)
- [Derivative](calculus.md#derivative)
- [Derivative along a curve](calculus.md#derivative-along-a-curve)
- [Derivative criterion for monotonicity](calculus.md#derivative-criterion-for-monotonicity)
- [Derivative seminorms on a compact interval](topological-vector-space.md#derivative-seminorms-on-a-compact-interval)
- [Deterministic finite automaton](foundations-of-mathematics.md#deterministic-finite-automaton)
- [Differentiability implies continuity](analysis.md#differentiability-implies-continuity)
- [Differential calculus](calculus.md#differential-calculus)
- [Differential equation](differential-equation.md)
- [Differential form](differential-form.md)
- [Differential operator](analysis.md#differential-operator)
- [Differentiation](calculus.md#differentiation)
- [Dirac measure](measure.md#dirac-measure)
- [Directed limit of elementary embeddings](model-theory.md#directed-limit-of-elementary-embeddings)
- [Directional derivative](multivariable-calculus.md#directional-derivative)
- [Discontinuity of a function](calculus.md#discontinuity-of-a-function)
- [Discrete Fourier transform](discrete-fourier-transform.md)
- [Discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution)
- [Double-coset Hecke algebra](group-theory.md#double-coset-hecke-algebra)
- [Dyadic conditional averages recover integrable functions](measure-theory.md#dyadic-conditional-averages-recover-integrable-functions)
- [Edge coloring](graph-coloring.md#edge-coloring)
- [Effective diagonal lemma](mathematical-logic.md#effective-diagonal-lemma)
- [Effective domain](real-analysis.md#effective-domain)
- [Efron–Stein inequality](probability-inequality.md#efron-stein-inequality)
- [Electric potential](electric-field.md#electric-potential)
- [Empirical spectral measure](probability-theory.md#empirical-spectral-measure)
- [Entire function](holomorphic-function.md#entire-function)
- [Epsilon-delta definition of continuity](calculus.md#epsilon-delta-definition-of-continuity)
- [Equality in Minkowski inequality](real-analysis.md#equality-in-minkowski-inequality)
- [Equation](algebra.md#equation)
- [Equilibrium solution of an ordinary differential equation](differential-equation.md#equilibrium-solution-of-an-ordinary-differential-equation)
- [Equivalence of partial functions modulo finite changes](set-theory.md#equivalence-of-partial-functions-modulo-finite-changes)
- [Equivalence relation induced by a function](set-theory.md#equivalence-relation-induced-by-a-function)
- [Essential infimum](real-analysis.md#essential-infimum)
- [Essential infimum and essential supremum](real-analysis.md#essential-infimum-and-essential-supremum)
- [Essential range](measure-theory.md#essential-range)
- [Essential supremum](measure-theory.md#essential-supremum)
- [Essentially bounded function](real-analysis.md#essentially-bounded-function)
- [Events determined by a random variable](probability-space.md#events-determined-by-a-random-variable)
- [Exponential-linear separable potential](analysis.md#exponential-linear-separable-potential)
- [Exponential order](integral-transform.md#exponential-order)
- [Extrapolation](interpolation.md#extrapolation)
- [Extreme-point criterion for the L-infinity unit ball](convex-set.md#extreme-point-criterion-for-the-l-infinity-unit-ball)
- [Factorial](combinatorics.md#factorial)
- [Factorization through a surjection](#factorization-through-a-surjection)
- [Failure of L2 closure of the global BV domain](inverse-problem.md#failure-of-l2-closure-of-the-global-bv-domain)
- [Failure of Minkowski inequality below exponent one](real-analysis.md#failure-of-minkowski-inequality-below-exponent-one)
- [Fano's inequality via an error indicator](information-theory.md#fano-s-inequality-via-an-error-indicator)
- [Fast-growing hierarchy](ordinal.md#fast-growing-hierarchy)
- [Feasible region](mathematical-optimization.md#feasible-region)
- [Fiber of a function](#fiber-of-a-function)
- [Finite coloring](ramsey-theory.md#finite-coloring)
- [Finite-cost optimal transport converse](mathematical-optimization.md#finite-cost-optimal-transport-converse)
- [Finite difference](finite-difference.md)
- [Finite samples do not certify quadrature accuracy](numerical-integration.md#finite-samples-do-not-certify-quadrature-accuracy)
- [Finite witness array coding](computability-theory.md#finite-witness-array-coding)
- [First three derivatives of an inverse function](multivariable-calculus.md#first-three-derivatives-of-an-inverse-function)
- [Foundations of mathematics](foundations-of-mathematics.md)
- [Four-neighbour mean expansion](finite-difference.md#four-neighbour-mean-expansion)
- [Fourier analysis](fourier-analysis.md)
- [Fourier coefficient](fourier-series.md#fourier-coefficient)
- [Fourier inversion theorem](fourier-analysis.md#fourier-inversion-theorem)
- [Fourier partial sum](fourier-series.md#fourier-partial-sum)
- [Fourier series](fourier-series.md)
- [Fourier series of a periodically extended exponential](fourier-series.md#fourier-series-of-a-periodically-extended-exponential)
- [Fourier sine coefficient](fourier-series.md#fourier-sine-coefficient)
- [Frequency spectrum](fourier-analysis.md#frequency-spectrum)
- [Full second-order replacement rank obstruction](set-theory.md#full-second-order-replacement-rank-obstruction)
- [Full shift](dynamical-systems.md#full-shift)
- [Full transformation monoid](algebraic-operation.md#full-transformation-monoid)
- [Function](function.md)
- [Function class](#function-class)
- [Function collision](#function-collision)
- [Function composition](#function-composition)
- [Function in extension](computability-theory.md#function-in-extension)
- [Function input](#function-input)
- [Function output](#function-output)
- [Function space](functional-analysis.md#function-space)
- [Functional](calculus-of-variations.md#functional)
- [Functional analysis](functional-analysis.md)
- [Functional equation](analysis.md#functional-equation)
- [Functional graph](graph-theory.md#functional-graph)
- [Functor](functor.md)
- [Fundamental theorem for line integrals](multivariable-calculus.md#fundamental-theorem-for-line-integrals)
- [Fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus)
- [Gaussian initial data for the heat equation](diffusion-equation.md#gaussian-initial-data-for-the-heat-equation)
- [Gaussian process regression](gaussian-process.md#gaussian-process-regression)
- [Gaussian quadrature](numerical-analysis.md#gaussian-quadrature)
- [Gaussian white noise model](gaussian-process.md#gaussian-white-noise-model)
- [Geometric power-series remainder](sequence-and-series.md#geometric-power-series-remainder)
- [Germ (mathematics)](#germ-mathematics)
- [Globally Lipschitz function](real-analysis.md#globally-lipschitz-function)
- [Golden-section search](numerical-analysis.md#golden-section-search)
- [Golgi cargo processing](biological-cell.md#golgi-cargo-processing)
- [Goodstein function](integer.md#goodstein-function)
- [Gradient](multivariable-calculus.md#gradient)
- [Graph coloring](graph-coloring.md)
- [Graph homomorphism](graph-theory.md#graph-homomorphism)
- [Graph of a function](#graph-of-a-function)
- [Great Picard theorem](holomorphic-function.md#great-picard-theorem)
- [Group action](group-action.md)
- [Haar projection](fourier-analysis.md#haar-projection)
- [Haar projection error for a Lipschitz function](fourier-analysis.md#haar-projection-error-for-a-lipschitz-function)
- [Hamiltonian trace functional on monic differential operators](analysis.md#hamiltonian-trace-functional-on-monic-differential-operators)
- [Hardy's integral inequality for an interval indicator](real-analysis.md#hardy-s-integral-inequality-for-an-interval-indicator)
- [Harmonic function for a Markov chain](markov-chain.md#harmonic-function-for-a-markov-chain)
- [Hash collision](computer-science.md#hash-collision)
- [Hash function](computer-science.md#hash-function)
- [Hessian matrix](multivariable-calculus.md#hessian-matrix)
- [Hilbert space](hilbert-space.md)
- [History function of a delay differential equation](differential-equation.md#history-function-of-a-delay-differential-equation)
- [History of Hölder's inequality](real-analysis.md#history-of-holder-s-inequality)
- [History of total variation of a function](real-analysis.md#history-of-total-variation-of-a-function)
- [Hölder-Taylor remainder bound](sobolev-space.md#holder-taylor-remainder-bound)
- [Holomorphic function](holomorphic-function.md)
- [Homogeneous function](real-analysis.md#homogeneous-function)
- [Homogeneous linear differential equation](differential-equation.md#homogeneous-linear-differential-equation)
- [Horizontal line test](#horizontal-line-test)
- [Hyperbolic function](calculus.md#hyperbolic-function)
- [Idempotent function](#idempotent-function)
- [Identity function](#identity-function)
- [Image and preimage of a function](set-theory.md#image-and-preimage-of-a-function)
- [Image of a function](set-theory.md#image-of-a-function)
- [Implicit equation](algebra.md#implicit-equation)
- [Implicit function](#implicit-function)
- [Implicit function theorem](multivariable-calculus.md#implicit-function-theorem)
- [Independent random variables](random-variable.md#independent-random-variables)
- [Infinite-dimensional Hamiltonian integrability](integrable-systems.md#infinite-dimensional-hamiltonian-integrability)
- [Infinite path through a binary tree](geometry-and-topology.md#infinite-path-through-a-binary-tree)
- [Influence-function representer](statistical-inference.md#influence-function-representer)
- [Initial value problem](differential-equation.md#initial-value-problem)
- [Injection-chain proof of the Cantor-Schröder-Bernstein theorem](cardinal-number.md#injection-chain-proof-of-the-cantor-schroder-bernstein-theorem)
- [Inner product](inner-product.md)
- [Integrable singularity](real-analysis.md#integrable-singularity)
- [Integral](integral.md)
- [Integral comparison for a nonincreasing nonnegative function](sequence-and-series.md#integral-comparison-for-a-nonincreasing-nonnegative-function)
- [Integral kernel](functional-analysis.md#integral-kernel)
- [Integral representation](integral.md#integral-representation)
- [Integrand](integral.md#integrand)
- [Integrating factor](linear-ordinary-differential-equation.md#integrating-factor)
- [Intermediate value theorem hypotheses and counterexamples](calculus.md#intermediate-value-theorem-hypotheses-and-counterexamples)
- [Interpolant](interpolation.md#interpolant)
- [Interpolation](interpolation.md)
- [Interval arithmetic](numerical-analysis.md#interval-arithmetic)
- [Interval bisection](numerical-analysis.md#interval-bisection)
- [Interval dependency problem](numerical-analysis.md#interval-dependency-problem)
- [Interval enclosure](numerical-analysis.md#interval-enclosure)
- [Interval root exclusion](numerical-analysis.md#interval-root-exclusion)
- [Interval square range](numerical-analysis.md#interval-square-range)
- [Inverse Ackermann function](computability-theory.md#inverse-ackermann-function)
- [Inverse function](#inverse-function)
- [Inverse-function linearization of a first-order equation](differential-equation.md#inverse-function-linearization-of-a-first-order-equation)
- [Inverse function theorem](multivariable-calculus.md#inverse-function-theorem)
- [Jensen gap](real-analysis.md#jensen-gap)
- [Jensen's inequality](real-analysis.md#jensen-s-inequality)
- [Joint injectivity of a pair of functions](set-theory.md#joint-injectivity-of-a-pair-of-functions)
- [Jordan decomposition of a function of bounded variation](real-analysis.md#jordan-decomposition-of-a-function-of-bounded-variation)
- [Jump response of a localized analyzing function](fourier-analysis.md#jump-response-of-a-localized-analyzing-function)
- [Kahane-Katznelson divergence theorem](fourier-series.md#kahane-katznelson-divergence-theorem)
- [Kernel density estimation](nonparametric-statistics.md#kernel-density-estimation)
- [Kernel support-vector coefficient from hinge activity](statistical-learning.md#kernel-support-vector-coefficient-from-hinge-activity)
- [Kinetic energy](energy.md#kinetic-energy)
- [Kolmogorov axioms](probability-space.md#kolmogorov-axioms)
- [Kuratowski ordered pair](set.md#kuratowski-ordered-pair)
- [L-infinity norm](real-analysis.md#l-infinity-norm)
- [Lagrangian duality](mathematical-optimization.md#lagrangian-duality)
- [Lambda definition of primitive recursion by pair iteration](computability-theory.md#lambda-definition-of-primitive-recursion-by-pair-iteration)
- [Lambda representation of partial computable functions](computability-theory.md#lambda-representation-of-partial-computable-functions)
- [Laplace transform](integral-transform.md#laplace-transform)
- [Lebesgue integral](measure-theory.md#lebesgue-integral)
- [Left inverse](#left-inverse)
- [Legendre symbol](quadratic-residue.md#legendre-symbol)
- [Leibniz integral rule](analysis.md#leibniz-integral-rule)
- [Lenard-Magri recursion](symplectic-geometry.md#lenard-magri-recursion)
- [Lie algebra](lie-algebra.md)
- [Life glider](computer-science.md#life-glider)
- [Life oscillator](computer-science.md#life-oscillator)
- [Linear approximation](calculus.md#linear-approximation)
- [Linear combination](vector-space.md#linear-combination)
- [Linear differential equation](differential-equation.md#linear-differential-equation)
- [Linearity of expectation](expected-value.md#linearity-of-expectation)
- [Linearity of integration](integral.md#linearity-of-integration)
- [Lipschitz constant](real-analysis.md#lipschitz-constant)
- [Lipschitz continuity](real-analysis.md#lipschitz-continuity)
- [Local extremum](mathematical-optimization.md#local-extremum)
- [Local maximum](analysis.md#local-maximum)
- [Local minimum](analysis.md#local-minimum)
- [Locally Lipschitz function](real-analysis.md#locally-lipschitz-function)
- [Locally square-integrable function](measure-theory.md#locally-square-integrable-function)
- [Logarithm](calculus.md#logarithm)
- [Logarithmic differentiation](calculus.md#logarithmic-differentiation)
- [Logarithmic integral representation of the natural logarithm](calculus.md#logarithmic-integral-representation-of-the-natural-logarithm)
- [Logarithmic parameter integral with Cauchy weight](analysis.md#logarithmic-parameter-integral-with-cauchy-weight)
- [Logarithmic polar coordinate change](multivariable-calculus.md#logarithmic-polar-coordinate-change)
- [Long chain under eventual domination](set-theory.md#long-chain-under-eventual-domination)
- [Low-pass filter of a multiresolution analysis](fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis)
- [Lp norm](real-analysis.md#lp-norm)
- [Markov information source](information-theory.md#markov-information-source)
- [Matrix inverse](matrix-inverse.md)
- [Mean value theorem](calculus.md#mean-value-theorem)
- [Measure](measure.md)
- [Mellin transform in logarithmic coordinates](integral-transform.md#mellin-transform-in-logarithmic-coordinates)
- [Memoization](algorithm.md#memoization)
- [Memoization key](algorithm.md#memoization-key)
- [Metric](topological-analysis.md#metric)
- [Metric space](topological-analysis.md#metric-space)
- [Minkowski inequality](real-analysis.md#minkowski-inequality)
- [Minkowski inequality for error aggregation](real-analysis.md#minkowski-inequality-for-error-aggregation)
- [Mollification](distribution-theory.md#mollification)
- [Monotonic function](calculus.md#monotonic-function)
- [Multipartite hypergraph](hypergraph.md#multipartite-hypergraph)
- [Multiple integral](integral.md#multiple-integral)
- [Multiplicative function](arithmetic-function.md#multiplicative-function)
- [Multiresolution analysis](fourier-analysis.md#multiresolution-analysis)
- [Natural density](number-theory.md#natural-density)
- [Natural interval extension](numerical-analysis.md#natural-interval-extension)
- [Natural transformation](functor.md#natural-transformation)
- [Negative part of a real-valued function](#negative-part-of-a-real-valued-function)
- [Noise sensitivity of a quadrature rule](numerical-integration.md#noise-sensitivity-of-a-quadrature-rule)
- [Nonconstant function](#nonconstant-function)
- [Nondecreasing function](calculus.md#nondecreasing-function)
- [Nondegenerate critical point](multivariable-calculus.md#nondegenerate-critical-point)
- [Nondeterministic finite automaton](foundations-of-mathematics.md#nondeterministic-finite-automaton)
- [Nonlinear ordinary differential equation](differential-equation.md#nonlinear-ordinary-differential-equation)
- [Nonparametric statistics](nonparametric-statistics.md)
- [Normal ultrafilter on small subsets](set-theory.md#normal-ultrafilter-on-small-subsets)
- [Normalizing constant](continuous-probability-distribution.md#normalizing-constant)
- [Numerical integration](numerical-integration.md)
- [Omitted value](holomorphic-function.md#omitted-value)
- [Ordinary differential equation](differential-equation.md#ordinary-differential-equation)
- [Orthogonal polynomial](orthogonal-polynomial.md)
- [Orthogonal polynomial projection kernel](functional-analysis.md#orthogonal-polynomial-projection-kernel)
- [Orthogonal projection](hilbert-space.md#orthogonal-projection)
- [Orthogonal vectors](inner-product.md#orthogonal-vectors)
- [Pair-factor correlation bound for the three-dimensional box norm](additive-combinatorics.md#pair-factor-correlation-bound-for-the-three-dimensional-box-norm)
- [Pairing function](computability-theory.md#pairing-function)
- [Parametric equation](geometry-and-topology.md#parametric-equation)
- [Partial derivative](multivariable-calculus.md#partial-derivative)
- [Partial differential equation](partial-differential-equation.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1.md#a1/a/i/solution)
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
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#10/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#12/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#section-a/10/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#section-a/10/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#section-b/3/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#section-b/9/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1.md#19/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1.md#19/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2.md#13/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2.md#15/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#11/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#11/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#14/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#16/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#18/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#18/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#20/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#20/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#20/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2.md#11/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2.md#19/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#13/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#19/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2.md#15/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2.md#17/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2.md#20/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#13/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#17/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#17/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2.md#8/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2.md#9/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#17/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#19/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#20/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2.md#13/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2.md#14/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2.md#17/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#12/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#7/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#9/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2.md#16/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#18/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#19/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#19/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2.md#17/b/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2.md#17/b/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1.md#14/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#15/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#18/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#18/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#18/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#19/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#20/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#9/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#18/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#14/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#15/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#18/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#17/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#17/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#19/d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2.md#19/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#14/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#20/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#18/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#18/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#18/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#16/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#18/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#18/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#7/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2.md#19/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2.md#19/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2.md#20/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#10/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#9/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#3/i/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a.md#section-d/d17/c/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a.md#section-d/d17/d/solution)
- [Peano zero](calculus.md#peano-zero)
- [Penrose-Ward correspondence](general-relativity.md#penrose-ward-correspondence)
- [Period average](#period-average)
- [Period of a function](mathematics.md#period-of-a-function)
- [Periodic domain](partial-differential-equation.md#periodic-domain)
- [Periodic extension](#periodic-extension)
- [Periodic function](#periodic-function)
- [Periodic function without a least positive period](#periodic-function-without-a-least-positive-period)
- [Periodic phase change of a scaling function](fourier-analysis.md#periodic-phase-change-of-a-scaling-function)
- [Periodic upwind finite volume advection](finite-volume-method.md#periodic-upwind-finite-volume-advection)
- [Permutation](combinatorics.md#permutation)
- [Picard iteration](differential-equation.md#picard-iteration)
- [Picard theorem](holomorphic-function.md#picard-theorem)
- [Piecewise continuous function](analysis.md#piecewise-continuous-function)
- [Pigeonhole principle](combinatorics.md#pigeonhole-principle)
- [Pointed set](set.md#pointed-set)
- [Pointwise convergence](sequence-and-series.md#pointwise-convergence)
- [Pointwise convergence of a piecewise smooth Fourier series](fourier-series.md#pointwise-convergence-of-a-piecewise-smooth-fourier-series)
- [Pointwise limit](sequence-and-series.md#pointwise-limit)
- [Poisson pencil](symplectic-geometry.md#poisson-pencil)
- [Poisson summation formula](fourier-analysis.md#poisson-summation-formula)
- [Pole at infinity](isolated-singularity.md#pole-at-infinity)
- [Polynomial function](polynomial.md#polynomial-function)
- [Polynomial interpolation](interpolation.md#polynomial-interpolation)
- [Polynomial kernel](positive-semidefinite-kernel.md#polynomial-kernel)
- [Positively homogeneous function (degree one)](real-analysis.md#positively-homogeneous-function-degree-one)
- [Potential of a conservative vector field](multivariable-calculus.md#potential-of-a-conservative-vector-field)
- [Power law](analysis.md#power-law)
- [Power series](sequence-and-series.md#power-series)
- [Preimage](set-theory.md#preimage)
- [Preserve the domain when simplifying a function](#preserve-the-domain-when-simplifying-a-function)
- [Primitive recursive pairing function](computability-theory.md#primitive-recursive-pairing-function)
- [Principal minor resolvent trace bound](functional-analysis.md#principal-minor-resolvent-trace-bound)
- [Probability density](wave-function.md#probability-density)
- [Probability space](probability-space.md)
- [Productive set](computability-theory.md#productive-set)
- [Progression partition with nearly constant linear phase](additive-combinatorics.md#progression-partition-with-nearly-constant-linear-phase)
- [Projection (mathematics)](#projection-mathematics)
- [Proof outline of Hardy's integral inequality](real-analysis.md#proof-outline-of-hardy-s-integral-inequality)
- [Propagation of uncertainty](wave-equation.md#propagation-of-uncertainty)
- [Pushforward filter](set-theory.md#pushforward-filter)
- [Pushforward ultrafilter](set-theory.md#pushforward-ultrafilter)
- [Quadratic polynomial](polynomial.md#quadratic-polynomial)
- [Quadratic spline](uniform-approximation.md#quadratic-spline)
- [Quadrature rule](numerical-integration.md#quadrature-rule)
- [Quantum collision finding](theoretical-computer-science.md#quantum-collision-finding)
- [Quantum spectral filtering](quantum-fourier-transform.md#quantum-spectral-filtering)
- [Quotient of functions](#quotient-of-functions)
- [Quotient set](set-theory.md#quotient-set)
- [Qutrit linear-function identification](quantum-theory.md#qutrit-linear-function-identification)
- [Radial flux through a truncated unit sphere](multivariable-calculus.md#radial-flux-through-a-truncated-unit-sphere)
- [Radius of a Maclaurin series from successive derivatives](sequence-and-series.md#radius-of-a-maclaurin-series-from-successive-derivatives)
- [Random variable](random-variable.md)
- [Real analysis](real-analysis.md)
- [Reduced-denominator function unbounded on every interval](mathematics.md#reduced-denominator-function-unbounded-on-every-interval)
- [Regular variation](real-analysis.md#regular-variation)
- [Residue](analysis.md#residue)
- [Residue theorem](analysis.md#residue-theorem)
- [Restriction (mathematics)](#restriction-mathematics)
- [Retarded delay differential equation](differential-equation.md#retarded-delay-differential-equation)
- [Reversible density-ratio propagation](markov-chain.md#reversible-density-ratio-propagation)
- [Richardson extrapolation](numerical-analysis.md#richardson-extrapolation)
- [Right inverse](#right-inverse)
- [Rule of product](combinatorics.md#rule-of-product)
- [Runge's phenomenon](interpolation.md#runge-s-phenomenon)
- [Sample path](stochastic-process.md#sample-path)
- [Scalar-valued function](#scalar-valued-function)
- [Second-derivative test](multivariable-calculus.md#second-derivative-test)
- [Second-difference analyzing function](fourier-analysis.md#second-difference-analyzing-function)
- [Second-order Euler identity for homogeneous functions](real-analysis.md#second-order-euler-identity-for-homogeneous-functions)
- [Second-order logic](mathematical-logic.md#second-order-logic)
- [Sections of the degree-one line bundle on the projective line](complex-geometry.md#sections-of-the-degree-one-line-bundle-on-the-projective-line)
- [Self-bounding function](probability-inequality.md#self-bounding-function)
- [Self-map](#self-map)
- [Seminorm](topological-vector-space.md#seminorm)
- [Sequence](sequence-and-series.md#sequence)
- [Sequence of functions](sequence-and-series.md#sequence-of-functions)
- [Set](set.md)
- [Set theory](set-theory.md)
- [Sharp constant in Hardy's integral inequality](real-analysis.md#sharp-constant-in-hardy-s-integral-inequality)
- [Signal](electrical-engineering.md#signal)
- [Simpson's rule](numerical-integration.md#simpson-s-rule)
- [Skolem expansion](mathematical-logic.md#skolem-expansion)
- [Skolem function](mathematical-logic.md#skolem-function)
- [Slowly varying function](real-analysis.md#slowly-varying-function)
- [Smooth convergence on a compact interval](topological-vector-space.md#smooth-convergence-on-a-compact-interval)
- [Smoothness](analysis.md#smoothness)
- [Solution of a differential equation](differential-equation.md#solution-of-a-differential-equation)
- [Sort key](algorithm.md#sort-key)
- [Sorting algorithm](algorithm.md#sorting-algorithm)
- [Sparse-shift bijection between nonnegative and positive integers](cardinal-number.md#sparse-shift-bijection-between-nonnegative-and-positive-integers)
- [Spectral Lipschitz bound from Frobenius distance](linear-operator-theory.md#spectral-lipschitz-bound-from-frobenius-distance)
- [Square wave](fourier-series.md#square-wave)
- [Stability of a supremum under uniform perturbations](real-analysis.md#stability-of-a-supremum-under-uniform-perturbations)
- [Step-function proof of the Riemann-Lebesgue lemma](fourier-analysis.md#step-function-proof-of-the-riemann-lebesgue-lemma)
- [Stirling numbers of the second kind](combinatorics.md#stirling-numbers-of-the-second-kind)
- [Strict local maximum](analysis.md#strict-local-maximum)
- [Strict local minimum](analysis.md#strict-local-minimum)
- [Strong duality without dual attainment](mathematical-optimization.md#strong-duality-without-dual-attainment)
- [Strongly universal hash family](computer-science.md#strongly-universal-hash-family)
- [Subdifferential under scalar affine composition](convex-optimization.md#subdifferential-under-scalar-affine-composition)
- [Substructure of a first-order structure](mathematical-logic.md#substructure-of-a-first-order-structure)
- [Supporting measure lemma for affine upper envelopes](topological-vector-space.md#supporting-measure-lemma-for-affine-upper-envelopes)
- [Supremum error](sequence-and-series.md#supremum-error)
- [Supremum norm](normed-vector-space.md#supremum-norm)
- [Supremum of a sum](real-analysis.md#supremum-of-a-sum)
- [Tangent line](calculus.md#tangent-line)
- [Tangential boundary derivative](differential-equation.md#tangential-boundary-derivative)
- [Taylor expansion from a periodic derivative equation](calculus.md#taylor-expansion-from-a-periodic-derivative-equation)
- [Taylor polynomial](calculus.md#taylor-polynomial)
- [Taylor's theorem](calculus.md#taylor-s-theorem)
- [Taylor series](calculus.md#taylor-series)
- [Tensorization of entropy](probability-inequality.md#tensorization-of-entropy)
- [Thermodynamic internal pressure](internal-energy.md#thermodynamic-internal-pressure)
- [Thermometer](temperature.md#thermometer)
- [Threshold Choquet representation in L-infinity](topological-vector-space.md#threshold-choquet-representation-in-l-infinity)
- [Total computable diagonal over primitive recursive syntax](computability-theory.md#total-computable-diagonal-over-primitive-recursive-syntax)
- [Total derivative](calculus.md#total-derivative)
- [Total differential](multivariable-calculus.md#total-differential)
- [Total variation of a function](real-analysis.md#total-variation-of-a-function)
- [Transitive group action](group-action.md#transitive-group-action)
- [Translation continuity in Lp](measure-theory.md#translation-continuity-in-lp)
- [Translation of a Fourier series](fourier-series.md#translation-of-a-fourier-series)
- [Translation of a function](#translation-of-a-function)
- [Transport cost function](mathematical-optimization.md#transport-cost-function)
- [Trapped surface](general-relativity.md#trapped-surface)
- [Trigonometric function](geometry-and-topology.md#trigonometric-function)
- [Ultraproduct proof of the Ehrenfeucht-Mostowski theorem](model-theory.md#ultraproduct-proof-of-the-ehrenfeucht-mostowski-theorem)
- [Unbounded torsion obstructs uniform control of four-term progressions](additive-combinatorics.md#unbounded-torsion-obstructs-uniform-control-of-four-term-progressions)
- [Uniform approximation](uniform-approximation.md)
- [Uniform big O bound](real-analysis.md#uniform-big-o-bound)
- [Uniform convergence](sequence-and-series.md#uniform-convergence)
- [Uniform convergence preserves integrals on a compact interval](sequence-and-series.md#uniform-convergence-preserves-integrals-on-a-compact-interval)
- [Uniform derivative convergence with an anchored value](sequence-and-series.md#uniform-derivative-convergence-with-an-anchored-value)
- [Uniform limit theorem](sequence-and-series.md#uniform-limit-theorem)
- [Uniform negative curvature and global maximization](real-analysis.md#uniform-negative-curvature-and-global-maximization)
- [Uniform step approximation on a compact interval](uniform-approximation.md#uniform-step-approximation-on-a-compact-interval)
- [Uniformization of a binary relation](descriptive-set-theory.md#uniformization-of-a-binary-relation)
- [Uniformly continuous function](calculus.md#uniformly-continuous-function)
- [Uniqueness of the packed spherical bilayer radius](mathematical-biology.md#uniqueness-of-the-packed-spherical-bilayer-radius)
- [Universal property of Cartesian products](set-theory.md#universal-property-of-cartesian-products)
- [Upper half-plane (complex analysis)](complex-analysis.md#upper-half-plane-complex-analysis)
- [Upper semicontinuity](calculus.md#upper-semicontinuity)
- [Vanishing moment](fourier-analysis.md#vanishing-moment)
- [Variational principle](calculus-of-variations.md#variational-principle)
- [Vector](vector-space.md#vector)
- [Vector calculus in elliptic cylindrical coordinates](multivariable-calculus.md#vector-calculus-in-elliptic-cylindrical-coordinates)
- [Vector space](vector-space.md)
- [Vector-valued function](#vector-valued-function)
- [Wavelet](fourier-analysis.md#wavelet)
- [Wavelet polynomial annihilation](fourier-analysis.md#wavelet-polynomial-annihilation)
- [Weak gradient](distribution-theory.md#weak-gradient)
- [Weierstrass approximation does not preserve derivatives](functional-analysis.md#weierstrass-approximation-does-not-preserve-derivatives)
- [Weighted arithmetic mean](arithmetic.md#weighted-arithmetic-mean)
- [Weighted inner product](inner-product.md#weighted-inner-product)
- [Wiener algebra](fourier-series.md#wiener-algebra)
- [Wiener-Hopf kernel](boundary-value-problem.md#wiener-hopf-kernel)
- [Window function](fourier-transform.md#window-function)
- [Wronskian](linear-ordinary-differential-equation.md#wronskian)
- [Zero set](polynomial.md#zero-set)
- [Zeta series truncation error](bernoulli-number.md#zeta-series-truncation-error)
