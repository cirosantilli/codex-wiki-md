# Paper 21

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_21.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_21.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

**There is no computable presentation of a [nonstandard model of Peano arithmetic](../../../mathematical-logic.md#non-standard-model-of-arithmetic).** We prove [Tennenbaum theorem](../../../mathematical-logic.md#tennenbaum-s-theorem) by obtaining a [computable set](../../../foundations-of-mathematics.md#computable-set) separating two [recursively inseparable sets](../../../foundations-of-mathematics.md#recursively-inseparable-sets).

Fix an effective enumeration $(\varphi_e)$ of [partial computable functions](../../../foundations-of-mathematics.md#computable-function), implemented by deterministic machines, and put

$$
U=\{e:\varphi_e(e)\downarrow=0\},\qquad V=\{e:\varphi_e(e)\downarrow=1\}.
$$

These are disjoint [computably enumerable sets](../../../foundations-of-mathematics.md#recursively-enumerable-set). To see that they are [recursively inseparable sets](../../../foundations-of-mathematics.md#recursively-inseparable-sets), suppose a [computable set](../../../foundations-of-mathematics.md#computable-set) $D$ contains $U$ and avoids $V$. Its [indicator function](../../../measure-theory.md#indicator-function) has some index $k$. If $\varphi_k(k)=0$, then $k\in U\subseteq D$, contradicting that output. If $\varphi_k(k)=1$, then $k\in V$, contradicting $D\cap V=\varnothing$. Thus neither output is possible.

Let $M\models\mathrm{PA}$ be a [nonstandard model of Peano arithmetic](../../../mathematical-logic.md#non-standard-model-of-arithmetic). A [recursive presentation of a structure](../../../foundations-of-mathematics.md#recursive-presentation-of-a-structure) here means a presentation on $\mathbb N$ in which its arithmetic operations are [total computable functions](../../../foundations-of-mathematics.md#total-computable-function); equality of presentation codes is ordinary equality. Write $\bar n$ for the element represented by the standard numeral $n$. The presentation codes of $\bar0,\bar1$ are fixed constants, so $n\mapsto\bar n$ is a [total computable function](../../../foundations-of-mathematics.md#total-computable-function) obtained by repeated addition. Presentation codes and the arithmetic values they name must be kept distinct.

Use [bounded simulation of a computation](../../../foundations-of-mathematics.md#bounded-simulation-of-a-computation) predicates $H_i(e,t)$ saying that machine $e$, on input $e$, has halted by time $t$ with output $i$. We can choose these as [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function) predicates represented in [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic). Determinism and induction on the computation length give, provably in [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic), monotonicity in $t$ and

$$
\forall e\,\forall t\,\forall s\;\neg\bigl(H_0(e,t)\land H_1(e,s)\bigr).
$$

A genuine standard halting computation has a finite certificate which [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic) verifies. Consequently, if $e\in U$ or $e\in V$, the corresponding $H_i(\bar e,\bar t)$ holds in $M$ for some standard $t$.

Choose a nonstandard element $c$ of $M$. It exceeds every standard numeral. Let $p_e$ be the $e$th [prime number](../../../number-theory.md#prime-number), starting with $p_0=2$. [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic) proves the [prime-divisibility coding of a finite set](../../../mathematical-logic.md#prime-divisibility-coding-of-a-finite-set) needed here: for each $c$, an element $d$ can be formed as the product of precisely those $p_e$ with $e<c$ for which $H_0(e,c)$ holds. Formally,

$$
M\models\forall e<c\;\bigl(p_e\mid d\ \longleftrightarrow\ H_0(e,c)\bigr).
$$

This is an internally finite product, not a claim that its externally observed index set is finite. Its existence follows by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on the cutoff: start with $1$, multiply by the next distinct [prime number](../../../number-theory.md#prime-number) when its predicate holds, and otherwise retain the product. [Unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) ensures that earlier divisibility decisions are preserved. The standard prime enumeration and these finite-product constructions are provably total in [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic).

Define the external subset $D=\{e\in\mathbb N:M\models p_{\bar e}\mid d\}$. If $e\in U$, its standard halting time is below $c$, and monotonicity gives $H_0(\bar e,c)$, so $e\in D$. If $e\in V$, its output-one certificate and the provable incompatibility above exclude $H_0(\bar e,c)$, so $e\notin D$. Hence $D$ separates $U$ and $V$.

Finally $D$ is a [computable set](../../../foundations-of-mathematics.md#computable-set). Given standard $e$, compute the ordinary integer $p_e$ and its numeral in the presentation. Enumerate all presentation codes $q$, and for each test the finitely many standard remainders $0\le r<p_e$ for

$$
 d=\bar p_e\cdot q+\bar r.
$$

Each test is decidable using the assumed [total computable functions](../../../foundations-of-mathematics.md#total-computable-function). The division theorem of [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic) guarantees a quotient and a remainder below the standard numeral $\bar p_e$. Every element below that numeral is one of $\bar0,\ldots,\overline{p_e-1}$, so the search terminates; the remainder is unique. Return yes exactly when $r=0$. This makes $D$ a [computable set](../../../foundations-of-mathematics.md#computable-set), contradicting the [recursively inseparable sets](../../../foundations-of-mathematics.md#recursively-inseparable-sets) construction. Therefore

$$
\boxed{M\models\mathrm{PA}\text{ nonstandard}\ \Longrightarrow\ M\text{ has no recursive presentation}.}
$$

## 2

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

**The minimal [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton) is unique up to an [isomorphism](../../../algebra.md#isomorphism) preserving the initial state, transitions and accepting states.** We use complete [deterministic finite automata](../../../foundations-of-mathematics.md#deterministic-finite-automaton) over the fixed [alphabet](../../../information-theory.md#alphabet); the PDF's abbreviation FDA has this meaning. State names themselves cannot be unique.

For [words](../../../foundations-of-mathematics.md#string) $u,v\in\Sigma^*$, introduce the [Myhill-Nerode equivalence](../../../foundations-of-mathematics.md#myhill-nerode-equivalence)

$$
u\sim_Lv\quad\Longleftrightarrow\quad\forall w\in\Sigma^*\;\bigl(uw\in L\iff vw\in L\bigr).
$$

It is an [equivalence relation](../../../set-theory.md#equivalence-relation), and appending the same letter to equivalent [words](../../../foundations-of-mathematics.md#string) preserves it: a suffix $w$ after $ua$ is the suffix $aw$ after $u$. Since $L$ is a [regular language](../../../foundations-of-mathematics.md#regular-language), take any recognizing [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton). Words reaching the same state are equivalent, since every further suffix gives the same computation. Thus $\sim_L$ has finite index.

The [canonical residual automaton](../../../foundations-of-mathematics.md#canonical-residual-automaton) has one state $[u]$ for each class, initial state $[\epsilon]$, transition $[u]\xrightarrow{a}[ua]$, and accepting states those with $u\in L$. These choices are well-defined by [Myhill-Nerode equivalence](../../../foundations-of-mathematics.md#myhill-nerode-equivalence). Induction on the input length shows that reading $u$ reaches $[u]$, so the [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton) recognizes $L$, and all its states are [accessible states of a deterministic finite automaton](../../../foundations-of-mathematics.md#accessible-state-of-a-deterministic-finite-automaton). The same state can be described by the [left quotient of a formal language](../../../foundations-of-mathematics.md#left-quotient-of-a-formal-language)

$$
u^{-1}L=\{w:uw\in L\}.
$$

Two states are different precisely when some suffix distinguishes their acceptance behavior.

Every recognizing [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton) has at least as many states as there are classes: pick a representative from each class; two different representatives cannot reach the same state. The [canonical residual automaton](../../../foundations-of-mathematics.md#canonical-residual-automaton) attains this bound, and therefore is a [minimal deterministic finite automaton](../../../foundations-of-mathematics.md#minimal-deterministic-finite-automaton).

For uniqueness, let $\mathcal A$ be any [minimal deterministic finite automaton](../../../foundations-of-mathematics.md#minimal-deterministic-finite-automaton). All its states are accessible, since removing inaccessible states leaves a complete recognizing [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton) with fewer states. Map a state reached by $u$ to $[u]$. This is well-defined because two [words](../../../foundations-of-mathematics.md#string) reaching the same state are equivalent. It is surjective because every class has a representative. Both sets have the minimal number of states, so it is a [bijection](../../../function.md#bijection). It preserves the initial state and transitions by construction, and preserves accepting states by taking the [empty word](../../../foundations-of-mathematics.md#empty-word) as the suffix. This is the required [isomorphism](../../../algebra.md#isomorphism) with the [canonical residual automaton](../../../foundations-of-mathematics.md#canonical-residual-automaton), proving

$$
\boxed{\text{minimal number of states}=|\Sigma^*/{\sim_L}|,\quad\text{uniqueness up to isomorphism}.}
$$

The [empty word](../../../foundations-of-mathematics.md#empty-word) is included throughout, and empty or universal [regular languages](../../../foundations-of-mathematics.md#regular-language) have the corresponding one-state complete [deterministic finite automata](../../../foundations-of-mathematics.md#deterministic-finite-automaton).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

**Yes: [regular languages](../../../foundations-of-mathematics.md#regular-language) are closed under the [shuffle of formal languages](../../../foundations-of-mathematics.md#shuffle-of-formal-languages).** The construction must allow letters common to both [alphabets](../../../information-theory.md#alphabet) to be assigned to either input [word](../../../foundations-of-mathematics.md#string).

Take complete [deterministic finite automata](../../../foundations-of-mathematics.md#deterministic-finite-automaton) $\mathcal A_i=(Q_i,\Sigma_i,\delta_i,s_i,F_i)$ recognizing $L_i$. Construct a [nondeterministic finite automaton](../../../foundations-of-mathematics.md#nondeterministic-finite-automaton) on $Q_1\times Q_2$ over $\Sigma=\Sigma_1\cup\Sigma_2$. Its initial state is $(s_1,s_2)$ and its accepting states form $F_1\times F_2$. On a letter $a$, its possible moves from $(p,q)$ are

$$
\begin{aligned}
(p,q)&\longrightarrow(\delta_1(p,a),q)&&\text{if }a\in\Sigma_1,\\
(p,q)&\longrightarrow(p,\delta_2(q,a))&&\text{if }a\in\Sigma_2.
\end{aligned}
$$

Both moves are allowed when $a$ belongs to both [alphabets](../../../information-theory.md#alphabet). They may coincide; that causes no difficulty.

For every run, record whether each move updated the first or the second coordinate. The letters assigned to each coordinate, in their original order, form two [words](../../../foundations-of-mathematics.md#string) $u_1,u_2$. The final coordinate states are exactly the states reached by reading $u_i$ in $\mathcal A_i$. Thus an accepting run expresses the input as an interleaving of a [word](../../../foundations-of-mathematics.md#string) of $L_1$ and a [word](../../../foundations-of-mathematics.md#string) of $L_2$.

Conversely, given such an interleaving, assign each input position to the [word](../../../foundations-of-mathematics.md#string) from which it came. The corresponding choices of transitions form a run ending in $F_1\times F_2$. This proves equality between the recognized [formal language](../../../computer-science.md#formal-language) and the [shuffle of formal languages](../../../foundations-of-mathematics.md#shuffle-of-formal-languages), in both directions. No assumption of disjoint [alphabets](../../../information-theory.md#alphabet) is needed. If one contributing [word](../../../foundations-of-mathematics.md#string) is the [empty word](../../../foundations-of-mathematics.md#empty-word), no move need update that coordinate; the initial pair is accepting exactly when both [empty words](../../../foundations-of-mathematics.md#empty-word) are accepted.

Apply the [powerset construction](../../../foundations-of-mathematics.md#powerset-construction) to this [nondeterministic finite automaton](../../../foundations-of-mathematics.md#nondeterministic-finite-automaton) to obtain a [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton). In particular,

$$
\boxed{L_1\oplus L_2\text{ is regular},\qquad \text{a recognizing DFA has at most }2^{|Q_1||Q_2|}\text{ states}.}
$$

## 3

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

**Every countable structure in a countable [first-order language](../../../mathematical-logic.md#first-order-language) has a [Scott sentence](../../../mathematical-logic.md#scott-sentence) whose countable models are precisely its [isomorphic](../../../algebra.md#isomorphism) copies.** In particular two countable structures with the same [countable infinitary logic](../../../mathematical-logic.md#countable-infinitary-logic) sentences are [isomorphic](../../../algebra.md#isomorphism). Countability of both structures is essential to the back-and-forth conclusion; the sentence need not exclude uncountable models.

Let $M$ be a nonempty countable structure in a countable [first-order language](../../../mathematical-logic.md#first-order-language). The [countable infinitary logic](../../../mathematical-logic.md#countable-infinitary-logic) $L_{\omega_1,\omega}$ permits countable [logical conjunctions](../../../mathematical-logic.md#logical-conjunction) and [logical disjunctions](../../../mathematical-logic.md#logical-disjunction), but only finite strings of quantifiers and finitely many [free variables](../../../mathematical-logic.md#free-variable) in each formula. We construct a [Scott formula](../../../mathematical-logic.md#scott-formula) $\phi_{\bar a}^{\alpha}(\bar x)$ for every finite [tuple](../../../set-theory.md#finite-tuple) $\bar a$ from $M$ and every countable [ordinal](../../../set-theory.md#ordinal) $\alpha$.

At stage zero, let $\phi_{\bar a}^{0}$ be the conjunction of all [atomic formulas](../../../mathematical-logic.md#atomic-formula) true of $\bar a$ and the negations of all [atomic formulas](../../../mathematical-logic.md#atomic-formula) false of $\bar a$. Include atomic formulas involving arbitrary terms and constants, not just relation symbols applied directly to variables. There are only countably many such formulas. This complete atomic description ensures that matching [tuples](../../../set-theory.md#finite-tuple) determine a [partial isomorphism of structures](../../../foundations-of-mathematics.md#partial-embedding).

At successors put

$$
\begin{aligned}
\phi_{\bar a}^{\alpha+1}(\bar x)=\;&\phi_{\bar a}^{\alpha}(\bar x)\\
&\land\bigwedge_{b\in M}\exists y\;\phi_{\bar a,b}^{\alpha}(\bar x,y)\\
&\land\forall y\;\bigvee_{b\in M}\phi_{\bar a,b}^{\alpha}(\bar x,y).
\end{aligned}
$$

At a nonzero limit [ordinal](../../../set-theory.md#ordinal) $\lambda<\omega_1$, put $\phi_{\bar a}^{\lambda}=\bigwedge_{\beta<\lambda}\phi_{\bar a}^{\beta}$. All these are formulas of [countable infinitary logic](../../../mathematical-logic.md#countable-infinitary-logic): each indexing set is countable, and the [free variables](../../../mathematical-logic.md#free-variable) are only the fixed finite [tuple](../../../set-theory.md#finite-tuple). Rename bound variables when necessary. [Transfinite induction](../../../set-theory.md#transfinite-induction) also shows $M\models\phi_{\bar a}^{\alpha}(\bar a)$.

For [tuples](../../../set-theory.md#finite-tuple) of the same length within $M$, define $\bar a\equiv_\alpha\bar b$ by $M\models\phi_{\bar a}^{\alpha}(\bar b)$. Induction identifies this with the usual symmetric [back-and-forth method](../../../foundations-of-mathematics.md#back-and-forth-method) equivalence: the [tuples](../../../set-theory.md#finite-tuple) have the same atomic description at stage zero, and at a successor every one-element extension on either side has a matching extension at the previous stage. Thus these are decreasing [equivalence relations](../../../set-theory.md#equivalence-relation), simultaneously for every finite [tuple](../../../set-theory.md#finite-tuple) length.

There are only countably many pairs of finite [tuples](../../../set-theory.md#finite-tuple) in $M$. A pair can cease to be equivalent at most once. The supremum of the first separation stages of all pairs that separate below $\omega_1$ is a countable [ordinal](../../../set-theory.md#ordinal). Choose a countable $\alpha$ at least that supremum. No pair can first separate at $\alpha+1$, so

$$
\equiv_\alpha\;=\;\equiv_{\alpha+1}\quad\text{on every }M^n.
$$

This justifies stabilization without assuming that all [tuples](../../../set-theory.md#finite-tuple) stabilize at one predetermined finite stage.

Now form the following [Scott sentence](../../../mathematical-logic.md#scott-sentence), where the case $n=0$ has no displayed variables or quantifiers:

$$
\sigma_M=\phi_{\varnothing}^{\alpha}\ \land\
\bigwedge_{n<\omega}\ \bigwedge_{\bar a\in M^n}
\forall\bar x\;\bigl(\phi_{\bar a}^{\alpha}(\bar x)\to\phi_{\bar a}^{\alpha+1}(\bar x)\bigr).
$$

It is a sentence of [countable infinitary logic](../../../mathematical-logic.md#countable-infinitary-logic), because the family of all finite [tuples](../../../set-theory.md#finite-tuple) is countable. The stabilization above and the truth of $\phi_{\varnothing}^{\alpha}$ show $M\models\sigma_M$.

Suppose a countable structure $N$ satisfies $\sigma_M$. Start with the empty matching [tuples](../../../set-theory.md#finite-tuple), and maintain $N\models\phi_{\bar a}^{\alpha}(\bar b)$. The corresponding conjunct of $\sigma_M$ upgrades this to $N\models\phi_{\bar a}^{\alpha+1}(\bar b)$. The existential conjuncts extend the match by any specified element of $M$. The universal-disjunction conjunct extends it by any specified element of $N$. The [atomic formula](../../../mathematical-logic.md#atomic-formula) information makes a new element on one side match a new element on the other, and makes repeated elements agree with their earlier matches.

Enumerate both structures and alternate these two extension steps, including the least element not yet covered at each step. The union is a [bijection](../../../function.md#bijection) preserving and reflecting every [atomic formula](../../../mathematical-logic.md#atomic-formula), hence an [isomorphism](../../../algebra.md#isomorphism); for function symbols, eventually include both a [tuple](../../../set-theory.md#finite-tuple) and the value of its function term to see explicitly that the function is preserved. For finite structures the same construction stops when both are covered. Conversely every [isomorphic](../../../algebra.md#isomorphism) copy of $M$ satisfies $\sigma_M$, since [isomorphisms](../../../algebra.md#isomorphism) preserve formulas of [countable infinitary logic](../../../mathematical-logic.md#countable-infinitary-logic) by induction on their construction. Therefore

$$
\boxed{\text{for countable }N,\qquad N\models\sigma_M\iff N\cong M.}
$$

If countable $M,N$ have the same $L_{\omega_1,\omega}$ sentences, $N$ satisfies this [Scott sentence](../../../mathematical-logic.md#scott-sentence) of $M$ and is [isomorphic](../../../algebra.md#isomorphism) to $M$. This proves [Scott isomorphism theorem](../../../mathematical-logic.md#scott-isomorphism-theorem).

## 4

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

**Yes. There is a [computable isomorphism](../../../foundations-of-mathematics.md#computable-isomorphism), obtained by an [effective back-and-forth construction](../../../foundations-of-mathematics.md#effective-back-and-forth-construction).** Decidability of the two orders makes the usual existence argument into an algorithm.

Maintain a finite [order-preserving](../../../set.md#order-preserving-function) [partial isomorphism of structures](../../../foundations-of-mathematics.md#partial-embedding) $f_s$ from $(\mathbb N,<_A)$ to $(\mathbb N,<_B)$, starting with the empty map. At a forth step, take the least ordinary natural number $a$ outside its domain. Look at the finitely many mapped elements below and above $a$ in $<_A$. Their images impose an [open interval](../../../topology.md#open-interval) in $<_B$: it lies above all the lower images and below all the upper images, with a missing bound interpreted as an unbounded side.

This interval contains a fresh element. If both bounds exist they are ordered correctly by the induction hypothesis; density supplies an element strictly between them. If there is just one bound, the absence of endpoints supplies an element beyond it; if there are no bounds, choose any element. Density and the absence of endpoints moreover give infinitely many points in every such [open interval](../../../topology.md#open-interval), so finitely many already used images can always be avoided.

Enumerate $b=0,1,2,\ldots$ in the ordinary presentation order, test whether $b$ is unused and satisfies every required $<_B$ inequality, and choose the first successful candidate. All tests are decidable, and the existence argument proves termination. Extend $f_s$ by $a\mapsto b$.

At a back step, take the least natural number outside the range, interchange the roles of $A$ and $B$, and carry out exactly the same search for a fresh preimage. Alternate forth and back steps. Every stage is an effective terminating finite computation, and every stage remains an [order-preserving](../../../set.md#order-preserving-function) [partial isomorphism of structures](../../../foundations-of-mathematics.md#partial-embedding).

Let $f=\bigcup_s f_s$. The least-unused scheduling puts every element of $A$ into the domain and every element of $B$ into the range. For example, after $n+1$ forth steps, all ordinary presentation numbers at most $n$ have been included, since each step removes the least missing one. Thus $f$ is a [bijection](../../../function.md#bijection) preserving and reflecting the orders. To compute $f(n)$, simulate the construction until $n$ appears in its domain; this terminates. The corresponding range search computes its inverse. Hence

$$
\boxed{f:(\mathbb N,<_A)\cong(\mathbb N,<_B),\qquad f,f^{-1}\text{ are computable}.}
$$

The searches use the decidable presentations, rather than a possibly ineffective choice of points in an abstract [dense linear order without endpoints](../../../foundations-of-mathematics.md#dense-linear-order-without-endpoints).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write $Q=(A\to B)\to A$ and $P=Q\to A$. The displayed formula is $(P\to B)\to B$. A proof of [logical implication](../../../mathematical-logic.md#logical-implication) may use its temporary assumption more than once; this is ordinary [natural deduction](../../../mathematical-logic.md#natural-deduction), not a linear proof system.

Assume $h:P\to B$, then $f:Q$, then $a:A$, then $g:Q$. The [identity weakening rule](../../../mathematical-logic.md#identity-weakening-rule) derives $a:A$ from the hypotheses $a:A$ and $g:Q$. Discharging $g$ by the [implication introduction rule](../../../mathematical-logic.md#implication-introduction-rule) gives $\lambda g^Q.a:P$. Applying $h$ by the [implication elimination rule](../../../mathematical-logic.md#implication-elimination-rule) gives $h(\lambda g^Q.a):B$. Discharge $a$ to obtain $\lambda a^A.h(\lambda g^Q.a):A\to B$. Applying $f$ gives an $A$; discharge $f$ to obtain a $P$; apply $h$ once more to obtain $B$, and finally discharge $h$.

Here is the complete decorated [natural deduction](../../../mathematical-logic.md#natural-deduction) derivation, split at its intermediate $A\to B$ conclusion to keep the tree readable. Superscript labels mark which assumption occurrences are discharged; both occurrences labelled $1$ are discharged together.

$$
\frac{
 \frac{
  [h:P\to B]^1\qquad
  \frac{\frac{[a:A]^3\quad[g:Q]^4}{a:A}\;\mathrm{Id}}
  {\lambda g^Q.a:P}\;\to I_4
 }{h(\lambda g^Q.a):B}\;\to E
}{\lambda a^A.h(\lambda g^Q.a):A\to B}\;\to I_3
$$

To avoid an excessively wide final tree, continue the same derivation as follows, using the right-hand derived premise above:

$$
\frac{
 \frac{
  [f:Q]^2\qquad \lambda a^A.h(\lambda g^Q.a):A\to B
 }{f(\lambda a^A.h(\lambda g^Q.a)):A}\;\to E
}{\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a)):P}\;\to I_2
$$

followed by

$$
\frac{
 \frac{[h:P\to B]^1\quad\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a)):P}
 {h(\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a))):B}\;\to E
}{\lambda h^{P\to B}.h(\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a))):(P\to B)\to B}\;\to I_1.
$$

Thus the concise [lambda term](../../../foundations-of-mathematics.md#lambda-term), with bound-variable types determined by the displayed tree, is

$$
\boxed{\lambda h.\;h\bigl(\lambda f.\;f(\lambda a.\;h(\lambda g.\;a))\bigr).}
$$

Under the [Curry-Howard correspondence](../../../mathematical-logic.md#curry-howard-correspondence), [implication introduction rules](../../../mathematical-logic.md#implication-introduction-rule) correspond to [lambda abstractions](../../../foundations-of-mathematics.md#lambda-abstraction), [implication elimination rules](../../../mathematical-logic.md#implication-elimination-rule) to applications, and the [identity weakening rule](../../../mathematical-logic.md#identity-weakening-rule) retains the first term while allowing an unused second hypothesis. No other inference rule or classical axiom is required.

## 5

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

A [well-quasi-ordering](../../../set.md#well-quasi-ordering) is a reflexive transitive relation for which every infinite [sequence](../../../real-analysis.md#sequence) has $i<j$ with $x_i\le x_j$. A [bad sequence](../../../set.md#bad-sequence) has no such pair. **The [labelled version of Kruskal's tree theorem](../../../set.md#labelled-version-of-kruskal-s-tree-theorem) says that finite [rooted trees](../../../combinatorics.md#rooted-tree) labelled in any [well-quasi-ordering](../../../set.md#well-quasi-ordering) are themselves [well-quasi-ordered](../../../set.md#well-quasi-ordering) by [label-monotone tree embedding](../../../combinatorics.md#label-monotone-tree-embedding).**

More explicitly, an embedding is an injective map of vertices preserving [lowest common ancestors](../../../combinatorics.md#lowest-common-ancestor), and satisfying $\ell_T(v)\le\ell_S(h(v))$ at every vertex. The root need not map to the host root. This is a [homeomorphic embedding of a rooted tree](../../../combinatorics.md#homeomorphic-embedding-of-a-rooted-tree): an edge can map to a longer path, but distinct branches must separate at the image of their common ancestor. We shall prove the stronger version in which every vertex's children are linearly ordered and embeddings respect that ordering. Forgetting the child order gives the stated result for unordered [rooted trees](../../../combinatorics.md#rooted-tree).

We first establish the two [well-quasi-ordering](../../../set.md#well-quasi-ordering) facts used in the proof. Every infinite [sequence](../../../real-analysis.md#sequence) in a [well-quasi-ordering](../../../set.md#well-quasi-ordering) has an infinite nondecreasing [subsequence](../../../real-analysis.md#subsequence). Indeed, color an index pair $i<j$ according to whether $x_i\le x_j$. The infinite two-color [Ramsey theorem](../../../graph-theory.md#ramsey-theorem) gives a homogeneous infinite set; the negative color would be a [bad sequence](../../../set.md#bad-sequence), so the positive color gives the required [subsequence](../../../real-analysis.md#subsequence). It follows that the componentwise product of two [well-quasi-orderings](../../../set.md#well-quasi-ordering) is a [well-quasi-ordering](../../../set.md#well-quasi-ordering): first extract a nondecreasing [subsequence](../../../real-analysis.md#subsequence) in one coordinate, then find a good pair in the other.

Next prove [Higman lemma](../../../set.md#higman-s-lemma): finite [words](../../../foundations-of-mathematics.md#string) over a [well-quasi-ordering](../../../set.md#well-quasi-ordering) $Q$, ordered by subsequence embedding with coordinatewise increase of letters, are a [well-quasi-ordering](../../../set.md#well-quasi-ordering). Suppose not, and choose a [minimal bad sequence](../../../set.md#minimal-bad-sequence) $w_0,w_1,\ldots$ by making the length of $w_n$ minimal among all choices admitting an infinite bad continuation of the already fixed prefix. No [word](../../../foundations-of-mathematics.md#string) is the [empty word](../../../foundations-of-mathematics.md#empty-word), since that embeds in every later [word](../../../foundations-of-mathematics.md#string). Write $w_n=v_na_n$ with $a_n\in Q$. Extract indices $i_0<i_1<\cdots$ for which $a_{i_0}\le a_{i_1}\le\cdots$. Consider

$$
w_0,\ldots,w_{i_0-1},v_{i_0},v_{i_1},\ldots.
$$

It cannot be a [bad sequence](../../../set.md#bad-sequence), since its first replacement is shorter than the minimal choice $w_{i_0}$. But a good pair within the original prefix is impossible. A prefix [word](../../../foundations-of-mathematics.md#string) embedding into $v_{i_j}$ would embed into $w_{i_j}$, contradicting the original [bad sequence](../../../set.md#bad-sequence). And $v_{i_j}$ embedding into $v_{i_k}$ would, after appending the ordered last letters, embed $w_{i_j}$ into $w_{i_k}$, also impossible. This contradiction proves [Higman lemma](../../../set.md#higman-s-lemma), including [words](../../../foundations-of-mathematics.md#string) of arbitrary finite length.

Now suppose there is a [bad sequence](../../../set.md#bad-sequence) of finite ordered labelled [rooted trees](../../../combinatorics.md#rooted-tree). Choose a [minimal bad sequence](../../../set.md#minimal-bad-sequence) $T_0,T_1,\ldots$ by minimizing the number of vertices of $T_n$, subject to the fixed prefix having an infinite bad continuation. Existence of a least possible size uses ordinary well-ordering of the natural numbers; after selecting such a tree retain a bad continuation to make the next choice.

Let $\mathcal S$ be the collection of all proper rooted subtrees of all $T_n$, with inherited labels and child ordering. These are the subtrees rooted at vertices other than the root, and each embeds into its containing tree. We claim $\mathcal S$ is a [well-quasi-ordering](../../../set.md#well-quasi-ordering) under the same [label-monotone tree embedding](../../../combinatorics.md#label-monotone-tree-embedding).

Otherwise choose a [bad sequence](../../../set.md#bad-sequence) $U_0,U_1,\ldots$ from $\mathcal S$, and choose for each a containing tree $T_{n_j}$. The indices $n_j$ are unbounded in every tail: finitely many containing trees have only finitely many rooted subtrees, and an infinite [bad sequence](../../../set.md#bad-sequence) cannot repeatedly use one of these, since it embeds into itself. Passing to a [subsequence](../../../real-analysis.md#subsequence), arrange $n_0<n_1<\cdots$. The spliced [sequence](../../../real-analysis.md#sequence)

$$
T_0,\ldots,T_{n_0-1},U_0,U_1,\ldots
$$

is bad. A good pair within either piece is already excluded. A comparison $T_k\preceq U_j$, where $k<n_0\le n_j$, would compose with $U_j\preceq T_{n_j}$ to give $T_k\preceq T_{n_j}$, contradicting the original [bad sequence](../../../set.md#bad-sequence). But $U_0$ is smaller than $T_{n_0}$, contradicting the minimal choice at that position. This proves the claim about $\mathcal S$.

Describe $T_n$ by its root label $q_n\in Q$ and its finite ordered list $C_n$ of child subtrees. Every entry of $C_n$ lies in $\mathcal S$. By [Higman lemma](../../../set.md#higman-s-lemma), $\mathcal S^*$ is a [well-quasi-ordering](../../../set.md#well-quasi-ordering); hence so is $Q\times\mathcal S^*$. There exist $i<j$ with $q_i\le q_j$ and an increasing injection matching the child subtrees in $C_i$ to child subtrees in $C_j$, each by an embedding. Map root to root and combine these child embeddings. Different matched children lie in different target branches, so their paths meet exactly at the target root; within each branch the chosen embedding already preserves [lowest common ancestors](../../../combinatorics.md#lowest-common-ancestor). The resulting map is a [label-monotone tree embedding](../../../combinatorics.md#label-monotone-tree-embedding) $T_i\preceq T_j$, a contradiction. Therefore

$$
\boxed{Q\text{ wqo}\quad\Longrightarrow\quad\mathcal T(Q)\text{ wqo under labelled homeomorphic embedding}.}
$$

The empty labelled tree, if included by convention, embeds into every tree and causes no exception. A common stronger formulation requires the source root to map to the target root. It also follows: the theorem just proved makes all labelled child subtrees a [well-quasi-ordering](../../../set.md#well-quasi-ordering), and the product $Q\times\mathcal T(Q)^*$ then provides a good pair with roots explicitly matched, by the same final assembly. Internal child roots may map further down their matched branches. This must not be confused with edge-to-edge embedding, for which the theorem is false in general.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

**As printed, yes: the relation is universal.** The original PDF puts the existentially quantified element in the same subset as the universally quantified element; this is not an OCR substitution. For each element of that subset, choose the element itself as witness, using reflexivity of the underlying [well-quasi-ordering](../../../set.md#well-quasi-ordering). For an empty subset the condition is vacuous. The truth value therefore never depends on the proposed target subset. On the [power set](../../../set.md#power-set) this is a reflexive transitive relation, and every two terms of any infinite [sequence](../../../real-analysis.md#sequence) are related:

$$
\boxed{\text{literal printed relation}=\mathcal P(X)\times\mathcal P(X),\qquad\text{hence it is a well-quasi-ordering}.}
$$

A [well-quasi-ordering](../../../set.md#well-quasi-ordering) need not be antisymmetric, so universal comparability is allowed.

If the existential element is instead intended to belong to the target subset, the natural relation is the [Hoare domination preorder](../../../set.md#hoare-domination-preorder)

$$
S\le_H T\quad\Longleftrightarrow\quad\forall s\in S\;\exists t\in T\;(s\le_Xt).
$$

**For arbitrary subsets the answer to that corrected question is no.** Here is a complete counterexample, the [Rado order](../../../set.md#rado-order). Take

$$
R=\{(m,n)\in\mathbb N^2:m<n\},\qquad
(m,n)\le_R(k,l)\quad\Longleftrightarrow\quad
\bigl(m=k\text{ and }n\le l\bigr)\ \text{or}\ n<k.
$$

This is a [partial order](../../../set.md#partially-ordered-set). Reflexivity is immediate. For transitivity, two same-row comparisons compose ordinarily. If the first comparison crosses rows and the second stays in its row, its target first coordinate is unchanged, so the cross-row inequality persists. If the first stays in its row and the second crosses, use $n\le l<k'$; if both cross, use $n<k<l<k'$. Antisymmetry follows because comparisons across distinct rows in both directions would require $n<k<l<m<n$.

The [Rado order](../../../set.md#rado-order) is a [well-quasi-ordering](../../../set.md#well-quasi-ordering). Given an infinite [sequence](../../../real-analysis.md#sequence) $(m_i,n_i)$, if a first coordinate $m$ repeats infinitely often, its corresponding natural-number second coordinates have a nondecreasing pair, giving a same-row comparison. Otherwise each first coordinate occurs only finitely often, so the first coordinates in every tail are unbounded. In particular some later $m_j$ exceeds $n_0$, giving $(m_0,n_0)\le_R(m_j,n_j)$.

For each $m$, take the infinite row $S_m=\{(m,n):n>m\}$. For distinct $m,k$, choose $n>\max(m,k)$. The element $(m,n)\in S_m$ is below no member $(k,l)$ of $S_k$, since its first coordinate is different and $n<k$ fails. Thus $S_m\not\le_HS_k$ for every pair of distinct indices. These subsets form an infinite [antichain](../../../extremal-set-theory.md#antichain), so the [Hoare domination preorder](../../../set.md#hoare-domination-preorder) on $\mathcal P(R)$ is not a [well-quasi-ordering](../../../set.md#well-quasi-ordering).

If only finite subsets were intended, the answer changes again: **the [finite-subset lifting of a well-quasi-order](../../../set.md#finite-subset-lifting-of-a-well-quasi-order) is a [well-quasi-ordering](../../../set.md#well-quasi-ordering).** Enumerate each finite subset as a finite [word](../../../foundations-of-mathematics.md#string). [Higman lemma](../../../set.md#higman-s-lemma) gives an earlier [word](../../../foundations-of-mathematics.md#string) embedding into a later one with every letter increased, which witnesses [Hoare domination preorder](../../../set.md#hoare-domination-preorder) comparison of the underlying subsets. The PDF specifies no finiteness restriction, so this observation supplements rather than replaces the literal answer and the arbitrary-subset counterexample.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
