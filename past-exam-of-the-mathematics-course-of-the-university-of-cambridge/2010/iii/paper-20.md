# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper20.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)

## 1

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The printed arrow is a partial-function arrow. Thus the central objects are [partial computable functions](../../../foundations-of-mathematics.md#computable-function) $f:\mathbb N^k\rightharpoonup\mathbb N$, with [total computable functions](../../../foundations-of-mathematics.md#total-computable-function) as the special case in which every input has an output. Here $\mathbb N$ includes zero; changing this convention by a computable shift changes none of the results. A program computing $f$ must halt with output $f(\mathbf x)$ exactly on its domain, and run forever elsewhere. A finite program is a [function in intension](../../../foundations-of-mathematics.md#function-in-intension), whereas its possibly partial input-output map is a [function in extension](../../../foundations-of-mathematics.md#function-in-extension); many programs have the same extension.

A precise machine model is a [register machine](../../../foundations-of-mathematics.md#register-machine) with finitely many instructions to increment a register, decrement it conditionally, jump, and halt. Registers hold [natural numbers](../../../arithmetic.md#natural-number). A [Turing machine](../../../computer-science.md#turing-machine) instead uses a finite transition table, a finite alphabet and an unbounded tape. These models simulate one another: encode the finite nonblank tape, state and head position as numbers for the register simulation; conversely represent each register by a finite tape block and implement its increment and decrement by finite scans. Tuple inputs can be encoded by a [primitive recursive pairing function](../../../foundations-of-mathematics.md#primitive-recursive-pairing-function). The equivalence of these formal models is a mathematical result. Their identification with every informal effective procedure is the [Church–Turing thesis](../../../foundations-of-mathematics.md#church-turing-thesis), rather than an additional mathematical theorem about an already formal notion.

There is also an algebraic description. Begin with zero, successor and projections, close under [composition of partial functions](../../../function.md#composition-of-partial-functions) and [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion), and then under [unbounded minimization](../../../foundations-of-mathematics.md#mu-operator). The [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion) scheme is

$$
f(\mathbf x,0)=g(\mathbf x),\qquad f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)).
$$

Applied within the [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function) class it produces only total functions, by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $n$. [Unbounded minimization](../../../foundations-of-mathematics.md#mu-operator) searches $y=0,1,\ldots$ for the first zero of $g(\mathbf x,y)$; its output is defined only if that search reaches such a zero with every preceding necessary computation defined. Composition is likewise strict about the intermediate values it requires. These schemes compile into machine programs using finite subroutines, loops and an unbounded search loop.

For the converse, encode a machine's finite configurations and finite computation histories using [Gödel numbering](../../../mathematical-logic.md#godel-numbering). Testing that a history starts with the specified input, that every adjacent pair follows the transition table, and that its final configuration halts is [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function): all the tests are bounded by the finite code. Extracting the final output is [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function) too. For a suitable checking predicate $T$ and output decoder $V$ this proves the [Kleene normal form theorem](../../../foundations-of-mathematics.md#kleene-normal-form-theorem):

$$
\varphi_e(\mathbf x)\simeq V\bigl(\mu s\,T(e,\mathbf x,s)\bigr).
$$

The symbol $\simeq$ means equality of values and of definedness. A halting computation has a passing history code and every passing history has its actual output; a nonhalting computation has none. This proves that the partial recursive and machine-computable functions coincide, including their domains of divergence.

Finite programs can be effectively listed. Simulating the program with index $e$ gives a [universal partial computable function](../../../foundations-of-mathematics.md#universal-partial-computable-function) $U(e,\mathbf x)\simeq\varphi_e(\mathbf x)$. Fixing some inputs is effective syntactically: prepend instructions writing those constants and then call the original program. This proves the [S-m-n theorem](../../../foundations-of-mathematics.md#smn-theorem) in this machine presentation. In particular, reductions that construct a program from numerical parameters really do produce its index effectively.

The [primitive recursive functions](../../../foundations-of-mathematics.md#primitive-recursive-function) are a proper subclass of the [total computable functions](../../../foundations-of-mathematics.md#total-computable-function). Enumerate all valid unary [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function) descriptions, interpreting invalid descriptions as zero. Evaluating any fixed valid description terminates by [structural induction](../../../foundations-of-mathematics.md#structural-induction). Thus the diagonal map $d(n)=g_n(n)+1$ is total and computable, but cannot be one of the enumerated [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function) maps, since $d(e)\ne g_e(e)$. This is a [total computable diagonal over primitive recursive syntax](../../../foundations-of-mathematics.md#total-computable-diagonal-over-primitive-recursive-syntax). The evaluator can terminate on every particular description without itself being [primitive recursive](../../../foundations-of-mathematics.md#primitive-recursive-function).

In contrast, one cannot effectively enumerate exactly the programs for all [total computable functions](../../../foundations-of-mathematics.md#total-computable-function). If such an infinite enumeration were available, wait for its $n$th program and run it on $n$, then add one. Totality makes this another [total computable function](../../../foundations-of-mathematics.md#total-computable-function), while its diagonal disagrees with every listed function. Equivalently, there is no total computable universal evaluator listing precisely all total computable maps.

The [halting problem](../../../foundations-of-mathematics.md#halting-problem) is undecidable. If $H(e,x)$ decided whether program $e$ halts on $x$, construct a program $D$ which halts on input $e$ exactly when $H(e,e)$ says that it does not halt. Taking $e$ to be $D$'s own index gives a contradiction. The halting relation is nevertheless [computably enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set), since finite halting histories can be searched for.

More generally, a set is [computably enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set) exactly when it is the domain of a [partial computable function](../../../foundations-of-mathematics.md#computable-function). From an enumeration, halt on $x$ when $x$ appears; in the other direction use [dovetailing](../../../foundations-of-mathematics.md#dovetailing) over all inputs of a partial program to enumerate its halting inputs. A set is a [computable set](../../../foundations-of-mathematics.md#computable-set) exactly when both it and its complement are [computably enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set): dovetail the two searches and return the answer from the one that succeeds. Neither a semidecision procedure nor an unbounded search supplies a uniform negative answer.

Finally, the [Rice theorem](../../../foundations-of-mathematics.md#rice-s-theorem) explains the scope of this obstruction. Let $P$ be a nontrivial property of the extension of a partial computable program. Choose a partial computable $g$ whose $P$-status differs from that of the nowhere-defined function. Given a program $e$ and input $x$, effectively form the program which, on $z$, first waits for $e(x)$ to halt and then computes $g(z)$. If $e(x)$ never halts its extension is nowhere defined; otherwise its extension is $g$. A decision procedure for $P$ would therefore decide the [halting problem](../../../foundations-of-mathematics.md#halting-problem). **Effective descriptions allow universal simulation and positive verification, but not a decision procedure for every semantic property or for termination.**

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Represent the arena by a pruned [set-theoretic tree](../../../set.md#set-theoretic-tree) $T$ of legal finite positions. Players I and II alternate; every position has a legal continuation. The usual terminal-position convention can also be handled by adding terminal wins and losses at the initial stage. Give the branches the [product topology](../../../geometry-and-topology.md#product-topology) generated by finite-position cylinders, and let $A$ be I's winning [open set](../../../topology.md#open-set).

Define the [winning-position attractor in an infinite game](../../../descriptive-set-theory.md#winning-position-attractor-in-an-infinite-game) by [transfinite recursion](../../../set-theory.md#transfinite-recursion). Start with

$$
W_0=\{s\in T:[s]\subseteq A\}.
$$

At a successor stage retain $W_\alpha$ and add I-positions with at least one child in $W_\alpha$, and II-positions with every child in $W_\alpha$. At a limit stage take the union. The increasing sequence stabilizes because the positions form a set: strict increases at arbitrarily many stages would select too many distinct positions. Write $W$ for the stable set. The rank of a position in $W$ is its first entry stage; any positive such rank is a successor [ordinal](../../../set-theory.md#ordinal).

If the initial position belongs to $W$, at every I-position of positive rank choose a child that was present at the preceding stage. Every move by II also leads to a child of smaller rank, by the rule for II-positions. There is no infinite strictly decreasing sequence of [ordinals](../../../set-theory.md#ordinal), so every play following this [strategy in an infinite game](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) reaches $W_0$ after finitely many moves. Its complete branch then belongs to $A$. Hence this is a [winning strategy in an infinite game](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game) for I.

If the initial position is outside $W$, every move of I stays outside $W$. At a II-position outside $W$ at least one child is outside $W$: otherwise the entry ranks of its set of children have a common [ordinal](../../../set-theory.md#ordinal) bound, and that position would enter at the next stage. Choose such a child. This gives II a [strategy in an infinite game](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) that never enters $W_0$. A resulting branch cannot belong to $A$, because $A$ is an [open set](../../../topology.md#open-set) and would therefore have a finite prefix whose whole cylinder lies in $A$, namely a member of $W_0$. Thus II wins. This proves **the [Gale-Stewart theorem](../../../descriptive-set-theory.md#open-determinacy) for an arbitrary set-sized arena**, in the ordinary metatheory with choice. Countability of the move set was never used.

The restriction on the payoff is essential. Under the [axiom of choice](../../../set-theory.md#axiom-of-choice), already for binary moves there is an undetermined game. There are $\mathfrak c=2^{\aleph_0}$ strategies for each player, since a strategy is a binary-valued map on a countable set of positions. List I's strategies $\sigma_\alpha$ and II's strategies $\tau_\alpha$ for $\alpha<\mathfrak c$. Each strategy is compatible with $\mathfrak c$ different plays, obtained by varying all the opponent's binary moves.

At stage $\alpha$, choose a fresh play $x_\alpha$ following $\sigma_\alpha$ and then a different fresh play $y_\alpha$ following $\tau_\alpha$, avoiding every previously chosen play. Fewer than $\mathfrak c$ plays have been used at that stage, even when $\mathfrak c$ is singular, so these choices are possible. Let $B=\{y_\alpha:\alpha<\mathfrak c\}$. No I-strategy wins $B$, because its selected $x_\alpha$ is outside $B$; no II-strategy wins, because its selected $y_\alpha$ is inside $B$. Future choices avoid all earlier $x_\alpha$, so they never spoil the first assertion. This is the [choice diagonalization of an undetermined game](../../../descriptive-set-theory.md#choice-diagonalization-of-an-undetermined-game). Consequently **determinacy for all payoff sets is incompatible with the [axiom of choice](../../../set-theory.md#axiom-of-choice)**. The attractor still makes sense for a nonopen payoff, but an avoiding play may then enter the payoff without ever having a winning finite prefix.

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Here and throughout, a [filter on a set](../../../set-theory.md#filter-set-theory) is proper: it contains the whole underlying set, excludes the empty set, and is upward closed and closed under finite intersections. An improper filter cannot be extended to a proper [ultrafilter](../../../set-theory.md#ultrafilter).

Order the proper filter extensions of $\mathcal F$ by inclusion. The union of a chain is again a proper [filter on a set](../../../set-theory.md#filter-set-theory): any two members already occur in one member of the chain, where their intersection belongs; the empty set never appears. By [Zorn lemma](../../../set-theory.md#zorn-s-lemma), take a maximal proper extension $\mathcal U$. If $B\notin\mathcal U$, adjoining $B$ must make the generated filter improper, so some $C\in\mathcal U$ has $C\cap B=\varnothing$. Upward closure then gives $B^c\in\mathcal U$. Exactly one of $B,B^c$ belongs to $\mathcal U$, proving the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma).

Let $M_i$ be nonempty structures for a common [first-order language](../../../mathematical-logic.md#first-order-language), and let $\mathcal U$ be an [ultrafilter](../../../set-theory.md#ultrafilter) on the index set $I$. In the [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) $M=\prod_iM_i/\mathcal U$, identify functions $f,g$ when $\{i:f(i)=g(i)\}\in\mathcal U$; interpret function symbols coordinatewise and relations by membership of their coordinate truth sets in $\mathcal U$. The [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) states, for every [first-order formula](../../../mathematical-logic.md#first-order-formula) $\phi$,

$$
M\models\phi([f_1],\ldots,[f_n])\quad\Longleftrightarrow\quad\{i:M_i\models\phi(f_1(i),\ldots,f_n(i))\}\in\mathcal U.
$$

Changing representatives changes a coordinate truth set only outside a member of $\mathcal U$, so the definitions are well defined.

Prove the theorem by [structural induction](../../../foundations-of-mathematics.md#structural-induction) on formulas. An induction on terms gives $t^M([\bar f])=[i\mapsto t^{M_i}(\bar f(i))]$, and therefore the required equivalence for atomic equality and relation formulas. For conjunction the truth set is an intersection, and a finite intersection belongs to a proper [filter on a set](../../../set-theory.md#filter-set-theory) exactly when each constituent does. For negation it is a complement, and the [ultrafilter](../../../set-theory.md#ultrafilter) decides exactly one of a set and its complement. These prove the Boolean induction steps.

For the existential step, a witness $[g]$ in $M$ gives, by induction, a member of $\mathcal U$ on which $\phi(g(i),\bar f(i))$ holds. It is contained in the coordinate existential truth set, so that set belongs to $\mathcal U$. Conversely, if

$$
J=\{i:M_i\models\exists x\,\phi(x,\bar f(i))\}\in\mathcal U,
$$

choose a coordinate witness $g(i)$ for $i\in J$, and any element of the nonempty factor otherwise. Then the truth set of $\phi(g(i),\bar f(i))$ contains $J$. Induction gives a witness $[g]$ in the [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct). Universal quantification follows from negation and existence. This completes the actual proof of the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem).

For the [compactness theorem](../../../mathematical-logic.md#compactness-theorem), take $I$ to be the set of finite subsets $\Delta$ of $T$, and choose a model $M_\Delta$ of each such subset. The cones

$$
I_\Gamma=\{\Delta\in I:\Gamma\subseteq\Delta\}\qquad(\Gamma\subseteq T\text{ finite})
$$

are nonempty and satisfy $I_{\Gamma_1}\cap I_{\Gamma_2}=I_{\Gamma_1\cup\Gamma_2}$. They generate a proper [filter on a set](../../../set-theory.md#filter-set-theory), which extends to an [ultrafilter](../../../set-theory.md#ultrafilter) $\mathcal U$ by the proved lemma. For every $\sigma\in T$, the coordinate truth set of $\sigma$ contains $I_{\{\sigma\}}\in\mathcal U$. The [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) therefore gives

$$
\boxed{\prod_{\Delta\in I}M_\Delta/\mathcal U\models T.}
$$

This proves the requested [compactness theorem](../../../mathematical-logic.md#compactness-theorem). In fact the same proof works without the countability restriction on the language.

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Fix an effective syntax encoding for the language. Let $E_s$ be the finite set of axioms observed in the first $s$ steps of an enumeration of the given [semidecidable axiomatization](../../../mathematical-logic.md#semidecidable-axiomatization). These finite approximations can be computed in bounded time, even if the original axiom set is empty or finite. For each $\phi\in E_s$, form the precisely bracketed [logical conjunction](../../../mathematical-logic.md#logical-conjunction)

$$
C_s(\phi)=\underbrace{(\cdots((\phi\wedge\phi)\wedge\phi)\cdots\wedge\phi)}_{s+1\text{ copies of }\phi},
$$

with $C_0(\phi)=\phi$. Let $D=\{C_s(\phi):\phi\in E_s,\ s\geq0\}$.

Each $C_s(\phi)$ is logically equivalent to $\phi$, so all members of $D$ follow from the original axioms. Every original axiom eventually belongs to some $E_s$, and its corresponding member $C_s(\phi)$ implies it. Hence $D$ axiomatizes exactly the same theory.

To decide whether a candidate sentence $\psi$ belongs to $D$, let $N$ be its syntactic length. A conjunction of $s+1$ copies has length at least $s+1$, so a representation $\psi=C_s(\phi)$ can only use $s<N$. Compute each $E_s$ for $s<N$, construct its finitely many candidates, and compare them literally with $\psi$. This finite procedure always terminates and accepts exactly $D$. It does not wait for a nonexistent next axiom, nor assume that conjunction parsing determines the original repeated formula uniquely. Thus **$D$ is a decidable equivalent axiomatization**, proving the [Craig trick](../../../mathematical-logic.md#craig-trick).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the logical truth constants $\top,\bot$, and put

$$
A'=A[p:=\top],\qquad A''=A[p:=\bot].
$$

For a truth assignment with $p$ true, $A$ has the value of $A'$ and $(A'\wedge p)\vee(A''\wedge\neg p)$ has the same value. For an assignment with $p$ false, both have the value of $A''$. Thus the [propositional variable elimination](../../../mathematical-logic.md#propositional-variable-elimination) identity is

$$
\boxed{A\equiv(A[p:=\top]\wedge p)\vee(A[p:=\bot]\wedge\neg p).}
$$

Neither substituted formula contains $p$.

Let $P=\operatorname{Var}(A)\setminus\operatorname{Var}(B)$, and eliminate all the private letters of $A$ by taking

$$
C=\bigvee_{\varepsilon:P\to\{0,1\}}A[P:=\varepsilon],
$$

where a Boolean assignment substitutes $\top$ or $\bot$ for each letter. Then $\operatorname{Var}(C)\subseteq\operatorname{Var}(A)\cap\operatorname{Var}(B)$. Every assignment satisfying $A$ satisfies the disjunct corresponding to its own private-letter values, so $A\models C$.

If an assignment satisfies $C$, choose a disjunct witnessing this, and modify only its values on $P$ to the corresponding $\varepsilon$. The modified assignment satisfies $A$, hence satisfies $B$ by soundness of $A\vdash B$. Its values on every letter of $B$ have remained unchanged, so the original assignment also satisfies $B$. Therefore $C\models B$. The [propositional completeness theorem](../../../mathematical-logic.md#completeness-theorem-for-propositional-logic) converts these two valid implications into

$$
\boxed{A\vdash C\quad\text{and}\quad C\vdash B,}
$$

proving [propositional interpolation](../../../mathematical-logic.md#propositional-interpolation) constructively.

If the syntax does not initially include $\top,\bot$, they can be admitted as logical constants without adding propositional letters. This convention matters when the common vocabulary is empty: a grammar in which every formula must contain a letter has no letter-free interpolant at all. For example, two tautologies using disjoint letters entail one another but cannot have an interpolant in that grammar. The truth-constant convention supplies exactly the necessary empty-vocabulary case.

## 5

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Work inside a model $V$ of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory). Let $\pi:V\to V$ be a definable class bijection, with definable inverse, so that its image and inverse image of every set are sets by [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement). Define new membership by

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

This is the [Rieger-Bernays permutation model](../../../set-theory.md#rieger-bernays-permutation-model) convention used here. Its basic advantage is that every prescribed old set $b$ is the new extension of the object $\pi^{-1}(b)$. We verify the axioms rather than treating a membership permutation as automatically harmless.

The new [axiom of extensionality](../../../set-theory.md#axiom-of-extensionality) follows because equality of the new extensions means $\pi(x)=\pi(y)$, hence $x=y$. The new empty set and unordered pair are $\pi^{-1}(\varnothing)$ and $\pi^{-1}(\{x,y\})$. Union and [power set](../../../set.md#power-set) are represented by

$$
\operatorname{Union}_E(a)=\pi^{-1}\left(\bigcup_{u\in\pi(a)}\pi(u)\right),\qquad \operatorname{Pow}_E(a)=\pi^{-1}\left(\{\pi^{-1}(b):b\subseteq\pi(a)\}\right).
$$

Indeed, the elements of the first object are exactly the new elements of new elements of $a$; the elements of the second are exactly the objects whose new extensions are subsets of $\pi(a)$.

Translate an arbitrary formula recursively by replacing each atomic $xEy$ by $x\in\pi(y)$. This is an ordinary definable formula in the old model. Old [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) forms any specified subclass $b$ of $\pi(a)$, and $\pi^{-1}(b)$ supplies the new separated set. Old [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) similarly collects the uniquely specified images of all elements of $\pi(a)$, and applying $\pi^{-1}$ supplies its new representative. This verifies the full schemas, including formulas with unbounded quantifiers.

For [axiom of infinity](../../../set-theory.md#axiom-of-infinity), define $e_0=\pi^{-1}(\varnothing)$ and

$$
e_{n+1}=\pi^{-1}\bigl(\pi(e_n)\cup\{e_n\}\bigr).
$$

Then $\pi(e_n)=\{e_0,\ldots,e_{n-1}\}$. These objects are distinct by induction: equality of $e_n$ with an earlier $e_m$ would equate old sets of respectively $n$ and $m$ distinct members. Old replacement collects $S=\{e_n:n\in\omega\}$, and $\pi^{-1}(S)$ is a new inductive set. Thus the construction satisfies **every axiom of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) except possibly [Axiom of foundation](../../../set-theory.md#axiom-of-regularity)**.

Now interchange the old objects $\varnothing$ and $\{\varnothing\}$ and fix everything else. For $q=\varnothing$ we have $\pi(q)=\{q\}$, so its new sole member is itself: $q=\{q\}_E$. This [Quine atom](../../../set-theory.md#quine-atom) contradicts [Axiom of foundation](../../../set-theory.md#axiom-of-regularity). The identity permutation preserves the original model and its foundation. Hence, relative to consistency of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory), **foundation is independent of the other ZF axioms**.

For the further independence result, a full permutation of a model of choice is insufficient. If the old model satisfies [axiom of choice](../../../set-theory.md#axiom-of-choice), then for any new family $a$ of nonempty new sets, old choice selects $g(x)\in\pi(x)$ for every $x\in\pi(a)$. Encode its graph using the new ordered pairs, and represent that graph by $\pi^{-1}$. This is a new [choice function](../../../set-theory.md#choice-function). We therefore add a hereditary finite-support restriction to a universe with many [Quine atoms](../../../set-theory.md#quine-atom).

Start now with a model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Put $a_n=\omega+n$, and let $\pi$ interchange $a_n$ and $\{a_n\}$ for every $n\in\omega$, fixing other objects. All these transpositions are disjoint: the infinite [ordinals](../../../set-theory.md#ordinal) $a_n$ are distinct and none is a singleton. In the resulting membership structure, $A=\{a_n:n\in\omega\}$ is an infinite family of [Quine atoms](../../../set-theory.md#quine-atom).

Build its universe $W$ by the internal transfinite hierarchy

$$
W_0=A,\qquad W_{\alpha+1}=A\cup\{\pi^{-1}(b):b\subseteq W_\alpha\},\qquad W_\lambda=\bigcup_{\alpha<\lambda}W_\alpha.
$$

Write $W$ for the union over the old [ordinals](../../../set-theory.md#ordinal). Apart from the atomic self-loops, an object's new members have lower construction ranks. Every permutation $\sigma$ of $A$ therefore extends recursively to $W$: on atoms use the prescribed permutation, and on other objects put

$$
\widehat\sigma(x)=\pi^{-1}\bigl(\widehat\sigma\,``\pi(x)\bigr).
$$

This is well defined and preserves $E$. A nonatom cannot be sent to an atom, since an extension consisting solely of one atom already represents that atom. Recursing with $\sigma^{-1}$ gives the inverse, so these maps are genuine automorphisms.

Say that $x$ has finite support $S\subseteq A$ if every such permutation fixing $S$ pointwise fixes $x$. Let $H$ consist of the atoms and the objects with finite support all of whose new members, recursively away from atomic self-loops, belong to $H$. This is the [hereditarily finite-supported Quine-atom model](../../../set-theory.md#hereditarily-finite-supported-quine-atom-model). We check why it still has the required set-theoretic axioms.

It is closed under taking new members, so extensionality remains valid. The empty object and the pure finite [ordinals](../../../set-theory.md#ordinal) have empty support. Their internally represented infinite collection also has empty support, giving infinity. Pairs and unions use the finite unions of their constituents' supports; all their members remain hereditary members of $H$.

For a set $a\in H$, take all objects $b\in H$ whose new extensions are subsets of $\pi(a)$. They form an old set, since the unrestricted new [power set](../../../set.md#power-set) is an old set and membership in $H$ is definable. Its representative has support contained in a support of $a$, because an automorphism fixing $a$ permutes precisely these hereditary subsets. All its members belong to $H$. Hence this is the [power set](../../../set.md#power-set) required inside $H$, not a claim that unrestricted external subsets are retained.

For separation, relativize the formula to $H$. A support for $a$ together with supports of the finitely many parameters fixes the resulting subclass; its members are hereditary, so its representative belongs to $H$. For replacement, old replacement applied to this relativized definable functional relation collects the range. Its members have a common bound on their construction ranks, by taking the supremum of the set of ranks, so the range's representative lies in $W$. The same finite union of parameter and domain supports fixes the range by uniqueness of each image. It is therefore hereditary and belongs to $H$. These arguments verify the full schemas. Thus $H\models\mathrm{ZF}-\mathrm{Foundation}$.

Finally $A$ and the family of its two-element subsets belong to $H$ with empty support. Suppose a [choice function](../../../set-theory.md#choice-function) $c$ for this family belongs to $H$, and let $S$ be a finite support for $c$. Choose distinct atoms $u,v\notin S$ and transpose them. This permutation fixes $c$ and fixes the unordered pair $\{u,v\}_E$, but interchanges its two possible selected members. Equivariance would require

$$
c(\{u,v\}_E)=\widehat\sigma\bigl(c(\{u,v\}_E)\bigr),
$$

which is impossible. Hence **choice fails in $H$**. Together with a model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), or with its full permuted model satisfying choice and failing foundation, this proves independence of [axiom of choice](../../../set-theory.md#axiom-of-choice) from [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) minus foundation, relative to consistency of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). All hierarchy and support arguments are internal to the starting model; no transitive-model assumption is needed.

## 6

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem), let $M$ be an infinite [first-order structure](../../../mathematical-logic.md#first-order-structure) and $I$ any linear order. Choose a full [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) $M^*$: add witness functions for existential formulas, repeat in the expanded languages, and take their union. We will construct a model of its theory containing distinct generators $c_i$, $i\in I$, forming an [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence).

Adjoin the elementary diagram of $M^*$, the inequalities $c_i\ne c_j$ for $i\ne j$, and for every expanded-language formula $\phi(x_1,\ldots,x_r)$ and every two increasing $r$-tuples of indices, the sentences

$$
\phi(c_{i_1},\ldots,c_{i_r})\leftrightarrow\phi(c_{j_1},\ldots,c_{j_r}).
$$

Every finite subcollection is satisfiable in $M^*$. To prove this, choose a countably infinite sequence of distinct elements of $M$, and for each of the finitely many relevant arities color its increasing index tuples by the finite vector of truth values of the formulas of that arity. Repeated applications of the [Ramsey's theorem](../../../ramsey-theory.md#ramsey-s-theorem) give an infinite subsequence homogeneous for all these finitely many [finite colorings](../../../ramsey-theory.md#finite-coloring). Interpret the finitely many mentioned $c_i$ by its elements in their index order. All indiscernibility and distinctness constraints hold, and the finite diagram fragment holds because the ambient structure is still $M^*$.

By [compactness theorem](../../../mathematical-logic.md#compactness-theorem), a model $N^*$ of the full enlarged theory exists. Its [Skolem hull](../../../mathematical-logic.md#skolem-hull) $H$ generated by the $c_i$ is elementary: whenever an existential formula with parameters in $H$ holds in $N^*$, its chosen witness function returns a value in $H$, so the [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test) applies. Its reduct is a model of $\operatorname{Th}(M)$. If the index order has size $\kappa$, the hull has size at most $\kappa+|L|+\aleph_0$, and it contains $|I|$ distinct generators.

Every order automorphism $h$ of $I$ induces the automorphism

$$
t(c_{i_1},\ldots,c_{i_r})\longmapsto t(c_{h(i_1)},\ldots,c_{h(i_r)}).
$$

To check well-definedness, write any two terms being compared over the same increasing list of their generators. Their equality is an expanded-language formula; indiscernibility of the [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence) preserves its truth under $h$. The same argument preserves each relation, and the term construction preserves the functions. Applying $h^{-1}$ gives the inverse. The extension is unique in the specified Skolem language since every hull element is a term in the generators; no uniqueness among all automorphisms of the reduct is being asserted. This proves the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem), including its usual automorphism consequence.

For [simple typed set theory with atoms](../../../set-theory.md#simple-typed-set-theory-with-atoms), use sorts $0,1,\ldots$, predicates $S_i$ for sets, and typed membership from sort $i$ to sort $i+1$. Atoms have no members, extensionality compares sets, and every well-typed formula defines a set of the next sort. [Typical ambiguity](../../../set-theory.md#typical-ambiguity) is the schema $\phi\leftrightarrow\phi^+$ for every closed typed sentence, where the superscript raises all types by one.

Here are concrete full typed models before imposing the ambiguity schema. Choose increasing natural numbers $n_{-1}<n_0<n_1<\cdots$ and set

$$
D_i=V_{\omega+2n_i},\qquad S_i=\mathcal P(D_{i-1})\subseteq D_i.
$$

The auxiliary $D_{-1}$ merely interprets the set predicate at the lowest sort. Define typed membership by

$$
x\mathrel{\in_i}y\quad\Longleftrightarrow\quad y\in S_{i+1}\text{ and }x\in y.
$$

Then the other objects of $D_{i+1}$ are atoms, regardless of their old membership. Every subset of $D_i$ has its representative in $S_{i+1}$, giving comprehension even for formulas with higher-sort quantifiers and parameters. Extensionality holds for the set representatives and atoms have no typed members. The rank gaps leave infinitely many atoms at each sort, and all sorts are infinite.

Consider finitely many ambiguity instances with unraised sentences $\phi_1,\ldots,\phi_t$, and choose a fixed window length $r$ sufficient to include every sort used and its auxiliary predecessor. Color every increasing $r$-tuple of natural numbers by the vector of truth values of these unraised sentences in its finite rank-window interpretation. There are only $2^t$ colors. The [Ramsey's theorem](../../../ramsey-theory.md#ramsey-s-theorem) gives an infinite homogeneous set. Choose $r+1$ successive points from it. The first $r$ points and last $r$ points have the same color, while the latter interpretation of $\phi_j$ is exactly the former model's interpretation of $\phi_j^+$. The auxiliary predecessor shifts too, so this remains true for sentences mentioning the lowest set predicate. Extend the chosen rank sequence arbitrarily to interpret the remaining sorts. This yields a model of typed set theory satisfying all the specified ambiguity instances.

Thus every finite subset of the typed axioms together with all ambiguity instances has a model. Applying multisorted [compactness theorem](../../../mathematical-logic.md#compactness-theorem) gives

$$
\boxed{\operatorname{Con}(\mathrm{TSTU}+\mathrm{Typical\ ambiguity}).}
$$

The final model satisfies first-order typed comprehension, with quantification over its own sorts and sets as in [Henkin semantics](../../../mathematical-logic.md#henkin-semantics).

## 7

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

The exponent-two [Erdős-Rado theorem for pairs](../../../set-theory.md#erdos-rado-theorem-for-pairs) says that for every infinite [cardinal](../../../set-theory.md#cardinal-number) $\lambda$,

$$
\boxed{(2^\lambda)^+\longrightarrow(\lambda^+)^2_\lambda.}
$$

In particular, a finite or countable coloring of pairs from $(2^{\aleph_0})^+$ has an uncountable [monochromatic](../../../ramsey-theory.md#monochromatic-set) subset. We prove the general statement by an end-homogeneous tree construction.

Let $c:[\mu]^2\to\nu$ be any coloring on an [ordinal](../../../set-theory.md#ordinal) $\mu$. Route a vertex $\beta$ through an increasing sequence of preceding vertices as follows. Start with the least vertex. After ancestors $a_\eta$, $\eta<\xi$, have been selected, choose the least remaining candidate $\gamma\leq\beta$, above those ancestors, satisfying

$$
c(\{a_\eta,\gamma\})=c(\{a_\eta,\beta\})\qquad(\eta<\xi).
$$

The terminal candidate $\beta$ always qualifies, so the procedure eventually reaches it. Candidate sets shrink and their least elements increase. If an intermediate candidate is $\gamma$, its route is precisely the earlier part of the route to $\beta$, because all earlier color tests agree. Consequently the routes define a [set-theoretic tree](../../../set.md#set-theoretic-tree) on the vertices.

Along a branch, the color from an ancestor to every later branch vertex is constant. Also a node of height $\alpha$ is determined by its sequence of $\alpha$ colors to its ancestors: reconstruct the ancestors as successive least candidates with those prescribed colors, then reconstruct the node as the least final candidate. Thus its level has at most $\nu^{|\alpha|}$ nodes.

Apply this with $\mu=(2^\lambda)^+$ and $\nu=\lambda$. If every node had height less than $\lambda^+$, each level would have size at most $\lambda^\lambda\leq2^\lambda$, and there would be at most $\lambda^+$ such levels. Their total size would be at most $2^\lambda$, contradicting $|\mu|=(2^\lambda)^+$. Hence some route has at least $\lambda^+$ ancestors. For each ancestor mark its constant color to all later route points. Since there are only $\lambda$ colors, one occurs on $\lambda^+$ ancestors. Those ancestors form the required [monochromatic](../../../ramsey-theory.md#monochromatic-set) set. This proves the theorem.

To make the [ordinal](../../../set-theory.md#ordinal) function precise, one useful [ordinal partition-bound function](../../../set-theory.md#ordinal-partition-bound-function) is

$$
f(\alpha)=\min\{\beta\geq\alpha:\text{for every nonzero cardinal }\nu<\alpha,\ \beta\longrightarrow(\alpha)^2_\nu\}.
$$

The target here is [ordinal](../../../set-theory.md#ordinal) order type. For infinite $\alpha$, the proved theorem with $\lambda=|\alpha|$ supplies a bound $(2^\lambda)^+$: its homogeneous set has order type at least $\lambda^+>\alpha$, and it handles all the required color counts. Finite targets are handled by finite [Ramsey theorem](../../../graph-theory.md#ramsey-theorem) bounds. Thus $f$ is total, nondecreasing and $f(\alpha)\geq\alpha$.

Suppose a sequence of transfinite iterates $\alpha_{\xi+1}=f(\alpha_\xi)$, with suprema at limit stages, has supremum an uncountable [cardinal](../../../set-theory.md#cardinal-number) $\kappa$ at a limit stage, with every earlier iterate below $\kappa$. Then

$$
\theta<\kappa\quad\Longrightarrow\quad f(\theta)<\kappa:
$$

choose an earlier iterate at least $\theta$ and use the next one as a bound. If the iteration has already stabilized, it has already found a fixed point instead.

This closure forces $\kappa$ to be a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal). For any infinite $\lambda<\kappa$, color pairs of distinct binary strings of length $\lambda$ by their first differing coordinate. This uses $\lambda$ colors and has no [monochromatic](../../../ramsey-theory.md#monochromatic-set) triangle: three binary digits at one coordinate cannot be pairwise different. It gives a coloring on $2^\lambda$ with no homogeneous target of type $\lambda+1$. Since $\lambda$ colors are allowed when the target is the [ordinal](../../../set-theory.md#ordinal) $\lambda+1$, we have

$$
2^\lambda<f(\lambda+1)<\kappa.
$$

Finite exponents satisfy the strong-limit requirement automatically for uncountable $\kappa$.

The needed additional condition is the [tree property](../../../set.md#tree-property): every tree of height $\kappa$, with nonempty levels of size less than $\kappa$, has a cofinal branch. In the present convention it forces $\kappa$ to be a [regular cardinal](../../../set-theory.md#regular-cardinal). If $\kappa$ were singular, take a cofinal sequence of smaller [cardinals](../../../set-theory.md#cardinal-number) of length $\operatorname{cf}(\kappa)$ and form the disjoint union of chains of those lengths. This tree has height and total size $\kappa$, levels of size at most $\operatorname{cf}(\kappa)<\kappa$, but no branch of length $\kappa$, a contradiction.

For any $\nu<\kappa$, apply the preceding color-routing tree to a coloring $[\kappa]^2\to\nu$. If a route already has length $\kappa$, use it. Otherwise its levels are indexed below $\kappa$ and each has size

$$
\nu^{|\alpha|}\leq2^{\nu\cdot|\alpha|}<\kappa
$$

for infinite exponents, by the strong-limit property; finite cases satisfy the same needed bound directly. The tree has $\kappa$ nodes, so regularity forces its height to be $\kappa$. The [tree property](../../../set.md#tree-property) supplies a cofinal branch. The ancestor-color partition of that branch has one class of size $\kappa$, since $\nu<\kappa$ and $\kappa$ is regular. Thus $\kappa\to(\kappa)^2_\nu$ for every $\nu<\kappa$, and

$$
\boxed{f(\kappa)=\kappa.}
$$

We have proved that an uncountable function-closed [cardinal](../../../set-theory.md#cardinal-number) with the [tree property](../../../set.md#tree-property) is regular and strong limit, hence **strongly inaccessible**, and that it is the requested fixed point.

The paper's final sentence, read as a claim about the [tree property](../../../set.md#tree-property) alone, is false. Already $\aleph_0$ has it by the [König infinity lemma](../../../combinatorics.md#konig-s-lemma) but is not uncountable; even with uncountability stipulated, there are relative-consistency models with the [tree property](../../../set.md#tree-property) at $\aleph_2$. The latter counterexample is documented in [the research account of Mitchell forcing](https://scholar.harvard.edu/files/apoveda/files/210520.pdf). The rigorous conclusion in the iterated-function context is the one just proved: function closure supplies strong limit, and the [tree property](../../../set.md#tree-property) supplies regularity and a branch. Strong limit and regularity follow from distinct hypotheses in this context.

## 8

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

Let $M^*$ be a full [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) of an infinite structure $M$, choose distinct $b_n\in M$ for $n\in\mathbb N$, and extend the [cofinite filter](../../../set-theory.md#cofinite-filter) to a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) $U$ on $\mathbb N$. For a finite subset $F=\{i_1<\cdots<i_r\}$ of the desired index order $I$, define the ordered [Fubini product of ultrafilters](../../../set-theory.md#fubini-product-of-ultrafilters) $U_F$ on $\mathbb N^F$ by

$$
X\in U_F\quad\Longleftrightarrow\quad U n_{i_1}\,U n_{i_2}\cdots U n_{i_r}\,[\mathbf n\in X],
$$

where $U n\,P(n)$ means $\{n:P(n)\}\in U$. These nested tests decide complements and preserve intersections by induction on $r$, so $U_F$ is indeed an [ultrafilter](../../../set-theory.md#ultrafilter). For the empty set use the one-point index set and its principal [ultrafilter](../../../set-theory.md#ultrafilter).

Put $M_F=(M^*)^{\mathbb N^F}/U_F$. If $F\subseteq G$, projection of coordinates induces

$$
e_{FG}([h])=[h\circ\operatorname{pr}_{GF}].
$$

A truth test independent of a coordinate is unchanged by its dummy [ultrafilter](../../../set-theory.md#ultrafilter) quantifier. Consequently pullback preserves exactly the $U_F$-large subsets, proving that the map is well defined and injective. The [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem), applied to every formula rather than just to equality, proves that it is an [elementary embedding](../../../set-theory.md#elementary-embedding). Projections compose, so these elementary maps form a coherent directed system.

Take its [directed limit of elementary embeddings](../../../foundations-of-mathematics.md#directed-limit-of-elementary-embeddings) $N^*$. Explicitly identify two stage elements when their images agree at a common larger stage, and interpret functions and relations there. For an existential formula true in the limit, its parameters and a witness occur at a common stage; elementarity then pulls truth back to the stage of the original parameters. This verifies that all stage maps into the limit are elementary.

Let $a_i$ be the image in this limit of the coordinate class $[n\mapsto b_n]\in M_{\{i\}}$. These elements are distinct: in $U_{\{i,j\}}$, equality would require $n_i=n_j$, whose inner-coordinate section is a singleton and hence not in the nonprincipal $U$. For $i_1<\cdots<i_r$, the truth of any expanded-language formula on $(a_{i_1},\ldots,a_{i_r})$ is exactly

$$
U n_1\cdots U n_r\,[M^*\models\phi(b_{n_1},\ldots,b_{n_r})].
$$

This expression depends on the formula and the tuple length, not on the chosen increasing indices. Thus $(a_i)_{i\in I}$ is an [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence). The empty-coordinate stage embeds $M^*$ elementarily into $N^*$.

Their [Skolem hull](../../../mathematical-logic.md#skolem-hull) is elementary by the witness-function argument, and an order automorphism of $I$ extends to it by transporting the generators in every term. Equality and relation preservation follow from the displayed uniform truth test, and the inverse order automorphism gives the inverse map. Therefore **this proves the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem) through [ultrapowers](../../../foundations-of-mathematics.md#ultrapower) and their directed limit**, with no Ramsey-theoretic step.

## 9

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

A [model-theoretic ultralimit](../../../foundations-of-mathematics.md#model-theoretic-ultralimit) is the direct limit of a chain of successive [ultrapowers](../../../foundations-of-mathematics.md#ultrapower) along their diagonal elementary maps. It is not the topological notion of a limit along an [ultrafilter](../../../set-theory.md#ultrafilter). We first prove the precise relative embedding lemma needed to synchronize two such limits.

If $A\prec B$, then $B$ embeds elementarily into an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) of $A$, with the embedding restricting on $A$ to its diagonal map. To prove this [Frayne embedding lemma](../../../foundations-of-mathematics.md#frayne-embedding-lemma), use the elementary diagram of $B$ with the elements of $A$ treated as named parameters. Every finite fragment $\Delta$ of that diagram has a realization in $A$: replace its finitely many names from $B\setminus A$ by variables and existentially quantify their conjunction. It is true in $B$, and hence true in $A$ by elementarity. Choose these simultaneous realizations for each finite fragment, keeping every parameter from $A$ interpreted as itself; give unmentioned names an arbitrary default in the nonempty $A$.

On the index set of finite fragments, extend the filter of cones $\{\Delta:\Delta\supseteq\Gamma\}$ to an [ultrafilter](../../../set-theory.md#ultrafilter) $U$. For each $b\in B$, let $g_b(\Delta)$ be its value in the chosen coordinate realization. Every diagram sentence is satisfied on its cone, so the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) makes $b\mapsto[g_b]$ an [elementary embedding](../../../set-theory.md#elementary-embedding) $B\to A^I/U$. Inequalities in the diagram ensure injectivity. If $b\in A$, all its coordinates equal $b$, giving exactly the diagonal map.

There is also the initial version: if merely $A\equiv B$, then $A$ embeds elementarily into an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) of $B$. A finite fragment of the elementary diagram of $A$, with all its names replaced by variables, yields an existential sentence true in $A$ and hence in $B$. The identical finite-fragment and cone construction therefore proves this version without already assuming an embedding.

Start with $A_0=A$. Use the initial version to place $A_0$ elementarily in an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) $B_0$ of $B$. Relabel embedded copies so we can regard the elementary maps as inclusions. Apply the relative version to $A_0\prec B_0$ to obtain an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) $A_1$ of $A_0$ containing $B_0$, and whose inclusion of $A_0$ is its diagonal map. Next apply it to $B_0\prec A_1$ to obtain an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) $B_1$ of $B_0$ containing $A_1$, again fixing the earlier diagonal inclusion. Continuing gives an elementary chain

$$
A_0\prec B_0\prec A_1\prec B_1\prec A_2\prec B_2\prec\cdots.
$$

The common union $C$ is elementary over every stage by the [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem), and

$$
C=\bigcup_{n<\omega}A_n=\bigcup_{n<\omega}B_n.
$$

The first presentation is a [model-theoretic ultralimit](../../../foundations-of-mathematics.md#model-theoretic-ultralimit) of $A$. The second, preceded by the initial diagonal embedding of $B$ into $B_0$, is a [model-theoretic ultralimit](../../../foundations-of-mathematics.md#model-theoretic-ultralimit) of $B$. Each consecutive same-letter inclusion is precisely the corresponding [ultrapower](../../../foundations-of-mathematics.md#ultrapower) diagonal map, not just an unspecified [elementary embedding](../../../set-theory.md#elementary-embedding). Thus the two limits are identified with the same structure $C$, proving

$$
\boxed{A\equiv B\ \Longrightarrow\ A\text{ and }B\text{ have isomorphic model-theoretic ultralimits}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
