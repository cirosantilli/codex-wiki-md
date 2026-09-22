# Theoretical computer science

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theoretical_computer_science)

**Table of contents**

- [Formal language](#formal-language)
  - [L-system](#l-system)
  - [Binary string](#binary-string)
    - [Counting binary strings with bounded ones](#counting-binary-strings-with-bounded-ones)
    - [Self-delimiting binary code](#self-delimiting-binary-code)
  - [Concatenation of formal languages](#concatenation-of-formal-languages)
  - [Empty language](#empty-language)
- [Turing machine](#turing-machine)
  - [Instantaneous description of a Turing machine](#instantaneous-description-of-a-turing-machine)
  - [Instruction of a Turing machine](#instruction-of-a-turing-machine)
  - [Two-stack encoding of a Turing tape](#two-stack-encoding-of-a-turing-tape)
  - [Modular machine](#modular-machine)
    - [Group encoding of a modular machine](#group-encoding-of-a-modular-machine)
    - [Halting set at a designated terminal configuration](#halting-set-at-a-designated-terminal-configuration)
  - [Deterministic computation](#deterministic-computation)
  - [Reversible computation](#reversible-computation)
    - [Reversible circuit](#reversible-circuit)
  - [Nondeterministic Turing machine](#nondeterministic-turing-machine)
  - [Oracle machine](#oracle-machine)
    - [Relativization (complexity theory)](#relativization-complexity-theory)
- [Boolean operation](#boolean-operation)
  - [Boolean operations on events](#boolean-operations-on-events)
  - [Exclusive or](#exclusive-or)
    - [Exclusive or toggles and parity](#exclusive-or-toggles-and-parity)
  - [Negation](#negation)
  - [De Morgan's laws](#de-morgan-s-laws)
    - [De Morgan dual of a Boolean function](#de-morgan-dual-of-a-boolean-function)
- [Computational complexity theory](#computational-complexity-theory)
  - [Communication complexity](#communication-complexity)
  - [Promise problem](#promise-problem)
  - [Quantum complexity theory](#quantum-complexity-theory)
    - [BQP](#bqp)
      - [BQP error reduction](#bqp-error-reduction)
    - [Quantum witness](#quantum-witness)
    - [StoqMA](#stoqma)
    - [QMA](#qma)
      - [Witness acceptance operator](#witness-acceptance-operator)
        - [Trace-power witness optimization](#trace-power-witness-optimization)
      - [QMA error reduction](#qma-error-reduction)
      - [QMA parallel repetition with entangled witnesses](#qma-parallel-repetition-with-entangled-witnesses)
      - [Quantum verifier acceptance operator](#quantum-verifier-acceptance-operator)
    - [Quantum query complexity](#quantum-query-complexity)
      - [Polynomial method for quantum query lower bounds](#polynomial-method-for-quantum-query-lower-bounds)
      - [Exact quantum query complexity](#exact-quantum-query-complexity)
        - [Exact two-query majority algorithm](#exact-two-query-majority-algorithm)
      - [Quantum collision finding](#quantum-collision-finding)
        - [Brassard–Høyer–Tapp collision algorithm](#brassard-hoyer-tapp-collision-algorithm)
  - [Decision tree model](#decision-tree-model)
    - [Decision tree](#decision-tree)
      - [Binary decision tree](#binary-decision-tree)
      - [Three-bit majority decision tree](#three-bit-majority-decision-tree)
      - [Parity lower bound for Boolean queries](#parity-lower-bound-for-boolean-queries)
      - [Decision-tree query cost](#decision-tree-query-cost)
        - [Expected query cost](#expected-query-cost)
        - [Coordinate revealment](#coordinate-revealment)
      - [Decision-tree depth](#decision-tree-depth)
        - [Certificate complexity of a Boolean function](#certificate-complexity-of-a-boolean-function)
          - [Query certificate](#query-certificate)
        - [Evasive Boolean function](#evasive-boolean-function)
          - [Alternating-sum criterion for decision-tree evasiveness](#alternating-sum-criterion-for-decision-tree-evasiveness)
        - [Decision-tree adversary for a threshold function](#decision-tree-adversary-for-a-threshold-function)
  - [Computational problem](#computational-problem)
    - [Input (computer science)](#input-computer-science)
    - [Output (computing)](#output-computing)
    - [Decision problem](#decision-problem)
    - [Search problem](#search-problem)
      - [Search tree](#search-tree)
        - [Branching factor](#branching-factor)
      - [Constraint satisfaction problem](#constraint-satisfaction-problem)
        - [Sudoku](#sudoku)
        - [Kakuro](#kakuro)
        - [Forward checking](#forward-checking)
        - [Minimum remaining values](#minimum-remaining-values)
        - [Constraint propagation](#constraint-propagation)
        - [All-different constraint](#all-different-constraint)
        - [Minimum remaining values heuristic](#minimum-remaining-values-heuristic)
      - [Search-to-decision reduction](#search-to-decision-reduction)
  - [Complexity class](#complexity-class)
    - [Time complexity](#time-complexity)
      - [Quadratic time](#quadratic-time)
      - [Linear time](#linear-time)
      - [Constant time](#constant-time)
      - [Pseudo-polynomial time](#pseudo-polynomial-time)
      - [Amortized analysis](#amortized-analysis)
        - [Dynamic array doubling](#dynamic-array-doubling)
        - [Potential method](#potential-method)
          - [Amortized cost](#amortized-cost)
        - [Aggregate analysis](#aggregate-analysis)
        - [Accounting method](#accounting-method)
      - [Polynomial time](#polynomial-time)
        - [Polynomial-time algorithm](#polynomial-time-algorithm)
        - [P (complexity)](#p-complexity)
          - [P-completeness](#p-completeness)
        - [NP (complexity)](#np-complexity)
          - [Certificate (complexity)](#certificate-complexity)
    - [Space complexity](#space-complexity)
      - [Constant space](#constant-space)
      - [Polynomial space](#polynomial-space)
      - [Nondeterministic space complexity class](#nondeterministic-space-complexity-class)
        - [Savitch's theorem](#savitch-s-theorem)
          - [Space-bound discovery by exit reachability](#space-bound-discovery-by-exit-reachability)
      - [Deterministic space complexity class](#deterministic-space-complexity-class)
        - [PSPACE](#pspace)
      - [Polynomial-register real-arithmetic computation](#polynomial-register-real-arithmetic-computation)
      - [Logarithmic space](#logarithmic-space)
        - [L (complexity)](#l-complexity)
        - [NL (complexity)](#nl-complexity)
          - [NL-complete](#nl-complete)
            - [Directed cycle detection](#directed-cycle-detection)
            - [ST-connectivity](#st-connectivity)
              - [Configuration graph](#configuration-graph)
          - [co-NL](#co-nl)
            - [Immerman–Szelepcsényi theorem](#immerman-szelepcsenyi-theorem)
              - [Inductive counting](#inductive-counting)
  - [Polynomial-time reduction](#polynomial-time-reduction)
    - [Polynomial-time many-one reduction](#polynomial-time-many-one-reduction)
      - [Logspace many-one reduction](#logspace-many-one-reduction)
      - [NP-hardness](#np-hardness)
        - [NP-completeness](#np-completeness)
          - [Set cover problem](#set-cover-problem)
            - [Set cover reduction to equilibrium support](#set-cover-reduction-to-equilibrium-support)
          - [Cook-Levin theorem](#cook-levin-theorem)
          - [Subset sum problem](#subset-sum-problem)
            - [Special sum set](#special-sum-set)
          - [Boolean satisfiability problem](#boolean-satisfiability-problem)
            - [Satisfying assignment](#satisfying-assignment)
              - [Verifying a satisfying assignment](#verifying-a-satisfying-assignment)
            - [Unsatisfiable Boolean formula](#unsatisfiable-boolean-formula)
            - [Partial Boolean assignment](#partial-boolean-assignment)
            - [2-satisfiability](#2-satisfiability)
            - [Integer programming formulation of satisfiability](#integer-programming-formulation-of-satisfiability)
            - [Maximum satisfiability](#maximum-satisfiability)
              - [Literal-frequency greedy approximation for MAX-SAT](#literal-frequency-greedy-approximation-for-max-sat)
            - [2UN-SAT](#2un-sat)
            - [Maximum 2-satisfiability](#maximum-2-satisfiability)
              - [Golden ratio approximation for MAX-2SAT](#golden-ratio-approximation-for-max-2sat)
              - [Seven-clause gadget for MAX-2SAT](#seven-clause-gadget-for-max-2sat)
            - [Boolean formula](#boolean-formula)
              - [Disjunctive normal form](#disjunctive-normal-form)
              - [Conjunctive normal form](#conjunctive-normal-form)
                - [Tseytin transformation](#tseytin-transformation)
              - [Clause of a Boolean formula](#clause-of-a-boolean-formula)
              - [Boolean literal](#boolean-literal)
              - [Boolean variable](#boolean-variable)
            - [3-SAT](#3-sat)
            - [Horn clause](#horn-clause)
              - [Horn-SAT](#horn-sat)
                - [Horn-SAT forward-chaining algorithm](#horn-sat-forward-chaining-algorithm)
          - [Quadratic-equation satisfiability over F2](#quadratic-equation-satisfiability-over-f2)
          - [Ladner's theorem](#ladner-s-theorem)
  - [Circuit complexity](#circuit-complexity)
    - [NC1](#nc1)
      - [MOD3 binary divisibility problem](#mod3-binary-divisibility-problem)
      - [Balanced finite-monoid reduction circuit](#balanced-finite-monoid-reduction-circuit)
    - [Boolean circuit](#boolean-circuit)
      - [Circuit size](#circuit-size)
      - [Depth of a Boolean circuit](#depth-of-a-boolean-circuit)
      - [Circuit value problem](#circuit-value-problem)
        - [AND-NOT circuit value problem](#and-not-circuit-value-problem)
      - [Circuit satisfiability problem](#circuit-satisfiability-problem)
      - [Threshold function](#threshold-function)
        - [Majority function](#majority-function)
          - [Block conjunction of three-bit majorities](#block-conjunction-of-three-bit-majorities)
      - [Dual Boolean function](#dual-boolean-function)
    - [Circuit family](#circuit-family)
      - [Circuit size class](#circuit-size-class)
        - [Truth-table upper bound for circuit size](#truth-table-upper-bound-for-circuit-size)
      - [Polynomial-size circuit family](#polynomial-size-circuit-family)
        - [Undecidable unary languages with linear-size circuits](#undecidable-unary-languages-with-linear-size-circuits)
        - [P/poly](#p-poly)
    - [Constant-depth circuit complexity](#constant-depth-circuit-complexity)
      - [Håstad switching lemma](#hastad-switching-lemma)
        - [Switching-lemma depth reduction](#switching-lemma-depth-reduction)
    - [Monotone circuit complexity](#monotone-circuit-complexity)
      - [Monotone circuit](#monotone-circuit)
      - [Superpolynomial monotone clique lower bound](#superpolynomial-monotone-clique-lower-bound)
      - [Razborov approximation method](#razborov-approximation-method)
        - [Finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits)
          - [Negative colouring error of a forced-set closure](#negative-colouring-error-of-a-forced-set-closure)
          - [Positive clique error of a truncated lattice meet](#positive-clique-error-of-a-truncated-lattice-meet)
        - [Razborov closure](#razborov-closure)
          - [Sunflower bound for minimal members of a Razborov-closed family](#sunflower-bound-for-minimal-members-of-a-razborov-closed-family)
          - [Minimal-member bound for a Razborov-closed family](#minimal-member-bound-for-a-razborov-closed-family)
        - [Razborov gate-by-gate approximation lemma](#razborov-gate-by-gate-approximation-lemma)
    - [Natural proof](#natural-proof)
      - [Constructive property of Boolean functions](#constructive-property-of-boolean-functions)
      - [Large property of Boolean functions](#large-property-of-boolean-functions)
      - [Useful property against a circuit class](#useful-property-against-a-circuit-class)
      - [Razborov–Rudich natural-proofs barrier](#razborov-rudich-natural-proofs-barrier)
    - [Pseudorandom function family](#pseudorandom-function-family)
    - [Arithmetic circuit](#arithmetic-circuit)
  - [Counting complexity](#counting-complexity)
    - [Valiant's permanent reduction](#valiant-s-permanent-reduction)
      - [Variable gadget in Valiant's permanent reduction](#variable-gadget-in-valiant-s-permanent-reduction)
      - [Clause gadget in Valiant's permanent reduction](#clause-gadget-in-valiant-s-permanent-reduction)
      - [Exclusive-or gadget in Valiant's permanent reduction](#exclusive-or-gadget-in-valiant-s-permanent-reduction)
      - [Binary path-counting gadget](#binary-path-counting-gadget)
    - [Balanced number 3-SAT](#balanced-number-3-sat)
  - [Polynomial hierarchy](#polynomial-hierarchy)
    - [Second level of the polynomial hierarchy](#second-level-of-the-polynomial-hierarchy)
    - [Karp–Lipton theorem](#karp-lipton-theorem)
  - [Primality testing](#primality-testing)
    - [Prime-proof number](#prime-proof-number)
    - [Miller-Rabin primality test](#miller-rabin-primality-test)
      - [Deterministic Miller-Rabin primality test](#deterministic-miller-rabin-primality-test)
    - [Fermat primality test](#fermat-primality-test)
    - [Pseudoprime base](#pseudoprime-base)
    - [Agrawal–Biswas primality test](#agrawal-biswas-primality-test)
- [Abstract machine](#abstract-machine)
  - [Stack machine](#stack-machine)

## Formal language

↑ **Parent:** [Theoretical computer science](theoretical-computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Formal_language)

A formal language is a set of finite strings over a fixed finite alphabet.

### L-system

↑ **Parent:** [Formal language](#formal-language)

A parallel string-rewriting system: at each generation, every symbol is replaced simultaneously by its assigned word. Symbols can also encode drawing commands such as moving forward or turning. Large recursively defined drawings can be queried without expanding the whole word by precomputing the length, displacement, and rotation of each expanded block.

### Binary string

↑ **Parent:** [Formal language](#formal-language)

A [binary string](#binary-string) is a finite word over the alphabet $\{0,1\}$. There are $2^n$ strings of length $n$. Finite [binary strings](#binary-string) have an effective [bijection](function.md#bijection) with [natural numbers](arithmetic.md#natural-number), so computable enumerability and immunity apply to sets of strings.

#### Counting binary strings with bounded ones

↑ **Parent:** [Binary string](#binary-string)

A [binary string](#binary-string) with $n$ zeroes and $j$ ones is determined by its $j$ one-positions, giving $\binom{n+j}j$ possibilities. Sum for $0\le j\le m$ and apply the [hockey-stick identity](binomial-coefficient.md#hockey-stick-identity). Equivalently, distribute at most $m$ ones among the $n+1$ gaps around the zeroes and add a slack count; [stars and bars](combinatorics.md#stars-and-bars-combinatorics) counts $n+2$ nonnegative counts summing to $m$.

#### Self-delimiting binary code

↑ **Parent:** [Binary string](#binary-string)

A self-delimiting code permits a decoder to identify the end of a code without an external length marker. Encoding a binary word of length $\ell$ by $\ell$ ones, a zero and the word uses $2\ell+1$ bits. This yields an $O(\log n)$ description of a [natural number](arithmetic.md#natural-number) in an incompressibility proof.

### Concatenation of formal languages

↑ **Parent:** [Formal language](#formal-language)

For [formal languages](#formal-language) $L,M$ over the same [alphabet](information-theory.md#alphabet), concatenate each [word over an alphabet](foundations-of-mathematics.md#string) in $L$ with each [word over an alphabet](foundations-of-mathematics.md#string) in $M$. This operation is associative, has identity $\{\varepsilon\}$ and absorbing element the [empty language](#empty-language).

### Empty language

↑ **Parent:** [Formal language](#formal-language)

The [formal language](#formal-language) containing no [words over an alphabet](foundations-of-mathematics.md#string). It differs from the language containing only the [empty word](foundations-of-mathematics.md#empty-word), which is a multiplicative identity for [concatenation of formal languages](#concatenation-of-formal-languages).

## Turing machine

↑ **Parent:** [Theoretical computer science](theoretical-computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turing_machine)

A Turing machine is an abstract computational model with a finite control, an unbounded tape and a head that reads, writes and moves on the tape.

### Instantaneous description of a Turing machine

↑ **Parent:** [Turing machine](#turing-machine)

An instantaneous description records the current control state, head position, and tape contents. For a tape blank outside a finite window, a word $h\,u\,q\,v\,h$ records the symbols $u$ to the left of the head and $v$ from the scanned cell rightward, with unrecorded cells blank. If $v$ is empty, the head scans an implicit blank. Extra outer blanks can represent the same infinite tape. The [instruction of a Turing machine](#instruction-of-a-turing-machine) determines its successor description.

### Instruction of a Turing machine

↑ **Parent:** [Turing machine](#turing-machine)

For a deterministic single-tape [Turing machine](#turing-machine), an instruction reads a state $q$ and scanned tape symbol $a$, writes $b$, changes state to $p$, and moves the head one cell left, one cell right, or not at all according to $D$. The state and tape alphabets are finite; an undefined transition halts. A dedicated terminal state can be introduced by directing undefined transitions to it without changing whether computation halts.

### Two-stack encoding of a Turing tape

↑ **Parent:** [Turing machine](#turing-machine)

Encode the cells immediately left of the head in a reversed positional stack $L$, and the current and right cells in $R$. Quotient and remainder by the alphabet base read and remove cells; multiplication by that base pushes a cell. The resulting local tape transitions are [primitive recursive](computability-theory.md#primitive-recursive-function), which makes them directly implementable on [Church numerals](computability-theory.md#church-numeral).

### Modular machine

↑ **Parent:** [Turing machine](#turing-machine)

A modular machine of modulus $m>1$ acts on pairs in $\mathbb N^2$. Each instruction $(a,b,c,R)$ or $(a,b,c,L)$ has $0\le a,b<m$ and $0\le c<m^2$, and at most one instruction is assigned to each residue pair $(a,b)$. The two transition types are $(mu+a,mv+b)\mapsto(m^2u+c,v)$ and $(mu+a,mv+b)\mapsto(u,m^2v+c)$. These finite arithmetic operations can encode a [Turing machine](#turing-machine); a designated terminal configuration can have a nonrecursive [halting set](foundations-of-mathematics.md#halting-set).

#### Group encoding of a modular machine

↑ **Parent:** [Modular machine](#modular-machine)

A [modular machine](#modular-machine) can be encoded by [HNN extensions](geometric-group-theory.md#hnn-extension) of $K=\mathbb Z^2*\langle t\rangle$. The kernel of $K\to\mathbb Z^2$ has a [free basis of a group](geometric-group-theory.md#free-basis-of-a-group) $t(r,s)=x^{-r}y^{-s}tx^ry^s$. Associated-subgroup maps send these basis elements according to the two arithmetic transition types. In the resulting group, membership of $t(r,s)$ in the subgroup generated by $t$ and the instruction stable letters is equivalent to $(r,s)\in H_0(\mathcal M)$. One more [HNN extension](geometric-group-theory.md#hnn-extension) centralizes that finitely generated subgroup, converting membership to equality and hence to the [word problem for a group](geometric-group-theory.md#word-problem-for-groups).

#### Halting set at a designated terminal configuration

↑ **Parent:** [Modular machine](#modular-machine)

For a [modular machine](#modular-machine) whose $(0,0)$ is terminal, $H_0(\mathcal M)$ is the set of configurations whose forward computation reaches exactly $(0,0)$, including the zero-step computation there. It may differ from the set of configurations stopping at any terminal configuration. Determinism makes membership invariant along each instruction edge.

### Deterministic computation

↑ **Parent:** [Turing machine](#turing-machine)

In a deterministic computation, every configuration and input symbol determine at most one next configuration.

### Reversible computation

↑ **Parent:** [Turing machine](#turing-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reversible_computation)

A reversible computation has an injective transition function, so its preceding configuration can be recovered from its current configuration. Any finite classical computation can be simulated reversibly while retaining enough workspace to [uncompute](quantum-theory.md#uncomputation) its temporary results.

#### Reversible circuit

↑ **Parent:** [Reversible computation](#reversible-computation)

A reversible circuit is composed of bijective gates. The [Toffoli gate](quantum-theory.md#toffoli-gate) is universal for reversible Boolean computation when ancillary bits are available.

### Nondeterministic Turing machine

↑ **Parent:** [Turing machine](#turing-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nondeterministic_Turing_machine)

A nondeterministic computation may have several possible next configurations and accepts when at least one computation path accepts.

### Oracle machine

↑ **Parent:** [Turing machine](#turing-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oracle_machine)

An oracle machine may query membership in a fixed language in one computation step.

#### Relativization (complexity theory)

↑ **Parent:** [Oracle machine](#oracle-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Relativization_(complexity_theory))

A relativized complexity class $\mathcal C^A$ allows every machine defining $\mathcal C$ to query the same oracle $A$.

## Boolean operation

↑ **Parent:** [Theoretical computer science](theoretical-computer-science.md)

A [Boolean operation](#boolean-operation) is a [Boolean function](analysis-of-boolean-functions.md#boolean-function) taking [truth values](mathematical-logic.md#truth-value) encoded as [bits](information-theory.md#bit): $0$ means false and $1$ means true. These operations supply the concrete two-valued interpretation of a [Boolean algebra](mathematical-logic.md#boolean-algebra). A [Boolean valuation](mathematical-logic.md#boolean-valuation) fixes the inputs; a [truth table](mathematical-logic.md#truth-table) lists every possible input. With two input [bits](information-theory.md#bit) there are four rows.

The basic [logical connectives](mathematical-logic.md#logical-connective) are [logical conjunction](mathematical-logic.md#logical-conjunction) (AND, $P\wedge Q$, both true), [logical disjunction](mathematical-logic.md#logical-disjunction) (OR, $P\vee Q$, at least one true), [exclusive or](#exclusive-or) (XOR, $P\oplus Q$, exactly one true), and [logical negation](#negation) (NOT, $\neg P$, the opposite value). OR is inclusive: it accepts the case where both inputs are true.[Discrete Mathematics: An Open Introduction (3rd edition) by Oscar Levin; Discrete Mathematics: An Open Introduction, 3rd edition by Oscar Levin, §3.1, Truth Tables: conjunction, disjunction and negation tables](mathematics-bibliography.md#discrete-mathematics-an-open-introduction-3rd-edition-by-oscar-levin/3-1-propositional-logic)

<a id="image-four-input-pairs-distinguish-logical-conjunction-inclusive-logical-disjunction-exclusive-or-and-logical-negation"></a>
![](boolean-operation-truth-grid.png)

**[Figure 1](#image-four-input-pairs-distinguish-logical-conjunction-inclusive-logical-disjunction-exclusive-or-and-logical-negation). Four input pairs distinguish logical conjunction, inclusive logical disjunction, exclusive or, and logical negation**.

For an original program-condition example, let $P$ mean “the backup is recent” and $Q$ mean “the backup is verified”. A rule requiring a recent, verified backup uses [logical conjunction](mathematical-logic.md#logical-conjunction); one accepting either qualification uses [logical disjunction](mathematical-logic.md#logical-disjunction). A rule flagging a mismatch between the two qualifications uses [exclusive or](#exclusive-or). A recent, verified backup gives $(P,Q)=(1,1)$: AND and OR accept it, while XOR does not flag it. The last row of the [truth table](mathematical-logic.md#truth-table) makes this difference explicit.

The same small [Boolean operations](#boolean-operation) build larger tests and [Boolean circuits](#boolean-circuit). In a [programming language](programming-language.md), the value of a condition and the procedure for evaluating it both matter. For Boolean operands, [Python](programming-language.md#python-programming-language)'s `and`, `or`, and `not` implement these [logical connectives](mathematical-logic.md#logical-connective). Evaluation proceeds from the left; `and` skips its right operand if the left is false, and `or` skips it if the left is true. More generally, `and` and `or` return an operand, whereas `not` returns a Boolean.[Python 3.14 documentation; Python Language Reference, version 3.14, §6.11 Boolean operations: evaluation order and returned operands](computer-science-bibliography.md#python-3-14-documentation/expressions-python-3-14-language-reference)

For example, the [Python](programming-language.md#python-programming-language) condition `denominator != 0 and numerator / denominator > 2` avoids [division](arithmetic.md#division-mathematics) by zero because the [logical conjunction](mathematical-logic.md#logical-conjunction)'s second test is evaluated only when the first succeeds. Reversing the tests preserves the abstract [truth table](mathematical-logic.md#truth-table) for defined operands but can raise a division-by-zero error handled through [exception handling](programming-language.md#exception-handling). A rewrite involving a [side effect](programming-language.md#side-effect-computer-science) must also preserve the needed evaluation behavior.

### Boolean operations on events

↑ **Parent:** [Boolean operation](#boolean-operation)

[Events](probability-space.md#event) turn [Boolean operations](#boolean-operation) into operations on [sets](set.md). For a die with [sample space](probability-space.md#sample-space) $U=\{1,2,3,4,5,6\}$, let $A=\{2,4,6\}$ be the [event](probability-space.md#event) “even outcome” and $B=\{4,5,6\}$ the [event](probability-space.md#event) “outcome at least four”. At outcome $u$, use the [indicator functions](measure-theory.md#indicator-function) $P=\mathbf1_A(u)$ and $Q=\mathbf1_B(u)$. Then

$$
\begin{aligned}
\text{AND: }A\cap B&=\{4,6\},&\text{OR: }A\cup B&=\{2,4,5,6\},\\
\text{XOR: }A\mathbin\triangle B&=\{2,5\},&\text{NOT }A:\ U\setminus A&=\{1,3,5\}.
\end{aligned}
$$

Thus [logical conjunction](mathematical-logic.md#logical-conjunction) becomes [set intersection](set.md#set-intersection), [logical disjunction](mathematical-logic.md#logical-disjunction) becomes [set union](set.md#set-union), [exclusive or](#exclusive-or) becomes [symmetric difference](set.md#symmetric-difference), and [logical negation](#negation) becomes the [complement of a set](set.md#complement-of-a-set) within $U$. Outcome four satisfies both [events](probability-space.md#event), so inclusive [logical disjunction](mathematical-logic.md#logical-disjunction) includes it and [exclusive or](#exclusive-or) excludes it. If the die is fair, these four [events](probability-space.md#event) have [probabilities](probability-theory.md#probability) $1/3$, $2/3$, $1/3$, and $1/2$, respectively. No assumption of [independent events](probability-theory.md#independent-events) is needed for the [set](set.md) identities; indeed $A$ and $B$ here are not [independent](random-variable.md#independent-random-variables), since $1/3\ne(1/2)(1/2)$.

### Exclusive or

↑ **Parent:** [Boolean operation](#boolean-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exclusive_or)

[Exclusive or](#exclusive-or) returns one exactly when its two input [bits](information-theory.md#bit) differ. Its [truth table](mathematical-logic.md#truth-table) gives $0\oplus0=0$, $0\oplus1=1$, $1\oplus0=1$, and $1\oplus1=0$. The identities

$$
P\oplus Q=(P\vee Q)\wedge\neg(P\wedge Q)
=(P\wedge\neg Q)\vee(\neg P\wedge Q)
$$

express [exclusive or](#exclusive-or) using [logical conjunction](mathematical-logic.md#logical-conjunction), [logical disjunction](mathematical-logic.md#logical-disjunction), and [logical negation](#negation). The first expression accepts at least one input and then excludes both; the second explicitly lists the two accepted input pairs.

For numerical [bits](information-theory.md#bit), [exclusive or](#exclusive-or) is [addition](arithmetic.md#addition) in [modular arithmetic](modular-arithmetic.md) modulo two:

$$
x\oplus y=(x+y)\bmod2.
$$

The [binary operation](algebraic-operation.md#binary-operation) is [commutative](algebraic-operation.md#commutativity) and [associative](algebraic-operation.md#associative-property), because [addition](arithmetic.md#addition) modulo two has those properties. It satisfies $x\oplus0=x$, $x\oplus1=\neg x$, and $x\oplus x=0$. These identities explain why a [bit](information-theory.md#bit) can be toggled and restored with the same operation.

On [binary strings](#binary-string) of equal length, bitwise [exclusive or](#exclusive-or) applies the one-[bit](information-theory.md#bit) rule separately at each position. For example,

$$
1010\oplus0110=1100,\qquad1100\oplus0110=1010.
$$

A [bit mask](programming-language.md#bit-mask) of $0110$ toggles exactly the middle two [bits](information-theory.md#bit). Applying the mask twice restores the original [binary string](#binary-string): each selected [bit](information-theory.md#bit) changes twice, and each unselected [bit](information-theory.md#bit) stays fixed. This positional operation is distinct from taking the [exclusive or](#exclusive-or) of the overall [truth values](mathematical-logic.md#truth-value) of two [integers](integer.md).

#### Exclusive or toggles and parity

↑ **Parent:** [Exclusive or](#exclusive-or)

For [bits](information-theory.md#bit) $x_1,\ldots,x_n$, repeated [exclusive or](#exclusive-or) computes the [parity](quantum-mechanics.md#parity) of the number of ones:

$$
x_1\oplus\cdots\oplus x_n=\left(\sum_{i=1}^n x_i\right)\bmod2.
$$

An [induction](foundations-of-mathematics.md#mathematical-induction) proves this: the first [bit](information-theory.md#bit) gives its own [parity](quantum-mechanics.md#parity), and appending a zero preserves it while appending a one changes it. The [binary string](#binary-string) $10110$ has three ones, so its [parity bit](coding-theory.md#parity-bit) is one. Append that [parity bit](coding-theory.md#parity-bit) to obtain $101101$, whose six [bits](information-theory.md#bit) have even [parity](quantum-mechanics.md#parity). Flipping the second [bit](information-theory.md#bit) produces $111101$ and changes the combined [exclusive or](#exclusive-or) to one, detecting an error. Flipping the third [bit](information-theory.md#bit) as well produces $110101$, with four ones and combined [exclusive or](#exclusive-or) zero: an even number of flips can escape this check.

For three inputs, repeated [exclusive or](#exclusive-or) means an odd number of true inputs, rather than exactly one: $1\oplus1\oplus1=1$. The “exactly one” description applies to the two-input [exclusive or](#exclusive-or). This distinction matters when translating a requirement that exactly one option be selected into a program condition.

### Negation

↑ **Parent:** [Boolean operation](#boolean-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Negation)

[Logical negation](#negation) exchanges zero and one: $\neg0=1$ and $\neg1=0$. For a numerical [bit](information-theory.md#bit) $x$, this is $1-x$; applying [logical negation](#negation) twice restores $x$. It acts on the entire [propositional formula](mathematical-logic.md#propositional-formula) in its scope. Parentheses therefore matter: $\neg(P\vee Q)$ says that neither condition holds, while $(\neg P)\vee Q$ also accepts every case where $Q$ holds. At $(P,Q)=(1,1)$ their values are zero and one.

On a [set](set.md), [logical negation](#negation) becomes taking a [complement](set.md#complement-of-a-set) in a fixed [universal set](set.md#universal-set). In [Boolean operations on events](#boolean-operations-on-events), “not even” selects $\{1,3,5\}$. “Not both even and at least four” selects $\{1,2,3,5\}$; it does not require both qualifications to fail. [De Morgan's laws](#de-morgan-s-laws) make the scope of these compound negations precise.

<h3 id="de-morgan-s-laws">De Morgan's laws</h3>

↑ **Parent:** [Boolean operation](#boolean-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Morgan's_laws)

[De Morgan's laws](#de-morgan-s-laws) exchange [logical conjunction](mathematical-logic.md#logical-conjunction) and [logical disjunction](mathematical-logic.md#logical-disjunction) when a [logical negation](#negation) moves across them:

$$
\neg(P\wedge Q)\equiv(\neg P)\vee(\neg Q),
\qquad
\neg(P\vee Q)\equiv(\neg P)\wedge(\neg Q).
$$

Here $\equiv$ denotes [logical equivalence](mathematical-logic.md#logical-equivalence): the two [propositional formulas](mathematical-logic.md#propositional-formula) agree under every [Boolean valuation](mathematical-logic.md#boolean-valuation).[Discrete Mathematics: An Open Introduction (3rd edition) by Oscar Levin; Discrete Mathematics: An Open Introduction, 3rd edition by Oscar Levin, §3.1, Logical Equivalence: definition, Example 3.1.3 and De Morgan's Laws box](mathematics-bibliography.md#discrete-mathematics-an-open-introduction-3rd-edition-by-oscar-levin/3-1-propositional-logic)

A complete verification uses the four rows of a [truth table](mathematical-logic.md#truth-table). In input order $(0,0),(0,1),(1,0),(1,1)$, both sides of the first [logical equivalence](mathematical-logic.md#logical-equivalence) have output sequence $(1,1,1,0)$; both sides of the second have $(1,0,0,0)$. A proof in words is equally short: failure of “both” means at least one failure, whereas failure of “at least one” means both fail. The differing middle rows explain why simply pushing [logical negation](#negation) inward without changing AND to OR is wrong.

For the [events](probability-space.md#event) in [Boolean operations on events](#boolean-operations-on-events), the corresponding [set](set.md) identities are

$$
U\setminus(A\cap B)=(U\setminus A)\cup(U\setminus B)=\{1,2,3,5\},
$$



$$
U\setminus(A\cup B)=(U\setminus A)\cap(U\setminus B)=\{1,3\}.
$$

One can prove these identities by checking an arbitrary [set element](set.md#element-of-a-set) $u\in U$: its two membership [truth values](mathematical-logic.md#truth-value) obey [De Morgan's laws](#de-morgan-s-laws). The same reasoning works for any two [subsets](set.md#subset) of a common [universal set](set.md#universal-set).

<a id="image-de-morgan-s-laws-shade-the-same-set-whether-a-compound-event-is-complemented-first-or-its-component-events-are-complemented-first"></a>
![](de-morgan-event-regions.png)

**[Figure 2](#image-de-morgan-s-laws-shade-the-same-set-whether-a-compound-event-is-complemented-first-or-its-component-events-are-complemented-first). De Morgan's laws shade the same set whether a compound event is complemented first or its component events are complemented first**.

For a nested program test, let $R$ mean “backup recent”, $V$ mean “backup verified”, and $O$ mean “manual override authorized”. Rejecting when neither an acceptable backup nor an override is present gives

$$
\neg\bigl((R\wedge V)\vee O\bigr)
\equiv\bigl((\neg R)\vee(\neg V)\bigr)\wedge\neg O.
$$

The transformed condition reads “backup stale or unverified, and no override”. Apply the second of [De Morgan's laws](#de-morgan-s-laws) at the outside, then the first at the inner [logical conjunction](mathematical-logic.md#logical-conjunction). For $(R,V,O)=(1,0,0)$ it rejects; changing only $O$ to one makes it accept. With Boolean operands in [Python](programming-language.md#python-programming-language), `not ((recent and verified) or override)` and `((not recent) or (not verified)) and (not override)` have the same result and inspect the operands in the same order, with the same skipped operands.

#### De Morgan dual of a Boolean function

↑ **Parent:** [De Morgan's laws](#de-morgan-s-laws)

For a [Boolean function](analysis-of-boolean-functions.md#boolean-function) $f$ of $n$ input [bits](information-theory.md#bit), define its [De Morgan dual](#de-morgan-dual-of-a-boolean-function) by complementing every input, applying $f$, and complementing the output:

$$
f^*(x_1,\ldots,x_n)=1-f(1-x_1,\ldots,1-x_n).
$$

[De Morgan's laws](#de-morgan-s-laws) say that the [De Morgan dual](#de-morgan-dual-of-a-boolean-function) of [logical conjunction](mathematical-logic.md#logical-conjunction) is [logical disjunction](mathematical-logic.md#logical-disjunction), and conversely. The constant zero [Boolean function](analysis-of-boolean-functions.md#boolean-function) becomes constant one. This is different from merely negating the output: for AND, output [logical negation](#negation) gives one at $(0,0)$, whereas the [De Morgan dual](#de-morgan-dual-of-a-boolean-function) gives zero there.

Taking the [De Morgan dual](#de-morgan-dual-of-a-boolean-function) twice restores the original [Boolean function](analysis-of-boolean-functions.md#boolean-function):

$$
(f^*)^*(x)=1-\bigl(1-f(x)\bigr)=f(x).
$$

Here each input is complemented twice as well. For a [Boolean formula](#boolean-formula) built from AND, OR, NOT and constants, its [De Morgan dual](#de-morgan-dual-of-a-boolean-function) can therefore be obtained by exchanging AND with OR and zero with one throughout, leaving input names and NOT in place. A structural [induction](foundations-of-mathematics.md#mathematical-induction) proves the rule: it holds for an input and each constant, [De Morgan's laws](#de-morgan-s-laws) handle the two binary [logical connectives](mathematical-logic.md#logical-connective), and double [logical negation](#negation) handles NOT. This symmetry lets one translate a complex test systematically instead of guessing where its failures occur.

## Computational complexity theory

↑ **Parent:** [Theoretical computer science](theoretical-computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computational_complexity_theory)

Computational complexity theory classifies [computational problems](#computational-problem) by the resources needed to solve them.

### Communication complexity

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Communication_complexity)

Communication complexity studies how much information distributed parties must exchange to compute a function of their separately held inputs. Local computation is free; the resource being counted is communicated bits or qubits, with the allowed shared randomness, [quantum entanglement](bell-state.md#entangled-state) or other correlations specified separately. For a [Boolean function](analysis-of-boolean-functions.md#boolean-function) $f(x,y)$, a one-way exact protocol has the receiver output $f$ correctly for every input after a single message. [One-bit computation using Popescu–Rohrlich boxes](foundations-of-quantum-mechanics.md#one-bit-computation-using-popescu-rohrlich-boxes) shows that this resource measure changes drastically if ideal superquantum boxes are available.

### Promise problem

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)

A [promise problem](#promise-problem) consists of disjoint sets of YES and NO instances. An algorithm or verifier must obey its correctness guarantees only on their union. Energy problems with separated thresholds are naturally [promise problems](#promise-problem) because intermediate-energy instances require no prescribed answer.

### Quantum complexity theory

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_complexity_theory)

Quantum complexity theory studies resources needed by [quantum circuits](quantum-circuit.md) and quantum algorithms, including time, workspace, and [quantum query complexity](#quantum-query-complexity). Its models specify which input oracles and gate implementations are available; counting oracle calls is different from counting all elementary gates.

#### BQP

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

[BQP](#bqp) is the class of [promise problems](#promise-problem) decided by uniform polynomial-size [quantum circuits](quantum-circuit.md) with bounded error. Completeness $2/3$ and soundness $1/3$ are conventional; [BQP error reduction](#bqp-error-reduction) shows that other fixed separated thresholds give the same class.

##### BQP error reduction

↑ **Parent:** [BQP](#bqp)

Independent runs of a [BQP](#bqp) algorithm with fresh [ancilla qubits](quantum-information-theory.md#ancilla-qubit) can be combined by a classical threshold rule. If completeness exceeds soundness by $\gamma$, a [Hoeffding inequality](probability-inequality.md#hoeffding-inequality) bounds the error after $r$ runs by $e^{-r\gamma^2/2}$. Polynomial repetition handles inverse-polynomial gaps. This does not automatically preserve the restricted gate and measurement rules of a [stoquastic circuit](quantum-circuit.md#stoquastic-circuit).

#### Quantum witness

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

A [quantum witness](#quantum-witness) is a polynomial-size [quantum state](quantum-system.md#quantum-state) supplied to a verifier as evidence for a YES instance. The verifier fixes its own [ancilla qubits](quantum-information-theory.md#ancilla-qubit) independently. Pure [quantum witnesses](#quantum-witness) suffice when maximizing a linear acceptance functional on [density operators](density-matrix.md). [Quantum witnesses](#quantum-witness) are not generally restricted to basis vectors or product states.

#### StoqMA

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

[StoqMA](#stoqma) is a restricted quantum-verifier class using [stoquastic circuits](quantum-circuit.md#stoquastic-circuit) and polynomial-size [quantum witnesses](#quantum-witness). A YES instance has a [quantum witness](#quantum-witness) accepted with probability at least $a$; on a NO instance every [quantum witness](#quantum-witness) has acceptance at most $b$, with an inverse-polynomial gap $a-b$. An optimal [quantum witness](#quantum-witness) can be chosen with nonnegative amplitudes, since the [witness acceptance operator](#witness-acceptance-operator) is entrywise nonnegative. The [quantum witness](#quantum-witness) is generally a superposition, rather than a [computational basis](quantum-theory.md#computational-basis) vector. The [stoquastic acceptance floor](quantum-circuit.md#stoquastic-acceptance-floor) explains the lower limit $b\geq1/2$ for a nontrivial soundness promise.

#### QMA

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

[QMA](#qma) is the class of [promise problems](#promise-problem) with a polynomial-size quantum witness checked by a uniform polynomial-size [quantum circuit](quantum-circuit.md). YES instances have an accepting witness with probability at least $2/3$; NO instances have acceptance at most $1/3$ for every witness, including mixed states. The verifier's acceptance is linear in the witness [density operator](density-matrix.md). Inverse-polynomial or exponentially small error can be obtained through [QMA error reduction](#qma-error-reduction).

##### Witness acceptance operator

↑ **Parent:** [QMA](#qma)

For [quantum witness](#quantum-witness) embedding $J$, verifier unitary $U$ and accepting projector $\Pi$, the [witness acceptance operator](#witness-acceptance-operator) is the positive contraction $F=J^\dagger U^\dagger\Pi UJ$. The maximum acceptance over normalized [quantum witnesses](#quantum-witness) is $\lambda_{\max}(F)$ by the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient). Restricting to basis [quantum witnesses](#quantum-witness) only tests its diagonal entries and need not find that maximum.

###### Trace-power witness optimization

↑ **Parent:** [Witness acceptance operator](#witness-acceptance-operator)

For a positive [witness acceptance operator](#witness-acceptance-operator) on dimension $D$, large trace powers approximate its largest [eigenvalue](linear-operator-theory.md#eigenvalue). With an $m$-qubit [QMA](#qma) [quantum witness](#quantum-witness) and $d=2m+2$, the usual NO instances give $\operatorname{Tr}(F^d)<2^{-d}$ and YES instances give a value above $2^{-d}$. A closed product-index expansion computes the trace by recomputation with polynomial storage, avoiding logarithms and roots in a real-arithmetic implementation.

##### QMA error reduction

↑ **Parent:** [QMA](#qma)

Starting from completeness $2/3$ and soundness $1/3$, run an odd number $r$ of parallel copies and take majority. The [QMA parallel repetition with entangled witnesses](#qma-parallel-repetition-with-entangled-witnesses) argument proves soundness for arbitrary repeated witnesses. Exponential [Markov's inequality](probability-inequality.md#markov-s-inequality) gives majority error at most $(2\sqrt2/3)^r$. Hence $O(\log(1/\epsilon))$ copies suffice for error $\epsilon$, with polynomial overhead when the target error is inverse-polynomial or exponentially small in input length.

##### QMA parallel repetition with entangled witnesses

↑ **Parent:** [QMA](#qma)

Independent verifier circuits on $r$ witness registers induce a threshold acceptance effect built from tensor products of $M$ and $I-M$, where $M$ is the [quantum verifier acceptance operator](#quantum-verifier-acceptance-operator). In a product eigenbasis of $M$, the effect's [eigenvalues](linear-operator-theory.md#eigenvalue) are threshold probabilities for independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) with parameters given by the selected eigenvalues of $M$. Bounding every parameter on a NO instance bounds the effect's [operator norm](continuous-dual-space.md#operator-norm), even if the actual submitted witness is entangled. Independence is used only for the spectral calculation, not assumed for the witness.

##### Quantum verifier acceptance operator

↑ **Parent:** [QMA](#qma)

A verifier with clean ancillas and a designated output measurement induces an effect $0\leq M\leq I$ on the witness register. Its acceptance probability is $\operatorname{Tr}(M\rho)$, and the largest possible acceptance is $\|M\|$. Spectral bounds on $M$ make the soundness quantifier over all witnesses, including entangled repeated witnesses, explicit.

#### Quantum query complexity

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

The quantum query complexity of a task counts uses of an input oracle by a [quantum circuit](quantum-circuit.md), for a specified success probability. Known gates and workspace operations are not counted as oracle queries, although they contribute to the circuit's full runtime. An efficient query bound therefore need not, by itself, be an efficient gate bound.

##### Polynomial method for quantum query lower bounds

↑ **Parent:** [Quantum query complexity](#quantum-query-complexity)

After $T$ input-bit queries, every [probability amplitude](wave-function.md#probability-amplitude) is a [polynomial](polynomial.md) of degree at most $T$, because the bit-query matrix entries are affine in the input bits. An acceptance [probability](probability-theory.md#probability) is a sum of squared absolute amplitudes and has [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $2T$. [Multilinear reduction on the Boolean cube](polynomial.md#multilinear-reduction-on-the-boolean-cube) does not increase degree. Exact acceptance therefore implies $Q_E(f)\ge\lceil\deg(f)/2\rceil$. For bounded error the acceptance polynomial only approximates the [Boolean function](analysis-of-boolean-functions.md#boolean-function); its exact representing degree is not the relevant bound.

##### Exact quantum query complexity

↑ **Parent:** [Quantum query complexity](#quantum-query-complexity)

The least worst-case number of input-oracle calls made by a [quantum circuit](quantum-circuit.md) that computes a [Boolean function](analysis-of-boolean-functions.md#boolean-function) with zero error on every input. Known [unitary gates](quantum-circuit.md#quantum-logic-gate) and classical processing do not count toward this quantity; their runtime is a separate cost.

###### Exact two-query majority algorithm

↑ **Parent:** [Exact quantum query complexity](#exact-quantum-query-complexity)

One exact parity query determines whether the first two bits agree. If they agree, a second query reads one of them; otherwise it reads the third bit. Those values respectively determine the three-bit [majority function](#majority-function). The matching lower bound follows from its degree-three [multilinear polynomial](polynomial.md#multilinear-polynomial).

##### Quantum collision finding

↑ **Parent:** [Quantum query complexity](#quantum-query-complexity)

Given a [function](function.md) $f$ with an $m$-bit output, accessed through the [unitary operator](vector-space.md#unitary-operator) $U_f|x\rangle|y\rangle=|x\rangle|y\mathbin\oplus f(x)\rangle$, quantum collision finding asks for distinct inputs with equal outputs. Here $\oplus$ is bitwise [exclusive or](#exclusive-or) on the $m$-bit answer [quantum register](quantum-circuit.md#quantum-register). The distinctness requirement excludes the uninformative pair $(x,x)$. For a two-to-one function on $N$ inputs, [Grover search algorithm](quantum-theory.md#grover-s-algorithm) methods yield a cube-root [quantum query complexity](#quantum-query-complexity), despite a square-root cost for finding a partner of just one preselected input.

<h6 id="brassard-hoyer-tapp-collision-algorithm">Brassard–Høyer–Tapp collision algorithm</h6>

↑ **Parent:** [Quantum collision finding](#quantum-collision-finding)

Query a known set of $m$ inputs and store its output table. If no [function collision](function.md#function-collision) occurs there, each of its $m$ distinct outputs has exactly one partner in the complement, for a two-to-one function. A [compute-phase-uncompute construction](quantum-theory.md#compute-phase-uncompute-construction) marks those partners using two function queries and reversible table comparison. [Known-subset Grover search](quantum-theory.md#known-subset-grover-search) then uses $O(\sqrt{(N-m)/m})$ such phase queries. Including table preparation and a final verification query gives

$$
T(m)=m+O\!\left(\sqrt{\frac{N-m}{m}}\right)+1.
$$

Choosing $m\asymp N^{1/3}$ balances both terms and gives $T(m)=O(N^{1/3})$. The [Grover rotation angle](quantum-theory.md#grover-rotation-angle) rounding bound gives success tending to one. This is a query bound; it does not make reversible table lookup free in a gate or physical-memory cost model.

### Decision tree model

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decision_tree_model)

The decision tree model computes a function by adaptively querying input coordinates.

#### Decision tree

↑ **Parent:** [Decision tree model](#decision-tree-model)

A [decision tree](#decision-tree) represents a [deterministic computation](#deterministic-computation) of a known [Boolean function](analysis-of-boolean-functions.md#boolean-function) $f:\{0,1\}^n\to\{0,1\}$ by inspecting [input](#input-computer-science) [bits](information-theory.md#bit). Each internal [vertex](graph.md#vertex-graph-theory) of its [binary tree](data-structure.md#binary-tree) names a coordinate $i$ to query, its two outgoing [edges](graph-theory.md#edge-of-a-graph) carry answers 0 and 1, and each leaf carries the [output](#output-computing) 0 or 1. Starting at the [root of a tree](tree-graph-theory.md#root-of-a-tree), read the named [bit](information-theory.md#bit), follow its answer [edge](graph-theory.md#edge-of-a-graph), and repeat until a leaf is reached. Correctness requires the leaf's label to equal $f(x)$ for every [input](#input-computer-science) $x$.[Buhrman and de Wolf, Complexity Measures and Decision Tree Complexity: A Survey, section 3.1, manuscript p. 5: deterministic trees and D(f)](computer-science-bibliography.md#complexity-measures-and-decision-tree-complexity-a-survey-by-harry-buhrman-and-ronald-de-wolf)

The next coordinate, or the decision to stop, can depend on earlier answers: this is adaptive querying. The same [input](#input-computer-science) always follows the same [graph path](graph-theory.md#path-in-a-graph); adaptivity does not require randomness. A correct leaf must have the same [output](#output-computing) for every completion of the observed [bits](information-theory.md#bit). Thus a [decision tree](#decision-tree) can stop as soon as the observations form a [query certificate](#query-certificate). Querying an already known coordinate adds no information, so we use [decision trees](#decision-tree) without repeated coordinates on a [graph path](graph-theory.md#path-in-a-graph); an efficient tree also removes queries made after the [output](#output-computing) is already forced.

The motivation is exact computation with shortcuts. If inspecting an [input](#input-computer-science) entry is expensive, the question is how much of the [input](#input-computer-science) must actually be read. The [decision-tree query cost](#decision-tree-query-cost) counts these inspections, while local calculations on known values are free in this model; this cost need not equal an implementation's [time complexity](#time-complexity). Here the [Boolean function](analysis-of-boolean-functions.md#boolean-function) is specified in advance and must be computed exactly on every [input](#input-computer-science). [Decision tree learning](foundations-of-mathematics.md#decision-tree-learning) instead fits a predictor from data, with a different objective.

##### Binary decision tree

↑ **Parent:** [Decision tree](#decision-tree)

##### Three-bit majority decision tree

↑ **Parent:** [Decision tree](#decision-tree)

Three votes give a small but revealing [majority function](#majority-function):

$$
m(x_1,x_2,x_3)=\begin{cases}1,&x_1+x_2+x_3\geq2,\\0,&x_1+x_2+x_3<2.\end{cases}
$$

Our [decision tree](#decision-tree) queries $x_1$, then $x_2$. If these [bits](information-theory.md#bit) agree, return their common value: two equal votes already force the [majority function](#majority-function). If they disagree, query $x_3$ and return its value. The first two queries have a fixed order, but whether a third query occurs is adaptive.

<a id="image-an-exact-three-bit-majority-decision-tree-equal-first-answers-stop-after-two-queries"></a>
![](majority-three-bit-adaptive-decision-tree.png)

**[Figure 3](#image-an-exact-three-bit-majority-decision-tree-equal-first-answers-stop-after-two-queries). An exact three-bit majority decision tree: equal first answers stop after two queries**.

Each internal label in the diagram names the next [bit](information-theory.md#bit) to inspect. Each leaf lists its [output](#output-computing), [decision-tree query cost](#decision-tree-query-cost) $q$, and compatible [inputs](#input-computer-science); an asterisk denotes an unread [bit](information-theory.md#bit). The two shallow leaves each cover two [inputs](#input-computer-science), while each deeper leaf covers one. Reading every [bit](information-theory.md#bit) would also compute the [majority function](#majority-function), but would miss these exact shortcuts.

All eight [inputs](#input-computer-science) give the following exhaustive check. The [parity](quantum-mechanics.md#parity) column is the [parity](quantum-mechanics.md#parity) of $x_1+x_2+x_3$, computed by [exclusive or](#exclusive-or); its [decision-tree query cost](#decision-tree-query-cost) is justified under [parity lower bound for Boolean queries](#parity-lower-bound-for-boolean-queries).

| $x_1x_2x_3$ | [Majority function](#majority-function) [output](#output-computing) | Queried coordinates for the [majority function](#majority-function) | [Majority function](#majority-function) query count | [Parity](quantum-mechanics.md#parity) [output](#output-computing) | [Parity](quantum-mechanics.md#parity) query count | 000 | 0 | $1,2$ | 2 | 0 | 3 | 001 | 0 | $1,2$ | 2 | 1 | 3 | 010 | 0 | $1,2,3$ | 3 | 1 | 3 | 011 | 1 | $1,2,3$ | 3 | 0 | 3 | 100 | 0 | $1,2,3$ | 3 | 1 | 3 | 101 | 1 | $1,2,3$ | 3 | 0 | 3 | 110 | 1 | $1,2$ | 2 | 0 | 3 | 111 | 1 | $1,2$ | 2 | 1 | 3 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |

The worst [inputs](#input-computer-science) for this [decision tree](#decision-tree) are $010,011,100,101$, exactly those with $x_1\ne x_2$. Its actual depth is three. Every exact [decision tree](#decision-tree) for this [majority function](#majority-function) has depth at least three: after the first query, an adversary can answer the second distinct query with the opposite [bit](information-theory.md#bit), leaving the last [bit](information-theory.md#bit) decisive. Consequently its optimal [decision-tree depth](#decision-tree-depth) is $D(m)=3$, even though some [inputs](#input-computer-science) finish sooner. Every [input](#input-computer-science) has a two-[bit](information-theory.md#bit) [query certificate](#query-certificate), namely two agreeing votes; locating those votes can require a third query. This separates having a short [query certificate](#query-certificate) from finding one.

##### Parity lower bound for Boolean queries

↑ **Parent:** [Decision tree](#decision-tree)

For three [bits](information-theory.md#bit), the [Boolean function](analysis-of-boolean-functions.md#boolean-function) $p(x)=x_1\mathbin\oplus x_2\mathbin\oplus x_3$ outputs one when $x_1+x_2+x_3$ is odd, where $\oplus$ denotes [exclusive or](#exclusive-or). Unlike the [three-bit majority decision tree](#three-bit-majority-decision-tree), an exact [decision tree](#decision-tree) computing [parity](quantum-mechanics.md#parity) must inspect all three [bits](information-theory.md#bit) on every [input](#input-computer-science). If any coordinate is unread, two completions differing only at that coordinate follow the same observed [graph path](graph-theory.md#path-in-a-graph) but have opposite [parity](quantum-mechanics.md#parity). A single leaf cannot correctly label both.

The same argument works for $n$ [bits](information-theory.md#bit): [parity](quantum-mechanics.md#parity) needs all $n$ queries on every [input](#input-computer-science), whatever their order. Thus its [decision-tree depth](#decision-tree-depth) is $n$, its [expected query cost](#expected-query-cost) is $n$ for every [input](#input-computer-science) [probability distribution](probability-distribution.md), and each [coordinate revealment](#coordinate-revealment) is one. The algorithm remains required to be correct on the whole [Boolean cube](analysis-of-boolean-functions.md#boolean-hypercube), even if the chosen [probability distribution](probability-distribution.md) assigns some [inputs](#input-computer-science) zero [probability](probability-theory.md#probability); a promise restricting permitted [inputs](#input-computer-science) would be a different [computational problem](#computational-problem).

##### Decision-tree query cost

↑ **Parent:** [Decision tree](#decision-tree)

For a particular [decision tree](#decision-tree) $T$, its [decision-tree query cost](#decision-tree-query-cost) $q_T(x)$ is the number of queries along the [graph path](graph-theory.md#path-in-a-graph) followed by [input](#input-computer-science) $x$. Its actual tree depth is

$$
h(T)=\max_{x\in\{0,1\}^n}q_T(x).
$$

The query [vertices](graph.md#vertex-graph-theory) count as operations; each is followed by one answer [edge](graph-theory.md#edge-of-a-graph). Thus a leaf reached after $k$ queries has [graph path](graph-theory.md#path-in-a-graph) length $k$, and a tree consisting only of an [output](#output-computing) leaf has depth zero. With no repeated coordinates, $0\leq q_T(x)\leq n$. The [decision-tree depth](#decision-tree-depth) $D(f)$ minimizes $h(T)$ over all correct [decision trees](#decision-tree) for $f$; $h(T)$ measures the chosen algorithm, while $D(f)$ measures the [Boolean function](analysis-of-boolean-functions.md#boolean-function).

Choose an [input](#input-computer-science) [probability distribution](probability-distribution.md) $\mu$ and let $X$ have that distribution. Then $q_T(X)$ is a [random variable](random-variable.md) even when the [decision tree](#decision-tree) is deterministic. Its [probability mass function](probability-distribution.md#probability-mass-function) describes how often each path length occurs, and its [expected value](expected-value.md) is the [expected query cost](#expected-query-cost). None of these quantities changes the actual maximum depth of $T$.

<a id="image-uniform-three-bit-inputs-query-count-distributions-and-coordinate-revealment-for-majority-and-parity"></a>
![](majority-parity-query-cost-distributions.png)

**[Figure 4](#image-uniform-three-bit-inputs-query-count-distributions-and-coordinate-revealment-for-majority-and-parity). Uniform three-bit inputs: query-count distributions and coordinate revealment for majority and parity**.

The left panel aggregates the eight [inputs](#input-computer-science) from the [three-bit majority decision tree](#three-bit-majority-decision-tree): four cost two queries and four cost three. [Parity](quantum-mechanics.md#parity) always costs three. The right panel asks a different question, which coordinates are inspected: the [majority function](#majority-function) algorithm always queries coordinates 1 and 2, but queries coordinate 3 only on disagreements. These are [probabilities](probability-theory.md#probability) of inspection, not [probabilities](probability-theory.md#probability) that a [bit](information-theory.md#bit) equals one.

###### Expected query cost

↑ **Parent:** [Decision-tree query cost](#decision-tree-query-cost)

For a fixed [decision tree](#decision-tree) $T$ and [input](#input-computer-science) [probability distribution](probability-distribution.md) $\mu$, its [expected query cost](#expected-query-cost) is

$$
\mathbb E_\mu[q_T(X)]=\sum_{x\in\{0,1\}^n}\mu(x)q_T(x).
$$

Under the [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution) on the eight three-[bit](information-theory.md#bit) [inputs](#input-computer-science), the [three-bit majority decision tree](#three-bit-majority-decision-tree) has

$$
\Pr(q_T(X)=2)=\Pr(q_T(X)=3)=\frac12,\qquad \mathbb E[q_T(X)]=2\cdot\frac12+3\cdot\frac12=\frac52=2.5.
$$

This is an exact average, not a fractional query made during one execution. It is also optimal among exact deterministic [decision trees](#decision-tree) under this [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution): one observed [bit](information-theory.md#bit) never determines the [majority function](#majority-function); whichever two distinct coordinates are inspected first, their values disagree with [probability](probability-theory.md#probability) $1/2$, forcing a third query. In comparison, querying all three [bits](information-theory.md#bit) unconditionally has the same actual depth three but [expected query cost](#expected-query-cost) three.

For an arbitrary [input](#input-computer-science) [probability distribution](probability-distribution.md), the same fixed [three-bit majority decision tree](#three-bit-majority-decision-tree) gives $\mathbb E_\mu[q_T(X)]=2+\Pr_\mu(X_1\ne X_2)$. For three [independent random variables](random-variable.md#independent-random-variables), each a [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) with common one-[probability](probability-theory.md#probability) $p$, this becomes $2+2p(1-p)$; the value $2.5$ depends on $p=1/2$. Averaging over [inputs](#input-computer-science) should also be distinguished from averaging over an algorithm's internal random choices at a fixed [input](#input-computer-science).[O'Donnell, Saks, Schramm and Servedio, Every decision tree has an influential variable, sections 1.1–1.2, pp. 1–2: worst-input expected randomized cost R(f) versus input-distribution average Δ(T)](computer-science-bibliography.md#every-decision-tree-has-an-influential-variable-by-ryan-o-donnell-and-others)

###### Coordinate revealment

↑ **Parent:** [Decision-tree query cost](#decision-tree-query-cost)

The [coordinate revealment](#coordinate-revealment) of coordinate $i$ for a [decision tree](#decision-tree) $T$ under [input](#input-computer-science) [probability distribution](probability-distribution.md) $\mu$ is

$$
\delta_i(T,\mu)=\Pr_{X\sim\mu}(T\text{ queries coordinate }i).
$$

It depends on the chosen [decision tree](#decision-tree) and the [probability distribution](probability-distribution.md), not just on the [Boolean function](analysis-of-boolean-functions.md#boolean-function). Since no coordinate is queried twice on a [graph path](graph-theory.md#path-in-a-graph), [indicator functions](measure-theory.md#indicator-function) give

$$
q_T(X)=\sum_{i=1}^n\mathbf 1_{\{T\text{ queries }i\}},\qquad \mathbb E_\mu[q_T(X)]=\sum_{i=1}^n\delta_i(T,\mu).
$$

The second equality uses [linearity of expectation](expected-value.md#linearity-of-expectation); it does not require [independence of random variables](random-variable.md#independent-random-variables) or a [product measure](probability-theory.md#product-measure). The cited paper defines these inspection [probabilities](probability-theory.md#probability) and their sum for [product measures](probability-theory.md#product-measure); the displayed [indicator function](measure-theory.md#indicator-function) argument extends the identity to any [input](#input-computer-science) [probability distribution](probability-distribution.md).[O'Donnell, Saks, Schramm and Servedio, Every decision tree has an influential variable, section 1.2, p. 2: δ\_i(T) and Δ(T); section 3.1, p. 6: distinct coordinates along each root–leaf path](computer-science-bibliography.md#every-decision-tree-has-an-influential-variable-by-ryan-o-donnell-and-others)

For the [three-bit majority decision tree](#three-bit-majority-decision-tree) under the [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution), $(\delta_1,\delta_2,\delta_3)=(1,1,1/2)$, whose sum is $2.5$. Reading coordinate 3 first, then coordinate 1, and stopping on agreement gives the same [majority function](#majority-function), depth and [expected query cost](#expected-query-cost), but [coordinate revealments](#coordinate-revealment) $(1,1/2,1)$. The asymmetry belongs to the chosen query order. [Parity](quantum-mechanics.md#parity) gives $(1,1,1)$ for every exact [decision tree](#decision-tree) without repeated queries. If repeated queries were charged, inspection [probabilities](probability-theory.md#probability) would count distinct coordinates; total query count would instead require expected multiplicities.

##### Decision-tree depth

↑ **Parent:** [Decision tree](#decision-tree)

The [decision-tree depth](#decision-tree-depth) $D(f)$ of a [Boolean function](analysis-of-boolean-functions.md#boolean-function) $f$ is the smallest possible maximum number of [input](#input-computer-science) coordinates queried along any root-to-leaf [graph path](graph-theory.md#path-in-a-graph) of a [decision tree](#decision-tree) computing $f$:

$$
D(f)=\min_{T\text{ computes }f}\max_{x\in\{0,1\}^n}q_T(x)=\min_{T\text{ computes }f}h(T).
$$

The actual depth $h(T)$ of a particular [decision tree](#decision-tree) can exceed this optimum. A [constant function](function.md#constant-function) admits a depth-zero tree even though an inefficient algorithm could inspect its entire [input](#input-computer-science) before returning that constant. [Expected query cost](#expected-query-cost) and [coordinate revealment](#coordinate-revealment) additionally require an [input](#input-computer-science) [probability distribution](probability-distribution.md); $D(f)$ does not. The [three-bit majority decision tree](#three-bit-majority-decision-tree) and three-[bit](information-theory.md#bit) [parity](quantum-mechanics.md#parity) both have optimal [decision-tree depth](#decision-tree-depth) three, although only the former has the two-query shortcuts described above.

###### Certificate complexity of a Boolean function

↑ **Parent:** [Decision-tree depth](#decision-tree-depth)

A [query certificate](#query-certificate) fixes some input coordinates to their values in a chosen input and must force the output for every completion. The smallest such size is $C(f,x)$; maximizing over accepted or rejected inputs gives $C_1(f)$ or $C_0(f)$, and maximizing both gives $C(f)$. A one-sided maximum over an empty output class is defined as zero. This is [query certificate](#query-certificate) complexity, distinct from polynomial verification of a witness in [NP](#np-complexity).

###### Query certificate

↑ **Parent:** [Certificate complexity of a Boolean function](#certificate-complexity-of-a-boolean-function)

For a [Boolean function](analysis-of-boolean-functions.md#boolean-function) $f$ and a chosen input $x$, a set of coordinates $S$ is a [query certificate](#query-certificate) if every $y$ agreeing with $x$ on $S$ has $f(y)=f(x)$. It fixes actual input bits rather than supplying an independently guessed [certificate](#certificate-complexity) to an NP verifier. Minimizing its size at each input and then maximizing gives [query certificate complexity](#certificate-complexity-of-a-boolean-function).

###### Evasive Boolean function

↑ **Parent:** [Decision-tree depth](#decision-tree-depth)

A [Boolean function](analysis-of-boolean-functions.md#boolean-function) is evasive when every deterministic [decision tree](#decision-tree) computing it has a worst-case path that queries all input bits. The [alternating-sum criterion for decision-tree evasiveness](#alternating-sum-criterion-for-decision-tree-evasiveness) is one sufficient method for proving this lower bound.

###### Alternating-sum criterion for decision-tree evasiveness

↑ **Parent:** [Evasive Boolean function](#evasive-boolean-function)

A leaf reached before all $n$ input bits are queried leaves at least one coordinate free. Flipping that coordinate pairs its inputs with opposite alternating signs and equal output. Thus every such leaf contributes zero. If the total alternating sum is nonzero, a depth below $n$ is impossible.

###### Decision-tree adversary for a threshold function

↑ **Parent:** [Decision-tree depth](#decision-tree-depth)

To prove that a threshold function requires every input bit in the worst case, an adversary answers queries while keeping completions on both sides of the threshold possible. If this remains true until the final unqueried bit, every decision tree has depth equal to the number of variables.

### Computational problem

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computational_problem)

A computational problem specifies the required [output](#output-computing) for every permitted [input](#input-computer-science).

#### Input (computer science)

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Input_(computer_science))

An input is the finite data supplied to a computation.

#### Output (computing)

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Output_(computing))

An output is the data produced by a computation.

#### Decision problem

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decision_problem)

A decision problem asks for one of two answers, conventionally encoded as zero and one. Equivalently, it asks whether an input belongs to a [formal language](#formal-language).

#### Search problem

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Search_problem)

A search problem asks for a witness satisfying a specified relation rather than only whether one exists.

##### Search tree

↑ **Parent:** [Search problem](#search-problem)

A [rooted tree](tree-graph-theory.md#rooted-tree) whose nodes are partial search states and whose children are possible next choices. Leaves represent completed candidates or terminated branches. [Backtracking](algorithm.md#backtracking) traverses this tree while storing the current path, and [search pruning](algorithm.md#search-pruning) removes branches that cannot yield a useful completion.

###### Branching factor

↑ **Parent:** [Search tree](#search-tree)

The number of children of a node in a [search tree](#search-tree), or an upper bound on that number over the tree. With branching factor at most $b$ and depth at most $d$, a complete traversal visits at most $1+b+\cdots+b^d$ nodes.

##### Constraint satisfaction problem

↑ **Parent:** [Search problem](#search-problem)

Assign values from specified domains to variables so that all stated constraints hold simultaneously. A partial assignment can be rejected when it violates a constraint or leaves an unassigned variable with no permissible value. [Backtracking](algorithm.md#backtracking) applies this test during a [depth-first search](algorithm.md#depth-first-search).

###### Sudoku

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

A finite [constraint satisfaction problem](#constraint-satisfaction-problem) on a $9\times9$ [array](data-structure.md#array-data-structure). Each entry must be one of the [integers](integer.md) $1,\ldots,9$, and every row, column, and designated $3\times3$ box must contain each value once. Given entries constrain the possible completions; [backtracking](algorithm.md#backtracking) searches those completions.

###### Kakuro

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

###### Forward checking

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

###### Minimum remaining values

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

###### Constraint propagation

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

###### All-different constraint

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

###### Minimum remaining values heuristic

↑ **Parent:** [Constraint satisfaction problem](#constraint-satisfaction-problem)

Choose an unassigned variable with the fewest currently legal values. No legal values detects failure immediately; exactly one legal value forces a choice. This ordering can reduce the [search tree](#search-tree) without changing the set of solutions.

##### Search-to-decision reduction

↑ **Parent:** [Search problem](#search-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Search-to-decision_reduction)

A search-to-decision reduction reconstructs a witness by making queries that only decide whether a suitable witness exists.

### Complexity class

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complexity_class)

A complexity class is a collection of [computational problems](#computational-problem) sharing specified resource bounds and a computational model.

#### Time complexity

↑ **Parent:** [Complexity class](#complexity-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Time_complexity)

The time complexity of an [algorithm](algorithm.md) bounds its number of computation steps as a function of its input length.

Specify both the size parameter and the operations counted. For [binary search](algorithm.md#binary-search), take $n$ to be the number of [array](data-structure.md#array-data-structure) entries and count a three-way comparison of the target with one entry as one operation. Code using separate equality and less-than tests may perform two primitive tests per inspected entry; this changes a constant factor. The [input](#input-computer-science) size in bits is a different parameter when entries have variable-length representations.

Worst-case [time complexity](#time-complexity) maximizes the count over permitted [inputs](#input-computer-science) of size $n$. An absent target forces $n$ comparisons in [linear search](algorithm.md#linear-search). For [binary search](algorithm.md#binary-search), the worst-case count is $\lfloor\log_2 n\rfloor+1$ for $n\geq1$, attained by a target larger than every entry. Both have a best case of one comparison when the first inspected entry matches.

In [Big O notation](real-analysis.md#big-o-notation), the worst-case bounds are $O(n)$ and $O(\log n)$ respectively. Here $T(n)=O(g(n))$ means that fixed constants $C,n_0$ exist with $T(n)\leq Cg(n)$ for all $n\geq n_0$. It is an upper bound, so a logarithmic count is also $O(n)$; the sharper bound communicates its scaling better. The base of the [logarithm](calculus.md#logarithm) changes only a constant factor.

For $n=1{,}000{,}000$, [linear search](algorithm.md#linear-search) can require $1{,}000{,}000$ comparisons, whereas [binary search](algorithm.md#binary-search) needs at most $20$, since $2^{19}\leq n<2^{20}$. Doubling $n$ adds just one to the worst-case [binary search](algorithm.md#binary-search) count. These are operation counts, not measured machine runtimes. Translating them into logarithmic execution time assumes constant-cost indexed access, comparison and index arithmetic. Long entries can make comparison expensive; a [linked list](data-structure.md#linked-list) does not provide constant-cost access to an arbitrary middle index. Building or sorting the [array](data-structure.md#array-data-structure) is additional work: [merge sort](algorithm.md#merge-sort) can provide order for many subsequent searches, but its cost belongs in the analysis too.

##### Quadratic time

↑ **Parent:** [Time complexity](#time-complexity)

A [time complexity](#time-complexity) bounded by $O(n^2)$ for input size $n$. Examining every ordered pair of entries with constant work per pair has this bound.

##### Linear time

↑ **Parent:** [Time complexity](#time-complexity)

A [time complexity](#time-complexity) bounded by $O(n)$ for input size $n$. A single pass with constant work per input entry has this bound.

##### Constant time

↑ **Parent:** [Time complexity](#time-complexity)

A [time complexity](#time-complexity) bounded by $O(1)$ independently of input size, under a stated computational cost model. Fixed-size machine arithmetic may be constant time, whereas [arbitrary-precision arithmetic](arithmetic.md#arbitrary-precision-arithmetic) depends on operand length.

##### Pseudo-polynomial time

↑ **Parent:** [Time complexity](#time-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudo-polynomial_time)

An [algorithm](algorithm.md) has [pseudo-polynomial time](#pseudo-polynomial-time) when its running time is bounded by a [polynomial](polynomial.md) in the numerical magnitudes of input quantities, rather than necessarily in their encoded length. The [dynamic programming](mathematical-optimization.md#dynamic-programming) table for the [0-1 knapsack problem](mathematical-optimization.md#0-1-knapsack-problem) uses $O(nW)$ arithmetic operations for $n$ items and capacity $W$. A [binary numeral system](integer.md#binary-numeral-system) encoding needs only $O(\log(W+1))$ bits for that capacity, so the table bound can be exponential in the number of capacity bits. This distinction does not claim that every input requires exponential work.

##### Amortized analysis

↑ **Parent:** [Time complexity](#time-complexity)

[Amortized analysis](#amortized-analysis) bounds the total cost of every permitted [sequence](sequence-and-series.md#sequence) of operations from a specified initial state. An amortized $O(1)$ bound means that some constants $a,b$ satisfy $\sum_{i=1}^m c_i\leq am+b$ for every such [sequence](sequence-and-series.md#sequence) of length $m$. The cost model and allowed operations are part of the claim; [Big O notation](real-analysis.md#big-o-notation) alone does not specify them.

- A worst-case bound for one operation limits its cost in any reachable state. Summing these separate maxima can overestimate the cost of a whole [sequence](sequence-and-series.md#sequence) because expensive states may take many cheap operations to rebuild.
- An [amortized analysis](#amortized-analysis) limits the total over every allowed [sequence](sequence-and-series.md#sequence), including an unfavourably chosen one. Dividing that bound by the number of operations is a deterministic guarantee about the [sequence](sequence-and-series.md#sequence).
- A probabilistic average-case analysis bounds an [expected value](expected-value.md) under a stated [probability distribution](probability-distribution.md) on [inputs](#input-computer-science). For a [randomized algorithm](algorithm.md#randomized-algorithm), an [expected value](expected-value.md) can instead average over its random choices. Neither interpretation is required by a deterministic [amortized analysis](#amortized-analysis).

This distinction, and the credit and [potential method](#potential-method) viewpoints, are developed in [R. Endre Tarjan](computer-science.md#robert-tarjan)'s 1985 paper [Amortized Computational Complexity](https://epubs.siam.org/doi/10.1137/0606031), sections 1–2, pp. 306–308. The [dynamic array doubling](#dynamic-array-doubling) example below shows how an expensive operation can pay for itself through the cheap operations that precede it.

###### Dynamic array doubling

↑ **Parent:** [Amortized analysis](#amortized-analysis)

Consider a [dynamic array](data-structure.md#dynamic-array) holding fixed-size entries. Its size $n$ is the number of occupied slots and its capacity $C$ is the number of allocated slots. Start with $n=0$, $C=1$. The only operation is append: if $n=C$, allocate a new [array](data-structure.md#array-data-structure) of capacity $2C$, copy the $C$ existing entries, and release the old [array](data-structure.md#array-data-structure); then write the new entry and increase $n$ by one. There is no reserve operation, deletion or shrinking in this model.

Count one unit for writing the new entry and one unit per existing entry copied during resizing. Thus the $i$th append has actual cost $c_i=1$ without resizing and $c_i=C+1$ when the old capacity $C$ is full. Copying an entry, including its read and write, is one counted action. Allocation, deallocation, index [arithmetic operations](numerical-analysis.md#arithmetic-operation) and the initial one-slot allocation are outside this exact count. If these add only a constant per ordinary append and a linear cost per resize, the [Big O notation](real-analysis.md#big-o-notation) conclusions still hold, with different constants; costly entry copies require their own cost model.

The first ten costs are $1,2,3,1,5,1,1,1,9,1$. For example, append $9$ copies eight entries and writes one, so $c_9=9$. At that point the capacity becomes $16$, but the total cost of all nine appends is only $24$.

For $n\geq1$, the final capacity is $C_n=2^{\lceil\log_2 n\rceil}$. Every earlier capacity $1,2,4,\ldots,C_n/2$ was copied once. This [geometric series](sequence-and-series.md#geometric-series) sums to $C_n-1$, including the empty sum when $n=1$. Therefore [aggregate analysis](#aggregate-analysis) gives the exact total

$$
T(0)=0,\qquad T(n)=\sum_{i=1}^n c_i=n+C_n-1,\qquad n\leq C_n<2n\quad(n\geq1).
$$

Consequently $T(n)<3n$, so append has amortized $O(1)$ cost in [Big O notation](real-analysis.md#big-o-notation) for every prefix from this empty initial state. The values being appended do not affect the count. In contrast, an append to a full [dynamic array](data-structure.md#dynamic-array) with $n$ entries costs $n+1$: its worst-case cost is $O(n)$, and actually grows linearly along full-capacity states. A bound on total work does not promise a constant response time for each call.

<a id="image-individual-append-costs-and-cumulative-work-under-dynamic-array-doubling"></a>
![](amortized-analysis-doubling-costs.png)

**[Figure 5](#image-individual-append-costs-and-cumulative-work-under-dynamic-array-doubling). Individual append costs and cumulative work under dynamic array doubling**. The spikes include every copied entry and the new write. At append 33 the actual cost is 33; at append 64 the total cost is 127. Every prefix lies below the line $3n$.

The same policy controls [computer memory](computer-science.md#computer-memory): after each completed append, $n\leq C_n<2n$ for $n\geq1$, so fewer than $n$ slots are unused. This is a bound on the retained backing [array](data-structure.md#array-data-structure), with fixed-size slots. During a resize from full capacity $k$ to $2k$, a copying implementation can temporarily hold both [arrays](data-structure.md#array-data-structure), totalling $3k$ allocated slots before releasing the old one. Thus the retained-capacity bound does not bound this temporary peak by twice the live size. Allocator metadata and separately allocated objects are additional [computer memory](computer-science.md#computer-memory) costs.

The [geometric series](sequence-and-series.md#geometric-series) is the source of the efficiency. If capacity instead increases by one each time, the same count becomes $n+1+2+\cdots+(n-1)=n(n+1)/2$, a quadratic total. [Dynamic array doubling](#dynamic-array-doubling) buys a linear total with bounded spare capacity, even when the final length is unknown.

###### Potential method

↑ **Parent:** [Amortized analysis](#amortized-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Potential_method)

The [potential method](#potential-method) assigns a number $\Phi(D)$ to each state $D$ of a [data structure](data-structure.md). Let $D_i$ be the state after operation $i$, $\Phi_i=\Phi(D_i)$, and $c_i$ its actual cost. Its [amortized cost](#amortized-cost) is the actual cost plus the change in potential. Summing and cancelling adjacent potentials gives a [telescoping sum](arithmetic.md#telescoping-sum):

$$
\widehat c_i=c_i+\Phi_i-\Phi_{i-1},\qquad
\sum_{i=1}^m c_i=\sum_{i=1}^m\widehat c_i+\Phi_0-\Phi_m.
$$

If $\Phi_0=0$ and every reachable $\Phi_i\geq0$, the sum of [amortized costs](#amortized-cost) bounds the actual total for every prefix. A nonzero initial potential contributes the explicit additive term $\Phi_0$. Potential is proof bookkeeping; the [algorithm](algorithm.md) need not store it.[CS 312 at Cornell University; CS 312, lecture 20, “Amortized analysis”: definition of amortized time and cancellation of successive potential changes](computer-science-bibliography.md#cs-312-at-cornell-university/lecture-20-hash-tables-and-amortized-analysis)

For [dynamic array doubling](#dynamic-array-doubling), choose

$$
\Phi(n,C)=\max(0,2n-C).
$$

The [potential method](#potential-method) now starts at $\Phi(0,1)=0$. After every nonempty reachable state, $C<2n$, so the maximum equals $2n-C$. There are just three cases for append:

- First append: $(0,1)$ becomes $(1,1)$, so $c_1=1$ and $\widehat c_1=1+(1-0)=2$.
- Later append without resizing: $C$ stays fixed and $n$ increases by one, so $\Delta\Phi=2$ and $\widehat c_i=1+2=3$.
- Append to a full capacity $k$: $(k,k)$ becomes $(k+1,2k)$, so the potential changes from $k$ to $2$. Hence $\widehat c_i=(k+1)+(2-k)=3$, including the resize from capacity one to two.

For every $n\geq1$, the total charge is $2+3(n-1)=3n-1$, and the [telescoping sum](arithmetic.md#telescoping-sum) proves

$$
T(n)=3n-1-\Phi(n,C_n)\leq3n-1.
$$

This agrees exactly with $T(n)=n+C_n-1$. The unmodified choice $2n-C$ has initial value $-1$, so calling it nonnegative at the empty state would be incorrect. It also works if that initial constant is retained in the identity; alternatively, $2n-C+1$ starts at zero and is nonnegative on these reachable states. The maximum above keeps a literal nonnegative credit balance from the beginning. The proof covers append alone; allowing reserve or arbitrary deletion changes the reachable states and requires a new argument.

<a id="image-the-potential-method-as-a-credit-ledger-for-dynamic-array-doubling"></a>
![](amortized-analysis-potential-ledger.png)

**[Figure 6](#image-the-potential-method-as-a-credit-ledger-for-dynamic-array-doubling). The potential method as a credit ledger for dynamic array doubling**. Each row satisfies $\widehat c_i=c_i+\Delta\Phi_i$. Before append 9 there are eight credits; its charge of three and actual cost of nine leave two. Credits pay for counted work and do not represent spare [computer memory](computer-science.md#computer-memory) slots.

###### Amortized cost

↑ **Parent:** [Potential method](#potential-method)

In the [potential method](#potential-method), an operation's [amortized cost](#amortized-cost) is $\widehat c_i=c_i+\Phi_i-\Phi_{i-1}$. It can exceed or fall below its actual cost $c_i$. The endpoint potentials determine how the total charge compares with the total actual cost.

###### Aggregate analysis

↑ **Parent:** [Amortized analysis](#amortized-analysis)

[Aggregate analysis](#aggregate-analysis) bounds the total cost of a whole [sequence](sequence-and-series.md#sequence) directly, then divides by its length to obtain an amortized bound. Summing the copied capacities as a [geometric series](sequence-and-series.md#geometric-series) in [dynamic array doubling](#dynamic-array-doubling) is an example.

###### Accounting method

↑ **Parent:** [Amortized analysis](#amortized-analysis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Accounting_method)

The [accounting method](#accounting-method) charges operations enough to pay for their work and save credits for later work. A nonnegative balance from an initially empty account makes every prefix's total charge an upper bound on its actual cost. Choosing the balance to be $\Phi$ gives the [potential method](#potential-method); the ledger for [dynamic array doubling](#dynamic-array-doubling) illustrates this equivalence.[Robert Endre Tarjan, Amortized Computational Complexity, section 2, pp. 307–308: banker's credits and equivalence with the potential viewpoint](https://www.math.u-szeged.hu/~hajnal/courses/MSc_AlgoBony/2021/Tarjan.pdf)

// Destination: computer-science.bigb

##### Polynomial time

↑ **Parent:** [Time complexity](#time-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_time)

An algorithm runs in polynomial time when its running time is at most $O(n^k)$ for some constant $k$, where $n$ is the input length.

###### Polynomial-time algorithm

↑ **Parent:** [Polynomial time](#polynomial-time)

An algorithm runs in polynomial time if its worst-case running time is bounded by a fixed polynomial in the input length. Arithmetic with fixed-degree algebraic numbers also needs polynomial bit cost when used in such a guarantee. The [Edmonds–Karp algorithm](flow-network.md#edmonds-karp-algorithm) and the [method of conditional probabilities](algorithm.md#method-of-conditional-probabilities) with efficiently computable [clause](#clause-of-a-boolean-formula) expectations are examples.

###### P (complexity)

↑ **Parent:** [Polynomial time](#polynomial-time)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P_(complexity))

$\mathbf P$ is the class of [decision problems](#decision-problem) decidable by a [deterministic computation](#deterministic-computation) in [polynomial time](#polynomial-time).

###### P-completeness

↑ **Parent:** [P (complexity)](#p-complexity)

A language in [P](#p-complexity) to which every P language has a [logspace many-one reduction](#logspace-many-one-reduction). The reduction strength matters: using arbitrary polynomial-time reductions instead would make completeness trivial for nontrivial P decision problems.

###### NP (complexity)

↑ **Parent:** [Polynomial time](#polynomial-time)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NP_(complexity))

$\mathbf{NP}$ is the class of [decision problems](#decision-problem) whose positive instances have polynomial-length [certificates](#certificate-complexity) verifiable in [polynomial time](#polynomial-time). Equivalently, it is polynomial time on a [nondeterministic computation](#nondeterministic-turing-machine).

###### Certificate (complexity)

↑ **Parent:** [NP (complexity)](#np-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Certificate_(complexity))

A certificate for a positive instance is a polynomial-length string that makes a polynomial-time verifier accept that instance.

#### Space complexity

↑ **Parent:** [Complexity class](#complexity-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Space_complexity)

The space complexity of an algorithm bounds the amount of working memory it uses as a function of input length.

##### Constant space

↑ **Parent:** [Space complexity](#space-complexity)

##### Polynomial space

↑ **Parent:** [Space complexity](#space-complexity)

An algorithm uses polynomial space if its working memory is bounded by a fixed polynomial in the input length. Exponentially many possibilities can still be searched when each candidate and the search counter need polynomial space and storage is reused. The decision problems with deterministic polynomial-space algorithms form [PSPACE](#pspace).

##### Nondeterministic space complexity class

↑ **Parent:** [Space complexity](#space-complexity)

Languages accepted by [Nondeterministic Turing machines](#nondeterministic-turing-machine) using $O(s(n))$ work space on every computation path, with acceptance defined by existence of an accepting path. Bounded-space loops do not prevent the reachability interpretation in the finite [configuration graph](#configuration-graph).

<h6 id="savitch-s-theorem">Savitch's theorem</h6>

↑ **Parent:** [Nondeterministic space complexity class](#nondeterministic-space-complexity-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Savitch's_theorem)

Reachability within $2^k$ steps can be tested by enumerating a midpoint and recursively testing two half-paths. Configurations have $O(s)$ bits and recursion depth $O(s)$, yielding deterministic space $O(s^2)$. The [space-bound discovery by exit reachability](#space-bound-discovery-by-exit-reachability) permits this simulation without assuming that the supplied function $s$ is constructible.

###### Space-bound discovery by exit reachability

↑ **Parent:** [Savitch's theorem](#savitch-s-theorem)

For a bounded-space machine, start with a logarithmic work budget and test accepting reachability and reachability of a transition leaving the budget. Accept if acceptance is found, double the budget if an exit is reachable, and otherwise reject. If all paths use at most $Cs(n)$ space, doubling stops at $O(s(n))$. Each budget test uses the [Savitch theorem](#savitch-s-theorem) recursion and the storage is reused. The method discovers a sufficient bound without computing $s(n)$.

##### Deterministic space complexity class

↑ **Parent:** [Space complexity](#space-complexity)

Languages decidable by deterministic [Turing machines](#turing-machine) using $O(s(n))$ work-tape cells with a read-only input. Input-head addresses take $O(\log n)$ bits, while the input itself is not charged to work space. The definition does not require the bound to be computed by the deciding machine.

###### PSPACE

↑ **Parent:** [Deterministic space complexity class](#deterministic-space-complexity-class)

PSPACE consists of decision problems solvable using a polynomial amount of work space. Running time may be exponential. Enumerating all polynomial-length relation encodings and reusing working storage preserves this bound, as does complementation. In particular fixed-sentence [second-order logic](mathematical-logic.md#second-order-logic) model checking lies in PSPACE.

##### Polynomial-register real-arithmetic computation

↑ **Parent:** [Space complexity](#space-complexity)

A [polynomial-register real-arithmetic computation](#polynomial-register-real-arithmetic-computation) stores polynomially many real numbers and may use arbitrarily many additions, subtractions and multiplications, with comparison tests for decisions. Register count does not bound precision or time. Fixed gate constants or sufficiently accurate computable approximations must be specified. This resource model is distinct from ordinary bit-cost computation.

##### Logarithmic space

↑ **Parent:** [Space complexity](#space-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_space)

A logarithmic-space computation uses $O(\!\log n)$ work-tape cells on inputs of length $n$.

###### L (complexity)

↑ **Parent:** [Logarithmic space](#logarithmic-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/L_(complexity))

$\mathbf L$ consists of decision problems solvable by a deterministic [logarithmic space](#logarithmic-space) computation.

###### NL (complexity)

↑ **Parent:** [Logarithmic space](#logarithmic-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NL_(complexity))

$\mathbf{NL}$ consists of decision problems solvable by a nondeterministic [logarithmic space](#logarithmic-space) computation.

###### NL-complete

↑ **Parent:** [NL (complexity)](#nl-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NL-complete)

A decision problem is NL-complete when it belongs to [NL](#nl-complexity) and every problem in NL reduces to it by a deterministic logarithmic-space many-one reduction.

###### Directed cycle detection

↑ **Parent:** [NL-complete](#nl-complete)

Decide whether a [directed graph](graph-theory.md#directed-graph) has a nonempty directed cycle; self-loops count. This problem is [NL-complete](#nl-complete). Membership guesses a returning walk of at most the vertex count. For hardness, layer a reachability instance into $N+1$ layers with wait arcs, then add only the backward edge from the target in the last layer to the source in the first. The otherwise acyclic layering has a cycle exactly when the original target is reachable. Zero-length paths must not be treated as cycles.

###### ST-connectivity

↑ **Parent:** [NL-complete](#nl-complete)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ST-connectivity)

The directed graph reachability problem asks whether a directed graph contains a directed path from a specified vertex $s$ to a specified vertex $t$. It is NL-complete.

###### Configuration graph

↑ **Parent:** [ST-connectivity](#st-connectivity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Configuration_graph)

The configuration graph of a machine on a fixed input has one vertex for each machine configuration and a directed edge for each valid computation step.

###### co-NL

↑ **Parent:** [NL (complexity)](#nl-complexity)

$\mathbf{co\text{-}NL}$ consists of complements of languages in [NL](#nl-complexity).

<h6 id="immerman-szelepcsenyi-theorem">Immerman–Szelepcsényi theorem</h6>

↑ **Parent:** [co-NL](#co-nl)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Immerman–Szelepcsényi_theorem)

The Immerman–Szelepcsényi theorem states that $\mathbf{NL}=\mathbf{co\text{-}NL}$. Its proof uses [inductive counting](#inductive-counting) of reachable configurations.

###### Inductive counting

↑ **Parent:** [Immerman–Szelepcsényi theorem](#immerman-szelepcsenyi-theorem)

Inductive counting certifies the number of vertices reachable within successively larger path-length bounds. Knowing the exact earlier count lets a logarithmic-space nondeterministic machine certify that no reachable predecessor has been omitted.

### Polynomial-time reduction

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial-time_reduction)

A polynomial-time reduction transforms instances of one computational problem into instances of another using a polynomial-time algorithm.

#### Polynomial-time many-one reduction

↑ **Parent:** [Polynomial-time reduction](#polynomial-time-reduction)

A polynomial-time many-one reduction from a [decision problem](#decision-problem) $A$ to a decision problem $B$ is a polynomial-time computable function $r$ satisfying $x\in A$ exactly when $r(x)\in B$.

##### Logspace many-one reduction

↑ **Parent:** [Polynomial-time many-one reduction](#polynomial-time-many-one-reduction)

A total mapping $f$ with $x\in A$ exactly when $f(x)\in B$, computed by a deterministic logarithmic-work-space transducer with read-only input and write-only output. Such reductions compose, and are used for [NL-completeness](#nl-complete) and [P-completeness](#p-completeness). The output can be polynomially larger than the work storage.

##### NP-hardness

↑ **Parent:** [Polynomial-time many-one reduction](#polynomial-time-many-one-reduction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NP-hardness)

A decision problem is NP-hard when every problem in [NP](#np-complexity) polynomial-time many-one reduces to it.

###### NP-completeness

↑ **Parent:** [NP-hardness](#np-hardness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NP-completeness)

A decision problem is NP-complete when it is both in [NP](#np-complexity) and [NP-hard](#np-hardness).

###### Set cover problem

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Set_cover_problem)

Given subsets $S_1,\ldots,S_m$ of a finite universe, the decision problem asks whether at most $k$ of them cover the universe. It is [NP-complete](#np-completeness). If $k<m$, existence of a cover by at most $k$ subsets is equivalent to existence of a cover by exactly $k$, by adding unused subsets. The promise that every element occurs in some subset loses no hardness: an uncovered element can be detected in polynomial time and mapped to a fixed negative instance.

// Target: mathematical-optimization.bigb

###### Set cover reduction to equilibrium support

↑ **Parent:** [Set cover problem](#set-cover-problem)

Assume $2\leq k<m$ and $\bigcup_iS_i=S$. Construct a two-player game with row $i$ for $S_i$ and columns $0,1,\ldots,n$. Column $0$ pays both players one; column $j>0$ pays $(1,0)$ when $j\in S_i$, and $(0,k/(k-1))$ otherwise. There is a [Nash equilibrium](game-theory.md#nash-equilibrium) whose row player's [support of a mixed strategy](game-theory.md#support-of-a-mixed-strategy) has size $k$ exactly when $k$ rows cover the universe. A uniform mixture on a cover makes column $0$ a [best response](game-theory.md#best-response). Conversely, if some element is uncovered by the support, the column player's [best responses](game-theory.md#best-response) are uncovered elements and the row player's current payoff is zero. The union promise provides a profitable row deviation. Without the union promise the equivalence is false: a globally uncovered element is a [best response](game-theory.md#best-response) against every row mixture.

// Target: mathematical-optimization.bigb

###### Cook-Levin theorem

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cook–Levin_theorem)

Every [NP](#np-complexity) verifier can be compiled into a polynomial-size [Boolean circuit](#boolean-circuit) whose inputs encode its [certificate](#certificate-complexity), and then into an equisatisfiable [conjunctive normal form](#conjunctive-normal-form) by a [Tseitin transformation](#tseytin-transformation). This gives a [polynomial-time many-one reduction](#polynomial-time-many-one-reduction) from every [NP](#np-complexity) language to [SAT](#boolean-satisfiability-problem). Checking a guessed assignment proves membership, so [SAT](#boolean-satisfiability-problem) is [NP-complete](#np-completeness).

###### Subset sum problem

↑ **Parent:** [NP-completeness](#np-completeness)

Given finitely encoded nonnegative integers $s_i$ and target $t$, the subset sum problem asks whether some subset sums to $t$. Taking equal item weights and profits reduces it to testing whether a [0-1 knapsack problem](mathematical-optimization.md#0-1-knapsack-problem) with capacity $t$ attains value $t$.

###### Special sum set

↑ **Parent:** [Subset sum problem](#subset-sum-problem)

A finite [set](set.md) $A$ of [positive integers](integer.md#positive-integer) such that nonempty [disjoint sets](set.md#disjoint-sets) contained in $A$ have different [sums](arithmetic.md#sum), and the larger subset has the larger [sum](arithmetic.md#sum) when their sizes differ. For $a_1<\cdots<a_n$, the size condition is equivalent to $a_1+\cdots+a_{k+1}>a_{n-k+1}+\cdots+a_n$ for $1\le k\le\lfloor(n-1)/2\rfloor$: the left side is the smallest possible sum of $k+1$ elements and the right side the largest sum of $k$ elements.

###### Boolean satisfiability problem

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_satisfiability_problem)

The [Boolean satisfiability problem](#boolean-satisfiability-problem) asks whether a [Boolean formula](#boolean-formula) has an assignment making it true. A complete assignment is a [Boolean valuation](mathematical-logic.md#boolean-valuation): it gives every [Boolean variable](#boolean-variable) a [truth value](mathematical-logic.md#truth-value), consistently at all occurrences. A [satisfying assignment](#satisfying-assignment), also called a [model of a Boolean formula](#satisfying-assignment), makes the entire [Boolean formula](#boolean-formula) true. A solver's answer `SAT` asserts that at least one [satisfying assignment](#satisfying-assignment) exists; `UNSAT` asserts that the input is an [unsatisfiable Boolean formula](#unsatisfiable-boolean-formula). These are statements about existence, rather than the [truth value](mathematical-logic.md#truth-value) under one particular [Boolean valuation](mathematical-logic.md#boolean-valuation).

For [conjunctive normal form](#conjunctive-normal-form), or [CNF](#conjunctive-normal-form), write

$$
F=C_1\land\cdots\land C_m,
\qquad C_i=\ell_{i1}\lor\cdots\lor\ell_{ik_i}.
$$

Each [Boolean literal](#boolean-literal) $\ell$ is a [Boolean variable](#boolean-variable) or its [logical negation](#negation). Each [Boolean clause](#clause-of-a-boolean-formula) uses inclusive [logical disjunction](mathematical-logic.md#logical-disjunction): one true [Boolean literal](#boolean-literal) suffices. The outer [logical conjunction](mathematical-logic.md#logical-conjunction) requires every [Boolean clause](#clause-of-a-boolean-formula) to succeed under the same [Boolean valuation](mathematical-logic.md#boolean-valuation). Choosing a different [Boolean valuation](mathematical-logic.md#boolean-valuation) for each [Boolean clause](#clause-of-a-boolean-formula) would answer a different question.

Consider the original three-[Boolean variable](#boolean-variable) example

$$
F=(x\lor y)\land(\neg x\lor z)\land(\neg y\lor\neg z),
\qquad C_1=x\lor y,\quad C_2=\neg x\lor z,\quad C_3=\neg y\lor\neg z.
$$

At the [Boolean valuation](mathematical-logic.md#boolean-valuation) $(x,y,z)=(0,1,0)$, the [Boolean literals](#boolean-literal) in $C_1$ have values $(0,1)$, those in $C_2$ have values $(1,0)$, and those in $C_3$ have values $(0,1)$. Every [Boolean clause](#clause-of-a-boolean-formula) therefore has [truth value](mathematical-logic.md#truth-value) one, so $F$ has [truth value](mathematical-logic.md#truth-value) one: this is a [satisfying assignment](#satisfying-assignment).

<a id="image-an-original-satisfying-assignment-evaluated-through-boolean-literals-three-boolean-clauses-and-their-logical-conjunction"></a>
![](satisfiability-assignment-clause-evaluation.png)

**[Figure 7](#image-an-original-satisfying-assignment-evaluated-through-boolean-literals-three-boolean-clauses-and-their-logical-conjunction). An original satisfying assignment evaluated through Boolean literals, three Boolean clauses, and their logical conjunction**.

The complete [truth table](mathematical-logic.md#truth-table) has $2^3=8$ [Boolean valuations](mathematical-logic.md#boolean-valuation). Exactly two are [satisfying assignments](#satisfying-assignment): $(0,1,0)$ and $(1,0,1)$. In particular, $(1,1,1)$ satisfies the first two [Boolean clauses](#clause-of-a-boolean-formula) but falsifies the third, so satisfying most [Boolean clauses](#clause-of-a-boolean-formula) does not suffice for [SAT](#boolean-satisfiability-problem). That different objective belongs to [maximum satisfiability](#maximum-satisfiability).

<a id="image-all-eight-boolean-valuations-of-the-original-cnf-example-with-its-two-satisfying-assignments-highlighted"></a>
![](satisfiability-eight-assignment-truth-table.png)

**[Figure 8](#image-all-eight-boolean-valuations-of-the-original-cnf-example-with-its-two-satisfying-assignments-highlighted). All eight Boolean valuations of the original CNF example, with its two satisfying assignments highlighted**.

A short proof of completeness avoids listing all eight rows. If $x=0$, the [Boolean clause](#clause-of-a-boolean-formula) $C_1$ forces $y=1$, after which $C_3$ forces $z=0$; $C_2$ is already true. If $x=1$, $C_2$ forces $z=1$, after which $C_3$ forces $y=0$; $C_1$ is already true. These two cases exhaust the [truth values](mathematical-logic.md#truth-value) of $x$ and produce precisely the two [satisfying assignments](#satisfying-assignment) above.

[Verifying a satisfying assignment](#verifying-a-satisfying-assignment) and finding a [satisfying assignment](#satisfying-assignment) are different tasks. Given a candidate, evaluate the [Boolean formula](#boolean-formula) once; finding a candidate requires choosing compatible [truth values](mathematical-logic.md#truth-value) across all its [Boolean clauses](#clause-of-a-boolean-formula). The [Cook-Levin theorem](#cook-levin-theorem) says that general [SAT](#boolean-satisfiability-problem) is [NP-complete](#np-completeness), even though a proposed [satisfying assignment](#satisfying-assignment) is efficiently checkable. Its proof encodes a bounded [nondeterministic computation](#nondeterministic-turing-machine) as a [Boolean formula](#boolean-formula) whose [satisfying assignments](#satisfying-assignment) describe accepting computations. [Stephen A. Cook](computer-science.md#stephen-a-cook)'s 1971 paper established this connection between [computational complexity theory](#computational-complexity-theory) and [propositional logic](mathematical-logic.md#propositional-logic).[The Complexity of Theorem-Proving Procedures by Stephen A. Cook, 1971, §1, Theorem 1 and proof, pp. 2–3 of the revision-3 transcription: CNF encodes accepting computations](computer-science-bibliography.md#the-complexity-of-theorem-proving-procedures-by-stephen-a-cook)

A concrete use is checking finite configuration rules. Let $x$ mean that an optional feature is enabled, $y$ that a fallback is selected, and $z$ that the feature's required component is installed. Require a feature or fallback, require the component whenever the feature is enabled, and forbid using the fallback with that component. [Logical implication](mathematical-logic.md#logical-implication) rewrites the second rule $x\to z$ as $\neg x\lor z$; [De Morgan's laws](#de-morgan-s-laws) rewrite the third rule $\neg(y\land z)$ as $\neg y\lor\neg z$. Their [logical conjunction](mathematical-logic.md#logical-conjunction) is exactly $F$, so its two [satisfying assignments](#satisfying-assignment) give the two allowed configurations. The usefulness of [SAT](#boolean-satisfiability-problem) lies in expressing local rules uniformly while demanding one globally consistent [Boolean valuation](mathematical-logic.md#boolean-valuation). The conclusion concerns exactly these encoded rules.

###### Satisfying assignment

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

A [satisfying assignment](#satisfying-assignment) is a complete [Boolean valuation](mathematical-logic.md#boolean-valuation) $v$ for which a [Boolean formula](#boolean-formula) $F$ has [truth value](mathematical-logic.md#truth-value) one, written $v\models F$. The notation describes a relation between the [Boolean valuation](mathematical-logic.md#boolean-valuation) and the [Boolean formula](#boolean-formula). For the example in [Boolean satisfiability problem](#boolean-satisfiability-problem), $(0,1,0)$ is a [model of a Boolean formula](#satisfying-assignment) $F$, whereas $(0,0,0)$ is not. [SAT](#boolean-satisfiability-problem) asks for existence of at least one [satisfying assignment](#satisfying-assignment), rather than for every [Boolean valuation](mathematical-logic.md#boolean-valuation) to work; the latter condition makes $F$ a [tautology](mathematical-logic.md#tautology).

###### Verifying a satisfying assignment

↑ **Parent:** [Satisfying assignment](#satisfying-assignment)

For a [CNF](#conjunctive-normal-form) input with $n$ [Boolean variables](#boolean-variable), $m$ [Boolean clauses](#clause-of-a-boolean-formula), and $L$ [Boolean literal](#boolean-literal) occurrences, first check that the supplied [Boolean valuation](mathematical-logic.md#boolean-valuation) gives each input [Boolean variable](#boolean-variable) exactly one [truth value](mathematical-logic.md#truth-value). Evaluate each [Boolean literal](#boolean-literal) by lookup or [logical negation](#negation), each [Boolean clause](#clause-of-a-boolean-formula) by [logical disjunction](mathematical-logic.md#logical-disjunction), and the [Boolean formula](#boolean-formula) by [logical conjunction](mathematical-logic.md#logical-conjunction). Indexed [Boolean variables](#boolean-variable) and constant-cost lookups give an $O(n+m+L)$ operation count; with a finite [binary string](#binary-string) encoding the check still takes [polynomial time](#polynomial-time). Thus a [satisfying assignment](#satisfying-assignment) is a [certificate in computational complexity](#certificate-complexity) for [SAT](#boolean-satisfiability-problem), proving that [SAT](#boolean-satisfiability-problem) belongs to [NP](#np-complexity). Finding it by exhaustive checking can require $2^n$ candidate [Boolean valuations](mathematical-logic.md#boolean-valuation); this enumeration cost is not a lower bound on every possible [SAT](#boolean-satisfiability-problem) [algorithm](algorithm.md).[CS 252, Lecture 8: Constraint Satisfaction Problems, p. 3, §3 opening paragraph: assignments as certificates and membership in NP](computer-science-bibliography.md#cs-252-lecture-8-constraint-satisfaction-problems-carnegie-mellon-university)

###### Unsatisfiable Boolean formula

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

An [unsatisfiable Boolean formula](#unsatisfiable-boolean-formula) has no [satisfying assignment](#satisfying-assignment). For

$$
G=x\land\neg x,
$$

the [Boolean valuation](mathematical-logic.md#boolean-valuation) $x=0$ falsifies the first [Boolean clause](#clause-of-a-boolean-formula), and $x=1$ falsifies the second. Both possible [truth values](mathematical-logic.md#truth-value) fail, proving `UNSAT`. Each [Boolean clause](#clause-of-a-boolean-formula) alone has a [satisfying assignment](#satisfying-assignment), but their [logical conjunction](mathematical-logic.md#logical-conjunction) does not: compatibility is the central issue. By contrast, finding just one failed [Boolean valuation](mathematical-logic.md#boolean-valuation) for a general [Boolean formula](#boolean-formula) only rejects that candidate. Finding one successful [Boolean valuation](mathematical-logic.md#boolean-valuation) proves `SAT`; proving `UNSAT` requires excluding every candidate, possibly with a compact argument rather than a full [truth table](mathematical-logic.md#truth-table).

###### Partial Boolean assignment

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

A [partial Boolean assignment](#partial-boolean-assignment) gives [truth values](mathematical-logic.md#truth-value) to some of a [Boolean formula](#boolean-formula)'s [Boolean variables](#boolean-variable). An extension is a complete [Boolean valuation](mathematical-logic.md#boolean-valuation) agreeing on the assigned [Boolean variables](#boolean-variable). In [CNF](#conjunctive-normal-form), a [Boolean clause](#clause-of-a-boolean-formula) containing a true assigned [Boolean literal](#boolean-literal) is already satisfied; a [Boolean clause](#clause-of-a-boolean-formula) whose every [Boolean literal](#boolean-literal) is assigned false rules out all extensions. A [Boolean clause](#clause-of-a-boolean-formula) with no true assigned [Boolean literal](#boolean-literal) and at least one unassigned [Boolean variable](#boolean-variable) is unresolved. An unresolved [Boolean clause](#clause-of-a-boolean-formula) need not have a compatible extension with the other [Boolean clauses](#clause-of-a-boolean-formula).

For $F$ in [Boolean satisfiability problem](#boolean-satisfiability-problem), setting $x=y=0$ already falsifies $C_1$, so both choices of $z$ can be discarded. Setting only $x=0$ leaves $C_1$ unresolved and forces $y=1$ if a [satisfying assignment](#satisfying-assignment) is to survive; then $C_3$ forces $z=0$. Branching on an unassigned [Boolean variable](#boolean-variable) into its two [truth values](mathematical-logic.md#truth-value) and discarding branches with a false [Boolean clause](#clause-of-a-boolean-formula) is sound: every [satisfying assignment](#satisfying-assignment) follows one branch and cannot extend a false [Boolean clause](#clause-of-a-boolean-formula). If all branches are eliminated, the original [Boolean formula](#boolean-formula) is an [unsatisfiable Boolean formula](#unsatisfiable-boolean-formula).

###### 2-satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/2-satisfiability)

[2-satisfiability](#2-satisfiability) restricts [SAT](#boolean-satisfiability-problem) to [CNF](#conjunctive-normal-form) in which each [Boolean clause](#clause-of-a-boolean-formula) has at most two [Boolean literals](#boolean-literal). The example in [Boolean satisfiability problem](#boolean-satisfiability-problem) is therefore a [2-SAT](#2-satisfiability) instance. Unlike general [SAT](#boolean-satisfiability-problem) and [3-SAT](#3-sat), [2-SAT](#2-satisfiability) has a [polynomial-time algorithm](#polynomial-time-algorithm); its tractability concerns finding a [satisfying assignment](#satisfying-assignment) or deciding that none exists, not merely checking a candidate. [3-SAT](#3-sat) allows up to three [Boolean literals](#boolean-literal) per [Boolean clause](#clause-of-a-boolean-formula) and is [NP-complete](#np-completeness), even though it includes many individually easy instances such as this one.[CS 252, Lecture 8: Constraint Satisfaction Problems, pp. 1–2, §2 examples 1 and 3; p. 3, §3 classification items 1 and 3](computer-science-bibliography.md#cs-252-lecture-8-constraint-satisfaction-problems-carnegie-mellon-university)

The key [logical equivalence](mathematical-logic.md#logical-equivalence) is

$$
a\lor b\equiv(\neg a\to b)\land(\neg b\to a),
$$

where $a,b$ are [Boolean literals](#boolean-literal). It expresses a two-[Boolean literal](#boolean-literal) [Boolean clause](#clause-of-a-boolean-formula) as two [logical implications](mathematical-logic.md#logical-implication). Representing these [logical implications](mathematical-logic.md#logical-implication) as edges in a [directed graph](graph-theory.md#directed-graph) gives a route to the [polynomial-time algorithm](#polynomial-time-algorithm). In the example, $C_2$ says both $x\to z$ and $\neg z\to\neg x$: enabling the feature requires its component, and an absent component excludes the feature.

###### Integer programming formulation of satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Encode each truth value by $t_k\in\{0,1\}$. A positive [Boolean literal](#boolean-literal) has value $t_k$ and its negation has value $1-t_k$. The sum of literal values in a clause is at least one exactly when that clause is true. Thus the displayed inequalities, with objective zero, express [Boolean satisfiability](#boolean-satisfiability-problem) as a binary [integer programming](mathematical-optimization.md#integer-programming) feasibility problem. For [maximum satisfiability](#maximum-satisfiability), introduce $q_i\in\{0,1\}$ with $q_i\leq\sum_{\ell\in C_i}L_\ell(t)$ and maximize $\sum_iq_i$. False clauses force zero indicators; true clauses permit indicators one, and maximization selects all of them. Hence the optimal objective equals the maximum number of true clauses.

###### Maximum satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Maximum satisfiability asks for a truth assignment maximizing the number of true clauses of a [conjunctive normal form](#conjunctive-normal-form) formula. The [Boolean satisfiability problem](#boolean-satisfiability-problem) asks whether all its clauses can be made true. Binary clause indicators give an [integer programming](mathematical-optimization.md#integer-programming) formulation, and the [literal-frequency greedy approximation for MAX-SAT](#literal-frequency-greedy-approximation-for-max-sat) guarantees at least half the optimum. Counts of clauses, rather than multiplicities of repeated literals within one clause, are relevant to this objective.

###### Literal-frequency greedy approximation for MAX-SAT

↑ **Parent:** [Maximum satisfiability](#maximum-satisfiability)

In the residual unsatisfied formula, choose a [Boolean literal](#boolean-literal) contained in the largest number $a$ of clauses and make it true. Its opposite occurs in at most $a$ clauses, since it too was an eligible literal. The step permanently satisfies $a$ clauses; only clauses containing the opposite can become empty, so it loses at most $a$ clauses. Delete satisfied clauses and false literals and repeat. No satisfied clause or newly empty clause is counted twice. Summing gives total lost nonempty clauses at most total satisfied clauses $G$. All initially nonempty clauses are eventually in one of these classes, so $G\geq N_+/2\geq\operatorname{OPT}/2$. Initial empty clauses can never be satisfied and are excluded from $N_+$. This proves the [approximation algorithm](mathematical-optimization.md#approximation-algorithm) guarantee even with tautological clauses or repeated literals.

###### 2UN-SAT

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Satisfiability of [conjunctive normal form](#conjunctive-normal-form) formulas whose [clauses](#clause-of-a-boolean-formula) have at most two unnegated variables. It is [NP-complete](#np-completeness): binary AND/OR and unary NOT gate equivalences in a [Tseitin transformation](#tseytin-transformation) already satisfy that restriction. [Clauses](#clause-of-a-boolean-formula) may contain arbitrarily many negative [literals](#boolean-literal); the total [clause](#clause-of-a-boolean-formula) width is not restricted to two.

###### Maximum 2-satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Maximum 2-satisfiability asks for an assignment satisfying as many [clause](#clause-of-a-boolean-formula) occurrences as possible when every nonempty [clause](#clause-of-a-boolean-formula) has at most two [literals](#boolean-literal). Occurrences are counted even when a [clause](#clause-of-a-boolean-formula) is repeated. Its decision problem is [NP-complete](#np-completeness) by the [seven-clause gadget for MAX-2SAT](#seven-clause-gadget-for-max-2sat), while the [method of conditional probabilities](algorithm.md#method-of-conditional-probabilities) gives a polynomial-time half approximation.

###### Golden ratio approximation for MAX-2SAT

↑ **Parent:** [Maximum 2-satisfiability](#maximum-2-satisfiability)

When each variable appears in at most one normalized singleton [clause](#clause-of-a-boolean-formula), satisfy that favored [literal](#boolean-literal) with [probability](probability-theory.md#probability) $p>1/2$ and choose independent variables. Every proper binary [clause](#clause-of-a-boolean-formula) is then satisfied with [probability](probability-theory.md#probability) at least $1-p^2$, and every singleton with [probability](probability-theory.md#probability) $p$. Maximize the common lower bound by $p=1-p^2$, giving the reciprocal of the [golden ratio](algebra.md#golden-ratio). The [method of conditional probabilities](algorithm.md#method-of-conditional-probabilities) derandomizes the construction, obtaining [approximation ratio](mathematical-optimization.md#approximation-ratio) $p$. Tautologies are harmless; the singleton restriction must be applied after removing repeated [literals](#boolean-literal) within [clauses](#clause-of-a-boolean-formula).

###### Seven-clause gadget for MAX-2SAT

↑ **Parent:** [Maximum 2-satisfiability](#maximum-2-satisfiability)

A three-[literal](#boolean-literal) disjunction can be represented by ten unit or two-[literal](#boolean-literal) [clause](#clause-of-a-boolean-formula) occurrences with one fresh auxiliary variable. If the number $r$ of true input [literals](#boolean-literal) is zero, the best auxiliary choice satisfies six; for $r=1,2,3$, the best count is seven. Applying separate gadgets to all [clauses](#clause-of-a-boolean-formula) of a [3-SAT](#3-sat) instance gives target seven times the original [clause](#clause-of-a-boolean-formula) count, proving [NP-completeness](#np-completeness) of the decision form of [MAX-2SAT](#maximum-2-satisfiability). The local counting argument is essential: no gadget may exceed seven and compensate for an unsatisfied input [clause](#clause-of-a-boolean-formula).

###### Boolean formula

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

A [Boolean formula](#boolean-formula) is a finite expression built from [Boolean variables](#boolean-variable) and [Boolean operations](#boolean-operation), equivalently a [propositional formula](mathematical-logic.md#propositional-formula) with two-valued semantics. A [Boolean valuation](mathematical-logic.md#boolean-valuation) determines its [truth value](mathematical-logic.md#truth-value). In $(x\lor y)\land\neg x$, [logical negation](#negation) acts only on $x$, and the outer [logical conjunction](mathematical-logic.md#logical-conjunction) combines $x\lor y$ with $\neg x$. Occurrences of the same [Boolean variable](#boolean-variable) share one [truth value](mathematical-logic.md#truth-value). The [Boolean satisfiability problem](#boolean-satisfiability-problem) asks whether some [Boolean valuation](mathematical-logic.md#boolean-valuation) makes the [Boolean formula](#boolean-formula) true.

###### Disjunctive normal form

↑ **Parent:** [Boolean formula](#boolean-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disjunctive_normal_form)

A [Boolean formula](#boolean-formula) is in disjunctive normal form when it is a disjunction of conjunctions of [Boolean literals](#boolean-literal). Width bounds the number of literals in each conjunction, not the number of conjunctions. A depth-$s$ [decision tree](#decision-tree) gives such a formula of width at most $s$ by taking the disjunction of its accepting leaf conditions; rejecting leaves give the dual [conjunctive normal form](#conjunctive-normal-form).

###### Conjunctive normal form

↑ **Parent:** [Boolean formula](#boolean-formula)

A [Boolean formula](#boolean-formula) is in [conjunctive normal form](#conjunctive-normal-form) when it is a [logical conjunction](mathematical-logic.md#logical-conjunction) of [Boolean clauses](#clause-of-a-boolean-formula). It is true precisely when every [Boolean clause](#clause-of-a-boolean-formula) is true under the same [Boolean valuation](mathematical-logic.md#boolean-valuation); an empty [logical conjunction](mathematical-logic.md#logical-conjunction) is true. For example, $(x\lor\neg y)\land(z)$ has two [Boolean clauses](#clause-of-a-boolean-formula) with widths two and one. Width counts [Boolean literal](#boolean-literal) occurrences within a [Boolean clause](#clause-of-a-boolean-formula), whereas the [Boolean clause](#clause-of-a-boolean-formula) count counts the conjuncts. [2-SAT](#2-satisfiability) bounds width by two, and [3-SAT](#3-sat) bounds width by three. A [Boolean formula](#boolean-formula) with an empty [Boolean clause](#clause-of-a-boolean-formula) is an [unsatisfiable Boolean formula](#unsatisfiable-boolean-formula).

###### Tseytin transformation

↑ **Parent:** [Conjunctive normal form](#conjunctive-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tseytin_transformation)

Introduce a [Boolean variable](#boolean-variable) for each gate output and impose its equivalence to the gate's input function with a constant number of [clauses](#clause-of-a-boolean-formula). A final unit [clause](#clause-of-a-boolean-formula) forces acceptance. For a bounded-fan-in [Boolean circuit](#boolean-circuit), the formula size is linear in the gate count and it is satisfiable exactly when some input makes the [Boolean circuit](#boolean-circuit) output one. Auxiliary variables extend the satisfying assignments; this is equisatisfiability, not equality as functions of the enlarged variable set.

###### Clause of a Boolean formula

↑ **Parent:** [Boolean formula](#boolean-formula)

A [Boolean clause](#clause-of-a-boolean-formula) is an expression $\ell_1\lor\cdots\lor\ell_k$ formed from [Boolean literals](#boolean-literal), true when at least one [Boolean literal](#boolean-literal) is true. The empty [Boolean clause](#clause-of-a-boolean-formula) is false. Repeating a [Boolean literal](#boolean-literal) does not change the [truth value](mathematical-logic.md#truth-value). A [CNF](#conjunctive-normal-form) [Boolean formula](#boolean-formula) is a [logical conjunction](mathematical-logic.md#logical-conjunction) of these [Boolean clauses](#clause-of-a-boolean-formula).

For $(\neg x\lor z)$, the only failing pair is $(x,z)=(1,0)$: its two [Boolean literals](#boolean-literal) then both have [truth value](mathematical-logic.md#truth-value) zero. The one-[Boolean literal](#boolean-literal) [Boolean clause](#clause-of-a-boolean-formula) $(x)$ requires $x=1$. A [Boolean clause](#clause-of-a-boolean-formula) containing both $x$ and $\neg x$ is a [tautology](mathematical-logic.md#tautology), since one of those [Boolean literals](#boolean-literal) is true under every [Boolean valuation](mathematical-logic.md#boolean-valuation). These observations separate [Boolean clause](#clause-of-a-boolean-formula) satisfaction from the simultaneous satisfaction required by [SAT](#boolean-satisfiability-problem).

###### Boolean literal

↑ **Parent:** [Boolean formula](#boolean-formula)

A [Boolean literal](#boolean-literal) is a [Boolean variable](#boolean-variable) $u$ or its [logical negation](#negation) $\neg u$. The two [Boolean literals](#boolean-literal) have opposite [truth values](mathematical-logic.md#truth-value): a [Boolean valuation](mathematical-logic.md#boolean-valuation) $v$ gives $v(\neg u)=1-v(u)$ when false and true are encoded as zero and one. Thus $u=0$ makes the positive [Boolean literal](#boolean-literal) $u$ false and the negative [Boolean literal](#boolean-literal) $\neg u$ true. A [Boolean clause](#clause-of-a-boolean-formula) combines [Boolean literals](#boolean-literal), and a [Boolean-pair colouring gadget](graph-coloring.md#boolean-pair-colouring-gadget) represents a [Boolean variable](#boolean-variable) and its [logical negation](#negation) by two [vertices](graph.md#vertex-graph-theory) with opposite Boolean colours.

###### Boolean variable

↑ **Parent:** [Boolean formula](#boolean-formula)

A [Boolean variable](#boolean-variable) takes one of two [truth values](mathematical-logic.md#truth-value), false or true, encoded as zero or one. It is an input to a [Boolean formula](#boolean-formula); a [Boolean literal](#boolean-literal) uses the [Boolean variable](#boolean-variable) either positively or with [logical negation](#negation). A [Boolean valuation](mathematical-logic.md#boolean-valuation) assigns one [truth value](mathematical-logic.md#truth-value) to each distinct [Boolean variable](#boolean-variable), so three distinct [Boolean variables](#boolean-variable) give eight possible complete assignments regardless of how often each appears.

###### 3-SAT

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

3-SAT is the [Boolean satisfiability problem](#boolean-satisfiability-problem) restricted to [Boolean formulas](#boolean-formula) in [conjunctive normal form](#conjunctive-normal-form) with at most three [Boolean literals](#boolean-literal) per [Boolean clause](#clause-of-a-boolean-formula). It is [NP-complete](#np-completeness). A nonempty short [Boolean clause](#clause-of-a-boolean-formula) can be padded to three positions by repeating a [Boolean literal](#boolean-literal), without changing satisfiability.

###### Horn clause

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horn_clause)

A Horn clause is a disjunction of literals containing at most one positive literal. It can be read as an implication whose antecedent is a conjunction of variables.

###### Horn-SAT

↑ **Parent:** [Horn clause](#horn-clause)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horn-SAT)

Horn-SAT asks whether a conjunction of [Horn clauses](#horn-clause) is satisfiable.

###### Horn-SAT forward-chaining algorithm

↑ **Parent:** [Horn-SAT](#horn-sat)

The Horn-SAT forward-chaining algorithm starts with every variable false and repeatedly makes the conclusion of any enabled implication true. It reports failure if it enables a clause with no positive conclusion; otherwise the fixed point is the least satisfying assignment.

###### Quadratic-equation satisfiability over F2

↑ **Parent:** [NP-completeness](#np-completeness)

Quadratic-equation satisfiability over $\mathbb F_2$ asks whether a finite system of polynomial equations of degree at most two over the [finite field](algebra.md#finite-field) $\mathbb F_2$ has a common solution.

<h6 id="ladner-s-theorem">Ladner's theorem</h6>

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ladner's_theorem)

If $\mathbf P\ne\mathbf{NP}$, then [NP](#np-complexity) contains a decision problem that is neither in [P](#p-complexity) nor [NP-complete](#np-completeness).

### Circuit complexity

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circuit_complexity)

Circuit complexity studies the size and depth of circuits computing finite-input functions.

#### NC1

↑ **Parent:** [Circuit complexity](#circuit-complexity)

Languages computable by polynomial-size [Boolean circuit](#boolean-circuit) families of bounded fan-in and depth $O(\log n)$. One can specify the nonuniform or logspace-uniform convention explicitly. Balanced constant-size operations give examples such as the [MOD3 binary divisibility problem](#mod3-binary-divisibility-problem) without nonuniform advice.

##### MOD3 binary divisibility problem

↑ **Parent:** [NC1](#nc1)

For a binary numeral, its remainder is the sum of its bits weighted alternately by $+1$ and $-1$ from the least significant position. A [balanced finite-monoid reduction circuit](#balanced-finite-monoid-reduction-circuit) adds these residues modulo three in two-bit encodings. A final zero test gives a uniform linear-size logarithmic-depth [Boolean circuit](#boolean-circuit), proving membership in [NC1](#nc1).

##### Balanced finite-monoid reduction circuit

↑ **Parent:** [NC1](#nc1)

A fixed finite [monoid](algebraic-operation.md#monoid) operation has a constant-size Boolean truth-table [Boolean circuit](#boolean-circuit) on its constant-bit encodings. Reduce $n$ elements in a balanced binary tree to get linear size and logarithmic depth. Associativity ensures that tree grouping does not change the product. [MOD3](#mod3-binary-divisibility-problem) uses addition in the three-element residue group, with input-position signs handled at the leaves.

#### Boolean circuit

↑ **Parent:** [Circuit complexity](#circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_circuit)

A Boolean circuit is a finite directed acyclic graph of [Boolean gates](#boolean-operation) with designated inputs and outputs.

##### Circuit size

↑ **Parent:** [Boolean circuit](#boolean-circuit)

The size of a [Boolean circuit](#boolean-circuit) counts its gates, or in another common convention its wires. The convention must be fixed when stating quantitative bounds. In switching arguments, new clauses created from a [decision tree](#decision-tree) are not separate original gates to be charged in the failure union bound.

##### Depth of a Boolean circuit

↑ **Parent:** [Boolean circuit](#boolean-circuit)

Circuit depth is the largest number of counted gates on any input-to-output path in the [Boolean circuit](#boolean-circuit). For an AND/OR circuit with negations on input literals, only the AND/OR gates are counted. This convention makes the restriction argument for the [Linial-Mansour-Nisan theorem](computer-science.md#linial-mansour-nisan-theorem) precise.

##### Circuit value problem

↑ **Parent:** [Boolean circuit](#boolean-circuit)

Given a finite acyclic [Boolean circuit](#boolean-circuit) and its input assignment, determine the output bit. Topological gate evaluation places the problem in [P](#p-complexity); it is a standard [P-complete](#p-completeness) problem under [logspace many-one reductions](#logspace-many-one-reduction). [Boolean circuit](#boolean-circuit) evaluation is different from [Circuit satisfiability problem](#circuit-satisfiability-problem), which asks whether some assignment succeeds.

###### AND-NOT circuit value problem

↑ **Parent:** [Circuit value problem](#circuit-value-problem)

The [circuit value problem](#circuit-value-problem) restricted to AND and NOT gates remains [P-complete](#p-completeness). Replace each OR by $\neg(\neg x\wedge\neg y)$, using a constant-size gadget. Gate indices and gadget positions can be emitted in [logarithmic space](#logarithmic-space), and assignments are preserved. Constants, when needed, can be represented by fixed-valued input nodes.

##### Circuit satisfiability problem

↑ **Parent:** [Boolean circuit](#boolean-circuit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circuit_satisfiability_problem)

The circuit satisfiability problem asks whether a [Boolean circuit](#boolean-circuit) has an input on which its designated output is one. It is [NP-complete](#np-completeness).

##### Threshold function

↑ **Parent:** [Boolean circuit](#boolean-circuit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Threshold_function)

A threshold Boolean function outputs one exactly when a weighted sum of its input bits reaches a specified threshold. The unweighted threshold function $f_{n,r}$ tests whether at least $r$ of its $n$ inputs are one.

###### Majority function

↑ **Parent:** [Threshold function](#threshold-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Majority_function)

A majority [Boolean function](analysis-of-boolean-functions.md#boolean-function) outputs one when more than half its input bits are one. An odd number of inputs avoids a tie convention. For three bits its unique [multilinear polynomial](polynomial.md#multilinear-polynomial) is $x_1x_2+x_1x_3+x_2x_3-2x_1x_2x_3$, so the [polynomial method for quantum query lower bounds](#polynomial-method-for-quantum-query-lower-bounds) requires at least two exact queries.

###### Block conjunction of three-bit majorities

↑ **Parent:** [Majority function](#majority-function)

Its $n$ disjoint triples give a product of degree-three [multilinear polynomials](polynomial.md#multilinear-polynomial), with all-variable coefficient $(-2)^n$. Hence its degree is $3n$ and its [exact quantum query complexity](#exact-quantum-query-complexity) is at least $\lceil3n/2\rceil$. At the input consisting of repeated $110$ triples, each of the $2n$ one bits is a disjoint sensitive singleton. Thus [block sensitivity](analysis-of-boolean-functions.md#block-sensitivity) is at least $2n$, implying a bounded-error [quantum query complexity](#quantum-query-complexity) lower bound $\Omega(\sqrt n)$.

##### Dual Boolean function

↑ **Parent:** [Boolean circuit](#boolean-circuit)

The dual of a Boolean function $f$ is $f^*(x)=\neg f(\neg x)$. Swapping AND with OR and zero with one in a monotone circuit for $f$ produces a circuit for $f^*$ by [De Morgan's laws](#de-morgan-s-laws).

#### Circuit family

↑ **Parent:** [Circuit complexity](#circuit-complexity)

A circuit family $(C_n)$ contains one circuit for each input length $n$. The circuit for one length may be chosen independently of those for other lengths, so a family is a nonuniform model of computation.

##### Circuit size class

↑ **Parent:** [Circuit family](#circuit-family)

The languages whose length-$n$ [indicator functions](measure-theory.md#indicator-function) have [Boolean circuits](#boolean-circuit) with at most $T(n)$ gates for sufficiently large $n$, over a fixed bounded-fan-in complete basis. The family need not be constructible by one algorithm. Polynomial-size bounds give [P/poly](#p-poly); the [truth-table upper bound for circuit size](#truth-table-upper-bound-for-circuit-size) applies even to [undecidable](computability-theory.md#undecidable-decision-problem) languages.

###### Truth-table upper bound for circuit size

↑ **Parent:** [Circuit size class](#circuit-size-class)

OR together one minterm for each accepted length-$n$ input. Each minterm is an AND of the appropriate [Boolean literals](#boolean-literal). There are at most $2^n$ minterms, and their negated input wires can be shared, giving $O(n2^n)$ bounded-fan-in gates. This is a nonuniform existence statement, not an algorithm for determining an [undecidable](computability-theory.md#undecidable-decision-problem) truth table.

##### Polynomial-size circuit family

↑ **Parent:** [Circuit family](#circuit-family)

A circuit family has polynomial size when $C_n$ has at most $n^{O(1)}$ gates.

###### Undecidable unary languages with linear-size circuits

↑ **Parent:** [Polynomial-size circuit family](#polynomial-size-circuit-family)

For any set of lengths $A$, choose at length $n$ a constant-zero [Boolean circuit](#boolean-circuit) when $n\notin A$, and an AND of all inputs when $n\in A$. This uses $O(n+1)$ gates. If $A$ is [undecidable](computability-theory.md#undecidable-decision-problem), so is $U_A$, yet it belongs to [P/poly](#p-poly). Since all [NP](#np-complexity) languages are decidable by certificate enumeration, this proves [P/poly](#p-poly) is not equal to [NP](#np-complexity); it does not resolve containment in the other direction.

<h6 id="p-poly">P/poly</h6>

↑ **Parent:** [Polynomial-size circuit family](#polynomial-size-circuit-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P/poly)

$\mathbf P/\mathrm{poly}$ is the class of [decision problems](#decision-problem) decided by [polynomial-size circuit families](#polynomial-size-circuit-family).

#### Constant-depth circuit complexity

↑ **Parent:** [Circuit complexity](#circuit-complexity)

Constant-depth circuit complexity studies circuit families whose depth is bounded independently of the input length.

<h5 id="hastad-switching-lemma">Håstad switching lemma</h5>

↑ **Parent:** [Constant-depth circuit complexity](#constant-depth-circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Håstad_switching_lemma)

The Håstad switching lemma says that a small-width DNF or CNF becomes representable by a shallow [decision tree](#decision-tree) with high probability under a sufficiently sparse random restriction. Iterating it is a central method for proving lower bounds against constant-depth circuits.

###### Switching-lemma depth reduction

↑ **Parent:** [Håstad switching lemma](#hastad-switching-lemma)

Switching-lemma depth reduction applies the [Håstad switching lemma](#hastad-switching-lemma) to every bottom-layer gate, replaces each restricted gate by a shallow decision tree, and merges adjacent layers of the same gate type. Repetition reduces a constant-depth circuit to a bounded-depth decision tree while retaining many live variables.

#### Monotone circuit complexity

↑ **Parent:** [Circuit complexity](#circuit-complexity)

Monotone circuit complexity studies Boolean circuits built only from AND and OR gates, without negations. Such circuits compute [monotone Boolean functions](analysis-of-boolean-functions.md#monotone-boolean-function), but some monotone functions require much larger monotone circuits than unrestricted circuits.

##### Monotone circuit

↑ **Parent:** [Monotone circuit complexity](#monotone-circuit-complexity)

A monotone [Boolean circuit](#boolean-circuit) uses only AND and OR gates, variables, and optional constants. It computes a [monotone Boolean function](analysis-of-boolean-functions.md#monotone-boolean-function); negation gates are excluded.

##### Superpolynomial monotone clique lower bound

↑ **Parent:** [Monotone circuit complexity](#monotone-circuit-complexity)

In the [finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits), set $m=r=\lfloor n^{1/4}\rfloor$ and $\ell=\lfloor\log_2n\rfloor$. A nonuniversal output accepts at most $\sum_{s=2}^\ell s!(r-1)^s(m/n)^s\leq2(\ell rm/n)^2$ of uniform positive [cliques](graph-theory.md#clique-graph-theory). Its missing positives require the circuit size times the [positive clique error of a truncated lattice meet](#positive-clique-error-of-a-truncated-lattice-meet) to be bounded below. A universal output accepts every negative colouring input; those errors require the circuit size times the [negative colouring error of a forced-set closure](#negative-colouring-error-of-a-forced-set-closure) to be at least one. Both alternatives imply the displayed superpolynomial bound by the [Razborov gate-by-gate approximation lemma](#razborov-gate-by-gate-approximation-lemma).

##### Razborov approximation method

↑ **Parent:** [Monotone circuit complexity](#monotone-circuit-complexity)

The Razborov approximation method replaces the AND and OR operations of a monotone circuit by tractable lattice operations. If each gate introduces only a controlled set of positive or negative errors, a small circuit cannot separate all positive inputs from all negative inputs.

###### Finite lattice approximation for monotone clique circuits

↑ **Parent:** [Razborov approximation method](#razborov-approximation-method)

Take upward-closed [set families](extremal-set-theory.md#set-family) of subsets of $[n]$ of size at most $\ell$, closed under the forcing rule in [Razborov closure](#razborov-closure). Normalize any family containing a set of size at most one to the full family, since its clique predicate is identically true. Intersection is the [meet in a lattice](mathematical-logic.md#meet-in-a-lattice); closure of the union is the [join in a lattice](mathematical-logic.md#join-in-a-lattice). A family represents the [graphs](graph.md) containing a [clique](graph-theory.md#clique-graph-theory) on at least one of its members. The approximate meet can lose positive inputs and the approximate join can acquire negative inputs. The [Razborov gate-by-gate approximation lemma](#razborov-gate-by-gate-approximation-lemma) charges output errors to those local errors.

###### Negative colouring error of a forced-set closure

↑ **Parent:** [Finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits)

Independently colour each [vertex](graph.md#vertex-graph-theory) with one of $m-1$ colours and join differently coloured [vertices](graph.md#vertex-graph-theory). This [complete multipartite graph](graph-theory.md#complete-multipartite-graph) has no $m$-[clique](graph-theory.md#clique-graph-theory). If a forced set $W$ is rainbow but its $r$ witnesses are not, condition on the colours of $W$. The disjoint petals make those failure events [conditionally independent](random-variable.md#conditional-independence). For each witness of size at most $\ell$, the probability of a colour collision is at most $\binom{\ell}{2}/(m-1)$. If this is at most $1/2$, one closure step causes an error with probability at most $2^{-r}$. There are at most $n^{\ell+1}$ possible steps; apply the [union bound](probability-inequality.md#boole-s-inequality).

###### Positive clique error of a truncated lattice meet

↑ **Parent:** [Finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits)

Choose a uniform $m$-subset $Z$ and the [graph](graph.md) consisting only of its [clique](graph-theory.md#clique-graph-theory). Acceptance by two approximating [set families](extremal-set-theory.md#set-family) but rejection by their intersection requires two minimal witnesses whose union has size greater than $\ell$. At least one has size greater than $\ell/2$. The [sunflower bound for minimal members of a Razborov-closed family](#sunflower-bound-for-minimal-members-of-a-razborov-closed-family) and $\mathbb P(W\subseteq Z)\leq(m/n)^{|W|}$ give $2\sum_{s>\ell/2}s!(r-1)^s(m/n)^s\leq4q^{\ell/2}$.

###### Razborov closure

↑ **Parent:** [Razborov approximation method](#razborov-approximation-method)

Fix integers $r$ and $l$. The Razborov closure of a family of vertex sets of size at most $l$ repeatedly adjoins a set $W$ whenever there are $r$ existing sets $W_1,\ldots,W_r$ whose pairwise intersections are contained in $W$. A family equal to its closure is called $r$-closed.

###### Sunflower bound for minimal members of a Razborov-closed family

↑ **Parent:** [Razborov closure](#razborov-closure)

An inclusion-minimal $s$-set in an upward-closed family cannot belong to an $r$-member [delta-system](set-theory.md#delta-system) of such minimal sets: its proper core would be adjoined by [Razborov closure](#razborov-closure), violating minimality. The [Erdős–Rado sunflower lemma](set-theory.md#erdos-rado-sunflower-lemma) therefore bounds the number $a_s$ of minimal $s$-sets. This weaker factorial bound is sufficient for the [superpolynomial monotone clique lower bound](#superpolynomial-monotone-clique-lower-bound).

###### Minimal-member bound for a Razborov-closed family

↑ **Parent:** [Razborov closure](#razborov-closure)

An $r$-closed family has at most $(r-1)^k$ inclusion-minimal members of cardinality $k$. This limits the number of cliques accepted by a proper closed approximation.

###### Razborov gate-by-gate approximation lemma

↑ **Parent:** [Razborov approximation method](#razborov-approximation-method)

The Razborov gate-by-gate approximation lemma compares a monotone circuit with the lattice computation obtained by replacing each gate by an approximate meet or join. Every disagreement at the output is charged to an error introduced by one of the circuit's gates.

#### Natural proof

↑ **Parent:** [Circuit complexity](#circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_proof)

A natural proof lower bound is based on a property of Boolean functions that is simultaneously [constructive](#constructive-property-of-boolean-functions), [large](#large-property-of-boolean-functions), and [useful](#useful-property-against-a-circuit-class) against the circuit class being bounded.

##### Constructive property of Boolean functions

↑ **Parent:** [Natural proof](#natural-proof)

A property of $n$-variable Boolean functions is constructive when membership can be decided from a $2^n$-bit truth table in time polynomial in $2^n$.

##### Large property of Boolean functions

↑ **Parent:** [Natural proof](#natural-proof)

A property of Boolean functions is large when it contains a nonnegligible fraction, customarily at least $2^{-O(n)}$, of all $n$-variable Boolean functions.

##### Useful property against a circuit class

↑ **Parent:** [Natural proof](#natural-proof)

A property is useful against a circuit class when it contains functions at infinitely many input lengths but eventually excludes every function family computed by circuits of the target size in that class.

<h5 id="razborov-rudich-natural-proofs-barrier">Razborov–Rudich natural-proofs barrier</h5>

↑ **Parent:** [Natural proof](#natural-proof)

The Razborov–Rudich natural-proofs barrier says that the existence of sufficiently secure [pseudorandom function families](#pseudorandom-function-family) rules out constructive, large properties useful against the associated circuit class.

#### Pseudorandom function family

↑ **Parent:** [Circuit complexity](#circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudorandom_function_family)

A pseudorandom function family is an efficiently computable keyed family whose oracle behavior cannot be distinguished from that of a uniformly random function by the specified class of resource-bounded algorithms.

#### Arithmetic circuit

↑ **Parent:** [Circuit complexity](#circuit-complexity)

An arithmetic circuit is a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) whose input nodes are [variables](mathematics.md#variable-mathematics) or constants in a [field](algebra.md#field), and whose internal gates perform [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), or [multiplication](arithmetic.md#multiplication). Gates may reuse earlier outputs, so the circuit can represent a [polynomial](polynomial.md) without listing all its [monomials](polynomial.md#monomial).

### Counting complexity

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_complexity)

Counting complexity studies the resources needed to count witnesses, paths, assignments, or other combinatorial objects rather than merely decide whether one exists.

<h4 id="valiant-s-permanent-reduction">Valiant's permanent reduction</h4>

↑ **Parent:** [Counting complexity](#counting-complexity)

Valiant's permanent reduction encodes satisfying assignments as [cycle covers](graph-theory.md#cycle-cover-of-a-directed-graph) so that their weighted sum is the [permanent of a matrix](linear-algebra.md#permanent-mathematics). Local gadgets enforce variable consistency and clause satisfaction, while signed contributions cancel invalid covers.

<h5 id="variable-gadget-in-valiant-s-permanent-reduction">Variable gadget in Valiant's permanent reduction</h5>

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

The variable gadget has two relevant cycle-cover states, representing the two truth values, and exposes ports that transmit the chosen value to occurrences of the variable.

<h5 id="clause-gadget-in-valiant-s-permanent-reduction">Clause gadget in Valiant's permanent reduction</h5>

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

The clause gadget contributes the required fixed weight precisely when at least one incident literal port represents a satisfying value.

<h5 id="exclusive-or-gadget-in-valiant-s-permanent-reduction">Exclusive-or gadget in Valiant's permanent reduction</h5>

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

The exclusive-or gadget connects two ports while allowing exactly one corresponding external edge to participate. Signed edge weights pair and cancel unwanted cycle covers.

##### Binary path-counting gadget

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

A binary path-counting gadget replaces an edge of nonnegative integer weight $w$ by a zero-one directed graph with exactly $w$ routes from its entrance to its exit. Repeated doubling and conditional addition follow the binary expansion of $w$ using only linearly many vertices in its bit length.

#### Balanced number 3-SAT

↑ **Parent:** [Counting complexity](#counting-complexity)

Balanced number 3-SAT is the counting version of 3-SAT under a promise that every variable has equally many positive and negative occurrences.

### Polynomial hierarchy

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_hierarchy)

The polynomial hierarchy consists of decision problems described by a constant number of alternating polynomially bounded existential and universal quantifiers with a polynomial-time predicate.

#### Second level of the polynomial hierarchy

↑ **Parent:** [Polynomial hierarchy](#polynomial-hierarchy)

A language is in $\Sigma_2^{\mathbf P}$ when membership has the form $\exists u\,\forall v\,R(x,u,v)$ for a polynomial-time predicate $R$ and polynomially bounded strings. Reversing the quantifiers defines $\Pi_2^{\mathbf P}$.

<h4 id="karp-lipton-theorem">Karp–Lipton theorem</h4>

↑ **Parent:** [Polynomial hierarchy](#polynomial-hierarchy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karp–Lipton_theorem)

The Karp–Lipton theorem states that $\mathbf{NP}\subseteq\mathbf P/\mathrm{poly}$ implies that the [polynomial hierarchy](#polynomial-hierarchy) collapses to its second level.

### Primality testing

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primality_testing)

Primality testing is the decision problem of determining whether an input integer is a [prime number](prime-number.md).

#### Prime-proof number

↑ **Parent:** [Primality testing](#primality-testing)

An [integer](integer.md) for which replacing any one decimal [numerical digit](integer.md#numerical-digit) by a different digit never produces a [prime number](prime-number.md). The convention must specify whether changes creating a leading zero are permitted. An exact test enumerates the allowed substitutions and applies [primality testing](#primality-testing) to each result.

#### Miller-Rabin primality test

↑ **Parent:** [Primality testing](#primality-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Miller–Rabin_primality_test)

For an odd candidate $n>3$, write $n-1=2^s d$ with $d$ odd. A base $a$ passes when $a^d\equiv1\pmod n$ or $a^{2^jd}\equiv-1\pmod n$ for some $0\le j<s$; a nontrivial common divisor of $a,n$ or failure of these conditions proves compositeness. A prime passes every base, while an odd composite passes at most one quarter of possible bases. Independent rounds give a false probable-prime probability at most $4^{-r}$. A passing composite is a [strong pseudoprime](number-theory.md#strong-pseudoprime), stronger than a [Fermat pseudoprime](number-theory.md#fermat-pseudoprime).

##### Deterministic Miller-Rabin primality test

↑ **Parent:** [Miller-Rabin primality test](#miller-rabin-primality-test)

#### Fermat primality test

↑ **Parent:** [Primality testing](#primality-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat_primality_test)

The Fermat test looks for a coprime base $a$ with $a^{N-1}\not\equiv1\pmod N$. Such a witness proves compositeness by the [Fermat little theorem](number-theory.md#fermat-little-theorem), but [Carmichael numbers](number-theory.md#carmichael-number) pass for every coprime base.

#### Pseudoprime base

↑ **Parent:** [Primality testing](#primality-testing)

A base $b$ coprime to the tested odd composite $N$ for which a specified probable-prime criterion passes. The sets of passing bases depend on the criterion and need not be subgroups.

<h4 id="agrawal-biswas-primality-test">Agrawal–Biswas primality test</h4>

↑ **Parent:** [Primality testing](#primality-testing)

The Agrawal–Biswas primality test checks the identity $(X+1)^n=X^n+1$ modulo $n$ and a random low-degree monic polynomial. Prime inputs always pass, while a composite input that is not a prime power fails with inverse-polynomial probability per trial.

## Abstract machine

↑ **Parent:** [Theoretical computer science](theoretical-computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abstract_machine)

An [abstract machine](#abstract-machine) specifies a computational state and rules for advancing that state without requiring one particular physical implementation. A [Turing machine](#turing-machine) and a [stack machine](#stack-machine) give different ways to organize the state and its transitions.

### Stack machine

↑ **Parent:** [Abstract machine](#abstract-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stack_machine)

An execution model whose instructions obtain operands from a [stack](data-structure.md#stack-data-structure) and put results back on that [stack](data-structure.md#stack-data-structure).

## ↑ Ancestors (2)

1. [Computer science](computer-science.md)
2. [Codex Wiki](README.md)
