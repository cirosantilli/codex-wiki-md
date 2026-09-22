# Paper 135

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_135.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_135.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [1](#1/1)
    - [Solution](#1/1/solution)
  - [2](#1/2)
    - [Solution](#1/2/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 135](paper-135.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work in [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) with the [law of excluded middle](../../../mathematical-logic.md#law-of-excluded-middle), without the [axiom of choice](../../../set-theory.md#axiom-of-choice). The paper's terminology is an [infinite Dedekind-finite set](../../../set.md#infinite-dedekind-finite-set). The useful common principle is [countable union of explicitly ordered finite lists without choice](../../../set-theory.md#countable-union-of-explicitly-ordered-finite-lists-without-choice): given an actual [sequence](../../../real-analysis.md#sequence) of finite lists, enumerate their entries by list number and position using a [Cantor pairing function](../../../set-theory.md#cantor-pairing-function). If the union of entries is infinite, repeatedly take the entry with the least code not already selected. This produces an injection from $\mathbb N$ without choosing any enumerations of unordered [sets](../../../set.md).

Consequently, if a family of objects has an explicitly ordered finite list of labels for each object, and only finitely many objects can be made from any given finite pool of labels, then a countably infinite list of distinct objects forces a countably infinite subset of the label [set](../../../set.md). For a Dedekind-finite label [set](../../../set.md) this is impossible. If the label [set](../../../set.md) embeds into the object family as well, infinitude is preserved. Thus

$$
\boxed{\text{explicit ordered finite supports + finite pools of objects preserve infinite Dedekind-finiteness.}}
$$

The distinction between ordered lists supplied by the data and arbitrary finite subsets is essential: a blanket countable-union theorem for unordered [finite sets](../../../set.md#finite-set) would introduce a choice principle.

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Let $\operatorname{Inj}({<}\omega,X)$ denote the [finite repetition-free sequences](../../../real-analysis.md#finite-repetition-free-sequence), including the empty [sequence](../../../real-analysis.md#sequence). The map $x\mapsto(x)$ is injective, so this [set](../../../set.md) is infinite when $X$ is infinite. Suppose, for a contradiction, that it contains a countably infinite subset. Fix its given injective enumeration $s_0,s_1,\ldots$; this is part of the supposition, not a choice from a family of [sets](../../../set.md).

Enumerate all pairs $(n,j)$ with $j<\operatorname{length}(s_n)$ by their natural-number pairing codes, recording the corresponding entries $s_n(j)$. If the union of entries were infinite, recursively selecting the first new entry would give an injection $\mathbb N\to X$, contradicting Dedekind-finiteness. Therefore the union is a [finite set](../../../set.md#finite-set) $F$, say of size $m$. A repetition-free [sequence](../../../real-analysis.md#sequence) over $F$ has length at most $m$, and there are exactly

$$
\sum_{k=0}^m m(m-1)\cdots(m-k+1)=\sum_{k=0}^m\frac{m!}{(m-k)!}
$$

such [sequences](../../../real-analysis.md#sequence), with the empty product equal to one. All $s_n$ would belong to this [finite set](../../../set.md#finite-set), contradicting their distinctness. Finite counting and the least-code construction use no [axiom of choice](../../../set-theory.md#axiom-of-choice). This proves [finite repetition-free sequences preserve Dedekind-finiteness](../../../set.md#finite-repetition-free-sequences-preserve-dedekind-finiteness) and the required infinitude:

$$
\boxed{\operatorname{Inj}({<}\omega,X)\text{ is an infinite Dedekind-finite set.}}
$$

<h3 id="1/2">2</h3>

↑ **Parent:** [1](#1)

<h4 id="1/2/solution">Solution</h4>

↑ **Parent:** [2](#1/2)

Write $\mathcal T(D)$ for the [recursively repetition-free labelled trees](../../../combinatorics.md#recursively-repetition-free-labelled-tree). Each [rooted tree](../../../combinatorics.md#rooted-tree) is finite because the inductive definition forms it from an already constructed finite list of finite child [rooted trees](../../../combinatorics.md#rooted-tree). Its label list is obtained by visiting the root first, then each child subtree in its prescribed order, using a [depth-first traversal of a tree](../../../combinatorics.md#depth-first-traversal-of-a-tree). This list can have repetitions. In particular, different branches may use the same label; the children are required to be distinct [rooted trees](../../../combinatorics.md#rooted-tree), not to have distinct root labels.

For any finite label pool $F$, prove by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $|F|$ that $\mathcal T(F)$ is finite. For $F=\varnothing$ it is empty. For each root $d\in F$, the children form a [finite repetition-free sequence](../../../real-analysis.md#finite-repetition-free-sequence) from $\mathcal T(F\setminus\{d\})$, which is finite by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction). There are therefore finitely many child lists for that root, and the finite union over $d\in F$ is finite. More explicitly, if $t_m$ is the number of [rooted trees](../../../combinatorics.md#rooted-tree) on a pool of $m$ labels, then

$$
t_0=0,\qquad t_m=m\sum_{k=0}^{t_{m-1}}\frac{t_{m-1}!}{(t_{m-1}-k)!}.
$$

There is no countable choice in this finite [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction).

Now suppose $T_0,T_1,\ldots$ were an injective enumeration of a countably infinite subset of $\mathcal T(D)$. Their canonical traversal lists give an explicit enumeration of all labels used. If infinitely many different labels occur, the least-first-occurrence procedure gives a countably infinite subset of $D$, a contradiction. Otherwise all labels belong to one [finite set](../../../set.md#finite-set) $F$. Every $T_n$ then belongs to $\mathcal T(F)$: recursively its root lies in $F$ and its child [rooted trees](../../../combinatorics.md#rooted-tree) use only $F$ with that root removed. But $\mathcal T(F)$ is finite by the preceding [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction), again a contradiction. Finally $d\mapsto$ the single-vertex [rooted tree](../../../combinatorics.md#rooted-tree) labelled $d$ is injective, so $\mathcal T(D)$ is infinite. Hence [recursively repetition-free labelled trees preserve Dedekind-finiteness](../../../combinatorics.md#recursively-repetition-free-labelled-trees-preserve-dedekind-finiteness):

$$
\boxed{\mathcal T(D)\text{ is an infinite Dedekind-finite set.}}
$$

<h2 id="2">2</h2>

↑ **Parent:** [Paper 135](paper-135.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For subsets $A,B\subseteq\mathbb N$, a [many-one reduction](../../../foundations-of-mathematics.md#many-one-reduction) $A\leq_m B$ is a [total computable function](../../../foundations-of-mathematics.md#total-computable-function) $h$ with $n\in A\iff h(n)\in B$. A [Turing reduction](../../../foundations-of-mathematics.md#turing-reduction) $A\leq_T B$ is an [oracle machine](../../../computer-science.md#oracle-machine) with oracle $B$ computing the total [indicator function](../../../measure-theory.md#indicator-function) $\chi_A$. It may make several adaptive oracle queries. A [many-one reduction](../../../foundations-of-mathematics.md#many-one-reduction) gives a [Turing reduction](../../../foundations-of-mathematics.md#turing-reduction) using one query; the definitions impose no enumerability assumption on $A,B$.

The [Friedberg–Muchnik theorem](../../../foundations-of-mathematics.md#friedberg-muchnik-theorem) asserts that there exist [computably enumerable sets](../../../foundations-of-mathematics.md#recursively-enumerable-set) $A,B$ with

$$
\boxed{A\not\leq_T B\quad\text{and}\quad B\not\leq_T A.}
$$

We give the [finite-injury priority construction](../../../foundations-of-mathematics.md#finite-injury-priority-construction). Fix an effective list $\Phi_e$ of [Turing functionals](../../../foundations-of-mathematics.md#turing-functional) and impose

$$
R_e:\Phi_e^B\ne\chi_A,\qquad S_e:\Phi_e^A\ne\chi_B,
$$

in priority order $R_0,S_0,R_1,S_1,\ldots$. Each strategy has an unassigned, waiting or protected state; a private witness $x$ when assigned; and a restraint on the oracle [set](../../../set.md) when protected. All witnesses, even abandoned ones, are permanently recorded and never reused. A strategy for $R_e$ is the only strategy ever allowed to enumerate its witness into $A$; the analogous statement holds for $S_e$ and $B$.

Start with [finite sets](../../../set.md#finite-set) $A_0=B_0=\varnothing$. At stage $s$, inspect the first $s+1$ strategies. An unassigned strategy needs attention. A waiting $R_e$ strategy needs attention if the computation $\Phi_e^{B_s}(x)$ converges within $s$ steps; waiting $S_e$ is symmetric. Act on the highest-priority strategy needing attention, if any. On assignment choose a fresh witness greater than $s$, every earlier witness and every higher-priority restraint, and enter the waiting state. On a convergence with output $v$ and [oracle use](../../../foundations-of-mathematics.md#oracle-use) $u$, act as follows: if $v=0$, enumerate the witness into its own target [set](../../../set.md); if $v\ne0$, leave the witness out. Enter the protected state and restrain the oracle below $u$. The current characteristic value at the witness is now different from $v$, including outputs other than zero or one. Whenever a strategy acts, initialize every lower-priority strategy, discarding its current witness and restraint but retaining the permanent record of used witnesses. If none needs attention, change nothing.

Every enumeration respects higher-priority restraints: its witness was chosen beyond them after its last initialization, and a later higher-priority action would have initialized it. Each stage is effective, finite and monotone in $A_s,B_s$, so $A=\bigcup_s A_s$ and $B=\bigcup_s B_s$ are computably enumerable. Lower-priority restraints may be violated by a higher-priority action, exactly the allowed injuries.

Induct on priority to verify [finite injury](../../../foundations-of-mathematics.md#finite-injury) and satisfaction. Once all higher-priority strategies have made their last actions, the current strategy receives its final assignment and can act at most once more, on a convergence. If convergence is observed it is then protected permanently; otherwise it waits without further action. In either case every strategy acts only finitely often. After the final initialization of $R_e$, if it acts on a convergence, no higher strategy subsequently changes its assumptions and every lower strategy respects its restraint. The observed oracle computation therefore remains valid for the final $B$, while the permanently private witness retains the opposite characteristic value in $A$.

If it waits forever, then $\Phi_e^B(x)$ cannot converge. A convergent final computation uses only finitely many oracle bits; those bits in the increasing enumeration $B_s$ eventually equal their final values. For a sufficiently large stage the same finite computation would have been observed, and after the higher strategies have stopped it would receive attention, contradicting perpetual waiting. Thus $R_e$ is satisfied either by disagreement or by divergence. The same proof satisfies every $S_e$. This is [private-witness diagonalization for incomparable enumerable sets](../../../foundations-of-mathematics.md#private-witness-diagonalization-for-incomparable-enumerable-sets), with the finite-injury verification supplying the required permanent disagreements.

A computable [set](../../../set.md) reduces to every oracle, so incomparability makes both [sets](../../../set.md) noncomputable. Every [computably enumerable set](../../../foundations-of-mathematics.md#recursively-enumerable-set) reduces to the [halting problem](../../../foundations-of-mathematics.md#halting-problem); if either of these [sets](../../../set.md) had the halting degree, the other would reduce to it. Thus their c.e. degrees are also incomplete, giving the intermediate degrees sought by the [Post problem](../../../foundations-of-mathematics.md#post-problem).

## 3

↑ **Parent:** [Paper 135](paper-135.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The countable form of the [omitting types theorem](../../../foundations-of-mathematics.md#omitting-types-theorem) is as follows. Let $L$ be a countable [first-order language](../../../mathematical-logic.md#first-order-language) and $T$ a consistent [first-order theory](../../../mathematical-logic.md#first-order-theory) in $L$. For any countable family $p_0,p_1,\ldots$ of [nonprincipal partial types](../../../mathematical-logic.md#nonprincipal-partial-type) in finite tuples of variables, there is an at most countable [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $T$ omitting all of them. Nonprincipality means that no $T$-consistent [first-order formula](../../../mathematical-logic.md#first-order-formula) $\theta(\mathbf x)$ entails every member of the type modulo $T$. A complete [first-order theory](../../../mathematical-logic.md#first-order-theory) with nonisolated [complete types](../../../foundations-of-mathematics.md#complete-type) is the usual special case; neither an uncountable language nor an arbitrary uncountable family is covered by this statement.

Use the [Godel completeness theorem](../../../mathematical-logic.md#godel-s-completeness-theorem) to pass between consistency and the existence of a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory). Adjoin a countable stock $C$ of new constants. Construct finite conditions $\Gamma_s$ with $T\cup\Gamma_s$ consistent, interleaving three countable lists of requirements: decide each $L(C)$-sentence; provide a fresh constant witness for each existential sentence; and, for each $p_i$ and each tuple $\mathbf t$ of closed terms of its arity, add $\neg\psi(\mathbf t)$ for some $\psi\in p_i$. Sentence decisions preserve consistency by choosing a consistent sign. For an existential sentence $\exists x\,\varphi(x)$, add $\exists x\,\varphi(x)\to\varphi(c)$ with $c$ fresh for that condition and [first-order formula](../../../mathematical-logic.md#first-order-formula). This is consistent: any [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of the old condition can interpret $c$ as a witness if one exists, and otherwise arbitrarily in the nonempty domain.

The omission step is the key [Henkin omission extension lemma](../../../foundations-of-mathematics.md#henkin-omission-extension-lemma). Let $\sigma(\mathbf c)$ be the [logical conjunction](../../../mathematical-logic.md#logical-conjunction) of the current finite condition, listing every new constant occurring either there or in $\mathbf t$. If adding $\neg\psi(\mathbf t)$ were inconsistent for every $\psi\in p_i$, then $T$ would entail $\sigma(\mathbf c)\to\psi(\mathbf t(\mathbf c))$ for each such $\psi$. Replace the new constants by fresh variables $\mathbf z$ and form

$$
\theta(\mathbf x)=\exists\mathbf z\bigl(\sigma(\mathbf z)\land\bigwedge_j x_j=t_j(\mathbf z)\bigr).
$$

It is consistent with $T$ and entails every $\psi\in p_i$, contradicting nonprincipality. Hence some omission extension is consistent. The construction need not be computable; countability merely permits all these requirements to be scheduled.

Let $T^*$ be the deductive closure of $T\cup\bigcup_s\Gamma_s$. It is consistent by the [finite character of formal proofs](../../../mathematical-logic.md#finite-character-of-formal-proofs), complete by sentence decisions, and has the [Henkin witness property](../../../mathematical-logic.md#henkin-witness-property). Its [term model](../../../mathematical-logic.md#term-model) consists of closed terms modulo provable [logical equality](../../../mathematical-logic.md#logical-equality) and has at most countably many elements. The [truth lemma for a Henkin term model](../../../mathematical-logic.md#truth-lemma-for-a-henkin-term-model) proves that it is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $T^*$. Every tuple in it is represented by closed terms, whose scheduled omission requirement supplies a negated member of each corresponding type. Thus

$$
\boxed{\text{there is an at most countable }M\models T\text{ omitting every }p_i.}
$$

A [universal sentence](../../../mathematical-logic.md#universal-sentence) has the form $\forall\mathbf x\,\psi(\mathbf x)$ with quantifier-free $\psi$, including an empty quantifier block. Embeddings preserve and reflect quantifier-free truth, so [universal sentences](../../../mathematical-logic.md#universal-sentence) pass to [substructures of a first-order structure](../../../mathematical-logic.md#substructure-of-a-first-order-structure). For the converse [Łoś-Tarski preservation theorem](../../../mathematical-logic.md#los-tarski-preservation-theorem), let $T_\forall$ be all universal consequences of an arbitrary [first-order theory](../../../mathematical-logic.md#first-order-theory) $T$, and take $A\models T_\forall$. We claim $T\cup\operatorname{Diag}(A)$ is consistent, where the [diagram of a structure](../../../foundations-of-mathematics.md#diagram-mathematical-logic) contains both atomic and negated atomic sentences in constants naming the elements of $A$.

If inconsistent, the [compactness theorem](../../../mathematical-logic.md#compactness-theorem) gives a finite [logical conjunction](../../../mathematical-logic.md#logical-conjunction) $\delta(c_{a_1},\ldots,c_{a_r})$ of diagram sentences for which $T\models\neg\delta(c_{a_1},\ldots,c_{a_r})$. The added constants do not occur in $T$, so

$$
T\models\forall x_1\cdots x_r\,\neg\delta(x_1,\ldots,x_r).
$$

This [universal sentence](../../../mathematical-logic.md#universal-sentence) belongs to $T_\forall$ but is false in $A$ at the named tuple, a contradiction. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) therefore produces $B\models T$ containing an isomorphic embedded copy of $A$. The signed diagram ensures a genuine [substructure of a first-order structure](../../../mathematical-logic.md#substructure-of-a-first-order-structure): [functions](../../../function.md) are preserved, constants are included and relations are preserved and reflected. If the [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) class of $T$ is closed under [substructures of a first-order structure](../../../mathematical-logic.md#substructure-of-a-first-order-structure), this copy, and hence $A$, is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $T$. We have proved

$$
\boxed{\operatorname{Mod}(T)=\operatorname{Mod}(T_\forall).}
$$

No countability assumption is needed for this second argument. An inconsistent [first-order theory](../../../mathematical-logic.md#first-order-theory) is covered as well, with a universally false axiom and an empty [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) class.

## 4

↑ **Parent:** [Paper 135](paper-135.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

One form of the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem) says that, for every infinite [first-order structure](../../../mathematical-logic.md#first-order-structure) $M$ and every [total order](../../../set.md#total-order) $I$, an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) contains distinct elements $(a_i)_{i\in I}$ forming an [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence). After a suitable [Skolem expansion](../../../mathematical-logic.md#skolem-expansion), their [Skolem hull](../../../mathematical-logic.md#skolem-hull) is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $\operatorname{Th}(M)$, and every [order automorphism](../../../set.md#order-automorphism) of $I$ extends to a [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) of that hull. If $M$ has a definable infinite linearly ordered subset $P$, the generators may lie in $P$ and their order may agree with that definable order. Uniqueness of the extended [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) is asserted in the chosen [Skolem expansion](../../../mathematical-logic.md#skolem-expansion), rather than for every [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) of its reduct.

Here is an [ultraproduct proof of the Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ultraproduct-proof-of-the-ehrenfeucht-mostowski-theorem). First expand $M$ to $M^+$ with [Skolem functions](../../../mathematical-logic.md#skolem-function) for all existential [first-order formulas](../../../mathematical-logic.md#first-order-formula), iterating through the enlarged languages if necessary. This is done in the ordinary classical metatheory; the choice restriction in question 1 is not a restriction on this question. Fix a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) $\mathcal U$ on $\mathbb N$.

We can obtain an infinite [sequence](../../../real-analysis.md#sequence) of distinct elements $b_0,b_1,\ldots$ in an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) $M_0$ of $M^+$ by one preliminary [ultrapower](../../../foundations-of-mathematics.md#ultrapower). For each $n\geq1$ choose a finite list of $n$ distinct elements of $M^+$. Represent $b_j$ by the [function](../../../function.md) taking the $j$th entry when $n>j$, with an arbitrary default otherwise. Distinctness holds on a [cofinite set](../../../set-theory.md#cofinite-set), so follows from [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem). In the definably ordered variant, first name any parameters defining $P$, and choose each finite list increasingly inside $P$ instead; then $M_0\models P(b_j)$ and $b_j<b_k$ for $j<k$. Infinitude of an ordered [set](../../../set.md) supplies every finite increasing chain. This preparatory step uses no [Ramsey theorem](../../../graph-theory.md#ramsey-theorem).

For a finite subset $F=\{i_1<\cdots<i_r\}$ of $I$, define the [ultrafilter](../../../set-theory.md#ultrafilter) $\mathcal U_F$ on $\mathbb N^F$ by nested membership, in this order:

$$
E\in\mathcal U_F\quad\Longleftrightarrow\quad(\mathcal U n_{i_1})\cdots(\mathcal U n_{i_r})\,[\mathbf n\in E],
$$

where $(\mathcal U n)\,Q(n)$ means $\{n:Q(n)\}\in\mathcal U$. This is the ordered [Fubini product of ultrafilters](../../../set-theory.md#fubini-product-of-ultrafilters). Closure under intersections and the decision between a [set](../../../set.md) and its complement hold at each nested level, proving it is an [ultrafilter](../../../set-theory.md#ultrafilter). For $F=\varnothing$ take the [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) on the one-point product. Put

$$
N_F=M_0^{\mathbb N^F}/\mathcal U_F.
$$

If $F\subseteq G$, pull a [function](../../../function.md) back along the projection $\mathbb N^G\to\mathbb N^F$. A test independent of an omitted coordinate is unchanged by its [ultrafilter](../../../set-theory.md#ultrafilter) quantifier, so projection pushes $\mathcal U_G$ to $\mathcal U_F$. The induced map $N_F\to N_G$ is therefore an [elementary embedding](../../../set-theory.md#elementary-embedding) by [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem). These maps are coherent, giving a directed system indexed by finite subsets of $I$.

Take its [directed limit of elementary embeddings](../../../foundations-of-mathematics.md#directed-limit-of-elementary-embeddings) $N$. One can verify elementarity directly: representatives of a finite tuple occur at a common stage; [functions](../../../function.md) and atomic relations are interpreted there. In the existential step, a witness in the limit occurs with the parameters at some later common stage, and elementarity pulls the existence statement back. Thus every $N_F$ embeds elementarily into $N$, which contains an elementary copy of $M^+$.

For $i\in F$, let $a_i$ be the class of the coordinate [function](../../../function.md) $\mathbf n\mapsto b_{n_i}$. Projection coherence makes this independent of $F$. If $i<j$, then for each fixed $n_i$ the [set](../../../set.md) $\{n_j:n_j\ne n_i\}$ is cofinite. The nested test therefore gives $a_i\ne a_j$. In the ordered variant, the same argument with $n_j>n_i$ gives $P(a_i)$ and $a_i<a_j$.

For every [first-order formula](../../../mathematical-logic.md#first-order-formula) $\varphi$ of the expanded language and every increasing tuple $i_1<\cdots<i_r$, [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) gives

$$
N\models\varphi(a_{i_1},\ldots,a_{i_r})\quad\Longleftrightarrow\quad(\mathcal U n_1)\cdots(\mathcal U n_r)\,[M_0\models\varphi(b_{n_1},\ldots,b_{n_r})].
$$

The right-hand side depends on the [first-order formula](../../../mathematical-logic.md#first-order-formula) and tuple length, not on the indices. This proves order indiscernibility in the expanded language. Let $H$ be the [Skolem hull](../../../mathematical-logic.md#skolem-hull) of the generators in $N$. The [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test) gives $H\prec N$, and its reduct is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $\operatorname{Th}(M)$.

An [order automorphism](../../../set.md#order-automorphism) $\pi$ of $I$ acts by

$$
t(a_{i_1},\ldots,a_{i_r})\longmapsto t(a_{\pi(i_1)},\ldots,a_{\pi(i_r)}).
$$

Indiscernibility makes this well defined: combine the finite supports of two term expressions into one increasing tuple, and apply indiscernibility to their [logical equality](../../../mathematical-logic.md#logical-equality). Applying it to relation [first-order formulas](../../../mathematical-logic.md#first-order-formula) proves preservation of all relations; the inverse is induced by $\pi^{-1}$. Every element of the hull is such a term, so the extension is unique among [structure automorphisms](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) preserving the [Skolem expansion](../../../mathematical-logic.md#skolem-expansion). Moreover

$$
\boxed{|H|\leq\max(|I|,|L|,\aleph_0),\quad\text{and }|H|=|I|\text{ if }|I|\geq|L|+\aleph_0.}
$$

This proves the theorem, including its ordered version and [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) conclusion, using [ultrapowers](../../../foundations-of-mathematics.md#ultrapower) and a directed limit throughout.

## 5

↑ **Parent:** [Paper 135](paper-135.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the [Gödel-Gentzen negative translation](../../../mathematical-logic.md#godel-gentzen-negative-translation), writing $A^N$ for the translated [first-order formula](../../../mathematical-logic.md#first-order-formula). On [atomic formulas](../../../mathematical-logic.md#atomic-formula) $P$, including [logical equality](../../../mathematical-logic.md#logical-equality), put $P^N=\neg\neg P$, and put $\bot^N=\bot$. Extend recursively by

$$
\begin{aligned}
(A\land B)^N&=A^N\land B^N,&(A\to B)^N&=A^N\to B^N,\\
(\forall x\,A)^N&=\forall x\,A^N,&(A\lor B)^N&=\neg\neg(A^N\lor B^N),\\
(\exists x\,A)^N&=\neg\neg\exists x\,A^N.&
\end{aligned}
$$

[Logical negation](../../../computer-science.md#negation) abbreviates [logical implication](../../../mathematical-logic.md#logical-implication) to [logical falsity](../../../mathematical-logic.md#logical-falsity), so $(\neg A)^N=\neg A^N$. The displayed [logical disjunction](../../../mathematical-logic.md#logical-disjunction) and existential clauses are intuitionistically equivalent to the usual negative clauses $\neg(\neg A^N\land\neg B^N)$ and $\neg\forall x\,\neg A^N$, respectively. Thus these clauses specify the same [negative interpretation](../../../mathematical-logic.md#godel-gentzen-negative-translation). Translation commutes with [capture-avoiding substitution](../../../foundations-of-mathematics.md#capture-avoiding-substitution) of terms for [free variables](../../../mathematical-logic.md#free-variable).

First prove by [structural induction](../../../foundations-of-mathematics.md#structural-induction) the [stability of a formula under double negation](../../../mathematical-logic.md#stability-of-a-formula-under-double-negation):

$$
\mathrm{IL}\vdash\neg\neg A^N\to A^N.
$$

Every double [logical negation](../../../computer-science.md#negation) is stable, since [intuitionistic first-order logic](../../../mathematical-logic.md#intuitionistic-first-order-logic) proves $\neg\neg\neg\neg C\to\neg\neg C$; [logical falsity](../../../mathematical-logic.md#logical-falsity) is stable as well. Stability passes to [logical conjunction](../../../mathematical-logic.md#logical-conjunction) by obtaining double [logical negation](../../../computer-science.md#negation) of each component. For a [logical implication](../../../mathematical-logic.md#logical-implication) $C\to D$ with stable $D$, assume $\neg\neg(C\to D)$ and $C$. An assumption $\neg D$ would give $\neg(C\to D)$, a contradiction, so $\neg\neg D$ and then $D$. For a universal [first-order formula](../../../mathematical-logic.md#first-order-formula), $\neg\neg\forall x\,C(x)$ implies $\neg\neg C(y)$ for arbitrary fresh $y$; use stability pointwise and generalize. [Logical disjunction](../../../mathematical-logic.md#logical-disjunction) and existential translations are already double negations. This proves all cases.

Now regard classical first-order [natural deduction](../../../mathematical-logic.md#natural-deduction) as intuitionistic [natural deduction](../../../mathematical-logic.md#natural-deduction) plus unrestricted [double-negation elimination](../../../mathematical-logic.md#double-negation-elimination), and induct on a classical derivation. The rules for [logical conjunction](../../../mathematical-logic.md#logical-conjunction), [logical implication](../../../mathematical-logic.md#logical-implication), [universal quantification](../../../mathematical-logic.md#universal-quantification) and [logical falsity](../../../mathematical-logic.md#logical-falsity) translate directly. [Logical disjunction](../../../mathematical-logic.md#logical-disjunction) introduction gives $A^N\lor B^N$ and then its double [logical negation](../../../computer-science.md#negation). For [logical disjunction](../../../mathematical-logic.md#logical-disjunction) elimination, the translated premise is $\neg\neg(A^N\lor B^N)$ and the two translated branches yield the stable conclusion $C^N$. Assuming $\neg C^N$ makes each branch contradictory, giving $\neg A^N$ and $\neg B^N$, hence $\neg(A^N\lor B^N)$, which contradicts the premise. We have $\neg\neg C^N$ and remove it by stability.

Existential introduction likewise adds a double [logical negation](../../../computer-science.md#negation) to the ordinary witness introduction. In existential elimination, the witness branch $A^N(y)\vdash C^N$ has the original fresh-variable condition. Assuming $\neg C^N$ makes that branch give $\neg A^N(y)$; generalization gives $\forall y\,\neg A^N(y)$ and therefore $\neg\exists y\,A^N(y)$, contradicting the translated premise. Again stability supplies $C^N$. The universal-rule side conditions are preserved because the translation introduces no new [free variables](../../../mathematical-logic.md#free-variable).

For [logical equality](../../../mathematical-logic.md#logical-equality), reflexivity gives $t=t$ and then its double [logical negation](../../../computer-science.md#negation). For substitution, from $\neg\neg(s=t)$ and $A^N(s)$, temporarily assume $\neg A^N(t)$. An assumption $s=t$ would transport $A^N(s)$ to $A^N(t)$ by intuitionistic [logical equality](../../../mathematical-logic.md#logical-equality) substitution, so it gives a contradiction and hence $\neg(s=t)$. The first premise contradicts this. Thus $\neg\neg A^N(t)$ holds and stability gives $A^N(t)$. Finally a classical [double-negation elimination](../../../mathematical-logic.md#double-negation-elimination) step translates precisely to $\neg\neg A^N\to A^N$, already proved. Every rule is therefore covered, giving [negative translation of a classical proof](../../../mathematical-logic.md#negative-translation-of-a-classical-proof):

$$
\boxed{\Gamma\vdash_{\mathrm{CL}}\varphi\quad\Longrightarrow\quad\Gamma^N\vdash_{\mathrm{IL}}\varphi^N.}
$$

In particular a classical thesis has an intuitionistic, constructive translated proof. If nonlogical assumptions are present, they must be translated too.

In classical logic, [double-negation elimination](../../../mathematical-logic.md#double-negation-elimination) gives $P^N\leftrightarrow P$ on atoms. [Structural induction](../../../foundations-of-mathematics.md#structural-induction) propagates equivalence through [logical conjunction](../../../mathematical-logic.md#logical-conjunction), [logical implication](../../../mathematical-logic.md#logical-implication) and both quantifiers, and removes the added double negations on [logical disjunction](../../../mathematical-logic.md#logical-disjunction) and existence. Therefore

$$
\boxed{\mathrm{CL}\vdash\varphi^N\leftrightarrow\varphi,\qquad\mathrm{CL}\vdash\varphi\ \Longrightarrow\ \mathrm{IL}\vdash\varphi^N.}
$$

## 6

↑ **Parent:** [Paper 135](paper-135.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use [untyped lambda calculus](../../../foundations-of-mathematics.md#untyped-lambda-calculus) and [normal-order beta reduction](../../../foundations-of-mathematics.md#normal-order-beta-reduction). Write $c_n=\lambda f x.f^n x$ for the [Church numeral](../../../foundations-of-mathematics.md#church-numeral) of $n$. We will construct a closed term $F$ such that

$$
F c_{n_1}\cdots c_{n_k}\longrightarrow_\beta^*c_{f(\mathbf n)}
$$

when $f(\mathbf n)$ is defined, and with no [head normal form](../../../foundations-of-mathematics.md#head-normal-form) otherwise. The latter condition implies that the result is not in [beta equivalence](../../../foundations-of-mathematics.md#beta-equivalence) with any [Church numeral](../../../foundations-of-mathematics.md#church-numeral), so both definedness and the output are represented.

First represent all total [primitive recursive functions](../../../foundations-of-mathematics.md#primitive-recursive-function). The [zero function](../../../foundations-of-mathematics.md#zero-function) is $\lambda\mathbf x.c_0$, the [successor function](../../../foundations-of-mathematics.md#successor-function) is

$$
\mathsf{Succ}=\lambda n f x.f(nfx),
$$

and the $i$th [projection function](../../../foundations-of-mathematics.md#projection-function) is $\lambda x_1\cdots x_k.x_i$. [Function composition in recursion theory](../../../foundations-of-mathematics.md#function-composition-in-recursion-theory) is represented by $\lambda\mathbf x.G(H_1\mathbf x)\cdots(H_r\mathbf x)$. This composition claim is used here for total [functions](../../../function.md), whose inner terms all reduce to numerals.

For [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion) use [Church pairs](../../../foundations-of-mathematics.md#church-pair) and iteration. Put

$$
\mathsf T=\lambda a b.a,\quad\mathsf F=\lambda a b.b,\quad\mathsf{Pair}=\lambda a b p.pab,\quad\mathsf{Fst}=\lambda p.p\mathsf T,\quad\mathsf{Snd}=\lambda p.p\mathsf F.
$$

Suppose $G,H$ represent the total constituents of $f(\mathbf x,0)=g(\mathbf x)$ and $f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n))$. Define

$$
\begin{aligned}
\mathsf{Step}_{\mathbf x}&=\lambda p.\mathsf{Pair}\bigl(\mathsf{Succ}(\mathsf{Fst}\,p)\bigr)\bigl(H\mathbf x(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)\bigr),\\
R&=\lambda\mathbf x n.\mathsf{Snd}\bigl(n\mathsf{Step}_{\mathbf x}(\mathsf{Pair}\,c_0\,(G\mathbf x))\bigr).
\end{aligned}
$$

After $j$ iterations the pair reduces to $\mathsf{Pair}\,c_j\,c_{f(\mathbf x,j)}$, by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $j$. Its second projection is the required result. This [lambda definition of primitive recursion by pair iteration](../../../foundations-of-mathematics.md#lambda-definition-of-primitive-recursion-by-pair-iteration) and [structural induction](../../../foundations-of-mathematics.md#structural-induction) on the primitive recursive construction give terms for all [primitive recursive functions](../../../foundations-of-mathematics.md#primitive-recursive-function).

For an arbitrary [partial computable function](../../../foundations-of-mathematics.md#computable-function) use the [Kleene normal form theorem](../../../foundations-of-mathematics.md#kleene-normal-form-theorem) with its program index fixed. There are total [primitive recursive functions](../../../foundations-of-mathematics.md#primitive-recursive-function) $C(\mathbf x,s)$ and $U(s)$ such that $C$ is zero exactly when $s$ codes a valid halting computation history on $\mathbf x$, and $U$ extracts that history's output. Checking finite coded configurations and each transition is primitive recursive. Determinism ensures that every accepted history on an input has the same output. Hence

$$
f(\mathbf x)=U(\mu s\,[C(\mathbf x,s)=0]).
$$

If the input computation never halts, no history is accepted. Let $\widehat C,\widehat U$ be the total numeral-representing terms already obtained. The [Church numeral zero test](../../../foundations-of-mathematics.md#church-numeral-zero-test) is $\mathsf{Zero}=\lambda n.n(\lambda z.\mathsf F)\mathsf T$, returning $\mathsf T$ exactly on zero. A [Church Boolean](../../../foundations-of-mathematics.md#church-boolean) applied to two arguments selects the appropriate branch without evaluating the other.

Take the [fixed-point combinator](../../../foundations-of-mathematics.md#fixed-point-combinator) $Y=\lambda h.(\lambda z.h(zz))(\lambda z.h(zz))$. For the input tuple define

$$
G_{\mathbf x}=\lambda r s.\bigl(\mathsf{Zero}(\widehat C\mathbf x s)\bigr)\,(\widehat U s)\,(r(\mathsf{Succ}\,s)),\qquad F=\lambda\mathbf x.(YG_{\mathbf x})c_0.
$$

Expanding the displayed abbreviations gives a genuine finite [combinator](../../../foundations-of-mathematics.md#combinator). At a numeral code $c_j$, the total predicate computation terminates. If it returns a positive numeral, the false [Church Boolean](../../../foundations-of-mathematics.md#church-boolean) selects the next search code. If it returns zero, the true [Church Boolean](../../../foundations-of-mathematics.md#church-boolean) selects $\widehat U c_j$, which reduces to the output numeral. If the least accepted code is $s$, a finite [sequence](../../../real-analysis.md#sequence) of these tests reaches it and then produces $c_{U(s)}$.

If there is no accepted code, every test is false and head reduction moves through codes $0,1,2,\ldots$ forever. At no finite point can a head variable or an outer numeral abstraction be produced: the applied search term must first unfold the fixed point and evaluate the next total test, and the decoder branch is always discarded. Thus it has no [head normal form](../../../foundations-of-mathematics.md#head-normal-form). The standard head-normalization property, or the [Church-Rosser theorem](../../../foundations-of-mathematics.md#church-rosser-theorem) together with normalization of normal-order reduction, rules out [beta equivalence](../../../foundations-of-mathematics.md#beta-equivalence) to a numeral. In particular, we have avoided a lazy-composition pitfall: an outer [function](../../../function.md) that discards an argument need not force a divergent inner computation. The decoder is reached only after the guarded search succeeds. This proves [lambda representation of partial computable functions](../../../foundations-of-mathematics.md#lambda-representation-of-partial-computable-functions):

$$
\boxed{f(\mathbf n)\downarrow=m\Rightarrow F\mathbf c_{\mathbf n}\equiv_\beta c_m,\qquad f(\mathbf n)\uparrow\Rightarrow F\mathbf c_{\mathbf n}\text{ has no head normal form.}}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
