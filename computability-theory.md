# Computability theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computability_theory)

**Table of contents**

- [Recursive triple colouring with no computable infinite homogeneous set](#recursive-triple-colouring-with-no-computable-infinite-homogeneous-set)
- [Jockusch triple coloring computing the halting set](#jockusch-triple-coloring-computing-the-halting-set)
- [Function in intension](#function-in-intension)
  - [Function in extension](#function-in-extension)
- [Binary diagonally noncomputable function](#binary-diagonally-noncomputable-function)
- [Bounded simulation of a computation](#bounded-simulation-of-a-computation)
- [Productive set](#productive-set)
  - [Productivity of arithmetic truth](#productivity-of-arithmetic-truth)
- [Kolmogorov complexity](#kolmogorov-complexity)
  - [Plain Kolmogorov complexity](#plain-kolmogorov-complexity)
    - [Incompressible string](#incompressible-string)
      - [Immunity of incompressible strings](#immunity-of-incompressible-strings)
  - [Optimal description machine](#optimal-description-machine)
- [Undecidable decision problem](#undecidable-decision-problem)
- [Finite-injury priority construction](#finite-injury-priority-construction)
  - [Priority restraint](#priority-restraint)
    - [Preservation of a restrained oracle computation](#preservation-of-a-restrained-oracle-computation)
  - [Private-witness diagonalization for incomparable enumerable sets](#private-witness-diagonalization-for-incomparable-enumerable-sets)
  - [Friedberg–Muchnik theorem](#friedberg-muchnik-theorem)
  - [Finite injury](#finite-injury)
- [Turing reduction](#turing-reduction)
  - [Oracle-assisted finite-extension construction](#oracle-assisted-finite-extension-construction)
  - [Turing functional](#turing-functional)
    - [Oracle use](#oracle-use)
  - [Turing degree](#turing-degree)
    - [Kleene–Post incomparability theorem](#kleene-post-incomparability-theorem)
    - [Post problem](#post-problem)
- [Church–Turing thesis](#church-turing-thesis)
- [Pairing function](#pairing-function)
  - [Primitive recursive pairing function](#primitive-recursive-pairing-function)
  - [Decimal trailing-zero pairing function](#decimal-trailing-zero-pairing-function)
- [Register machine](#register-machine)
  - [String register machine](#string-register-machine)
    - [Characteristic-function register machine](#characteristic-function-register-machine)
      - [One-register separation for equal block lengths](#one-register-separation-for-equal-block-lengths)
      - [String register-machine suffix test](#string-register-machine-suffix-test)
      - [Complementing a characteristic-function register machine](#complementing-a-characteristic-function-register-machine)
- [Primitive recursive function](#primitive-recursive-function)
  - [Primitive recursive syntax and arity checking](#primitive-recursive-syntax-and-arity-checking)
    - [Total computable diagonal over primitive recursive syntax](#total-computable-diagonal-over-primitive-recursive-syntax)
    - [Primitive recursive function in intension](#primitive-recursive-function-in-intension)
  - [Bounded halting predicate](#bounded-halting-predicate)
  - [Bounded minimization](#bounded-minimization)
  - [Predecessor function](#predecessor-function)
  - [Initial function of recursion theory](#initial-function-of-recursion-theory)
    - [Zero function](#zero-function)
    - [Successor function](#successor-function)
    - [Projection function](#projection-function)
  - [Function composition in recursion theory](#function-composition-in-recursion-theory)
  - [Primitive recursion](#primitive-recursion)
  - [Composition-only recursive function](#composition-only-recursive-function)
  - [Structural induction for primitive recursive functions](#structural-induction-for-primitive-recursive-functions)
    - [Every primitive recursive function is total](#every-primitive-recursive-function-is-total)
  - [Existential bounded representation of a primitive recursive function](#existential-bounded-representation-of-a-primitive-recursive-function)
    - [Gödel beta-function sequence coding](#godel-beta-function-sequence-coding)
      - [Factorial graph formula via remainder coding](#factorial-graph-formula-via-remainder-coding)
      - [Finite witness array coding](#finite-witness-array-coding)
- [Diagonal argument](#diagonal-argument)
- [Recursively enumerable set](#recursively-enumerable-set)
  - [Simple set](#simple-set)
    - [Sparse-witness construction of a simple set](#sparse-witness-construction-of-a-simple-set)
  - [Immune set](#immune-set)
  - [Nonempty computably enumerable sets are primitive recursive ranges](#nonempty-computably-enumerable-sets-are-primitive-recursive-ranges)
  - [Computable set](#computable-set)
  - [Domain and range characterizations of a nonempty computably enumerable set](#domain-and-range-characterizations-of-a-nonempty-computably-enumerable-set)
- [Kleene's recursion theorem](#kleene-s-recursion-theorem)
- [Many-one reduction](#many-one-reduction)
  - [Many-one degree](#many-one-degree)
  - [Computable reduction by staged enumeration](#computable-reduction-by-staged-enumeration)
  - [Many-one complete set](#many-one-complete-set)
- [Index set](#index-set)
  - [Extensional property of programs](#extensional-property-of-programs)
  - [Rice's theorem](#rice-s-theorem)
  - [Infinite-domain index set](#infinite-domain-index-set)
    - [Infinite-domain range-restriction index set](#infinite-domain-range-restriction-index-set)
  - [Cofinite index set](#cofinite-index-set)
- [Padding lemma](#padding-lemma)
- [Dovetailing](#dovetailing)
- [Smn theorem](#smn-theorem)
- [Computable function](#computable-function)
  - [Universal partial computable function](#universal-partial-computable-function)
  - [Kleene normal form theorem](#kleene-normal-form-theorem)
  - [Mu operator](#mu-operator)
  - [Total computable function](#total-computable-function)
    - [Provably total computable function](#provably-total-computable-function)
  - [Truncated computation function](#truncated-computation-function)
  - [Ackermann function](#ackermann-function)
    - [Inverse Ackermann function](#inverse-ackermann-function)
- [Arithmetical hierarchy](#arithmetical-hierarchy)
  - [Bounded quantifier](#bounded-quantifier)
    - [Arithmetic bounded formula](#arithmetic-bounded-formula)
    - [Delta-0 formula](#delta-0-formula)
  - [Sigma-1 formula](#sigma-1-formula)
    - [Pi-1 formula](#pi-1-formula)
  - [Sigma-1 set](#sigma-1-set)
  - [Pi-2 set](#pi-2-set)
    - [Totality problem](#totality-problem)
      - [Totality problem is not computably enumerable](#totality-problem-is-not-computably-enumerable)
- [Recursively inseparable sets](#recursively-inseparable-sets)
- [Lambda calculus](#lambda-calculus)
  - [Normal-order reduction](#normal-order-reduction)
  - [Lambda model](#lambda-model)
    - [Reflexive domain](#reflexive-domain)
      - [Graph model of lambda calculus](#graph-model-of-lambda-calculus)
        - [Approximation theorem for the graph model](#approximation-theorem-for-the-graph-model)
        - [Indexed lambda term](#indexed-lambda-term)
          - [Indexed beta reduction](#indexed-beta-reduction)
  - [Lambda term](#lambda-term)
    - [Lambda application](#lambda-application)
    - [Lambda abstraction](#lambda-abstraction)
  - [Untyped lambda calculus](#untyped-lambda-calculus)
    - [Eta conversion](#eta-conversion)
    - [Combinatory logic](#combinatory-logic)
      - [Bracket abstraction](#bracket-abstraction)
      - [Combinatory logic term](#combinatory-logic-term)
        - [Weak combinatory reduction](#weak-combinatory-reduction)
    - [Head normal form](#head-normal-form)
      - [Böhm tree](#bohm-tree)
        - [Finite Böhm approximant](#finite-bohm-approximant)
        - [Böhm transformation](#bohm-transformation)
          - [Böhm-out lemma](#bohm-out-lemma)
            - [Böhm separation theorem](#bohm-separation-theorem)
      - [Unsolvable lambda term](#unsolvable-lambda-term)
        - [Easy lambda term](#easy-lambda-term)
      - [Solvable lambda term](#solvable-lambda-term)
    - [Beta reduction](#beta-reduction)
      - [Diamond property of a reduction relation](#diamond-property-of-a-reduction-relation)
        - [Church-Rosser property of a reduction relation](#church-rosser-property-of-a-reduction-relation)
      - [Parallel beta reduction](#parallel-beta-reduction)
        - [Complete development of a lambda term](#complete-development-of-a-lambda-term)
      - [Normal-order beta reduction](#normal-order-beta-reduction)
        - [Standardization theorem for beta reduction](#standardization-theorem-for-beta-reduction)
        - [Normal-order normalization theorem](#normal-order-normalization-theorem)
      - [Capture-avoiding substitution](#capture-avoiding-substitution)
      - [Beta equivalence](#beta-equivalence)
        - [Undecidability of beta equivalence](#undecidability-of-beta-equivalence)
      - [Beta-redex](#beta-redex)
      - [Beta-normal form](#beta-normal-form)
    - [Combinator](#combinator)
      - [Omega combinator](#omega-combinator)
      - [Fixed-point combinator](#fixed-point-combinator)
        - [Turing fixed-point combinator](#turing-fixed-point-combinator)
        - [Curry fixed-point combinator](#curry-fixed-point-combinator)
        - [Fixed-point theorem for the untyped lambda calculus](#fixed-point-theorem-for-the-untyped-lambda-calculus)
        - [Recursively enumerable fixed-point combinators](#recursively-enumerable-fixed-point-combinators)
  - [Alpha equivalence](#alpha-equivalence)
  - [Church-Rosser theorem](#church-rosser-theorem)
  - [Simply typed lambda calculus](#simply-typed-lambda-calculus)
    - [Typed lambda term](#typed-lambda-term)
    - [Weak normalization theorem for simply typed lambda calculus](#weak-normalization-theorem-for-simply-typed-lambda-calculus)
  - [Church encoding](#church-encoding)
    - [Church numeral](#church-numeral)
      - [Church numeral arithmetic](#church-numeral-arithmetic)
      - [Church numeral zero test](#church-numeral-zero-test)
      - [Church pair](#church-pair)
      - [Lambda-definable function](#lambda-definable-function)
        - [Lambda definition of the successor function](#lambda-definition-of-the-successor-function)
        - [Lambda definition of primitive recursion](#lambda-definition-of-primitive-recursion)
          - [Lambda definition of primitive recursion by pair iteration](#lambda-definition-of-primitive-recursion-by-pair-iteration)
        - [Lambda-definable partial function](#lambda-definable-partial-function)
          - [Lambda representation of partial computable functions](#lambda-representation-of-partial-computable-functions)
            - [Lambda simulation of a Turing machine](#lambda-simulation-of-a-turing-machine)
          - [Strict sequencing of partial numeral computations](#strict-sequencing-of-partial-numeral-computations)
          - [Lambda definition of unbounded minimization](#lambda-definition-of-unbounded-minimization)
    - [Church Boolean](#church-boolean)
  - [Normal form (abstract rewriting)](#normal-form-abstract-rewriting)
    - [Strong normalization theorem for simply typed lambda calculus](#strong-normalization-theorem-for-simply-typed-lambda-calculus)

## Recursive triple colouring with no computable infinite homogeneous set

↑ **Parent:** [Computability theory](computability-theory.md)

Let $K_s$ be increasing finite stage approximations to a noncomputable [computably enumerable set](#recursively-enumerable-set) $K$. For $x<y<z$, colour the triple zero exactly when $K_y\cap[0,x]=K_z\cap[0,x]$. An infinite homogeneous set has colour zero, since each bounded approximation eventually stabilizes. Its first two elements above any requested bound recover the final approximation at that bound, so the homogeneous set computes $K$. Thus no infinite homogeneous set is [computable](#computable-set). This illustrates the difference between a [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem) existence result and an effective construction.

## Jockusch triple coloring computing the halting set

↑ **Parent:** [Computability theory](computability-theory.md)

Let $K_s$ be a computable increasing finite-stage enumeration of the [halting problem](foundations-of-mathematics.md#halting-problem) set $K$. Color $x<y<z$ by whether the approximations below $x$ differ at stages $y,z$. This is a recursive two-color partition of triples. An infinite homogeneous set cannot have color one: for fixed $x$, the finite approximation below $x$ eventually stabilizes. If its color is zero, choose $x$ from that set above an input $n$, then another member $y>x$; agreement with arbitrarily large later stages gives $K(n)=K_y(n)$. Thus every infinite homogeneous set computes $K$, and none is a [recursive set](#computable-set). This makes the failure of an effective version of [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem) explicit.

## Function in intension

↑ **Parent:** [Computability theory](computability-theory.md)

A function in intension is a finite program or formal construction description. Its associated [function in extension](#function-in-extension) is the partial or total input-output map it denotes. A [Gödel number](mathematical-logic.md#godel-number) records the description rather than identifying all descriptions with the same extension.

### Function in extension

↑ **Parent:** [Function in intension](#function-in-intension)

A function in extension is a [function](function.md) specified by its domain and the value at each input in that domain. Distinct [functions in intension](#function-in-intension) can have this same extension. Properties of the extension of an arbitrary program are semantic properties, to which [Rice theorem](#rice-s-theorem) applies when the property is nontrivial.

## Binary diagonally noncomputable function

↑ **Parent:** [Computability theory](computability-theory.md)

A total binary-valued [function](function.md) is diagonally noncomputable if it differs from each defined diagonal value in an effective enumeration of [partial computable functions](#computable-function). Nonbinary diagonal outputs are automatically different. No such [function](function.md) is computable: its own program index would contradict the defining condition. Choosing the opposite bit at every defined binary diagonal value proves existence without supplying a computable procedure.

## Bounded simulation of a computation

↑ **Parent:** [Computability theory](computability-theory.md)

A bounded simulation records whether a specified deterministic program has halted, with a specified output, within a given finite number of steps. This is a primitive recursive predicate of the program code, input and time bound. [Peano arithmetic](mathematical-logic.md#peano-arithmetic) can verify genuine finite computation certificates and prove that two different outputs cannot both be the first halting output.

## Productive set

↑ **Parent:** [Computability theory](computability-theory.md)

A set $P$ is productive when a [partial computable function](#computable-function) returns an element of $P$ outside any [computably enumerable](#recursively-enumerable-set) subset supplied by its index. The [function](function.md) must halt for every index of a subset of $P$, including finite subsets. Productive sets are not [computably enumerable](#recursively-enumerable-set).

### Productivity of arithmetic truth

↑ **Parent:** [Productive set](#productive-set)

Uniformly diagonalize against the formula expressing membership in $W_e$ to obtain a sentence saying that its own code is not in $W_e$. If every enumerated sentence is true, this new sentence cannot be enumerated, and hence is true. Its code is a computable new element of [arithmetic truth](mathematical-logic.md#true-arithmetic) outside $W_e$.

## Kolmogorov complexity

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov_complexity)

[Kolmogorov complexity](#kolmogorov-complexity) measures the length of a shortest effective description of an object. Fixing an [optimal description machine](#optimal-description-machine) gives an invariant quantity up to an additive machine-dependent constant. [Plain Kolmogorov complexity](#plain-kolmogorov-complexity) is especially convenient for counting descriptions shorter than a [binary string](theoretical-computer-science.md#binary-string).

### Plain Kolmogorov complexity

↑ **Parent:** [Kolmogorov complexity](#kolmogorov-complexity)

For a fixed [optimal description machine](#optimal-description-machine) $U$, the [plain Kolmogorov complexity](#plain-kolmogorov-complexity) of a [binary string](theoretical-computer-science.md#binary-string) is the minimum length of a finite program producing it. The admissible programs need not satisfy a prefix restriction. There are at most $2^n-1$ descriptions shorter than $n$, which is the counting fact behind the existence of [incompressible strings](#incompressible-string).

#### Incompressible string

↑ **Parent:** [Plain Kolmogorov complexity](#plain-kolmogorov-complexity)

A [binary string](theoretical-computer-science.md#binary-string) is incompressible relative to a fixed [optimal description machine](#optimal-description-machine) when its [plain Kolmogorov complexity](#plain-kolmogorov-complexity) is at least its length. A counting argument gives at least one such string at each length, and their set is immune.

##### Immunity of incompressible strings

↑ **Parent:** [Incompressible string](#incompressible-string)

If an infinite [computably enumerable](#recursively-enumerable-set) family contained only [incompressible strings](#incompressible-string), select its first enumerated string of length at least $n$. This is a total computable selection rule, and its selected string has a description of length $O(\log n)$ encoding the threshold. For large $n$ that is shorter than the selected string. This contradiction proves immunity.

### Optimal description machine

↑ **Parent:** [Kolmogorov complexity](#kolmogorov-complexity)

A description machine is a partial computable map from finite binary programs to finite binary outputs. It is optimal if, for every other description machine $V$, there is a constant $c_V$ such that $C_U(\sigma)\leq C_V(\sigma)+c_V$. Encoding an interpreter index in a fixed prefix gives the constant-overhead descriptions used in incompressibility arguments.

## Undecidable decision problem

↑ **Parent:** [Computability theory](computability-theory.md)

A decision problem for which no [algorithm](algorithm.md) terminates with the correct yes-or-no answer on every input. For example, if the [diagonal halting set](foundations-of-mathematics.md#diagonal-halting-set) had a decision algorithm, a program could halt on its own code exactly when that algorithm says it does not halt, producing a contradiction. An [undecidable decision problem](#undecidable-decision-problem) may still admit a partial procedure that terminates on every yes-instance.

## Finite-injury priority construction

↑ **Parent:** [Computability theory](computability-theory.md)

A finite-injury priority construction orders countably many requirements so that each has finitely many predecessors. A strategy may discard lower-priority strategies' current witnesses and restraints when it acts. If each requirement acts finitely often after its last such initialization, induction on priority shows that every requirement is injured only finitely often and eventually has a stable strategy. The [Friedberg–Muchnik theorem](#friedberg-muchnik-theorem) is a central example.

### Priority restraint

↑ **Parent:** [Finite-injury priority construction](#finite-injury-priority-construction)

A [priority restraint](#priority-restraint) protects finitely many oracle answers by requiring lower-priority enumerations to avoid positions below a numerical bound. Higher-priority action can cancel the [priority restraint](#priority-restraint) by initializing its owner. After the last such injury, the protected computation is permanent.

#### Preservation of a restrained oracle computation

↑ **Parent:** [Priority restraint](#priority-restraint)

An oracle computation queries only finitely many positions. If the oracle remains unchanged below its use, the same computation has the same output. In a [finite-injury priority construction](#finite-injury-priority-construction), a successful requirement imposes this bound on lower priorities; the induction that higher priorities stop acting then makes the disagreement permanent.

### Private-witness diagonalization for incomparable enumerable sets

↑ **Parent:** [Finite-injury priority construction](#finite-injury-priority-construction)

To prevent a [Turing functional](#turing-functional) $\Phi_e^B$ from computing the [indicator function](measure-theory.md#indicator-function) of an enumerated [set](set.md) $A$, reserve a permanently unique fresh witness $x$. On observing a convergent computation with [oracle use](#oracle-use) $u$, enumerate $x$ into $A$ if the answer is zero; otherwise keep it out. Restrain subsequent lower-priority enumerations into $B$ below $u$. Higher-priority actions may initialize this strategy and retire its witness, but witnesses are never reused. In a [finite-injury priority construction](#finite-injury-priority-construction), [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on priority shows that the final computation, if observed, remains correct as a computation from the final oracle and disagrees with $A$ at $x$. If no computation is ever observed after the final initialization, the final oracle computation diverges, since any convergent computation uses only finitely many eventually stable oracle bits.

<h3 id="friedberg-muchnik-theorem">Friedberg–Muchnik theorem</h3>

↑ **Parent:** [Finite-injury priority construction](#finite-injury-priority-construction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Friedberg–Muchnik_theorem)

There are [computably enumerable sets](#recursively-enumerable-set) $A,B$ with $A\not\leq_TB$ and $B\not\leq_TA$. A [finite-injury priority construction](#finite-injury-priority-construction) alternates requirements preventing oracle programs for $B$ from computing $A$ and programs for $A$ from computing $B$. Each requirement uses a private witness, enumerates it when the opposing computation gives zero, and restrains the oracle segment preserving that disagreement. Verification inducts on priority. Both degrees are noncomputable and strictly below the halting degree, resolving [Post problem](#post-problem).

The incomparable-degree formulation is stated in [Steffen Lempp's notes, section 1.1](https://people.math.wisc.edu/~slempp/papers/prio.pdf).

### Finite injury

↑ **Parent:** [Finite-injury priority construction](#finite-injury-priority-construction)

An injury discards a strategy's current witness or restraint when a higher-priority action changes its assumptions. Finite injury means that each strategy experiences only finitely many such resets. The final uninjured strategy must still be checked to satisfy its requirement; finite injury alone is not the conclusion.

## Turing reduction

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turing_reduction)

A set $A$ is Turing-reducible to $B$ when an [oracle machine](theoretical-computer-science.md#oracle-machine) with membership oracle $B$ computes the characteristic function of $A$. Unlike a [many-one reduction](#many-one-reduction), it may make adaptive queries and reverse or combine oracle answers.

### Oracle-assisted finite-extension construction

↑ **Parent:** [Turing reduction](#turing-reduction)

Build an infinite oracle as an increasing union of finite [binary strings](theoretical-computer-science.md#binary-string). With the [diagonal halting set](foundations-of-mathematics.md#diagonal-halting-set) as an oracle, decide whether some finite extension makes a specified [Turing functional](#turing-functional) halt with a binary output at a fresh input. In a yes case, preserve that finite computation and commit the opposing set's bit to the opposite value. In a no case, no subsequent infinite extension can yield a characteristic-function value there. Length growth makes the resulting sets computable in the halting oracle.

### Turing functional

↑ **Parent:** [Turing reduction](#turing-reduction)

A Turing functional is a partial computation performed by an [oracle machine](theoretical-computer-science.md#oracle-machine), viewed as a function of both the oracle $B$ and input $x$. Oracle programs admit an effective enumeration. Every convergent computation inspects only a finite part of its oracle, recorded by its [oracle use](#oracle-use).

#### Oracle use

↑ **Parent:** [Turing functional](#turing-functional)

The use of a convergent oracle computation is one more than its largest queried position, or zero if there are no queries. Preserving the oracle below this number preserves the computation. This finite dependence supplies the restraints in a [finite-injury priority construction](#finite-injury-priority-construction).

### Turing degree

↑ **Parent:** [Turing reduction](#turing-reduction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turing_degree)

The Turing degree of a set is its equivalence class under mutual [Turing reducibility](#turing-reduction). Degrees inherit the partial order induced by Turing reducibility. The [Friedberg–Muchnik theorem](#friedberg-muchnik-theorem) gives incomparable degrees represented by [computably enumerable sets](#recursively-enumerable-set).

<h4 id="kleene-post-incomparability-theorem">Kleene–Post incomparability theorem</h4>

↑ **Parent:** [Turing degree](#turing-degree)

There are incomparable [Turing degrees](#turing-degree) strictly between the computable degree and the degree of the [diagonal halting set](foundations-of-mathematics.md#diagonal-halting-set). An [oracle-assisted finite-extension construction](#oracle-assisted-finite-extension-construction) alternately defeats each [Turing functional](#turing-functional) in the two directions. Since the sets are computable in the halting oracle, their degrees are at most $0'$; incomparability makes them nonzero and strictly below $0'$. This theorem does not require the constructed sets to be [computably enumerable](#recursively-enumerable-set). The [Friedberg–Muchnik theorem](#friedberg-muchnik-theorem) supplies that stronger conclusion.

#### Post problem

↑ **Parent:** [Turing degree](#turing-degree)

Post problem asks whether a [computably enumerable set](#recursively-enumerable-set) can have a [Turing degree](#turing-degree) strictly between the computable degree and the degree of the [halting problem](foundations-of-mathematics.md#halting-problem). The [Friedberg–Muchnik theorem](#friedberg-muchnik-theorem) answers yes by constructing two incomparable computably enumerable degrees.

<h2 id="church-turing-thesis">Church–Turing thesis</h2>

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Church–Turing_thesis)

The Church–Turing thesis asserts that every effectively calculable function is computable by a formal model equivalent to a [Turing machine](theoretical-computer-science.md#turing-machine). It identifies an informal notion of effective procedure with a mathematical class rather than stating a theorem within one formal system.

## Pairing function

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pairing_function)

A [pairing function](#pairing-function) is a [computable function](#computable-function) that gives a [bijection](function.md#bijection) from the [Cartesian product](set-theory.md#cartesian-product) $\mathbb N_0^2$ to $\mathbb N_0$, with two [computable functions](#computable-function) recovering its coordinates. Here $\mathbb N_0=\{0,1,2,\ldots\}$ consists of the [natural numbers](arithmetic.md#natural-number), including zero. If $p$ is the [pairing function](#pairing-function) and $L,R$ its decoding [functions](function.md), the requirements are

$$
L(p(x,y))=x,\qquad R(p(x,y))=y,\qquad p(L(z),R(z))=z.
$$

Every [ordered pair](set.md#ordered-pair) has exactly one code, every code represents an [ordered pair](set.md#ordered-pair), and decoding always terminates. For a [bijection](function.md#bijection) given by a [total computable function](#total-computable-function), computability of the [inverse function](function.md#inverse-function) also follows by enumerating all [ordered pairs](set.md#ordered-pair) until the one with code $z$ appears. A [primitive recursive pairing function](#primitive-recursive-pairing-function) makes the stronger requirement that both encoding and coordinate decoding are [primitive recursive](#primitive-recursive-function).

The [Cantor pairing function](cardinal-number.md#cantor-pairing-function) makes this concrete through [triangular numbers](arithmetic.md#triangular-number):

$$
T(s)=\frac{s(s+1)}2,\qquad \pi(x,y)=T(x+y)+y.
$$

On the diagonal $x+y=s$, list $(s,0),(s-1,1),\ldots,(0,s)$. There are $s+1$ [ordered pairs](set.md#ordered-pair) there, and $T(s)$ [ordered pairs](set.md#ordered-pair) on earlier diagonals. Their codes therefore occupy precisely the consecutive [natural numbers](arithmetic.md#natural-number) from $T(s)$ through $T(s+1)-1$. These intervals touch without overlapping and cover all [natural numbers](arithmetic.md#natural-number); within each interval the offset $y$ determines the [ordered pair](set.md#ordered-pair). This proves both [injectivity](algebra.md#injective-function) and [surjectivity](algebra.md#surjective-function), hence the [bijection](function.md#bijection). It also explains why the infinite grid is a [countably infinite set](cardinal-number.md#countably-infinite-set): every [ordered pair](set.md#ordered-pair) is reached after finitely many steps. A row-by-row listing would never finish its first infinite row. Authored treatments give the same diagonal construction with the coordinates exchanged.[Klaus Sutner, Primitive Recursion, Carnegie Mellon University, spring 2021, slides 9–13: pairing systems and the Cantor polynomial](https://www.cs.cmu.edu/~cdm/resources/02-coding.pdf)

For example, the [Cantor pairing function](cardinal-number.md#cantor-pairing-function) gives

$$
\pi(0,0)=0,\qquad \pi(1,0)=1,\qquad \pi(0,1)=2,\qquad \pi(2,3)=T(5)+3=18.
$$

The order of the coordinates matters: $(1,0)$ and $(0,1)$ are different [ordered pairs](set.md#ordered-pair) with different codes.

<a id="image-the-cantor-pairing-function-on-a-finite-window-labels-are-codes-and-the-first-21-ordered-pairs-fill-diagonals-zero-through-five"></a>
![](cantor-pairing-diagonal-enumeration.png)

**[Figure 1](#image-the-cantor-pairing-function-on-a-finite-window-labels-are-codes-and-the-first-21-ordered-pairs-fill-diagonals-zero-through-five). The Cantor pairing function on a finite window: labels are codes, and the first 21 ordered pairs fill diagonals zero through five**.

To decode a [natural number](arithmetic.md#natural-number) $z$, find the unique diagonal index $s$ satisfying

$$
T(s)\leq z<T(s+1),\qquad y=z-T(s),\qquad x=s-y.
$$

The [inequality](arithmetic.md#inequality-mathematics) gives $0\leq y\leq s$, so both recovered coordinates are [natural numbers](arithmetic.md#natural-number). At $z=18$, $T(5)=15\leq18<T(6)=21$, hence $s=5$, $y=18-15=3$, and $x=5-3=2$. At $z=0$, $s=0$ and both coordinates are zero. Solving the quadratic [inequality](arithmetic.md#inequality-mathematics) gives the equivalent [floor function](calculus.md#floor-function) expression

$$
s=\left\lfloor\frac{\sqrt{8z+1}-1}{2}\right\rfloor.
$$

This is exact as a statement about the [real numbers](arithmetic.md#real-number) and their [square roots](algebra.md#square-root). An implementation using [floating-point arithmetic](floating-point-arithmetic.md) can round across a diagonal boundary, especially for large $z$. Use an exact integer [square root](algebra.md#square-root) instead: with $q=\lfloor\sqrt{8z+1}\rfloor$ computed using integer arithmetic, $s=\lfloor(q-1)/2\rfloor$. Alternatively, search for the diagonal using exact integer comparisons. The [primitive recursive pairing function](#primitive-recursive-pairing-function) proof below uses [bounded minimization](#bounded-minimization) and needs no approximate [square root](algebra.md#square-root).

A [pairing function](#pairing-function) is a reversible encoding: unlike a [hash function](computer-science.md#hash-function) mapping arbitrarily many inputs into a fixed finite range, it loses no coordinates. This works because the mathematical [natural numbers](arithmetic.md#natural-number) have no upper bound. A machine word with $b$ [binary digits](integer.md#binary-digit) has $2^b$ possible values, while two such words have $2^{2b}$ possible [ordered pairs](set.md#ordered-pair); a [bijection](function.md#bijection) into one word of the same width is impossible. Evaluating the [Cantor pairing function](cardinal-number.md#cantor-pairing-function) in a fixed-width integer type can overflow, including in the intermediate product $(x+y)(x+y+1)$. Exact implementation requires sufficiently large integer storage or an explicit restricted input range. One mathematical code need not occupy fewer [binary digits](integer.md#binary-digit) than its two inputs.

Iterating a [pairing function](#pairing-function) gives a reversible encoding of [tuples](set-theory.md#finite-tuple) of any fixed positive length. With the left-nesting convention, the [Cantor pairing function](cardinal-number.md#cantor-pairing-function) encodes $(2,3,4)$ as

$$
\pi(\pi(2,3),4)=\pi(18,4)=T(22)+4=253+4=257.
$$

Decode the outer [ordered pair](set.md#ordered-pair) first: $T(22)\leq257<T(23)=276$ gives $(18,4)$. Decode its first coordinate $18$ to recover $(2,3)$, giving the nested [ordered pair](set.md#ordered-pair) $((2,3),4)$ and thus the original [tuple](set-theory.md#finite-tuple) $(2,3,4)$.

<a id="image-decoding-a-known-three-entry-tuple-first-unpair-257-into-18-4-then-unpair-18-into-2-3"></a>
![](pairing-function-tuple-decoding.png)

**[Figure 2](#image-decoding-a-known-three-entry-tuple-first-unpair-257-into-18-4-then-unpair-18-into-2-3). Decoding a known three-entry tuple: first unpair 257 into (18, 4), then unpair 18 into (2, 3)**

The [tuple](set-theory.md#finite-tuple) length and nesting convention must be known. The same code $257$ represents $(18,4)$ as a two-entry [tuple](set-theory.md#finite-tuple) and $(2,3,4)$ as a three-entry [tuple](set-theory.md#finite-tuple); nesting alone does not make variable-length [tuples](set-theory.md#finite-tuple) self-describing. To encode variable-length [tuples](set-theory.md#finite-tuple), supply their length or another explicit termination convention as part of the encoding. This simple change of representation is useful in [computability theory](computability-theory.md) and [Gödel numbering](mathematical-logic.md#godel-numbering): a [function](function.md) of several [natural numbers](arithmetic.md#natural-number) can be studied through a single numerical input, while all coordinates remain recoverable. The striking fact is that a whole infinite grid can be serialized without omitting a point.

A historical reference for comparing [sets](set.md) through [bijections](function.md#bijection) is Georg Cantor's paper _Ein Beitrag zur Mannigfaltigkeitslehre_, published in 1878 in volume 84 of _Journal für die reine und angewandte Mathematik_, pages 242–258.[Georg Cantor, Ein Beitrag zur Mannigfaltigkeitslehre, 1878: publisher bibliographic record](https://doi.org/10.1515/crelle-1878-18788413)

### Primitive recursive pairing function

↑ **Parent:** [Pairing function](#pairing-function)

A [primitive recursive pairing function](#primitive-recursive-pairing-function) is a [pairing function](#pairing-function) whose encoding [function](function.md) and both coordinate [functions](function.md) of its [inverse function](function.md#inverse-function) are [primitive recursive functions](#primitive-recursive-function). Thus the [bijection](function.md#bijection) can be used in either direction inside a construction by [primitive recursion](#primitive-recursion) and [function composition in recursion theory](#function-composition-in-recursion-theory). A decoder that is merely a [computable function](#computable-function) would not establish this stronger closure property. Sutner's definition of a primitive recursive pairing system explicitly includes the decoding [functions](function.md); his more general systems need only be [injective](algebra.md#injective-function), whereas a [pairing function](#pairing-function) here is a [bijection](function.md#bijection).[Klaus Sutner, Primitive Recursion, slide 9: primitive recursive encoding and unpairing functions](https://www.cs.cmu.edu/~cdm/resources/02-coding.pdf)

The [Cantor pairing function](cardinal-number.md#cantor-pairing-function) is a [primitive recursive pairing function](#primitive-recursive-pairing-function). For its encoding, construct the [triangular numbers](arithmetic.md#triangular-number) directly by [primitive recursion](#primitive-recursion):

$$
T(0)=0,\qquad T(s+1)=T(s)+s+1,\qquad \pi(x,y)=T(x+y)+y.
$$

Since [addition](arithmetic.md#addition) is [primitive recursive](#primitive-recursive-function), so are $T$ and $\pi$ by [primitive recursion](#primitive-recursion) and [function composition in recursion theory](#function-composition-in-recursion-theory). This establishes the claim without treating [division](arithmetic.md#division-mathematics) by two as an unexplained primitive operation.

For decoding, use [bounded minimization](#bounded-minimization) to define

$$
s(z)=\min\{t\in\mathbb N_0:t\leq z\ \text{and}\ z<T(t+1)\}.
$$

The bound is valid for every [natural number](arithmetic.md#natural-number) $z$: $T(z+1)=(z+1)(z+2)/2>z$, so the candidate $t=z$ always succeeds. The search includes zero; when $z=0$, it immediately returns $s(0)=0$. If $s(z)>0$, the preceding candidate failed, which gives $T(s(z))\leq z$; when $s(z)=0$, that lower [inequality](arithmetic.md#inequality-mathematics) follows from $T(0)=0$. Thus this search finds exactly the diagonal in the [Cantor pairing function](cardinal-number.md#cantor-pairing-function) inverse, with

$$
T(s(z))\leq z<T(s(z)+1).
$$

The comparison is [primitive recursive](#primitive-recursive-function), and [bounded minimization](#bounded-minimization) of a [primitive recursive](#primitive-recursive-function) predicate is [primitive recursive](#primitive-recursive-function). Therefore $s$ is a [primitive recursive function](#primitive-recursive-function). Recover the coordinates by

$$
R(z)=z-T(s(z)),\qquad L(z)=s(z)-R(z).
$$

In constructions on the [natural numbers](arithmetic.md#natural-number), implement these [subtractions](arithmetic.md#subtraction) using the [primitive recursive](#primitive-recursive-function) operation $a\mathbin{\dot{-}}b=\max(a-b,0)$: apply the [predecessor function](#predecessor-function) $b$ times to $a$ by [primitive recursion](#primitive-recursion). On these inputs it agrees with ordinary [subtraction](arithmetic.md#subtraction), since the diagonal [inequalities](arithmetic.md#inequality-mathematics) imply $0\leq R(z)\leq s(z)$. Consequently $L$ and $R$ are [primitive recursive functions](#primitive-recursive-function), and $\pi(L(z),R(z))=z$. Zimmermann proves the relevant closure under [bounded minimization](#bounded-minimization) and the primitive recursive character of the Cantor encoding and coordinate decoding; his convention adds the first coordinate, so its coordinates are exchanged relative to $\pi$ here.[Karl-Heinz Zimmermann, Computability Theory, §2.3, Proposition 2.26 and Propositions 2.32–2.34, printed pages 18 and 21–22](https://tore.tuhh.de/bitstream/11420/1312/1/book.pdf)

For a worked [bounded minimization](#bounded-minimization), take $z=18$. Candidates $t=0,1,2,3,4$ give $T(t+1)=1,3,6,10,15$, none exceeding $18$. Candidate $t=5$ gives $T(6)=21>18$, so $s(18)=5$, $R(18)=3$, and $L(18)=2$. The search bound was $18$; it terminates much earlier in this example. The bound proves membership in the [primitive recursive functions](#primitive-recursive-function); it is not a claim that scanning all candidates is the fastest implementation.

For each fixed $k\geq1$, define a [tuple](set-theory.md#finite-tuple) encoder by

$$
E_1(a_1)=a_1,\qquad E_{k+1}(a_1,\ldots,a_{k+1})=\pi(E_k(a_1,\ldots,a_k),a_{k+1}).
$$

Each $E_k$ and each coordinate decoder is [primitive recursive](#primitive-recursive-function), by finitely many applications of [function composition in recursion theory](#function-composition-in-recursion-theory) to $\pi,L,R$. For the three-entry [tuple](set-theory.md#finite-tuple) encoded as $257$, applying $R$ returns $4$, applying $L$ returns $18$, and then $L(18)=2$, $R(18)=3$. The [tuple](set-theory.md#finite-tuple) length remains part of the agreed convention, as explained for a general [pairing function](#pairing-function).

This makes [primitive recursive pairing functions](#primitive-recursive-pairing-function) useful for encoding several evolving values as one state in [primitive recursion](#primitive-recursion). For example, store consecutive [Fibonacci numbers](sequence-and-series.md#fibonacci-number) as $c(0)=\pi(0,1)$ and update by

$$
c(n+1)=\pi(R(c(n)),L(c(n))+R(c(n))).
$$

The codes start $2,4,8,18$, decoding to $(0,1),(1,1),(1,2),(2,3)$. Every step uses [primitive recursive](#primitive-recursive-function) encoding, decoding and [addition](arithmetic.md#addition); a single numerical state therefore carries the two values needed for the next step. This is also the reason a suitable [Gödel numbering](mathematical-logic.md#godel-numbering) should permit sufficiently simple decoding: representation should preserve the class of [functions](function.md) being studied.

### Decimal trailing-zero pairing function

↑ **Parent:** [Pairing function](#pairing-function)

The bracket enumerates the positive [integers](integer.md) not divisible by $10$. Every positive [integer](integer.md) has exactly one decomposition into a power of $10$ times such an integer, so this formula is a [bijection](function.md#bijection) from $\mathbb N^2$ to $\mathbb N$. Subtracting one in the codomain includes zero without requiring a trailing-zero convention for its decimal representation. For the inverse, write $N+1=10^i q$ with $10\nmid q$, then $j=q-1-\lfloor q/10\rfloor$.

## Register machine

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Register_machine)

A register machine has finitely many states and finitely many addressed registers, together with instructions that inspect and modify register contents and change state. A computed partial function is defined by the contents at the halt state.

### String register machine

↑ **Parent:** [Register machine](#register-machine)

In a string register machine, $+_a(k,q)$ appends $a$ to register $k$; $?_a(k,p,q)$ branches according to whether its final letter is $a$; $?_\varepsilon(k,p,q)$ tests emptiness; and $-(k,p,q)$ branches to $p$ when empty, or deletes the final letter and branches to $q$ otherwise.

#### Characteristic-function register machine

↑ **Parent:** [String register machine](#string-register-machine)

A machine computes the characteristic function of a language $X$ when it halts on every input with the one-letter output $1$ for inputs in $X$ and $0$ for inputs outside $X$.

##### One-register separation for equal block lengths

↑ **Parent:** [Characteristic-function register machine](#characteristic-function-register-machine)

Two string registers can recognize $\{a^nb^n:n>0\}$ by storing one marker per $a$ and removing one per $b$. A machine with only its input register cannot: two different terminal $b$-block lengths eventually reach the same state and remaining prefix, forcing equal outputs for one member and one nonmember.

##### String register-machine suffix test

↑ **Parent:** [Characteristic-function register machine](#characteristic-function-register-machine)

To recognize words ending in a fixed symbol $a$, test the final input letter, choose one of two erasing loops, and append $1$ after the accepting loop or $0$ after the rejecting loop. The empty word follows the rejecting branch.

##### Complementing a characteristic-function register machine

↑ **Parent:** [Characteristic-function register machine](#characteristic-function-register-machine)

Replace the original halt state by a continuation state that tests whether its one-letter output is $0$ or $1$, removes it, appends the other symbol, and enters a new halt state. This computes the complement language without changing termination behavior.

## Primitive recursive function

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_recursive_function)

Primitive recursive functions are generated by zero, successor, and projections under composition and primitive recursion.

### Primitive recursive syntax and arity checking

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

For a decidable coding of finite construction trees, the codes of arity-$i$ [primitive recursive functions in intension](#primitive-recursive-function-in-intension) are decidable. Check initial-function tags, then verify the child arities at each composition and recursion node. This is a terminating finite syntax check, distinct from asking whether an arbitrary program's extension happens to be [primitive recursive](#primitive-recursive-function).

#### Total computable diagonal over primitive recursive syntax

↑ **Parent:** [Primitive recursive syntax and arity checking](#primitive-recursive-syntax-and-arity-checking)

Enumerate all valid unary [primitive recursive functions in intension](#primitive-recursive-function-in-intension) by their decidable codes $p_n$, and interpret each extension $F_{p_n}$. The [function](function.md) $d(n)=F_{p_n}(n)+1$ is a [total computable function](#total-computable-function), since each finite construction terminates. If it were [primitive recursive](#primitive-recursive-function), some $F_{p_j}$ would equal $d$, giving $d(j)=d(j)+1$. Repeated extensions in the syntax enumeration do not affect this argument.

#### Primitive recursive function in intension

↑ **Parent:** [Primitive recursive syntax and arity checking](#primitive-recursive-syntax-and-arity-checking)

A valid finite construction expression from the [initial functions of recursion theory](#initial-function-of-recursion-theory) by [function composition in recursion theory](#function-composition-in-recursion-theory) and [primitive recursion](#primitive-recursion). Its extension is a [primitive recursive function](#primitive-recursive-function). The construction grammar supplies both a decidable syntax and a total computable interpreter, but no uniformly primitive recursive interpreter for all valid codes.

### Bounded halting predicate

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

For a fixed effective machine coding, the predicate that program $e$ on input $x$ halts within $t$ steps is [primitive recursive](#primitive-recursive-function). Code finite configurations, iterate a total single-step function by [primitive recursion](#primitive-recursion), and test for the halt state. This supplies a bounded simulation even though the unrestricted [halting problem](foundations-of-mathematics.md#halting-problem) is undecidable.

### Bounded minimization

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

Search over the finite interval $0\leq y\leq b$ for the least witness to a [primitive recursive](#primitive-recursive-function) predicate, with an explicitly chosen default if there is none. The result is a [primitive recursive function](#primitive-recursive-function), by scanning this finite interval using [primitive recursion](#primitive-recursion). This differs from [unbounded minimization](#mu-operator), which may fail to terminate.

### Predecessor function

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

The predecessor function on the nonnegative integers is $\operatorname{pred}(0)=0$ and $\operatorname{pred}(n+1)=n$. This is a [primitive recursive function](#primitive-recursive-function) by primitive recursion from the zero and projection functions.

### Initial function of recursion theory

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

The initial functions are the zero function, the successor function, and all coordinate projections.

#### Zero function

↑ **Parent:** [Initial function of recursion theory](#initial-function-of-recursion-theory)

The zero function has the constant value

$$
Z(x)=0.
$$

Dummy variables give a zero function of any finite arity.

#### Successor function

↑ **Parent:** [Initial function of recursion theory](#initial-function-of-recursion-theory)

The successor function is

$$
S(n)=n+1.
$$

#### Projection function

↑ **Parent:** [Initial function of recursion theory](#initial-function-of-recursion-theory)

The $i$th $k$-ary projection returns its $i$th input:

$$
\pi_i^k(x_1,\ldots,x_k)=x_i.
$$

### Function composition in recursion theory

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

Given a $m$-ary function $g$ and $k$-ary functions $h_1,\ldots,h_m$, composition forms

$$
f(\mathbf x)=g(h_1(\mathbf x),\ldots,h_m(\mathbf x)).
$$

### Primitive recursion

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_recursion)

From $g:\mathbb N^k\to\mathbb N$ and $h:\mathbb N^{k+2}\to\mathbb N$, primitive recursion defines

$$
f(\mathbf x,0)=g(\mathbf x),
\qquad
f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)).
$$

### Composition-only recursive function

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

The functions generated from the initial functions using composition alone are exactly

$$
f(\mathbf x)=c
\quad\hbox{or}\quad
f(\mathbf x)=x_i+c
$$

for a constant $c\in\mathbb N$. Structural induction proves necessity, and iterating the successor function on zero or a projection proves sufficiency.

### Structural induction for primitive recursive functions

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

To prove a property of every primitive recursive function, prove it for the zero, successor, and projection functions, then prove that it is preserved by composition and by primitive recursion. This is structural induction on the finite construction of the function.

#### Every primitive recursive function is total

↑ **Parent:** [Structural induction for primitive recursive functions](#structural-induction-for-primitive-recursive-functions)

The initial functions are total, composition preserves totality, and ordinary induction on the recursion argument shows that primitive recursion applied to total functions is total. Structural induction therefore proves that every primitive recursive function is total.

### Existential bounded representation of a primitive recursive function

↑ **Parent:** [Primitive recursive function](#primitive-recursive-function)

The graph of every primitive recursive $f:\mathbb N^k\to\mathbb N$ has a formula

$$
y=f(\mathbf x)\quad\Longleftrightarrow\quad
\exists\mathbf z\,\delta(y,\mathbf x,\mathbf z)
$$

in the language of ordered rings, where every quantifier inside $\delta$ is bounded. Composition uses existentially quantified intermediate values, while primitive recursion uses a boundedly checked code for the finite sequence of intermediate values.

<h4 id="godel-beta-function-sequence-coding">Gödel beta-function sequence coding</h4>

↑ **Parent:** [Existential bounded representation of a primitive recursive function](#existential-bounded-representation-of-a-primitive-recursive-function)

The Gödel beta function codes finite sequences by remainders:

$$
\beta(b,c,i)=r
\quad\Longleftrightarrow\quad
r<1+(i+1)c\ \land\ \exists q\leq b\,[b=q(1+(i+1)c)+r].
$$

Choosing $c$ sufficiently large and divisible by the relevant small integers makes the moduli pairwise coprime, so the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) codes any prescribed finite sequence.

##### Factorial graph formula via remainder coding

↑ **Parent:** [Gödel beta-function sequence coding](#godel-beta-function-sequence-coding)

The graph of the [factorial](combinatorics.md#factorial) function has a fixed-length [first-order formula](mathematical-logic.md#first-order-formula) in the [language of ordered rings](mathematical-logic.md#language-of-ordered-rings) interpreted on the [natural numbers](arithmetic.md#natural-number). A remainder code records $a_0=1$, $a_n=y$, and $a_{i+1}=(i+1)a_i$ for every $i<n$. Uniqueness of remainders proves $y=n!$; sufficiently large pairwise-coprime moduli and the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) supply a code for every input. Formula length is independent of the input variable's value, although substituting a numeral adds its encoding length.

##### Finite witness array coding

↑ **Parent:** [Gödel beta-function sequence coding](#godel-beta-function-sequence-coding)

In a [primitive recursion](#primitive-recursion), an existential representation of the step [function](function.md) may need a different witness tuple at every time. Code each coordinate of the finite witness array by a separate beta-function code pair. All row witnesses then have bounded remainder quantifiers under the bounded time quantifier, while the finitely many code pairs remain in the outer unrestricted existential block.

## Diagonal argument

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diagonal_argument)

A list $f(n,k)$ of all functions in a class closed under diagonal substitution and successor misses $d(k)=f(k,k)+1$.

## Recursively enumerable set

↑ **Parent:** [Computability theory](computability-theory.md)

A set is computably enumerable when a program halts precisely on its members. Equivalently, it is the domain of a [partial computable function](#computable-function) or some algorithm lists its elements.

### Simple set

↑ **Parent:** [Recursively enumerable set](#recursively-enumerable-set)

A [computably enumerable set](#recursively-enumerable-set) is simple when its [complement of a set](set.md#complement-of-a-set) is an [immune set](#immune-set): the complement is infinite and contains no infinite [computably enumerable](#recursively-enumerable-set) subset. Equivalently, it is coinfinite and meets every infinite [computably enumerable set](#recursively-enumerable-set). A simple set is not decidable.

#### Sparse-witness construction of a simple set

↑ **Parent:** [Simple set](#simple-set)

Enumerate all [computably enumerable sets](#recursively-enumerable-set) as $W_e$. For each $e$, once a witness $x>2e$ appears in $W_e$, enumerate one such witness into $X$ and never act for $e$ again. Every infinite $W_e$ supplies a witness. Only requirements $e<n$ can put numbers into $[0,2n]$, so at least $n+1$ numbers in that interval stay outside $X$. Thus $X$ is a [simple set](#simple-set). The proof uses a numerical bound rather than an infinitude test.

### Immune set

↑ **Parent:** [Recursively enumerable set](#recursively-enumerable-set)

An [immune set](#immune-set) is infinite but contains no infinite [computably enumerable](#recursively-enumerable-set) subset. Thus its infinitude cannot be witnessed by any effective infinite listing that stays entirely inside the set. Finite strings can be treated as natural-number codes for this definition.

### Nonempty computably enumerable sets are primitive recursive ranges

↑ **Parent:** [Recursively enumerable set](#recursively-enumerable-set)

Every nonempty [computably enumerable set](#recursively-enumerable-set) $X\subseteq\mathbb N$ is the range of a [primitive recursive function](#primitive-recursive-function) $f:\mathbb N\to\mathbb N$. Choose $x_0\in X$, decode $n=\langle x,t\rangle$ using a [primitive recursive pairing function](#primitive-recursive-pairing-function), and output $x$ if the recognizing machine halts within $t$ steps, or $x_0$ otherwise. The [bounded halting predicate](#bounded-halting-predicate) makes this function [primitive recursive](#primitive-recursive-function), and every member of $X$ occurs for a sufficiently large bound. The [empty set](set.md#empty-set) is excluded because such a function is total.

### Computable set

↑ **Parent:** [Recursively enumerable set](#recursively-enumerable-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computable_set)

A set is computable when an algorithm decides membership for every input and always halts. Equivalently, both the set and its complement are [computably enumerable](#recursively-enumerable-set).

### Domain and range characterizations of a nonempty computably enumerable set

↑ **Parent:** [Recursively enumerable set](#recursively-enumerable-set)

For a nonempty set $A$ of words, the following are equivalent: $A$ is [computably enumerable](#recursively-enumerable-set), $A$ is the domain of a [partial computable function](#computable-function), $A$ is the range of a partial computable function, and $A$ is the range of a [total computable function](#total-computable-function). The nonempty hypothesis is needed only for the last formulation, since the range of a total function cannot be empty.

<h2 id="kleene-s-recursion-theorem">Kleene's recursion theorem</h2>

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kleene's_recursion_theorem)

Kleene recursion gives programs access to their own effective descriptions: every computable transformation of program indices has a semantic fixed point.

## Many-one reduction

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Many-one_reduction)

A many-one reduction $A\leq_mB$ is a total computable $f$ satisfying $x\in A$ exactly when $f(x)\in B$.

### Many-one degree

↑ **Parent:** [Many-one reduction](#many-one-reduction)

Two sets have the same many-one degree when each many-one reduces to the other.

### Computable reduction by staged enumeration

↑ **Parent:** [Many-one reduction](#many-one-reduction)

A staged-enumeration reduction controls an output language by enumerating more elements at each simulation stage and changing behavior when a source computation halts.

### Many-one complete set

↑ **Parent:** [Many-one reduction](#many-one-reduction)

A set $A$ is complete for a class $\mathcal C$ under many-one reductions when $A\in\mathcal C$ and every $B\in\mathcal C$ satisfies $B\leq_mA$.

## Index set

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Index_set_(computability))

An index set is a set of program codes whose membership depends only on the partial function or enumerable language computed, rather than the code's syntax.

### Extensional property of programs

↑ **Parent:** [Index set](#index-set)

An extensional program property gives identical answers to all codes computing the same object.

<h3 id="rice-s-theorem">Rice's theorem</h3>

↑ **Parent:** [Index set](#index-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rice's_theorem)

Every nontrivial extensional property of partial computable functions or computably enumerable languages is undecidable.

### Infinite-domain index set

↑ **Parent:** [Index set](#index-set)

For an effective enumeration $f_{w,1}$ of unary partial computable functions,

$$
\mathbf{Inf}=\{w:\operatorname{dom}(f_{w,1})\text{ is infinite}\}
$$

is an index set.

#### Infinite-domain range-restriction index set

↑ **Parent:** [Infinite-domain index set](#infinite-domain-index-set)

For a nonempty set $X$ of words, the property

$$
w\in\mathbf{Inf}
\quad\hbox{and}\quad
\operatorname{ran}(f_{w,1})\subseteq X
$$

is a nontrivial extensional property of unary partial computable functions: the nowhere-defined function fails it, while any total constant function with value in $X$ satisfies it. The [Rice theorem](#rice-s-theorem) therefore makes its index set undecidable.

### Cofinite index set

↑ **Parent:** [Index set](#index-set)

The cofinite index set contains codes whose enumerable language has finite complement.

## Padding lemma

↑ **Parent:** [Computability theory](computability-theory.md)

The padding lemma produces infinitely many syntactically distinct program indices for the same computed function or language.

## Dovetailing

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dovetailing_(computer_science))

Dovetailing interleaves finite stages of multiple computations so that every computation that halts is eventually observed.

## Smn theorem

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smn_theorem)

The S-m-n theorem says that fixed inputs can be compiled into program codes by a total computable transformation. For every $m,n\geq1$, there is a total computable $s_n^m$ such that

$$
f_{s_n^m(e,x_1,\ldots,x_m),n}(y_1,\ldots,y_n)
=f_{e,m+n}(x_1,\ldots,x_m,y_1,\ldots,y_n)
$$

whenever either side is defined.

## Computable function

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computable_function)

A partial function is computable when a program returns its value on every input in its domain and runs forever on inputs outside its domain.

### Universal partial computable function

↑ **Parent:** [Computable function](#computable-function)

A universal partial computable function simulates the program with index $e$ on input $\mathbf x$, reproducing both its output and its divergence. Decode the finite program and repeatedly apply its transition rule. This gives a [partial computable function](#computable-function) of the code and inputs. There can be no total computable evaluator whose rows are precisely all [total computable functions](#total-computable-function), because $n\mapsto U(n,n)+1$ would be a missing diagonal row.

### Kleene normal form theorem

↑ **Parent:** [Computable function](#computable-function)

For every [partial computable function](#computable-function) $f(\mathbf x)$, there are total [primitive recursive functions](#primitive-recursive-function) $C,U$ such that

$$
f(\mathbf x)=U(\mu s\,[C(\mathbf x,s)=0]).
$$

Here $C$ is zero exactly on codes of valid halting computation histories for the chosen program and input, and $U$ extracts the final output. Coding finite configurations and finite histories makes checking every local step a bounded primitive recursive operation. If a computation halts, some history code passes and every passing code has the same output; if it does not halt, none passes. This is the usual normal-form version with the program index fixed; a universal predicate can also retain that index as an input.

### Mu operator

↑ **Parent:** [Computable function](#computable-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mu_operator)

For a partial function $g(\mathbf x,y)$, unbounded minimization defines

$$
f(\mathbf x)=\mu y\,[g(\mathbf x,y)=0]
$$

as the least $y$ at which $g$ is zero, provided the preceding required computations are defined. If no such $y$ is found, $f(\mathbf x)$ is undefined. Closing the [primitive recursive functions](#primitive-recursive-function) under this operation gives the partial recursive functions.

### Total computable function

↑ **Parent:** [Computable function](#computable-function)

A [total computable function](#total-computable-function) is a [computable function](#computable-function) whose domain is the entire input space.

A total computable function is a computable function whose domain contains every allowed input.

#### Provably total computable function

↑ **Parent:** [Total computable function](#total-computable-function)

For a theory of arithmetic $T$ and a program index $e$, the function $\varphi_e$ is provably total in $T$ when $T$ proves its canonical totality sentence

$$
\forall x\,\exists y\,\operatorname{Comp}(e,x,y).
$$

If $T$ is recursively axiomatized, the indices of its provably total functions form a computably enumerable set.

### Truncated computation function

↑ **Parent:** [Computable function](#computable-function)

For a program code $e$, input $x$, and time bound $t$, the truncated computation simulates program $e$ on $x$ for at most $t$ steps and reports either its output or that no halt occurred within the bound. This is a total computable function of $(e,x,t)$.

### Ackermann function

↑ **Parent:** [Computable function](#computable-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ackermann_function)

One convention for the [Ackermann function](#ackermann-function) on [nonnegative integers](arithmetic.md#natural-number) is

$$
A(0,n)=n+1,\quad A(m+1,0)=A(m,1),\quad A(m+1,n+1)=A(m,A(m+1,n)).
$$

Its two-argument recursion defines a [computable function](#computable-function); fixing the convention matters when defining an [inverse Ackermann function](#inverse-ackermann-function).

#### Inverse Ackermann function

↑ **Parent:** [Ackermann function](#ackermann-function)

For the displayed [Ackermann function](#ackermann-function) convention, one possible inverse-growth scale is $\alpha(n)=\min\{m\geq1:A(m,m)\geq n\}$ for positive [integers](integer.md) $n$. It gives $\alpha(n)=1$ through $3$, $2$ from $4$ through $7$, and $3$ from $8$ through $61$. Several [inverse Ackermann function](#inverse-ackermann-function) conventions occur in [algorithm](algorithm.md) analysis; changing convention can shift these small values without changing the very slow growth relevant to the [disjoint-set data structure](data-structure.md#disjoint-set-data-structure). This inverse-growth definition does not invert a two-variable [function](function.md) as an ordinary one-variable [inverse function](function.md#inverse-function).

## Arithmetical hierarchy

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arithmetical_hierarchy)

The arithmetical hierarchy classifies sets by alternating blocks of number quantifiers over computable predicates.

### Bounded quantifier

↑ **Parent:** [Arithmetical hierarchy](#arithmetical-hierarchy)

A bounded quantifier has the form $\exists x<t\,\varphi$ or $\forall x<t\,\varphi$, where the term $t$ does not contain $x$. It ranges over a finite initial segment in the standard natural numbers.

#### Arithmetic bounded formula

↑ **Parent:** [Bounded quantifier](#bounded-quantifier)

An [arithmetic bounded formula](#arithmetic-bounded-formula) uses only quantifiers bounded by [arithmetic](arithmetic.md) terms, such as $\exists u<t$ and $\forall u<t$, with the bound not containing the quantified variable. Existential bounded representation of a [primitive recursive function](#primitive-recursive-function) places all unrestricted existential variables in a single outer block.

#### Delta-0 formula

↑ **Parent:** [Bounded quantifier](#bounded-quantifier)

A $\Delta_0$ formula is an arithmetical formula in which every quantifier is bounded.

### Sigma-1 formula

↑ **Parent:** [Arithmetical hierarchy](#arithmetical-hierarchy)

A $\Sigma_1$ formula is equivalent to $\exists\mathbf y\,\delta$ with $\delta$ bounded. A $\Pi_1$ formula is equivalent to $\forall\mathbf y\,\delta$ with $\delta$ bounded.

#### Pi-1 formula

↑ **Parent:** [Sigma-1 formula](#sigma-1-formula)

### Sigma-1 set

↑ **Parent:** [Arithmetical hierarchy](#arithmetical-hierarchy)

A set $A$ is in $\Sigma_1$ exactly when it is the domain of a partial computable function. Equivalently, there is a computable predicate $R$ such that

$$
x\in A\quad\Longleftrightarrow\quad\exists t\,R(x,t).
$$

### Pi-2 set

↑ **Parent:** [Arithmetical hierarchy](#arithmetical-hierarchy)

A set is in $\Pi_2$ when membership can be written with one universal block followed by one existential block over a computable predicate. Equivalently, in the word-function formulation, there is a partial computable $f$ such that

$$
w\in P\quad\Longleftrightarrow\quad
\forall v\;f(w,v)\mathbin\downarrow.
$$

#### Totality problem

↑ **Parent:** [Pi-2 set](#pi-2-set)

For an effective enumeration of computably enumerable languages $W_v$, the totality problem is

$$
\mathbf{Tot}=\{v:W_v=\mathbb W\}.
$$

It is $\Pi_2$-complete: a $\Pi_2$ condition $w\in P\iff\forall x\,f(w,x)\downarrow$ maps effectively to a program whose domain is $\{x:f(w,x)\downarrow\}$.

##### Totality problem is not computably enumerable

↑ **Parent:** [Totality problem](#totality-problem)

If all indices of total computable functions could be enumerated as $e_0,e_1,\ldots$, then

$$
g(n)=\varphi_{e_n}(n)+1
$$

would be total and computable. Some $e_k$ would index $g$, giving $g(k)=g(k)+1$. Thus the totality problem is not computably enumerable.

## Recursively inseparable sets

↑ **Parent:** [Computability theory](computability-theory.md)

Disjoint sets $A,B\subseteq\mathbb N$ are recursively inseparable when no recursive set $C$ satisfies $A\subseteq C$ and $B\cap C=\varnothing$.

## Lambda calculus

↑ **Parent:** [Computability theory](computability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lambda_calculus)

Lambda calculus forms terms from variables, abstraction, and application, and computes by substitution.

### Normal-order reduction

↑ **Parent:** [Lambda calculus](#lambda-calculus)

A reduction strategy that contracts the leftmost outermost reducible expression first. If a [lambda calculus](#lambda-calculus) expression has a [beta-normal form](#beta-normal-form), this strategy reaches it, although the intermediate expressions can be large.

### Lambda model

↑ **Parent:** [Lambda calculus](#lambda-calculus)

A lambda model interprets variables, [lambda application](#lambda-application) and [lambda abstraction](#lambda-abstraction) so that [capture-avoiding substitution](#capture-avoiding-substitution) agrees with environments and all [beta equivalence](#beta-equivalence) equations hold. A [reflexive domain](#reflexive-domain) gives such an interpretation. Validity of [eta conversion](#eta-conversion) requires an extra inverse law and does not follow merely from a retraction.

#### Reflexive domain

↑ **Parent:** [Lambda model](#lambda-model)

A [pointed complete partial order](set.md#pointed-complete-partial-order) $D$ is reflexive when there are [Scott continuous maps](set.md#scott-continuous-map) $e:[D\to D]\to D$ and $p:D\to[D\to D]$ with $p\circ e=\mathrm{id}$. Define $a\cdot b=p(a)(b)$ and interpret [lambda abstraction](#lambda-abstraction) using $e$. The inverse law gives beta soundness; $e\circ p=\mathrm{id}$ additionally gives eta soundness.

##### Graph model of lambda calculus

↑ **Parent:** [Reflexive domain](#reflexive-domain)

Let $P\omega=\mathcal P(\mathbb N)$ ordered by [subset](set.md#subset). Encode a finite subset $u$ and output $n$ by a natural number $\langle u,n\rangle$. Define $a\cdot b=\{n:\exists u\subseteq b\text{ finite},\ \langle u,n\rangle\in a\}$ and $e(f)=\{\langle u,n\rangle:n\in f(u)\}$. Every [Scott continuous map](set.md#scott-continuous-map) satisfies $f(b)=\bigcup_{u\subseteq b\text{ finite}}f(u)$, proving that application is the projection of a retraction. [Lambda abstraction](#lambda-abstraction) has graph $\{\langle u,n\rangle:n\in\llbracket M\rrbracket_{\rho[x:=u]}\}$.

###### Approximation theorem for the graph model

↑ **Parent:** [Graph model of lambda calculus](#graph-model-of-lambda-calculus)

The interpretation of a [lambda term](#lambda-term) in the [graph model of lambda calculus](#graph-model-of-lambda-calculus) is the union of the interpretations of all its [finite Böhm approximants](#finite-bohm-approximant). Every finite indexed interpretation reduces monotonically to an indexed normal approximant. Taking the union over all occurrence indices gives one inclusion; replacing subterms by bottom and using beta soundness gives the other. This identifies denotational information with finite observable parts of a [Böhm tree](#bohm-tree).

###### Indexed lambda term

↑ **Parent:** [Graph model of lambda calculus](#graph-model-of-lambda-calculus)

An indexed [lambda term](#lambda-term) assigns a natural number to every subterm occurrence; one also admits a constant $\bot$ with empty interpretation. In the [graph model of lambda calculus](#graph-model-of-lambda-calculus), every syntax constructor is interpreted as usual and then intersected with $\{0,\ldots,n\}$ at its occurrence index $n$. All indexed interpretations are finite subsets of the unindexed interpretation, and their directed union recovers that interpretation.

###### Indexed beta reduction

↑ **Parent:** [Indexed lambda term](#indexed-lambda-term)

Use the binary finite-set encoding $e_k$ and Cantor code $\langle k,t\rangle$. Contracting $(\lambda x.P^n)^{m+1}Q^p$ gives the substituted body with its root index lowered by taking the minimum with $\min(m,n)$, replacing each occurrence $x^r$ by a copy of $Q$ with root index $\min(m,p,r)$. A zero-indexed abstraction instead substitutes $\bot$ and gives the body root index zero. Indices strictly budget the argument information that can be used by application. Finite-witness inequalities for the pairing code prove that indexed reduction increases the interpretation, although it can decrease the underlying [Böhm tree](#bohm-tree).

### Lambda term

↑ **Parent:** [Lambda calculus](#lambda-calculus)

A lambda term is a variable, an abstraction $\lambda x.M$, or an application $MN$, formed recursively from lambda terms $M$ and $N$.

#### Lambda application

↑ **Parent:** [Lambda term](#lambda-term)

Application $MN$ applies the [lambda term](#lambda-term) $M$ to the [lambda term](#lambda-term) $N$. It associates to the left: $MNP=(MN)P$. Together with variables and [lambda abstraction](#lambda-abstraction), it generates all [lambda terms](#lambda-term).

#### Lambda abstraction

↑ **Parent:** [Lambda term](#lambda-term)

A lambda abstraction $\lambda x.t$ binds the variable $x$ in the [lambda term](#lambda-term) $t$. In the [simply typed lambda calculus](#simply-typed-lambda-calculus), if $t:B$ under $x:A$, the abstraction has type $A\to B$; this is the [implication introduction rule](mathematical-logic.md#implication-introduction-rule) under the [Curry-Howard correspondence](mathematical-logic.md#curry-howard-correspondence).

### Untyped lambda calculus

↑ **Parent:** [Lambda calculus](#lambda-calculus)

The untyped lambda calculus forms terms from variables, abstraction, and application without assigning types.

#### Eta conversion

↑ **Parent:** [Untyped lambda calculus](#untyped-lambda-calculus)

Eta conversion expresses extensionality for a [lambda abstraction](#lambda-abstraction) whose fresh argument is only passed to a function. The side condition prevents removal of a genuine dependency. In a categorical model with $D\cong D^D$, the inverse laws for [currying](category.md#currying) and evaluation validate this conversion as well as [beta reduction](#beta-reduction).

#### Combinatory logic

↑ **Parent:** [Untyped lambda calculus](#untyped-lambda-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Combinatory_logic)

Combinatory logic describes computation by application and fixed combinator constants, eliminating bound variables through [bracket abstraction](#bracket-abstraction). Its intensional weak reduction does not identify every pair of terms that becomes beta-equivalent after translation into [lambda calculus](#lambda-calculus).

##### Bracket abstraction

↑ **Parent:** [Combinatory logic](#combinatory-logic)

Bracket abstraction removes a free variable from a [combinatory logic term](#combinatory-logic-term). The displayed clauses are applied in that order, giving $FV([x]T)=FV(T)\setminus\{x\}$ and $([x]T)A\to^*T[x:=A]$. Under the standard lambda expansions of $S,K,I$, the result is beta-equivalent to $\lambda x.T$. The recursive translation of lambda terms therefore preserves variables and application and reflects weak equivalence, but need not preserve all beta equivalences.

##### Combinatory logic term

↑ **Parent:** [Combinatory logic](#combinatory-logic)

A finite applicative expression over free variables and the combinator constants $S,K,I$, with application associating to the left. One may instead take $I$ as the abbreviation $SKK$. There is no variable binder in this syntax.

###### Weak combinatory reduction

↑ **Parent:** [Combinatory logic term](#combinatory-logic-term)

Weak combinatory reduction closes the displayed contractions under application contexts. Weak equivalence is its reflexive, symmetric, transitive closure. The adjective distinguishes this syntactic reduction from an extensional rule equating functions that agree after an extra argument. A weak normal form has no subexpression matching a contraction rule; a partially applied combinator can be such a normal form.

#### Head normal form

↑ **Parent:** [Untyped lambda calculus](#untyped-lambda-calculus)

A [lambda term](#lambda-term) has head normal form when it beta-reduces to a term $\lambda x_1\cdots x_k.\,yM_1\cdots M_r$ with a variable $y$ at the head. The argument terms need not be in [beta-normal form](#beta-normal-form). A term with no head normal form cannot be beta-equivalent to a [Church numeral](#church-numeral).

<h5 id="bohm-tree">Böhm tree</h5>

↑ **Parent:** [Head normal form](#head-normal-form)

The Böhm tree of an [unsolvable lambda term](#unsolvable-lambda-term) is $\bot$. If $M\to_\beta^*\lambda x_1\cdots x_n.yM_1\cdots M_r$ is a [head normal form](#head-normal-form), its Böhm tree has root label $\lambda x_1\cdots x_n.y$ and ordered children $BT(M_1),\ldots,BT(M_r)$. The tree may be infinite. [Church-Rosser theorem](#church-rosser-theorem) and [alpha equivalence](#alpha-equivalence) make this independent of the selected head reduct.

<h6 id="finite-bohm-approximant">Finite Böhm approximant</h6>

↑ **Parent:** [Böhm tree](#bohm-tree)

A finite Böhm approximant is $\bot$ or a finite [lambda term](#lambda-term) in the grammar $\lambda x_1\cdots x_n.yA_1\cdots A_r$, obtained by pruning a [Böhm tree](#bohm-tree). Equivalently it is a beta-bottom normal form obtained from a beta-equivalent term by replacing subterms by $\bot$; bottom reduction contracts $\bot N$ and $\lambda x.\bot$ to $\bot$. Its interpretation in the [graph model of lambda calculus](#graph-model-of-lambda-calculus) is included in that of the original term.

<h6 id="bohm-transformation">Böhm transformation</h6>

↑ **Parent:** [Böhm tree](#bohm-tree)

A Böhm transformation is a finite composition of [capture-avoiding substitutions](#capture-avoiding-substitution) and [lambda applications](#lambda-application) to chosen auxiliary terms. It can extract a finite-address subtree of a [Böhm tree](#bohm-tree) as a substitution instance of the corresponding argument term.

<h6 id="bohm-out-lemma">Böhm-out lemma</h6>

↑ **Parent:** [Böhm transformation](#bohm-transformation)

For a finite path in a [Böhm tree](#bohm-tree), choose $q$ at least the head arity at every preceding node. Replace relevant variables by $U_q=\lambda z_1\cdots z_q w.wz_1\cdots z_q$. After exposing each node, supply its initial bound variables with $U_q$, pad its $m$ arguments to $q$, and apply the projection $\lambda z_1\cdots z_q.z_i$ selecting the next child. Each step returns that child with accumulated substitutions, so iteration reaches a substitution instance of the chosen subtree. Tupling preserves all children until selection, even when the same variable occurs at several nodes.

<h6 id="bohm-separation-theorem">Böhm separation theorem</h6>

↑ **Parent:** [Böhm-out lemma](#bohm-out-lemma)

Two distinct closed [lambda terms](#lambda-term) in normal form for both [beta reduction](#beta-reduction) and [eta conversion](#eta-conversion) admit a separating context that maps them respectively to the two [Church Booleans](#church-boolean). Finite [Böhm trees](#bohm-tree) and the [Böhm-out lemma](#bohm-out-lemma) isolate their first genuine head disagreement. The qualification about [eta conversion](#eta-conversion) matters: distinct beta-normal forms that are eta-equivalent cannot be separated this way.

##### Unsolvable lambda term

↑ **Parent:** [Head normal form](#head-normal-form)

An unsolvable [lambda term](#lambda-term) has no [head normal form](#head-normal-form), equivalently it is not a [solvable lambda term](#solvable-lambda-term). [Capture-avoiding substitution](#capture-avoiding-substitution) and [lambda application](#lambda-application) preserve unsolvability: until a head variable appears, head contractions proceed within the original term and cannot inspect the supplied terms.

###### Easy lambda term

↑ **Parent:** [Unsolvable lambda term](#unsolvable-lambda-term)

A closed [lambda term](#lambda-term) $E$ is easy if adjoining $E=M$ to the equations of [beta equivalence](#beta-equivalence) remains nontrivial for every closed [lambda term](#lambda-term) $M$. If $E$ is easy, then $ET$ is easy for every closed $T$: use the consistent equation $E=\lambda x.M$ to obtain $ET=M$. Since $I$ is not easy and solvability produces $I$ by applications, easy terms are unsolvable. The converse need not hold.

##### Solvable lambda term

↑ **Parent:** [Head normal form](#head-normal-form)

A [lambda term](#lambda-term) is solvable if its closure by [lambda abstractions](#lambda-abstraction) over its [free variables](mathematical-logic.md#free-variable) can be applied to finitely many closed [lambda terms](#lambda-term) to obtain $I=\lambda x.x$ in [beta equivalence](#beta-equivalence). This is equivalent to having a [head normal form](#head-normal-form). A head variable in a [head normal form](#head-normal-form) can be replaced by a projection returning $I$; conversely [standardization theorem for beta reduction](#standardization-theorem-for-beta-reduction) traces any successful head computation back to a head variable of the original term.

#### Beta reduction

↑ **Parent:** [Untyped lambda calculus](#untyped-lambda-calculus)

Beta reduction performs [capture-avoiding substitution](#capture-avoiding-substitution):

$$
(\lambda x.M)N\longrightarrow_\beta M[x:=N].
$$

##### Diamond property of a reduction relation

↑ **Parent:** [Beta reduction](#beta-reduction)

A reduction relation $\to$ has the diamond property if $a\to b$ and $a\to c$ imply a common one-step successor $b\to d\leftarrow c$. For relations allowing an identity step, the same definition includes zero-length joins. A finite grid of these diamonds proves confluence of $\to^*$. Ordinary one-step [beta reduction](#beta-reduction) fails this property because contracting before duplication can save two separate contractions.

###### Church-Rosser property of a reduction relation

↑ **Parent:** [Diamond property of a reduction relation](#diamond-property-of-a-reduction-relation)

A reduction relation has the Church-Rosser property when its [equivalence relation](set-theory.md#equivalence-relation) generated by forward and backward steps satisfies $b\leftrightarrow^*c\Rightarrow\exists d\;(b\to^*d\leftarrow^*c)$. It is equivalent to confluence of $\to^*$. The [Church-Rosser theorem](#church-rosser-theorem) establishes it for [beta reduction](#beta-reduction).

##### Parallel beta reduction

↑ **Parent:** [Beta reduction](#beta-reduction)

Parallel [beta reduction](#beta-reduction) permits simultaneous reduction in the body of a [lambda abstraction](#lambda-abstraction) and both sides of an application, together with $(\lambda x.M)N\Rightarrow M'[x:=N']$ when $M\Rightarrow M'$ and $N\Rightarrow N'$. Variables reduce to themselves. Its [capture-avoiding substitution](#capture-avoiding-substitution) lemma is $M\Rightarrow M',\ N\Rightarrow N'\Rightarrow M[x:=N]\Rightarrow M'[x:=N']$. Its transitive closure equals ordinary finite beta reduction, while its one-step diamond property yields the [Church-Rosser theorem](#church-rosser-theorem).

###### Complete development of a lambda term

↑ **Parent:** [Parallel beta reduction](#parallel-beta-reduction)

Define $x^\bullet=x$, $(\lambda x.M)^\bullet=\lambda x.M^\bullet$, and develop an application by contracting its root when that root is syntactically a [beta-redex](#beta-redex): $((\lambda x.M)N)^\bullet=M^\bullet[x:=N^\bullet]$. Otherwise $(MN)^\bullet=M^\bullet N^\bullet$. Newly created root redexes need not be contracted. Induction with the substitution lemma proves that if $M\Rightarrow N$, then $N\Rightarrow M^\bullet$. Thus any two parallel reducts share this reduct.

##### Normal-order beta reduction

↑ **Parent:** [Beta reduction](#beta-reduction)

Normal-order beta reduction contracts the leftmost outermost [beta-redex](#beta-redex). If a [lambda term](#lambda-term) has a [beta-normal form](#beta-normal-form), this strategy reaches it. It is useful for implementing [Church Boolean](#church-boolean) conditionals because an unused branch can be discarded before it is evaluated.

###### Standardization theorem for beta reduction

↑ **Parent:** [Normal-order beta reduction](#normal-order-beta-reduction)

A finite [beta reduction](#beta-reduction) can be rearranged into standard order, contracting earlier residual redexes before later ones. In particular, a [lambda term](#lambda-term) with a [head normal form](#head-normal-form) reaches one by head reduction, and a term with a [beta-normal form](#beta-normal-form) reaches it by [normal-order beta reduction](#normal-order-beta-reduction). Head reduction contracts the outermost redex on the left application spine, including under initial [lambda abstractions](#lambda-abstraction).

###### Normal-order normalization theorem

↑ **Parent:** [Normal-order beta reduction](#normal-order-beta-reduction)

If an untyped [lambda term](#lambda-term) has a [beta-normal form](#beta-normal-form), leftmost outermost [beta reduction](#beta-reduction) reaches a normal form. Thus an infinite normal-order computation certifies the absence of a [beta-normal form](#beta-normal-form). This is the normalization result needed to make a lambda simulation respect undefined outputs.

##### Capture-avoiding substitution

↑ **Parent:** [Beta reduction](#beta-reduction)

Capture-avoiding substitution $M[x:=N]$ replaces the free occurrences of $x$ in $M$ by $N$, renaming bound variables when necessary so that free variables of $N$ do not become bound.

##### Beta equivalence

↑ **Parent:** [Beta reduction](#beta-reduction)

Beta equivalence is the smallest equivalence relation containing [beta reduction](#beta-reduction); equivalently, $M\equiv_\beta N$ when a finite sequence of beta reductions and reversed beta reductions connects $M$ and $N$.

###### Undecidability of beta equivalence

↑ **Parent:** [Beta equivalence](#beta-equivalence)

[Beta equivalence](#beta-equivalence) is [semidecidable](#recursively-enumerable-set): enumerate finite conversion proofs. It is not decidable. A proposed total numeral-valued classifier of two nonempty disjoint [beta equivalence](#beta-equivalence) classes can be reversed by a [Church Boolean](#church-boolean) selector; a [self-quoting fixed point](mathematical-logic.md#self-quoting-fixed-point) of this reversal then belongs to the opposite class from the classifier output.

##### Beta-redex

↑ **Parent:** [Beta reduction](#beta-reduction)

A beta-redex is a subterm of the form $(\lambda x.M)N$, to which [beta reduction](#beta-reduction) can be applied.

##### Beta-normal form

↑ **Parent:** [Beta reduction](#beta-reduction)

A lambda term is in beta-normal form when it contains no [beta-redex](#beta-redex).

#### Combinator

↑ **Parent:** [Untyped lambda calculus](#untyped-lambda-calculus)

A combinator is a lambda term with no [free variables](mathematical-logic.md#free-variable).

##### Omega combinator

↑ **Parent:** [Combinator](#combinator)

The omega combinator is the divergent [untyped lambda calculus](#untyped-lambda-calculus) term

$$
\Omega=(\lambda x.xx)(\lambda x.xx),
$$

whose only [beta reduction](#beta-reduction) reproduces $\Omega$.

##### Fixed-point combinator

↑ **Parent:** [Combinator](#combinator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fixed-point_combinator)

An untyped lambda term $Y$ is a fixed-point combinator when $Yf\equiv_\beta f(Yf)$ for every term $f$.

###### Turing fixed-point combinator

↑ **Parent:** [Fixed-point combinator](#fixed-point-combinator)

Put $D=\lambda x f.f(xxf)$ and $\Theta=DD$. Then $\Theta f\to_\beta^*f(\Theta f)$. Unlike the [Curry fixed-point combinator](#curry-fixed-point-combinator), every finite reduct retains a closed subterm $DD$. Contracting this subterm recreates one; every other generated redex substitutes a variable and preserves it. The [Church-Rosser theorem](#church-rosser-theorem) therefore proves $Y\not\equiv_\beta\Theta$.

###### Curry fixed-point combinator

↑ **Parent:** [Fixed-point combinator](#fixed-point-combinator)

With $A_f=\lambda x.f(xx)$, the [combinator](#combinator) $Y=\lambda f.A_fA_f$ satisfies $Yf\equiv_\beta f(Yf)$. Every finite reduct of $Y$ is, up to [alpha equivalence](#alpha-equivalence), $\lambda f.f^n(A_fA_f)$: the remaining copy of $A_fA_f$ is its only [beta-redex](#beta-redex).

###### Fixed-point theorem for the untyped lambda calculus

↑ **Parent:** [Fixed-point combinator](#fixed-point-combinator)

Every lambda term $F$ has a fixed point: the term

$$
X=(\lambda x.F(xx))(\lambda x.F(xx))
$$

satisfies $X\equiv_\beta F(X)$. Equivalently, a [fixed-point combinator](#fixed-point-combinator) such as

$$
Y=\lambda f.(\lambda x.f(xx))(\lambda x.f(xx))
$$

satisfies $YF\equiv_\beta F(YF)$ for every $F$.

###### Recursively enumerable fixed-point combinators

↑ **Parent:** [Fixed-point combinator](#fixed-point-combinator)

The set of [fixed-point combinators](#fixed-point-combinator) is [recursively enumerable](#recursively-enumerable-set). Enumerate closed lambda terms and finite proofs of [beta equivalence](#beta-equivalence), and output $Y$ whenever a proof of $Yf\equiv_\beta f(Yf)$ appears for a fresh variable $f$.

### Alpha equivalence

↑ **Parent:** [Lambda calculus](#lambda-calculus)

Two lambda terms are alpha-equivalent when they differ only by consistent renaming of bound variables.

### Church-Rosser theorem

↑ **Parent:** [Lambda calculus](#lambda-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Church-Rosser_theorem)

If a lambda term beta-reduces to both $M$ and $N$, then $M$ and $N$ beta-reduce to a common term. Consequently two [beta-equivalent](#beta-equivalence) beta-normal forms are [alpha-equivalent](#alpha-equivalence).

### Simply typed lambda calculus

↑ **Parent:** [Lambda calculus](#lambda-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simply_typed_lambda_calculus)

The simply typed lambda calculus assigns arrow types to variables, abstractions, and applications according to syntax-directed typing rules.

#### Typed lambda term

↑ **Parent:** [Simply typed lambda calculus](#simply-typed-lambda-calculus)

A [typed lambda term](#typed-lambda-term) carries a type derivation under a context of typed free variables. The rules for variables, abstraction, and application correspond to assumptions, the [implication introduction rule](mathematical-logic.md#implication-introduction-rule), and the [implication elimination rule](mathematical-logic.md#implication-elimination-rule) under the [Implicational Curry-Howard correspondence](mathematical-logic.md#implicational-curry-howard-correspondence). General [fixed-point combinators](#fixed-point-combinator) belong to the [untyped lambda calculus](#untyped-lambda-calculus); self-application cannot be given a finite simple type.

#### Weak normalization theorem for simply typed lambda calculus

↑ **Parent:** [Simply typed lambda calculus](#simply-typed-lambda-calculus)

Every well-typed term in the simply typed lambda calculus has some finite beta-reduction sequence ending in a beta-normal form.

### Church encoding

↑ **Parent:** [Lambda calculus](#lambda-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Church_encoding)

[Church encoding](#church-encoding) represents data and operations as terms of the [lambda calculus](#lambda-calculus). A [Church numeral](#church-numeral) represents a natural number by repeated function application; a [Church Boolean](#church-boolean) selects one of two arguments.

#### Church numeral

↑ **Parent:** [Church encoding](#church-encoding)

The Church numeral $c_n=\lambda f.\lambda x.f^n x$ encodes the natural number $n$ by iteration.

##### Church numeral arithmetic

↑ **Parent:** [Church numeral](#church-numeral)

[Church numeral](#church-numeral) successor, addition, multiplication, and exponentiation are represented by $\lambda nfx.f(nfx)$, $\lambda mnfx.mf(nfx)$, $\lambda mnfx.m(nf)x$, and $\lambda mnfx.(nm)fx$. The last term takes the base first and the exponent second. Its outer abstractions preserve the usual numeral normal form at exponent zero, implementing $m^0=1$, including $0^0=1$. At base type $A$, exponentiation uses an exponent at Church type $C_{A\to A}$ and a base at $C_A=(A\to A)\to A\to A$.

##### Church numeral zero test

↑ **Parent:** [Church numeral](#church-numeral)

The [lambda term](#lambda-term)

$$
\mathsf{Zero}=\lambda n.n(\lambda z.\mathsf F)\mathsf T
$$

returns the [Church Boolean](#church-boolean) $\mathsf T$ on $c_0$ and $\mathsf F$ on every positive [Church numeral](#church-numeral). Zero iterations leave the initial true value, while at least one iteration replaces it by false. [Normal-order beta reduction](#normal-order-beta-reduction) evaluates a numeral conditional without evaluating an unchosen branch.

##### Church pair

↑ **Parent:** [Church numeral](#church-numeral)

With the [Church Booleans](#church-boolean) $\mathsf T=\lambda a b.a$ and $\mathsf F=\lambda a b.b$, encode a pair by

$$
\mathsf{Pair}=\lambda a b p.pab,\qquad \mathsf{Fst}=\lambda p.p\mathsf T,\qquad \mathsf{Snd}=\lambda p.p\mathsf F.
$$

Then $\mathsf{Fst}(\mathsf{Pair}\,A\,B)\to_\beta^*A$ and the second projection similarly returns $B$. Pairing an iteration counter with a computed value implements [primitive recursion](#primitive-recursion) using only [Church numeral](#church-numeral) iteration.

##### Lambda-definable function

↑ **Parent:** [Church numeral](#church-numeral)

A function $g:\mathbb N^k\to\mathbb N$ is lambda-definable when some [combinator](#combinator) $G$ satisfies

$$
G c_{n_1}\cdots c_{n_k}\equiv_\beta c_{g(n_1,\ldots,n_k)}
$$

for every tuple of natural numbers.

###### Lambda definition of the successor function

↑ **Parent:** [Lambda-definable function](#lambda-definable-function)

The [successor function](#successor-function) is lambda-defined on [Church numerals](#church-numeral) by

$$
\operatorname{Succ}=\lambda n.\lambda f.\lambda x.f(nfx),
$$

because $\operatorname{Succ}\,c_n\equiv_\beta c_{n+1}$.

###### Lambda definition of primitive recursion

↑ **Parent:** [Lambda-definable function](#lambda-definable-function)

Using a [fixed-point combinator](#fixed-point-combinator), Church Boolean conditionals, a zero test, and a predecessor term, lambda-definable $g$ and $h$ give

$$
R\mathbf x0=g(\mathbf x),
\qquad
R\mathbf x(n+1)=h(\mathbf x,n,R\mathbf x n).
$$

Normal-order beta reduction evaluates only the selected conditional branch, so this term implements primitive recursion on [Church numerals](#church-numeral).

###### Lambda definition of primitive recursion by pair iteration

↑ **Parent:** [Lambda definition of primitive recursion](#lambda-definition-of-primitive-recursion)

If total [functions](function.md) $g$ and $h$ are represented by [lambda terms](#lambda-term) $G,H$, define

$$
\mathsf{Step}_{\mathbf x}=\lambda p.\mathsf{Pair}(\mathsf{Succ}(\mathsf{Fst}\,p))(H\mathbf x(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)),
$$

and

$$
R=\lambda\mathbf x n.\mathsf{Snd}\bigl(n\mathsf{Step}_{\mathbf x}(\mathsf{Pair}\,c_0\,(G\mathbf x))\bigr).
$$

After $j$ iterations the [Church pair](#church-pair) holds $(c_j,c_{f(\mathbf x,j)})$, proved by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) using the defining recursion equations. Consequently $R$ represents the total [primitive recursive function](#primitive-recursive-function) $f$. This statement concerns total inputs and total recursion constituents; it is not an unguarded composition theorem for arbitrary partial [functions](function.md).

###### Lambda-definable partial function

↑ **Parent:** [Lambda-definable function](#lambda-definable-function)

A partial function is lambda-definable when one lambda term maps Church numerals in its domain to the numeral of the output and produces no numeral on inputs outside its domain.

###### Lambda representation of partial computable functions

↑ **Parent:** [Lambda-definable partial function](#lambda-definable-partial-function)

Every [partial computable function](#computable-function) is represented on [Church numerals](#church-numeral) by a closed [untyped lambda calculus](#untyped-lambda-calculus) term. First represent all [primitive recursive functions](#primitive-recursive-function) using zero, successor, projections, composition and [lambda definition of primitive recursion by pair iteration](#lambda-definition-of-primitive-recursion-by-pair-iteration). Apply the [Kleene normal form theorem](#kleene-normal-form-theorem) and search successive history codes with a [fixed-point combinator](#fixed-point-combinator). Test the represented total predicate using a [Church numeral zero test](#church-numeral-zero-test); return the decoded output only on the true branch. If no history passes, normal-order head reduction continues the search indefinitely and the term has no [head normal form](#head-normal-form), so cannot be in [beta equivalence](#beta-equivalence) with a [Church numeral](#church-numeral). This avoids the incorrect assumption that a lazy outer [function](function.md) must evaluate a divergent argument in an unguarded composition.

###### Lambda simulation of a Turing machine

↑ **Parent:** [Lambda representation of partial computable functions](#lambda-representation-of-partial-computable-functions)

Represent total machine configuration transitions and tests on [Church numerals](#church-numeral) and [Church pairs](#church-pair), then use a [fixed-point combinator](#fixed-point-combinator) to iterate until the halting test selects the output. Normal-order [beta reduction](#beta-reduction) follows the computation. A nonhalting machine gives an infinite required reduction, so the [normal-order normalization theorem](#normal-order-normalization-theorem) rules out a numeral normal form.

###### Strict sequencing of partial numeral computations

↑ **Parent:** [Lambda-definable partial function](#lambda-definable-partial-function)

The term $\mathrm{Force}\,c_m\,K$ beta-reduces to $K$ for every [Church numeral](#church-numeral) $c_m$. If its first argument has no [head normal form](#head-normal-form), the whole application has no head normal form. Nesting this operation forces each represented inner computation before applying an outer function, implementing [composition of partial functions](function.md#composition-of-partial-functions) even when an outer projection would discard an argument. The same guard makes [lambda definition of primitive recursion](#lambda-definition-of-primitive-recursion) strict in the preceding recursive value.

###### Lambda definition of unbounded minimization

↑ **Parent:** [Lambda-definable partial function](#lambda-definable-partial-function)

For a lambda-definable partial $g(\mathbf x,n)$, a fixed-point search term tests $n=0,1,2,\ldots$ and returns the first $n$ for which $g(\mathbf x,n)=0$. If no such value is reached, reduction produces no Church numeral. This realizes [unbounded minimization](#mu-operator) and therefore makes every partial recursive function lambda-definable.

#### Church Boolean

↑ **Parent:** [Church encoding](#church-encoding)

At type $\sigma\to\sigma\to\sigma$, the Church Booleans are $\top=\lambda x.\lambda y.x$ and $\bot=\lambda x.\lambda y.y$.

### Normal form (abstract rewriting)

↑ **Parent:** [Lambda calculus](#lambda-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_form_(abstract_rewriting))

An expression in [normal form](#normal-form-abstract-rewriting) admits no further reductions. A term is strongly normalizing when every reduction sequence from it terminates; weak normalization requires only one terminating sequence. [Strong normalization theorem for simply typed lambda calculus](#strong-normalization-theorem-for-simply-typed-lambda-calculus) establishes the stronger property for well-typed terms.

#### Strong normalization theorem for simply typed lambda calculus

↑ **Parent:** [Normal form (abstract rewriting)](#normal-form-abstract-rewriting)

This theorem establishes strong normalization in the [normal form](#normal-form-abstract-rewriting) sense. Every well-typed simply typed lambda term admits no infinite beta-reduction sequence.

## ↑ Ancestors (4)

1. [Foundations of mathematics](foundations-of-mathematics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Computable colouring](ramsey-theory.md#computable-colouring)
- [Computer science](computer-science.md)
- [Mathematical logic](mathematical-logic.md)
- [Oscar Levin](mathematics.md#oscar-levin)
- [Pairing function](#pairing-function)
