# Computational complexity

↑ **Parent:** [2015](../2015.md)

Solutions to all three questions of the [University of Oxford](../../university-of-oxford.md) [computer science](../../computer-science.md) finals paper held on 3 June 2015, Trinity Term 2015. The printed cover gives paper code A12071W1. Questions 2 and 3 are marked corrected in the source.[Cover and printed pp. 2–4, Questions 1–3](../../computer-science-bibliography.md#computational-complexity-examination-paper-of-the-university-of-oxford-2015)

The solutions use the original printed notation; the [integer parity](../../integer.md#parity-mathematics) convention needed in Question 3(e) is stated there explicitly.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)

## 1

↑ **Parent:** [Computational complexity](computational-complexity.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

**Exactly the [regular languages](../../foundations-of-mathematics.md#regular-language).** A [read-only-from-left Turing acceptor](../../theoretical-computer-science.md#read-only-from-left-turing-acceptor) has only its current control state as usable memory: it never changes a tape symbol, and its head never returns to an earlier cell. This is the behaviour of a [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) while it reads the [input](../../theoretical-computer-science.md#input-computer-science).

To make the correspondence precise, retain the control states and the transitions on the [input](../../theoretical-computer-science.md#input-computer-science) [alphabet](../../information-theory.md#alphabet). Replace accepting and rejecting halts by absorbing states, so that halting before the end of a [word over an alphabet](../../foundations-of-mathematics.md#string) has the same effect on every continuation. For each remaining state $q$, follow the transitions on blank symbols and mark $q$ accepting in the [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) exactly when this blank-only continuation eventually accepts. This marking is a finite calculation: either a halting state is reached or a state repeats, after which the blank-only run loops. The resulting [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) accepts exactly the same [formal language](../../theoretical-computer-science.md#formal-language) as the [read-only-from-left Turing acceptor](../../theoretical-computer-science.md#read-only-from-left-turing-acceptor). If the latter is a decider, the blank-only run from every reachable end-of-input state halts.

Conversely, simulate any [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) by a [read-only-from-left Turing acceptor](../../theoretical-computer-science.md#read-only-from-left-turing-acceptor), using its state transitions while reading the [input](../../theoretical-computer-science.md#input-computer-science). At the first blank symbol, halt and accept or reject according to the current [deterministic finite automaton](../../foundations-of-mathematics.md#deterministic-finite-automaton) state. This machine halts on every [input](../../theoretical-computer-science.md#input-computer-science) and decides the required [regular language](../../foundations-of-mathematics.md#regular-language).

$$
\boxed{\text{ROFL-decidable languages}=\text{regular languages}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[Rice's theorem](../../computability-theory.md#rice-s-theorem), in its [formal language](../../theoretical-computer-science.md#formal-language) version, says: **every nontrivial property of the [computably enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language) accepted by a [Turing machine](../../theoretical-computer-science.md#turing-machine) has an [undecidable](../../computability-theory.md#undecidable-decision-problem) set of machine descriptions.** Here nontrivial means that some [computably enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language) has the property and some does not. The property must be an [extensional property of programs](../../computability-theory.md#extensional-property-of-programs): any two [Turing machines](../../theoretical-computer-science.md#turing-machine) accepting the same [formal language](../../theoretical-computer-science.md#formal-language) must agree about it. It need not be a property of all [formal languages](../../theoretical-computer-science.md#formal-language), including those no [Turing machine](../../theoretical-computer-science.md#turing-machine) accepts.

Let $\mathscr P$ be such a property and write

$$
I_{\mathscr P}=\{\operatorname{enc}(N):\mathcal L(N)\in\mathscr P\}.
$$

We prove the theorem by a [many-one reduction](../../computability-theory.md#many-one-reduction) from the [halting problem](../../foundations-of-mathematics.md#halting-problem). First suppose the [empty language](../../theoretical-computer-science.md#empty-language) is not in $\mathscr P$. Nontriviality provides a fixed [Turing machine](../../theoretical-computer-science.md#turing-machine) $B$ with $\mathcal L(B)\in\mathscr P$. Given a [Turing machine](../../theoretical-computer-science.md#turing-machine) $M$ and a [word over an alphabet](../../foundations-of-mathematics.md#string) $w$, effectively construct a [Turing machine](../../theoretical-computer-science.md#turing-machine) $N_{M,w}$ which, on [input](../../theoretical-computer-science.md#input-computer-science) $x$, first simulates $M$ on $w$. If that simulation ever halts, it simulates $B$ on $x$ and accepts precisely when $B$ accepts. If the first simulation never halts, it never accepts $x$.

The [Turing machine encoding](../../theoretical-computer-science.md#turing-machine-encoding) of $N_{M,w}$ is computable from those of $M,w$: the description merely embeds $M,w$ and the fixed simulator for $B$. Constructing it does not require predicting whether $M$ halts. Its accepted [formal language](../../theoretical-computer-science.md#formal-language) is

$$
\mathcal L(N_{M,w})=
\begin{cases}
\mathcal L(B),&M\text{ halts on }w,\\
\varnothing,&M\text{ does not halt on }w.
\end{cases}
$$

Consequently

$$
M\text{ halts on }w\quad\Longleftrightarrow\quad
\operatorname{enc}(N_{M,w})\in I_{\mathscr P}.
$$

A decider for $I_{\mathscr P}$ would therefore decide the [halting problem](../../foundations-of-mathematics.md#halting-problem), a contradiction. Invalid descriptions can be mapped to a fixed description of a machine accepting the [empty language](../../theoretical-computer-science.md#empty-language), if the [many-one reduction](../../computability-theory.md#many-one-reduction) is formulated on all [strings](../../foundations-of-mathematics.md#string).

If the [empty language](../../theoretical-computer-science.md#empty-language) does belong to $\mathscr P$, apply the preceding argument to the opposite property, within the [computably enumerable languages](../../foundations-of-mathematics.md#recursively-enumerable-language). This opposite property is still nontrivial and excludes the [empty language](../../theoretical-computer-science.md#empty-language). A hypothetical decider for $I_{\mathscr P}$ would decide the opposite property's index set by first rejecting malformed [Turing machine encodings](../../theoretical-computer-science.md#turing-machine-encoding) and otherwise reversing its answer. The opposite property is [undecidable](../../computability-theory.md#undecidable-decision-problem) by the first case, giving the required contradiction in this case too.

$$
\boxed{I_{\mathscr P}\text{ is undecidable for every nontrivial extensional }\mathscr P.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For example, take

$$
\boxed{\mathcal L=\{\operatorname{enc}(M):M\text{ has an even number of states}\}.}
$$

This is a [decidable language](../../foundations-of-mathematics.md#recursive-language): check that the [input](../../theoretical-computer-science.md#input-computer-science) is a valid [Turing machine encoding](../../theoretical-computer-science.md#turing-machine-encoding), count its declared states, and test the count's [integer parity](../../integer.md#parity-mathematics). There are [Turing machines](../../theoretical-computer-science.md#turing-machine) with even state counts and [Turing machines](../../theoretical-computer-science.md#turing-machine) with odd state counts, so the [formal language](../../theoretical-computer-science.md#formal-language) contains some but not all valid descriptions.

**There is no contradiction with [Rice's theorem](../../computability-theory.md#rice-s-theorem) because this is a syntactic property of the description.** Add one unreachable state to a [Turing machine](../../theoretical-computer-science.md#turing-machine), assigning any permitted transitions to it. The accepted [formal language](../../theoretical-computer-science.md#formal-language) is unchanged, while the [integer parity](../../integer.md#parity-mathematics) of the state count changes. Thus the property is not an [extensional property of programs](../../computability-theory.md#extensional-property-of-programs), which is an essential hypothesis of [Rice's theorem](../../computability-theory.md#rice-s-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**$\mathcal L_{\ell3}$ is [undecidable](../../computability-theory.md#undecidable-decision-problem).** The condition depends only on the accepted [formal language](../../theoretical-computer-science.md#formal-language). It holds for a [Turing machine](../../theoretical-computer-science.md#turing-machine) accepting the [empty language](../../theoretical-computer-science.md#empty-language), and fails for a [Turing machine](../../theoretical-computer-science.md#turing-machine) accepting the singleton $\{aaaa\}$, where $a$ is an [alphabet](../../information-theory.md#alphabet) symbol. It is therefore a nontrivial [extensional property of programs](../../computability-theory.md#extensional-property-of-programs), and [Rice's theorem](../../computability-theory.md#rice-s-theorem) applies. In particular, the condition does not assert that the machine halts on every [input](../../theoretical-computer-science.md#input-computer-science); nonacceptance of long [words over an alphabet](../../foundations-of-mathematics.md#string) may result from rejection or from an infinite computation.

**$\mathcal L_{1\mathrm T}$ is a [decidable language](../../foundations-of-mathematics.md#recursive-language): it consists of every valid [Turing machine encoding](../../theoretical-computer-science.md#turing-machine-encoding).** Every [multitape Turing machine](../../theoretical-computer-science.md#multitape-turing-machine) has an equivalent [single-tape Turing machine](../../theoretical-computer-science.md#single-tape-turing-machine). To see this, represent the finitely used portions of its tapes on one tape, separated by delimiters, and mark each simulated head position. To simulate one step, scan these portions to read the marked symbols, retain this fixed number of symbols and the control state in finite control, and scan again to update the symbols and head marks. Extend a represented portion with a blank cell when necessary. Each simulated step takes finitely many real steps.

The [single-tape Turing machine](../../theoretical-computer-science.md#single-tape-turing-machine) accepts exactly when the simulated [multitape Turing machine](../../theoretical-computer-science.md#multitape-turing-machine) accepts; infinite computations remain infinite. The simulation may increase [time complexity](../../theoretical-computer-science.md#time-complexity), but the question only asks about accepted [formal languages](../../theoretical-computer-science.md#formal-language). Hence a decider simply checks the syntax of the [Turing machine encoding](../../theoretical-computer-science.md#turing-machine-encoding) and accepts every valid description. [Rice's theorem](../../computability-theory.md#rice-s-theorem) does not make this property [undecidable](../../computability-theory.md#undecidable-decision-problem), because the property is true of every [computably enumerable language](../../foundations-of-mathematics.md#recursively-enumerable-language) and is therefore trivial in the theorem's sense.

$$
\boxed{\mathcal L_{\ell3}\text{ is undecidable};\qquad\mathcal L_{1\mathrm T}\text{ is decidable}.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [clique decision problem](../../graph-theory.md#clique-decision-problem) is a [decidable language](../../foundations-of-mathematics.md#recursive-language): on a valid finite [graph](../../graph.md) and an [integer](../../integer.md) $k$, reject if $k$ exceeds the number of [vertices](../../graph.md#vertex-graph-theory), and otherwise examine all $k$-element [subsets](../../set.md#subset) of [vertices](../../graph.md#vertex-graph-theory), accepting if one is a [clique](../../graph-theory.md#clique-graph-theory). Each candidate can be checked by examining all its pairs of distinct [vertices](../../graph.md#vertex-graph-theory). This finite search gives at least one [Turing machine](../../theoretical-computer-science.md#turing-machine) deciding the problem, without any claim of [polynomial time](../../theoretical-computer-science.md#polynomial-time).

By [well-ordering](../../set.md#well-order) of the [natural numbers](../../arithmetic.md#natural-number), there is a least state count $n_0$ among [Turing machines](../../theoretical-computer-science.md#turing-machine) deciding the [clique decision problem](../../graph-theory.md#clique-decision-problem). For every $n\geq n_0$, add $n-n_0$ unreachable states to a machine with $n_0$ states. Its behaviour on every [input](../../theoretical-computer-science.md#input-computer-science) is unchanged, and it has exactly $n$ states. For $n<n_0$ there is no such machine, by minimality. Thus

$$
\boxed{\mathcal L_{\mathrm{cliqueTM}}
=\{\operatorname{enc}(n):n\geq n_0\}.}
$$

A [Turing machine](../../theoretical-computer-science.md#turing-machine) with the fixed constant $n_0$ in its description decides this [threshold language](../../foundations-of-mathematics.md#threshold-language) by validating the [input](../../theoretical-computer-science.md#input-computer-science) and comparing its value with $n_0$. **The argument proves the existence of a decider; it does not compute the smallest possible [clique decision problem](../../graph-theory.md#clique-decision-problem) decider.** There is no need to search through machine descriptions and attempt to certify their behaviour on every [input](../../theoretical-computer-science.md#input-computer-science).

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Let $V$ be the [decidable language](../../foundations-of-mathematics.md#recursive-language) of syntactically valid descriptions $\operatorname{enc}(M)\#\#w$. Then

$$
\mathcal L_{\mathrm H}\mathbin{\dot\cup}\mathcal L_{\mathrm{NH}}=V,
\qquad
\overline{\mathcal L_{\mathrm H}}
=\mathcal L_{\mathrm{NH}}\mathbin{\dot\cup}(\Sigma^*\setminus V).
$$

Here the [complement of a set](../../set.md#complement-of-a-set) on the left is taken in all [words over an alphabet](../../foundations-of-mathematics.md#string), while the non-halting problem only has valid machine-and-input descriptions as instances. **Any malformed description belongs to $\overline{\mathcal L_{\mathrm H}}$ but not to $\mathcal L_{\mathrm{NH}}$.** For example, the [empty word](../../foundations-of-mathematics.md#empty-word) has no separating `##`, so cannot be a valid instance under the displayed encoding.

Fix valid descriptions $h$ and $\ell$ of, respectively, an immediately halting [Turing machine](../../theoretical-computer-science.md#turing-machine) on the [empty word](../../foundations-of-mathematics.md#empty-word) and a [Turing machine](../../theoretical-computer-science.md#turing-machine) looping forever on the [empty word](../../foundations-of-mathematics.md#empty-word). Then

$$
h\in\mathcal L_{\mathrm H},\qquad
\ell\in\mathcal L_{\mathrm{NH}}.
$$

For the first [many-one reduction](../../computability-theory.md#many-one-reduction), use the total [computable function](../../computability-theory.md#computable-function)

$$
f(x)=
\begin{cases}
x,&x\in V,\\
\ell,&x\notin V.
\end{cases}
$$

For a valid [input](../../theoretical-computer-science.md#input-computer-science), nonmembership in $\mathcal L_{\mathrm H}$ is exactly membership in $\mathcal L_{\mathrm{NH}}$, so retaining it is correct. Every invalid [input](../../theoretical-computer-science.md#input-computer-science) is a yes-instance of $\overline{\mathcal L_{\mathrm H}}$, and $f$ sends it to the fixed yes-instance $\ell$. Therefore $x\in\overline{\mathcal L_{\mathrm H}}$ if and only if $f(x)\in\mathcal L_{\mathrm{NH}}$.

For the reverse [many-one reduction](../../computability-theory.md#many-one-reduction), use

$$
g(x)=
\begin{cases}
x,&x\in V,\\
h,&x\notin V.
\end{cases}
$$

The equivalence again holds on valid [inputs](../../theoretical-computer-science.md#input-computer-science). Invalid [inputs](../../theoretical-computer-science.md#input-computer-science) are no-instances of $\mathcal L_{\mathrm{NH}}$, and $h$ is a no-instance of $\overline{\mathcal L_{\mathrm H}}$. Syntax checking terminates, so $g$ is also a total [computable function](../../computability-theory.md#computable-function). We have proved

$$
\boxed{\overline{\mathcal L_{\mathrm H}}\leq_m\mathcal L_{\mathrm{NH}}
\quad\text{and}\quad
\mathcal L_{\mathrm{NH}}\leq_m\overline{\mathcal L_{\mathrm H}}.}
$$

## 2

↑ **Parent:** [Computational complexity](computational-complexity.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Writing $\mathrm{PTime}$ as [P](../../theoretical-computer-science.md#p-complexity) and $\mathrm{co\text{-}PTime}$ as [co-P](../../theoretical-computer-science.md#co-p), the known relationships among the four [complexity classes](../../theoretical-computer-science.md#complexity-class) are

$$
\boxed{\mathrm P=\mathrm{co\text{-}P},\qquad
\mathrm P\subseteq\mathrm{NP},\qquad
\mathrm P\subseteq\mathrm{co\text{-}NP}.}
$$

The equality supplies both inclusions between [P](../../theoretical-computer-science.md#p-complexity) and [co-P](../../theoretical-computer-science.md#co-p), and it also gives [co-P](../../theoretical-computer-science.md#co-p) $\subseteq$ [NP](../../theoretical-computer-science.md#np-complexity) and [co-P](../../theoretical-computer-science.md#co-p) $\subseteq$ [co-NP](../../theoretical-computer-science.md#co-np).

For the equality, a deterministic [polynomial-time algorithm](../../theoretical-computer-science.md#polynomial-time-algorithm) halts on every [input](../../theoretical-computer-science.md#input-computer-science); interchange its accepting and rejecting outcomes to decide the [complement of a set](../../set.md#complement-of-a-set) in the same [polynomial time](../../theoretical-computer-science.md#polynomial-time). For [P](../../theoretical-computer-science.md#p-complexity) $\subseteq$ [NP](../../theoretical-computer-science.md#np-complexity), a [Nondeterministic Turing machine](../../theoretical-computer-science.md#nondeterministic-turing-machine) can simply make no choices and follow the deterministic computation. Finally, if $A\in\mathrm P$, then $\overline A\in\mathrm P\subseteq\mathrm{NP}$, whence $A\in\mathrm{co\text{-}NP}$ by the definition of [co-NP](../../theoretical-computer-science.md#co-np).

Neither [NP](../../theoretical-computer-science.md#np-complexity) $\subseteq$ [co-NP](../../theoretical-computer-science.md#co-np) nor [co-NP](../../theoretical-computer-science.md#co-np) $\subseteq$ [NP](../../theoretical-computer-science.md#np-complexity) is known; either would imply equality by taking [complements](../../set.md#complement-of-a-set). Nor is either inclusion of [P](../../theoretical-computer-science.md#p-complexity) into [NP](../../theoretical-computer-science.md#np-complexity) or [co-NP](../../theoretical-computer-science.md#co-np) known to be strict. These unresolved relationships must not be presented as strict separations.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [linear speedup theorem](../../theoretical-computer-science.md#linear-speedup-theorem) concerns [multitape Turing machines](../../theoretical-computer-science.md#multitape-turing-machine) whose finite control and tape [alphabet](../../information-theory.md#alphabet) may change. Formally, for $k>1$, if a deterministic $k$-tape [Turing machine](../../theoretical-computer-science.md#turing-machine) decides $A$ within $T(n)$ steps on every [input](../../theoretical-computer-science.md#input-computer-science) of length $n$, then for every constant $c>0$ there is a deterministic $k$-tape [Turing machine](../../theoretical-computer-science.md#turing-machine) deciding the same [formal language](../../theoretical-computer-science.md#formal-language) with

$$
\boxed{T_c(n)\leq\frac{T(n)}c+n+O(1).}
$$

The additive constant is independent of $n$; in the usual normalized formulation the bound is $T(n)/c+n+2$, with the integer-rounding convention absorbed in the constant.[Slides 47–48, PDF pp. 62–63: statement for k \> 1 and block simulation](../../computer-science-bibliography.md#computational-complexity-slides-1-by-paul-w-goldberg-2023)

The construction packs a fixed number of old tape symbols into each new symbol and uses a larger finite control to simulate blocks of old steps. Initial [input](../../theoretical-computer-science.md#input-computer-science) packing explains the additive linear term. If $T(n)/n\to\infty$, choosing a larger constant $c$ makes the total asymptotic [time complexity](../../theoretical-computer-science.md#time-complexity) an arbitrarily small constant multiple of $T(n)$.

**It does not promise arbitrary speed increases on fixed hardware.** Larger packed symbols and transition tables cease to be single constant-cost hardware operations without limit. The theorem also retains the [input](../../theoretical-computer-science.md#input-computer-science)-reading overhead. It is a statement about changing the abstract machine description and primitive operations, rather than an unlimited implementation optimization on one processor.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $A\in\mathrm{NP}$, accepted by a fixed [Nondeterministic Turing machine](../../theoretical-computer-science.md#nondeterministic-turing-machine) $M$ in at most $p(n)$ steps on every computation branch, for a [polynomial](../../polynomial.md) $p$. Since the transition relation is finite, there is a fixed constant $b\geq2$ bounding the number of choices at any step. Every branch can be specified by a [word over an alphabet](../../foundations-of-mathematics.md#string) of length $p(n)$ over a $b$-symbol choice [alphabet](../../information-theory.md#alphabet), padding unused choices after halting.

A deterministic [Turing machine](../../theoretical-computer-science.md#turing-machine) enumerates all $b^{p(n)}$ such choice sequences and simulates the corresponding branches for at most $p(n)$ steps each. It accepts if some simulation accepts, and rejects after all have failed. Every possible accepting branch is included, and the time cutoff guarantees termination even on invalid choice sequences. A standard direct simulation has only [polynomial](../../polynomial.md) overhead per branch, giving

$$
b^{p(n)}p(n)^{O(1)}
=2^{O(p(n)+\log(p(n)+1))}
\leq 2^{q(n)}
$$

for a suitable [polynomial](../../polynomial.md) $q$. This is a deterministic [exponential time](../../theoretical-computer-science.md#exponential-time) bound. Therefore

$$
\boxed{\mathrm{NP}\subseteq\mathrm{EXPTIME}.}
$$

Here [EXPTIME](../../theoretical-computer-science.md#exptime) means the union of deterministic time bounds $2^{n^d}$ over fixed positive [integers](../../integer.md) $d$, allowing the usual constant factors and finitely many small [inputs](../../theoretical-computer-science.md#input-computer-science).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**Entail is [co-NP](../../theoretical-computer-science.md#co-np)-complete under [polynomial-time many-one reductions](../../theoretical-computer-science.md#polynomial-time-many-one-reduction).** For valid [propositional formulas](../../mathematical-logic.md#propositional-formula), [semantic entailment](../../mathematical-logic.md#semantic-entailment) holds exactly when the [logical conjunction](../../mathematical-logic.md#logical-conjunction) of the premise and the conclusion's [logical negation](../../theoretical-computer-science.md#negation) is an [unsatisfiable Boolean formula](../../theoretical-computer-science.md#unsatisfiable-boolean-formula):

$$
\varphi\models\psi
\quad\Longleftrightarrow\quad
\varphi\land\neg\psi\text{ is unsatisfiable}.
$$

A counterexample to [semantic entailment](../../mathematical-logic.md#semantic-entailment) is a [Boolean valuation](../../mathematical-logic.md#boolean-valuation) making $\varphi$ true and $\psi$ false. Guessing one [bit](../../information-theory.md#bit) for each distinct [Boolean variable](../../theoretical-computer-science.md#boolean-variable) and evaluating both [propositional formulas](../../mathematical-logic.md#propositional-formula) is a [polynomial-time algorithm](../../theoretical-computer-science.md#polynomial-time-algorithm). Thus the [complement](../../set.md#complement-of-a-set) of Entail belongs to [NP](../../theoretical-computer-science.md#np-complexity). Malformed descriptions, also in that [complement](../../set.md#complement-of-a-set), can be accepted after a deterministic syntax check. Hence Entail belongs to [co-NP](../../theoretical-computer-science.md#co-np) as a [formal language](../../theoretical-computer-science.md#formal-language) over all [strings](../../foundations-of-mathematics.md#string).

For hardness, the [unsatisfiable Boolean formula](../../theoretical-computer-science.md#unsatisfiable-boolean-formula) problem is [co-NP](../../theoretical-computer-science.md#co-np)-hard: if $A\in\mathrm{co\text{-}NP}$, then $\overline A\in\mathrm{NP}$, and the permitted [NP-hardness](../../theoretical-computer-science.md#np-hardness) of [SAT](../../theoretical-computer-science.md#boolean-satisfiability-problem) supplies a [polynomial-time many-one reduction](../../theoretical-computer-science.md#polynomial-time-many-one-reduction) $r$ with

$$
x\in\overline A\quad\Longleftrightarrow\quad r(x)\in\mathrm{SAT}.
$$

We may ensure $r(x)$ is always a valid [propositional formula](../../mathematical-logic.md#propositional-formula), replacing any malformed output by a fixed contradiction. It follows that $x\in A$ exactly when $r(x)$ is unsatisfiable. This justifies using the unsatisfiability problem as a hardness source without an extra assumption.

Map a valid [propositional formula](../../mathematical-logic.md#propositional-formula) $\theta$ to

$$
f(\theta)=\langle\theta,\ p\land\neg p\rangle,
$$

where $p$ is a fixed [Boolean variable](../../theoretical-computer-science.md#boolean-variable). The second [propositional formula](../../mathematical-logic.md#propositional-formula) is false under every [Boolean valuation](../../mathematical-logic.md#boolean-valuation). Consequently it is entailed by $\theta$ precisely when no [Boolean valuation](../../mathematical-logic.md#boolean-valuation) satisfies $\theta$. Thus

$$
\theta\text{ unsatisfiable}
\quad\Longleftrightarrow\quad f(\theta)\in\mathrm{Entail}.
$$

The output has only constant additional length and is computable in [polynomial time](../../theoretical-computer-science.md#polynomial-time). If the source unsatisfiability language rejects malformed [strings](../../foundations-of-mathematics.md#string), map them to the fixed no-instance $\langle p,p\land\neg p\rangle$. This completes a total [polynomial-time many-one reduction](../../theoretical-computer-science.md#polynomial-time-many-one-reduction) and proves the claimed [co-NP](../../theoretical-computer-science.md#co-np)-completeness.

$$
\boxed{\mathrm{Entail}\text{ is co-NP-complete}.}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [clique decision problem](../../graph-theory.md#clique-decision-problem) belongs to [NP](../../theoretical-computer-science.md#np-complexity). First reject $k>|V(G)|$. Otherwise a [complexity certificate](../../theoretical-computer-science.md#certificate-complexity) lists $k$ distinct [vertices](../../graph.md#vertex-graph-theory). Check distinctness and test that each of the $\binom k2$ pairs is an [edge](../../graph-theory.md#edge-of-a-graph). Under a conventional explicit [graph](../../graph.md) encoding, the [complexity certificate](../../theoretical-computer-science.md#certificate-complexity) length and verification [time complexity](../../theoretical-computer-science.md#time-complexity) are [polynomial](../../polynomial.md) in the [input](../../theoretical-computer-science.md#input-computer-science) length. The early rejection is relevant when $k$ is given in the [binary numeral system](../../integer.md#binary-numeral-system).

For [NP-hardness](../../theoretical-computer-science.md#np-hardness), first transform a [SAT](../../theoretical-computer-science.md#boolean-satisfiability-problem) instance into an equisatisfiable [conjunctive normal form](../../theoretical-computer-science.md#conjunctive-normal-form) $F=C_1\land\cdots\land C_m$ of [polynomial](../../polynomial.md) size using a [Tseitin transformation](../../theoretical-computer-science.md#tseytin-transformation). This step avoids the possibly exponential increase caused by distributing arbitrary [Boolean formulas](../../theoretical-computer-science.md#boolean-formula) into [conjunctive normal form](../../theoretical-computer-science.md#conjunctive-normal-form). Introduce a fresh [Boolean variable](../../theoretical-computer-science.md#boolean-variable) for each subformula, constrain it to have the connective's [truth value](../../mathematical-logic.md#truth-value) using a constant number of [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula), and require the top variable to be true. A [Boolean valuation](../../mathematical-logic.md#boolean-valuation) of the original [Boolean variables](../../theoretical-computer-science.md#boolean-variable) satisfies the original [Boolean formula](../../theoretical-computer-science.md#boolean-formula) exactly when it extends to a [satisfying assignment](../../theoretical-computer-science.md#satisfying-assignment) of these constraints.

Create one [vertex](../../graph.md#vertex-graph-theory) for each occurrence of a [Boolean literal](../../theoretical-computer-science.md#boolean-literal) in each [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula). Join two such [vertices](../../graph.md#vertex-graph-theory) by an [edge](../../graph-theory.md#edge-of-a-graph) exactly when they belong to different [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula) and their [Boolean literals](../../theoretical-computer-science.md#boolean-literal) are not a variable and its [logical negation](../../theoretical-computer-science.md#negation). Set $k=m$. There are at most as many [vertices](../../graph.md#vertex-graph-theory) as [Boolean literal](../../theoretical-computer-science.md#boolean-literal) occurrences and at most quadratically many [edges](../../graph-theory.md#edge-of-a-graph), so this construction takes [polynomial time](../../theoretical-computer-science.md#polynomial-time).

If $F$ has a [satisfying assignment](../../theoretical-computer-science.md#satisfying-assignment), choose one true [Boolean literal](../../theoretical-computer-science.md#boolean-literal) occurrence from each [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula). No two selected [Boolean literals](../../theoretical-computer-science.md#boolean-literal) are contradictory, so their $m$ [vertices](../../graph.md#vertex-graph-theory) form a [clique](../../graph-theory.md#clique-graph-theory). Conversely, an $m$-[clique](../../graph-theory.md#clique-graph-theory) contains at most one [vertex](../../graph.md#vertex-graph-theory) from each [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula), because there are no [edges](../../graph-theory.md#edge-of-a-graph) within a [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula). It therefore selects exactly one occurrence from each of the $m$ [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula). The selected [Boolean literals](../../theoretical-computer-science.md#boolean-literal) are pairwise noncontradictory, so assign their [Boolean variables](../../theoretical-computer-science.md#boolean-variable) the indicated [truth values](../../mathematical-logic.md#truth-value) and assign any other [Boolean variables](../../theoretical-computer-science.md#boolean-variable) arbitrarily. This [Boolean valuation](../../mathematical-logic.md#boolean-valuation) satisfies every [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula).

An empty [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) gives no [vertex](../../graph.md#vertex-graph-theory) in its group, correctly preventing an $m$-[clique](../../graph-theory.md#clique-graph-theory). An empty [logical conjunction](../../mathematical-logic.md#logical-conjunction) can instead be mapped to a fixed yes-instance, avoiding any convention about $k=0$. Malformed [SAT](../../theoretical-computer-science.md#boolean-satisfiability-problem) descriptions can be mapped to a fixed no-instance. We have proved

$$
F\text{ satisfiable}\quad\Longleftrightarrow\quad
\langle G_F,m\rangle\in\mathrm{Clique},
\qquad
\boxed{\mathrm{Clique}\text{ is NP-complete}.}
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

To establish [strong NP-completeness](../../theoretical-computer-science.md#strong-np-completeness), use an explicit [adjacency matrix](../../graph-theory.md#adjacency-matrix) encoding for a finite [simple graph](../../graph.md#simple-graph), with enough length information to recover its number $N$ of [vertices](../../graph.md#vertex-graph-theory). Let $\operatorname{bin}(k)$ be the canonical [binary numeral system](../../integer.md#binary-numeral-system) representation of the nonnegative [integer](../../integer.md) $k$. Define

$$
\mathcal L_{\mathrm{Clique}}
=\{\langle\operatorname{enc}(G),\operatorname{bin}(k)\rangle:
G\text{ has a clique of size }k\},
$$

and, using the [unary numeral system](../../mathematics.md#unary-numeral-system) for $k$,

$$
\mathcal L_{u\mathrm{Clique}}
=\{\langle\operatorname{enc}(G),1^k\rangle:
G\text{ has a clique of size }k\}.
$$

The surrounding pairing syntax delimits the two components, so the empty unary field can encode $k=0$ if zero is included in the convention for [natural numbers](../../arithmetic.md#natural-number). Malformed descriptions are excluded from both [formal languages](../../theoretical-computer-science.md#formal-language).

Fix a unary no-instance $u_0$, for example one isolated [vertex](../../graph.md#vertex-graph-theory) with requested size $2$. The [polynomial-time many-one reduction](../../theoretical-computer-science.md#polynomial-time-many-one-reduction) is

$$
f(\langle\operatorname{enc}(G),\operatorname{bin}(k)\rangle)
=\begin{cases}
\langle\operatorname{enc}(G),1^k\rangle,&0\leq k\leq N,\\
u_0,&k>N.
\end{cases}
$$

Map malformed [inputs](../../theoretical-computer-science.md#input-computer-science) to $u_0$ too. When $k\leq N$, only the numerical representation changes, so the existence of a $k$-[clique](../../graph-theory.md#clique-graph-theory) is unchanged. When $k>N$, the original instance is false, since a [subset](../../set.md#subset) of [vertices](../../graph.md#vertex-graph-theory) cannot be larger than the whole [vertex set](../../graph.md#vertex-set); $u_0$ is false as required.

The important size bound is $k\leq N$ in the branch that writes $1^k$. The original explicit [graph](../../graph.md) description already has length at least $N$, so the output has [polynomial](../../polynomial.md) length and can be written in [polynomial time](../../theoretical-computer-science.md#polynomial-time). If a huge [binary numeral system](../../integer.md#binary-numeral-system) value $k$ is supplied, compare it with $N$ using its digit length and, when needed, a digit comparison; do not first allocate or print $k$ symbols. Merely replacing an unrestricted binary $k$ by $1^k$ would not be a valid [polynomial-time reduction](../../theoretical-computer-science.md#polynomial-time-reduction).

Thus $\mathcal L_{\mathrm{Clique}}\leq_p\mathcal L_{u\mathrm{Clique}}$. The unary version is in [NP](../../theoretical-computer-science.md#np-complexity) by the same [clique](../../graph-theory.md#clique-graph-theory) [complexity certificate](../../theoretical-computer-science.md#certificate-complexity) verification, and is [NP-hard](../../theoretical-computer-science.md#np-hardness) by this [polynomial-time many-one reduction](../../theoretical-computer-science.md#polynomial-time-many-one-reduction) and part (e). Therefore

$$
\boxed{\mathrm{Clique}\text{ is strongly NP-complete}.}
$$

This conclusion uses the conventional explicit [graph](../../graph.md) encoding; a succinct circuit description of a [graph](../../graph.md) would be a different [input](../../theoretical-computer-science.md#input-computer-science) representation and a different problem.

## 3

↑ **Parent:** [Computational complexity](computational-complexity.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use [Turing machines](../../theoretical-computer-science.md#turing-machine) with a two-way read-only [input](../../theoretical-computer-science.md#input-computer-science) tape, bounded by endmarkers, and a fixed finite number of read-write work tapes over a fixed finite [alphabet](../../information-theory.md#alphabet). Work-tape cells count towards [space complexity](../../theoretical-computer-science.md#space-complexity); the read-only [input](../../theoretical-computer-science.md#input-computer-science) does not. For [input](../../theoretical-computer-science.md#input-computer-science) length $n$, use $O(\log(n+2))$ to include the small-length cases.

**$\mathrm{Logspace}$, or [L](../../theoretical-computer-science.md#l-complexity), is the class of [formal languages](../../theoretical-computer-science.md#formal-language) decided by a deterministic such machine using at most $c\log(n+2)$ work-tape cells for some fixed constant $c$.** It must halt on every [input](../../theoretical-computer-science.md#input-computer-science) and accept exactly the members.

**$\mathrm{NLogspace}$, or [NL](../../theoretical-computer-science.md#nl-complexity), is the class of [formal languages](../../theoretical-computer-science.md#formal-language) accepted by a [Nondeterministic Turing machine](../../theoretical-computer-science.md#nondeterministic-turing-machine) with the same work-space bound on every computation branch.** An [input](../../theoretical-computer-science.md#input-computer-science) is accepted if and only if at least one branch accepts. One may require all branches to halt: the [configuration graph](../../theoretical-computer-science.md#configuration-graph) has only a [polynomial](../../polynomial.md) number of [vertices](../../graph.md#vertex-graph-theory), so a [logarithmic space](../../theoretical-computer-science.md#logarithmic-space) counter can stop any branch that has taken more steps than that bound. If an accepting computation exists, one exists with no repeated [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine), so this convention does not change the [complexity class](../../theoretical-computer-science.md#complexity-class).

In standard [space complexity](../../theoretical-computer-science.md#space-complexity) notation,

$$
\boxed{\mathrm L=\mathrm{DSPACE}(O(\log n)),\qquad
\mathrm{NL}=\mathrm{NSPACE}(O(\log n)).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) is a deterministic [Turing machine](../../theoretical-computer-science.md#turing-machine) with a read-only [input](../../theoretical-computer-science.md#input-computer-science) tape, $O(\log(n+2))$ read-write work space, and a write-only output tape. It emits symbols successively and cannot reread the output; that output is not charged as working memory. For a total function it must halt on every [input](../../theoretical-computer-science.md#input-computer-science). A [logspace-computable function](../../theoretical-computer-science.md#logspace-computable-function) $f$ is a total [function](../../function.md) whose output $f(x)$ is produced by such a [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) on [input](../../theoretical-computer-science.md#input-computer-science) $x$.

A [logspace many-one reduction](../../theoretical-computer-science.md#logspace-many-one-reduction) $A\leq_m^{\log}B$ is a [logspace-computable function](../../theoretical-computer-science.md#logspace-computable-function) $f$ such that

$$
\boxed{x\in A\quad\Longleftrightarrow\quad f(x)\in B}
$$

for every [string](../../foundations-of-mathematics.md#string) $x$. The [logarithmic space](../../theoretical-computer-science.md#logarithmic-space) bound permits a [polynomial](../../polynomial.md)-length output, even when that output does not fit in work space. Indeed, a halting [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) cannot repeat its state, [input](../../theoretical-computer-science.md#input-computer-science)-head position and work-tape contents and head positions: the unreadable output cannot affect its subsequent behaviour. There are only a [polynomial](../../polynomial.md) number of such internal [Turing machine configurations](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine), hence a [polynomial](../../polynomial.md) bound on the number of steps and output symbols.

To prove a [formal language](../../theoretical-computer-science.md#formal-language) $B$ is [NL-complete](../../theoretical-computer-science.md#nl-complete), first give an [NL](../../theoretical-computer-science.md#nl-complexity) acceptance procedure for $B$. Then show every $A\in\mathrm{NL}$ has a [logspace many-one reduction](../../theoretical-computer-science.md#logspace-many-one-reduction) to $B$. Alternatively, reduce one already [NL-complete](../../theoretical-computer-science.md#nl-complete) [formal language](../../theoretical-computer-science.md#formal-language) to $B$, using transitivity of [logspace many-one reductions](../../theoretical-computer-science.md#logspace-many-one-reduction).

Transitivity requires [logspace composition by recomputation](../../theoretical-computer-science.md#logspace-composition-by-recomputation), rather than storing the intermediate output. To compose $g$ with $f$, simulate the [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) for $g$ with a virtual [input](../../theoretical-computer-science.md#input-computer-science) $f(x)$. Retain its virtual [input](../../theoretical-computer-science.md#input-computer-science)-head position in $O(\log n)$ [bits](../../information-theory.md#bit). Whenever it asks for a symbol, rerun the [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) for $f$ from the beginning and count its output symbols until that position is reached. Since $|f(x)|$ is [polynomial](../../polynomial.md) in $n$, the simulated work space $O(\log|f(x)|)$ and all output-position counters are $O(\log n)$. Repeated runs reuse their storage. This proves closure under composition and explains why the hardness argument works.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let a deterministic [Turing machine](../../theoretical-computer-science.md#turing-machine) $M$ decide $A$ with at most $s(n)=c\log(n+2)$ work-tape cells. Fix an [input](../../theoretical-computer-science.md#input-computer-science) $x$ of length $n$. A [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) is determined by the control state, the read-only [input](../../theoretical-computer-science.md#input-computer-science)-head position, the work-tape contents, and the work-head positions. For one work tape with [alphabet](../../information-theory.md#alphabet) $\Gamma$, their number is bounded, up to harmless fixed factors, by

$$
|Q|(n+2)(s(n)+1)|\Gamma|^{s(n)}.
$$

The factors respectively count the state, [input](../../theoretical-computer-science.md#input-computer-science)-head position, work-head position and work-tape contents. With a fixed number $r$ of work tapes, replace the last two factors by $(s(n)+1)^r|\Gamma|^{rs(n)}$ if each tape is allowed $s(n)$ cells; this still gives a valid [polynomial](../../polynomial.md) upper bound. Two-way work tapes only change fixed factors in the head-position bounds.

Since

$$
|\Gamma|^{c\log_2(n+2)}
=(n+2)^{c\log_2|\Gamma|},
$$

there are at most $(n+2)^d$ [Turing machine configurations](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) for some constant $d$ depending on $M$. If a deterministic computation repeats one of its [Turing machine configurations](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) on the fixed [input](../../theoretical-computer-science.md#input-computer-science), all subsequent steps repeat too, so it never halts. But $M$ is a decider. It therefore halts before any repetition and takes at most a [polynomial](../../polynomial.md) number of steps. The same [Turing machine](../../theoretical-computer-science.md#turing-machine) is consequently a [polynomial-time algorithm](../../theoretical-computer-science.md#polynomial-time-algorithm), establishing

$$
\boxed{\mathrm{Logspace}\subseteq\mathrm{PTime}.}
$$

It would be incorrect to count just the work-tape contents and omit the read-only [input](../../theoretical-computer-science.md#input-computer-science)-head position; that position is part of the [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) even though the [input](../../theoretical-computer-science.md#input-computer-science) itself is not charged as work space.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

**Directed reachability is [NL-complete](../../theoretical-computer-science.md#nl-complete) under [logspace many-one reductions](../../theoretical-computer-science.md#logspace-many-one-reduction).** For membership, let $N$ be the number of [vertices](../../graph.md#vertex-graph-theory). Store a current [vertex](../../graph.md#vertex-graph-theory), initially $v$, and a counter initially zero. Accept immediately if the current [vertex](../../graph.md#vertex-graph-theory) is $v'$. Otherwise guess a next [vertex](../../graph.md#vertex-graph-theory), verify by scanning the [input](../../theoretical-computer-science.md#input-computer-science) that the appropriate directed [edge](../../graph-theory.md#edge-of-a-graph) exists, move there and increment the counter. Reject a branch that has made $N-1$ steps without reaching $v'$.

Whenever a directed [walk](../../graph-theory.md#walk-in-a-graph) reaches $v'$, removing closed portions between repeated [vertices](../../graph.md#vertex-graph-theory) produces a [path in a graph](../../graph-theory.md#path-in-a-graph) with at most $N-1$ [edges](../../graph-theory.md#edge-of-a-graph). Thus this bound preserves all yes-instances. The current and guessed [vertices](../../graph.md#vertex-graph-theory) and the counter use $O(\log N)$ [bits](../../information-theory.md#bit), while adjacency checks only need repeated read-only [input](../../theoretical-computer-science.md#input-computer-science) scans. All branches halt, so directed reachability belongs to [NL](../../theoretical-computer-science.md#nl-complexity).

For hardness, let $A\in\mathrm{NL}$ and fix a [Nondeterministic Turing machine](../../theoretical-computer-science.md#nondeterministic-turing-machine) $M$ accepting $A$ in $O(\log n)$ work space. On [input](../../theoretical-computer-science.md#input-computer-science) $x$, construct its [configuration graph](../../theoretical-computer-science.md#configuration-graph) $C_x$. A [vertex](../../graph.md#vertex-graph-theory) is a possible [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) within the fixed work-space bound. Put a directed [edge](../../graph-theory.md#edge-of-a-graph) $C\to D$ exactly when one legal transition of $M$ on $x$ changes $C$ into $D$. Take the initial [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine) as source, and add a fresh target $t$ with an incoming [edge](../../graph-theory.md#edge-of-a-graph) from every accepting [Turing machine configuration](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine). Then

$$
x\in A
\quad\Longleftrightarrow\quad
\text{the initial configuration reaches }t\text{ in }C_x.
$$

There are only a [polynomial](../../polynomial.md) number of [Turing machine configurations](../../theoretical-computer-science.md#instantaneous-description-of-a-turing-machine), by the count used in part (c). More importantly, their encodings have length $O(\log n)$. A [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) can enumerate candidate encodings and pairs of candidate encodings with $O(\log n)$ [bits](../../information-theory.md#bit) of counters. For each pair, it checks the finite transition rule, the scanned [input](../../theoretical-computer-science.md#input-computer-science) symbol and the local work-tape change using $O(\log n)$ work space. It emits the corresponding [adjacency matrix](../../graph-theory.md#adjacency-matrix) entry or [edge](../../graph-theory.md#edge-of-a-graph)-list record. Invalid candidate encodings may be discarded or represented by isolated [vertices](../../graph.md#vertex-graph-theory).

The [configuration graph](../../theoretical-computer-science.md#configuration-graph) is thus output by a [logspace transducer](../../theoretical-computer-science.md#logspace-transducer), rather than stored in its work tapes. This supplies the required [logspace many-one reduction](../../theoretical-computer-science.md#logspace-many-one-reduction) from every $A\in\mathrm{NL}$ and proves [NL-completeness](../../theoretical-computer-science.md#nl-complete).

$$
\boxed{\mathrm{Reachability}\text{ is NL-complete}.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The printed question calls the route a [path in a graph](../../graph-theory.md#path-in-a-graph) and writes $p\subseteq E(G)$, without specifying whether repeated [vertices](../../graph.md#vertex-graph-theory) are allowed.[Printed p. 4, Question 3(e)](../../computer-science-bibliography.md#computational-complexity-examination-paper-of-the-university-of-oxford-2015) Use the computational reachability convention that a permitted route is a directed [walk](../../graph-theory.md#walk-in-a-graph): repeated [vertices](../../graph.md#vertex-graph-theory) are allowed and length counts traversed [edges](../../graph-theory.md#edge-of-a-graph) with multiplicity. This matters for the [integer parity](../../integer.md#parity-mathematics) restriction, because deleting a closed portion of odd length can change the [integer parity](../../integer.md#parity-mathematics). The proof below establishes the stated [NL](../../theoretical-computer-science.md#nl-complexity)-completeness for this convention; it does not establish that claim for a simple [path in a graph](../../graph-theory.md#path-in-a-graph).

For membership of [even-length directed reachability](../../theoretical-computer-science.md#even-length-directed-reachability) in [NL](../../theoretical-computer-science.md#nl-complexity), form the conceptual parity [graph](../../graph.md) with [vertex set](../../graph.md#vertex-set)

$$
V(G)\times\{0,1\}
$$

and directed [edges](../../graph-theory.md#edge-of-a-graph)

$$
(u,b)\longrightarrow(w,1-b)
\quad\Longleftrightarrow\quad (u,w)\in E(G).
$$

After a directed [walk](../../graph-theory.md#walk-in-a-graph) of length $j$ from $(v,0)$, the second coordinate equals $j\bmod2$. Therefore there is an even-length directed [walk](../../graph-theory.md#walk-in-a-graph) from $v$ to $v'$ in $G$ exactly when $(v',0)$ is reachable from $(v,0)$ in this parity [graph](../../graph.md). It has $2N$ [vertices](../../graph.md#vertex-graph-theory). Guess successive [edges](../../graph-theory.md#edge-of-a-graph) while storing the original current [vertex](../../graph.md#vertex-graph-theory), one [parity bit](../../coding-theory.md#parity-bit), and a counter bounded by $2N-1$. If the target pair is reachable, it has a simple [path in a graph](../../graph-theory.md#path-in-a-graph) in this enlarged [graph](../../graph.md) of at most $2N-1$ [edges](../../graph-theory.md#edge-of-a-graph). This is an [NL](../../theoretical-computer-science.md#nl-complexity) procedure; the parity [graph](../../graph.md) need not be materialized.

For [NL](../../theoretical-computer-science.md#nl-complexity)-hardness, reduce directed reachability by subdividing each directed [edge](../../graph-theory.md#edge-of-a-graph) $(u,w)$ with its own new [vertex](../../graph.md#vertex-graph-theory) $a_{uw}$:

$$
u\longrightarrow a_{uw}\longrightarrow w.
$$

Retain $v,v'$ as the endpoints and add no other [edges](../../graph-theory.md#edge-of-a-graph). Every original directed [walk](../../graph-theory.md#walk-in-a-graph) of length $j$ becomes a directed [walk](../../graph-theory.md#walk-in-a-graph) of even length $2j$. Conversely, a directed [walk](../../graph-theory.md#walk-in-a-graph) between original [vertices](../../graph.md#vertex-graph-theory) in the new [graph](../../graph.md) must alternate original and subdivision [vertices](../../graph.md#vertex-graph-theory). Compressing each two-[edge](../../graph-theory.md#edge-of-a-graph) segment recovers a directed [walk](../../graph-theory.md#walk-in-a-graph) in $G$. Hence

$$
\langle G,v,v'\rangle\in\mathrm{Reachability}
\quad\Longleftrightarrow\quad
\langle G',v,v'\rangle\in\mathrm{E\text{-}Reachability}.
$$

A [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) enumerates the original [edges](../../graph-theory.md#edge-of-a-graph), labels each new [vertex](../../graph.md#vertex-graph-theory) by its [edge](../../graph-theory.md#edge-of-a-graph) endpoints or its position in the [input](../../theoretical-computer-science.md#input-computer-science), and emits its two replacement [edges](../../graph-theory.md#edge-of-a-graph). All labels and counters take $O(\log n)$ [bits](../../information-theory.md#bit), and the output is of [polynomial](../../polynomial.md) size. Thus this is a [logspace many-one reduction](../../theoretical-computer-science.md#logspace-many-one-reduction), proving

$$
\boxed{\mathrm{E\text{-}Reachability}\text{ is NL-complete}.}
$$

As in ordinary reachability, a zero-length directed [walk](../../graph-theory.md#walk-in-a-graph) is permitted, so $v=v'$ is an immediate yes-instance. Both the membership procedure and the subdivision [many-one reduction](../../computability-theory.md#many-one-reduction) preserve that case.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

The [binary numeral system](../../integer.md#binary-numeral-system) representation is taken to be canonical, with no leading zeroes, for each positive [integer](../../integer.md). Delimiters separate the components of a pair or triple. Syntax, positivity and this representation convention can all be checked in [logarithmic space](../../theoretical-computer-science.md#logarithmic-space). The useful principle is that a large [integer](../../integer.md) need not be stored in order to compute its digits one at a time.

First consider Add. Let $x_i,y_i,z_i$ denote the [binary digits](../../integer.md#binary-digit) in position $i$, counting from the least significant position $i=0$ and taking out-of-range digits to be zero. Count the component lengths, and let $L$ be their maximum. Start with [arithmetic carry](../../arithmetic.md#carry-arithmetic) $c_0=0$. For $i=0,\ldots,L-1$, compute

$$
t_i=x_i+y_i+c_i,\qquad
s_i=t_i\bmod2,\qquad
c_{i+1}=\left\lfloor\frac{t_i}2\right\rfloor.
$$

Reject if $s_i\ne z_i$ at any position. After the last position, reject if $c_L=1$; otherwise accept. The final [arithmetic carry](../../arithmetic.md#carry-arithmetic) check prevents accepting a result with an omitted high digit, such as the false equality $11_2+11_2=10_2$ obtained by retaining only two [binary digits](../../integer.md#binary-digit).

The [binary-addition carry invariant](../../arithmetic.md#binary-addition-carry-invariant) is

$$
\sum_{j<i}x_j2^j+\sum_{j<i}y_j2^j
=\sum_{j<i}s_j2^j+c_i2^i.
$$

It holds initially and is preserved by the displayed one-column equations. At the end, it proves that the comparisons and the final [arithmetic carry](../../arithmetic.md#carry-arithmetic) check succeed exactly when $x+y=z$. Each requested [binary digit](../../integer.md#binary-digit) is recovered by scanning the corresponding [input](../../theoretical-computer-science.md#input-computer-science) field and counting to its position. The length counters, position $i$ and scan counters require $O(\log n)$ [bits](../../information-theory.md#bit), while $c_i$ and $t_i\in\{0,1,2,3\}$ require constant space. Thus

$$
\boxed{\mathrm{Add}\in\mathrm L.}
$$

For Pal-Add, construct a [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) producing the canonical [binary numeral system](../../integer.md#binary-numeral-system) representation of $x+y$. Put $m=\max(|x|,|y|)$. One least-to-most-significant pass using the same recurrence determines the final [arithmetic carry](../../arithmetic.md#carry-arithmetic) $c_m$. Positivity and canonical representations imply that the sum's digit length is

$$
\ell=\begin{cases}m+1,&c_m=1,\\m,&c_m=0.\end{cases}
$$

Indeed, one summand is at least $2^{m-1}$ and both are less than $2^m$. For each output position, from $\ell-1$ down to $0$, recompute the required sum digit from scratch: reset the [arithmetic carry](../../arithmetic.md#carry-arithmetic) to zero and run the column recurrence from position $0$ up to the requested position, reading [input](../../theoretical-computer-science.md#input-computer-science) digits by scans. Positions beyond the summands use zero digits, so position $m$ correctly emits the possible final [arithmetic carry](../../arithmetic.md#carry-arithmetic). Emit only the requested digit, then reuse the work space for the next position.

This produces most-significant-first output with $\ell\leq m+1$ digits. It uses $O(\log n)$ work space because it retains only a fixed number of digit indices, lengths, scan counters and one [arithmetic carry](../../arithmetic.md#carry-arithmetic); it never stores the whole sum. A direct implementation with repeated whole-[input](../../theoretical-computer-science.md#input-computer-science) scans uses at most $O(n^3)$ [time complexity](../../theoretical-computer-science.md#time-complexity), which is sufficient here. Hence $(x,y)\mapsto\operatorname{bin}(x+y)$ is a [logspace-computable function](../../theoretical-computer-science.md#logspace-computable-function).

Finally simulate the assumed [L](../../theoretical-computer-science.md#l-complexity) decider for [binary palindrome](../../integer.md#binary-palindrome) on this virtual output, using [logspace composition by recomputation](../../theoretical-computer-science.md#logspace-composition-by-recomputation) from part (b). Whenever the simulated [input](../../theoretical-computer-science.md#input-computer-science) head asks for a digit, rerun the addition [logspace transducer](../../theoretical-computer-science.md#logspace-transducer) until it emits that digit. The virtual [input](../../theoretical-computer-science.md#input-computer-science) length is $O(n)$, so both its work space and the addition work space are $O(\log n)$. The simulation accepts exactly when the canonical representation of $x+y$ is a [binary palindrome](../../integer.md#binary-palindrome). Therefore

$$
\boxed{\mathrm{Pal\text{-}Add}\in\mathrm L.}
$$

Equivalently, one could directly compare the sum digits in positions $i$ and $\ell-1-i$, recomputing each digit by the same recurrence. This gives the same [logarithmic space](../../theoretical-computer-science.md#logarithmic-space) conclusion without ever writing the full sum on a work tape.

## ↑ Ancestors (8)

1. [2015](../2015.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
