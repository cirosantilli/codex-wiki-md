# Paper 120

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_120.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_120.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Under the [Curry-Howard correspondence](../../../mathematical-logic.md#curry-howard-correspondence), [Intuitionistic propositional logic](../../../mathematical-logic.md#intuitionistic-propositional-logic) propositions are types and proofs are typed terms. Assumptions correspond to typed variables. The [logical implication](../../../mathematical-logic.md#logical-implication) $A\to B$ corresponds to the function type, [logical conjunction](../../../mathematical-logic.md#logical-conjunction) $A\wedge B$ to the product type, [logical disjunction](../../../mathematical-logic.md#logical-disjunction) $A\vee B$ to the sum type, [logical truth](../../../mathematical-logic.md#logical-truth) to the unit type, and [logical falsity](../../../mathematical-logic.md#logical-falsity) to the empty type.

The rules of [natural deduction](../../../mathematical-logic.md#natural-deduction) become term constructors. Implication introduction sends a derivation of $B$ from a variable $x:A$ to the abstraction $\lambda x.M:A\to B$, while implication elimination becomes application $MN$. Pairing and projection implement conjunction, and injections with case analysis implement disjunction. Under this correspondence, normalization of proofs is computation by [beta reduction](../../../foundations-of-mathematics.md#beta-reduction) in the [simply typed lambda calculus](../../../foundations-of-mathematics.md#simply-typed-lambda-calculus).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [Heyting algebra](../../../mathematical-logic.md#heyting-algebra) is a bounded [lattice](../../../mathematical-logic.md#lattice) $H$ equipped with an operation $a\Rightarrow b$ satisfying

$$
x\leq(a\Rightarrow b)
\quad\Longleftrightarrow\quad
x\wedge a\leq b.
$$

Thus, for fixed $a$, the map $x\mapsto x\wedge a$ is left adjoint to $y\mapsto a\Rightarrow y$. A left adjoint preserves joins, so

$$
a\wedge(b\vee c)=(a\wedge b)\vee(a\wedge c).
$$

This is one [distributive law for lattices](../../../mathematical-logic.md#distributive-law-for-lattices); the other follows from it and the absorption laws. Hence every Heyting algebra is a [distributive lattice](../../../mathematical-logic.md#distributive-lattice). This argument is the [distributivity of a Heyting algebra](../../../mathematical-logic.md#distributivity-of-a-heyting-algebra).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take a three-world [Kripke model for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-model-for-intuitionistic-propositional-logic) with a root $r$ and two incomparable terminal successors $u$ and $v$. Force $p$ only at $u$, force $q$ only at $v$, and force neither atom at $r$.

At $u$, the atom $p$ holds, so $u\Vdash\neg\neg p$, while $u\nVdash q$. Therefore

$$
r\nVdash\neg\neg p\to q.
$$

Likewise $v\Vdash\neg\neg q$ and $v\nVdash p$, so

$$
r\nVdash\neg\neg q\to p.
$$

The [Kripke forcing relation](../../../mathematical-logic.md#kripke-forcing-relation) for a disjunction requires one disjunct to be forced at the current world. Consequently

$$
r\nVdash(\neg\neg p\to q)\vee(\neg\neg q\to p),
$$

which is the required [Kripke countermodel](../../../mathematical-logic.md#kripke-countermodel).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Soundness follows by induction on derivations: assumptions are forced by hypothesis, implication introduction uses the definition of [Kripke forcing relation](../../../mathematical-logic.md#kripke-forcing-relation), and implication elimination uses it at the current world.

For completeness, form the [canonical Kripke model for implicational intuitionistic logic](../../../mathematical-logic.md#canonical-kripke-model-for-implicational-intuitionistic-logic). Its worlds are [deductively closed](../../../mathematical-logic.md#deductively-closed-set-of-formulae) implicational theories $\Delta$ extending $\operatorname{Cn}(\Gamma)$, ordered by inclusion, and

$$
\Delta\Vdash p\quad\Longleftrightarrow\quad p\in\Delta
$$

for each atom $p$. We prove the truth lemma

$$
\Delta\Vdash\alpha\quad\Longleftrightarrow\quad\alpha\in\Delta
$$

by induction on implicational formulas. The atomic case is the definition. For $\alpha\to\beta$, membership implies forcing by closure under implication elimination. Conversely, if $\alpha\to\beta\notin\Delta$, the implication-introduction rule shows that $\operatorname{Cn}(\Delta\cup\{\alpha\})$ does not contain $\beta$; this extension forces $\alpha$ but not $\beta$, so $\Delta$ does not force $\alpha\to\beta$.

If $\Gamma\nvdash_{\mathrm{IPC}(\to)}\varphi$, the root $\operatorname{Cn}(\Gamma)$ of this canonical model forces every member of $\Gamma$ but does not force $\varphi$. Together with soundness, this proves [Kripke completeness of implicational intuitionistic logic](../../../mathematical-logic.md#kripke-completeness-of-implicational-intuitionistic-logic).

Finally suppose the implicational formulas $\Gamma$ and $\varphi$ satisfy $\Gamma\vdash_{\mathrm{IPC}}\varphi$. The [soundness theorem for propositional logic](../../../mathematical-logic.md#soundness-theorem-for-propositional-logic) for intuitionistic Kripke semantics gives $\Gamma\models_{\mathrm{Kripke}}\varphi$, and the completeness just proved gives $\Gamma\vdash_{\mathrm{IPC}(\to)}\varphi$. This is the [conservativity of intuitionistic propositional logic over its implicational fragment](../../../mathematical-logic.md#conservativity-of-intuitionistic-propositional-logic-over-its-implicational-fragment).

## 2

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a [first-order theory](../../../mathematical-logic.md#first-order-theory) $T$ in a [first-order language](../../../mathematical-logic.md#first-order-language) $L$, a complete $n$-type is a maximal $T$-consistent set $p(x_1,\ldots,x_n)$ of [formulas](../../../mathematical-logic.md#first-order-formula) whose free variables lie among $x_1,\ldots,x_n$. Equivalently, it chooses exactly one of $\varphi$ and $\neg\varphi$ for every such formula while remaining consistent with $T$.

An [isolated type](../../../foundations-of-mathematics.md#isolated-type) $p$ is isolated by a formula $\theta(\bar x)$ when $T\cup\{\exists\bar x\,\theta(\bar x)\}$ is consistent and

$$
T\models\forall\bar x\,(\theta(\bar x)\to\varphi(\bar x))
$$

for every $\varphi\in p$. The type is an [omitted type](../../../foundations-of-mathematics.md#omitted-type) in an $L$-structure $M$ when no tuple $\bar a\in M^n$ satisfies every formula in $p$.

The [omitting types theorem](../../../foundations-of-mathematics.md#omitting-types-theorem) states that if $T$ is a consistent theory in a countable language and $(p_i)_{i\in\mathbb N}$ is a countable family of nonisolated finite-arity types, then $T$ has a countable model omitting every $p_i$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\mathcal U$ be a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) on an infinite set $I$. It contains no finite set, so a finite $X\subseteq I$ does not belong to $\mathcal U$. An [ultrafilter](../../../set-theory.md#ultrafilter) contains exactly one of a set and its complement; hence $I\setminus X\in\mathcal U$. Equivalently, every nonprincipal ultrafilter contains the [cofinite filter](../../../set-theory.md#cofinite-filter).

For structures $(M_i)_{i\in I}$ and a first-order formula $\varphi$, the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) says

$$
\prod_{i\in I}M_i/\mathcal U\models\varphi([a_i^1],\ldots,[a_i^k])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(a_i^1,\ldots,a_i^k)\}\in\mathcal U.
$$

Fix a [prime number](../../../number-theory.md#prime-number) $p$, take $I=\mathbb N_{>0}$, and choose a nonprincipal ultrafilter on $I$. The [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct)

$$
K=\prod_{n\geq1}\mathbb F_{p^n}/\mathcal U
$$

is a [field](../../../algebra.md#field) because each factor is a [finite field](../../../algebra.md#finite-field), and it has [characteristic](../../../algebra.md#characteristic-of-a-field) $p$ because each factor satisfies $p\cdot1=0$ and $m\cdot1\ne0$ for $1\leq m<p$. For every natural number $r$, all sufficiently large factors contain at least $r$ distinct elements. The first-order sentence asserting the existence of $r$ distinct elements therefore holds in $K$. Thus $K$ is infinite, as summarized by [infinite field of positive characteristic from an ultraproduct](../../../foundations-of-mathematics.md#infinite-field-of-positive-characteristic-from-an-ultraproduct).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem) says that if a first-order theory $T$ has an infinite model, then for every [total order](../../../set.md#total-order) $I$ there is a model $M\models T$ generated as the [Skolem hull](../../../mathematical-logic.md#skolem-hull) of distinct [order indiscernibles](../../../foundations-of-mathematics.md#order-indiscernible-sequence) $(a_i)_{i\in I}$, and every order automorphism of $I$ extends to an [automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) of $M$.

Given an infinite cardinal $\kappa$, let $I=\kappa\times\mathbb Q$ with the lexicographic order, viewed as $\kappa$ consecutive copies of the rational order. In each copy independently choose either the identity or a fixed nonidentity order automorphism of $\mathbb Q$. These choices give $2^\kappa$ distinct order automorphisms of $I$.

Apply the theorem to this order. Distinct order automorphisms act differently on the distinct generators $a_i$, so their extensions give an injection into the [automorphism group of a first-order structure](../../../mathematical-logic.md#automorphism-group-of-a-first-order-structure) $\operatorname{Aut}(M)$. Therefore $|\operatorname{Aut}(M)|\geq2^\kappa$, proving that $T$ has [models with arbitrarily large automorphism groups](../../../foundations-of-mathematics.md#models-with-arbitrarily-large-automorphism-groups).

## 3

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Church numeral](../../../foundations-of-mathematics.md#church-numeral) corresponding to the [natural number](../../../arithmetic.md#natural-number) $n$ is

$$
c_n=\lambda f.\lambda x.f^n x.
$$

A function $g:\mathbb N^k\to\mathbb N$ is a [lambda-definable function](../../../foundations-of-mathematics.md#lambda-definable-function) if some closed lambda term $G$ satisfies

$$
G c_{n_1}\cdots c_{n_k}\equiv_\beta c_{g(n_1,\ldots,n_k)}
$$

for all natural numbers $n_1,\ldots,n_k$.

Define

$$
\operatorname{Succ}=\lambda n.\lambda f.\lambda x.f(nfx).
$$

Then [beta reduction](../../../foundations-of-mathematics.md#beta-reduction) gives

$$
\operatorname{Succ}\,c_n
\equiv_\beta\lambda f.\lambda x.f(f^n x)
=c_{n+1}.
$$

**Therefore the [successor function](../../../foundations-of-mathematics.md#successor-function) is lambda-definable; this is the [lambda definition of the successor function](../../../foundations-of-mathematics.md#lambda-definition-of-the-successor-function).**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [combinator](../../../foundations-of-mathematics.md#combinator) is a lambda term without free variables. It is a [fixed-point combinator](../../../foundations-of-mathematics.md#fixed-point-combinator) when

$$
YF\equiv_\beta F(YF)
$$

for every lambda term $F$.

The [fixed-point theorem for the untyped lambda calculus](../../../foundations-of-mathematics.md#fixed-point-theorem-for-the-untyped-lambda-calculus) states that every untyped lambda term $F$ has a fixed point up to [beta equivalence](../../../foundations-of-mathematics.md#beta-equivalence). Put

$$
X=(\lambda x.F(xx))(\lambda x.F(xx)).
$$

One beta reduction gives

$$
X\longrightarrow_\beta F((\lambda x.F(xx))(\lambda x.F(xx)))=F(X),
$$

which proves the theorem. Equivalently,

$$
Y=\lambda f.(\lambda x.f(xx))(\lambda x.f(xx))
$$

is a fixed-point combinator.

Apply the theorem to the lambda term $\operatorname{Succ}$. Its fixed point $Y\operatorname{Succ}$ is a nonnormalizing lambda term satisfying $Y\operatorname{Succ}\equiv_\beta\operatorname{Succ}(Y\operatorname{Succ})$; it is not a [Church numeral](../../../foundations-of-mathematics.md#church-numeral). The definition of a [lambda-definable function](../../../foundations-of-mathematics.md#lambda-definable-function) describes the representing term only on Church-numeral inputs, so it does not turn this syntactic fixed point into a natural number $n$ satisfying $n+1=n$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

By assumption the set of [combinators](../../../foundations-of-mathematics.md#combinator) is [recursively enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set). Finite [beta reduction](../../../foundations-of-mathematics.md#beta-reduction) sequences, and hence finite certificates of [beta equivalence](../../../foundations-of-mathematics.md#beta-equivalence), are also recursively enumerable.

For a closed term $Y$, choose a fresh variable $f$. The term $Y$ is a fixed-point combinator exactly when

$$
Yf\equiv_\beta f(Yf).
$$

Indeed, substitution then gives the required equivalence for every $F$, and the forward direction follows by taking $F=f$. [Dovetail](../../../foundations-of-mathematics.md#dovetailing) the enumeration of closed terms with all finite beta-equivalence certificates. Whenever a certificate of the displayed equivalence is found, output $Y$. This enumerates exactly the fixed-point combinators, proving [recursively enumerable fixed-point combinators](../../../foundations-of-mathematics.md#recursively-enumerable-fixed-point-combinators).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
