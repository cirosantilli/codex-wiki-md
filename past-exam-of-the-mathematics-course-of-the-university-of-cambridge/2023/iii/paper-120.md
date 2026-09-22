# Paper 120

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_120.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_120.pdf)

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

## 1

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [Kripke model for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-model-for-intuitionistic-propositional-logic) is a triple $(W,\leq,V)$ in which $(W,\leq)$ is a [partially ordered set](../../../set.md#partially-ordered-set) of worlds and $V(p)\subseteq W$ is upward closed for every propositional variable $p$. The [Kripke forcing relation](../../../mathematical-logic.md#kripke-forcing-relation) is defined recursively by

$$
w\Vdash p\iff w\in V(p),
$$

with the usual clauses for $\top$, $\bot$, conjunction and disjunction, and with

$$
w\Vdash A\to B
\iff
\text{for every }v\geq w,\ v\Vdash A\Longrightarrow v\Vdash B.
$$

The upward closure of the valuation implies [persistence of intuitionistic Kripke forcing](../../../mathematical-logic.md#persistence-of-intuitionistic-kripke-forcing): if $w\leq v$ and $w\Vdash A$, then $v\Vdash A$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Kripke completeness theorem for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-completeness-theorem-for-intuitionistic-propositional-logic) states that, for every set of formulae $\Gamma$ and formula $A$,

$$
\Gamma\vdash_{\mathrm{IPC}}A
\quad\Longleftrightarrow\quad
\text{every world of every intuitionistic Kripke model that forces $\Gamma$ also forces $A$}.
$$

The forward implication is [soundness](../../../mathematical-logic.md#soundness-theorem-for-propositional-logic), and the reverse implication is completeness.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take two worlds $r<s$ and let $p$ be forced only at $s$. Neither world forces $\neg p$: at $s$ this follows from $s\Vdash p$, while at $r$ the extension $s$ forces $p$. Consequently every extension of $r$ that forces $\neg p$ also forces $p$ vacuously, so

$$
r\Vdash\neg p\to p.
$$

But $r\nVdash p$. The implication clause therefore gives

$$
r\nVdash(\neg p\to p)\to p,
$$

which is a finite [Kripke countermodel](../../../mathematical-logic.md#kripke-countermodel) and proves that the formula is not intuitionistically valid.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Both sequents follow directly from the introduction and elimination rules of the [implication-free fragment of intuitionistic propositional logic](../../../mathematical-logic.md#implication-free-fragment-of-intuitionistic-propositional-logic). From a proof of $\phi\wedge(\psi\vee\chi)$, eliminate the conjunction to obtain $\phi$ and $\psi\vee\chi$. Eliminate the disjunction: in the $\psi$ branch introduce $\phi\wedge\psi$ and then the left disjunct; in the $\chi$ branch introduce $\phi\wedge\chi$ and then the right disjunct. This yields

$$
\phi\wedge(\psi\vee\chi)
\vdash
(\phi\wedge\psi)\vee(\phi\wedge\chi).
$$

Conversely, eliminate the outer disjunction. From $\phi\wedge\psi$, obtain $\phi$ and introduce the left side of $\psi\vee\chi$; from $\phi\wedge\chi$, obtain $\phi$ and introduce its right side. In either branch, conjunction introduction produces $\phi\wedge(\psi\vee\chi)$. Hence

$$
(\phi\wedge\psi)\vee(\phi\wedge\chi)
\vdash
\phi\wedge(\psi\vee\chi).
$$

This is the proof-theoretic form of the [distributive law for lattices](../../../mathematical-logic.md#distributive-law-for-lattices).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Suppose neither $\phi$ nor $\psi$ is provable. By the [Kripke completeness theorem for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-completeness-theorem-for-intuitionistic-propositional-logic), there are rooted [Kripke countermodels](../../../mathematical-logic.md#kripke-countermodel) with roots $r_\phi\nVdash\phi$ and $r_\psi\nVdash\psi$. Take their disjoint union and place a fresh world $r$ below every world in both components, forcing no propositional variables at $r$ beyond those required by persistence.

If $r\Vdash\phi$, persistence would imply $r_\phi\Vdash\phi$, a contradiction; similarly $r\nVdash\psi$. Thus $r\nVdash\phi\vee\psi$. By soundness, $\phi\vee\psi$ is not provable. Taking the contrapositive proves the [disjunction property of intuitionistic propositional logic](../../../mathematical-logic.md#disjunction-property-of-intuitionistic-propositional-logic):

$$
\boxed{\vdash_{\mathrm{IPC}}\phi\vee\psi
\quad\Longrightarrow\quad
\vdash_{\mathrm{IPC}}\phi\ \text{or}\ \vdash_{\mathrm{IPC}}\psi.}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Assume that $A$ is not intuitionistically valid. Completeness gives a [Kripke countermodel](../../../mathematical-logic.md#kripke-countermodel) for $A$. Apply [filtration of a Kripke model](../../../mathematical-logic.md#filtration-of-a-kripke-model) through the finite set of subformulae of $A$: two worlds are identified when they force the same subformulae, and the quotient order is induced by inclusion of those finite theories. The filtration lemma preserves the forcing of every subformula of $A$, so the image of the original counterexample world still fails to force $A$. There are at most $2^n$ quotient worlds when $A$ has $n$ distinct subformulae. Hence the quotient is a finite countermodel.

This proves the [Finite model property of intuitionistic propositional logic](../../../mathematical-logic.md#finite-model-property-of-intuitionistic-propositional-logic). Its contrapositive says that a proposition forced by every finite intuitionistic Kripke model is intuitionistically valid.

## 2

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [overspill lemma](../../../mathematical-logic.md#overspill-lemma) says that if $\mathcal M$ is a [nonstandard model of Peano arithmetic](../../../mathematical-logic.md#non-standard-model-of-arithmetic) and a definable property $\varphi(x,\bar a)$, possibly with parameters from $\mathcal M$, holds for every standard natural number, then it also holds for some nonstandard element of $\mathcal M$.

Let

$$
A=\{x\in M:\mathcal M\models\varphi(x,\bar a)\}.
$$

If $A$ had no nonstandard member, its complement would be nonempty. The [least-number principle](../../../mathematical-logic.md#least-number-principle) in [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic) would give a least $c\notin A$. Because every standard number belongs to $A$, the element $c$ would be nonstandard and nonzero. Its predecessor $c-1$ would also be nonstandard, so the supposition gives $c-1\notin A$, whereas the minimality of $c$ gives $c-1\in A$. This contradiction proves that $A$ contains a nonstandard element.

Applying this argument to $\psi(y)\equiv\forall x\leq y\,\varphi(x,\bar a)$ gives the useful stronger form: there is a nonstandard $b$ such that $\varphi(x,\bar a)$ holds for every $x\leq b$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**No such formula exists.** If $\phi(x)$ defined precisely the [standard cut of a nonstandard model of arithmetic](../../../mathematical-logic.md#standard-cut-of-a-nonstandard-model-of-arithmetic), then $\mathcal M\models\phi(n)$ for every standard natural number $n$. The [overspill lemma](../../../mathematical-logic.md#overspill-lemma) would produce a nonstandard $b\in M$ satisfying $\phi(b)$, contradicting the proposed definition. Thus the standard elements form an external, nondefinable subset of every nonstandard model of [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A term is in [beta-normal form](../../../foundations-of-mathematics.md#beta-normal-form) when it contains no [beta-redex](../../../foundations-of-mathematics.md#beta-redex), meaning no subterm of the form

$$
(\lambda x.M)N.
$$

Equivalently, no [beta reduction](../../../foundations-of-mathematics.md#beta-reduction) can be performed anywhere in the term.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Weak normalization theorem for simply typed lambda calculus](../../../foundations-of-mathematics.md#weak-normalization-theorem-for-simply-typed-lambda-calculus) states that every well-typed term of the [simply typed lambda calculus](../../../foundations-of-mathematics.md#simply-typed-lambda-calculus) admits at least one finite sequence of [beta reductions](../../../foundations-of-mathematics.md#beta-reduction) ending in a [beta-normal form](../../../foundations-of-mathematics.md#beta-normal-form).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**No.** The [Omega combinator](../../../foundations-of-mathematics.md#omega-combinator) is

$$
\Omega=(\lambda x.xx)(\lambda x.xx).
$$

Its only [beta-redex](../../../foundations-of-mathematics.md#beta-redex) contracts back to $\Omega$ itself. Every reduction sequence therefore repeats the same term, which is not in [beta-normal form](../../../foundations-of-mathematics.md#beta-normal-form). Thus $\Omega$ has no beta-normal form.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Suppose a [fixed-point combinator](../../../foundations-of-mathematics.md#fixed-point-combinator) $F$ were typable in the [simply typed lambda calculus](../../../foundations-of-mathematics.md#simply-typed-lambda-calculus). By the [Weak normalization theorem for simply typed lambda calculus](../../../foundations-of-mathematics.md#weak-normalization-theorem-for-simply-typed-lambda-calculus), it would have a [beta-normal form](../../../foundations-of-mathematics.md#beta-normal-form). For a fresh variable $f$, the term $Ff$ would then also possess a beta-normal form, say $N$.

The fixed-point property gives

$$
Ff\equiv_\beta f(Ff).
$$

Reducing the occurrence of $Ff$ on the right to $N$ gives the normal form $fN$. The [Church-Rosser theorem](../../../foundations-of-mathematics.md#church-rosser-theorem) says that these [beta-equivalent](../../../foundations-of-mathematics.md#beta-equivalence) terms must have [alpha-equivalent](../../../foundations-of-mathematics.md#alpha-equivalence) normal forms. This is impossible because $fN$ contains more symbols than $N$. Hence no typing context and simple type can type $F$.

## 3

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [prime filter of a distributive lattice](../../../mathematical-logic.md#prime-filter-of-a-distributive-lattice) $P$ is a proper [lattice filter](../../../mathematical-logic.md#lattice-filter): it contains the top element, is upward closed, and is closed under finite meets. Primality means

$$
\boxed{a\vee b\in P
\quad\Longrightarrow\quad
a\in P\ \text{or}\ b\in P.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Priestley dual space](../../../mathematical-logic.md#priestley-dual-space) $\widehat L$ of a [distributive lattice](../../../mathematical-logic.md#distributive-lattice) $L$ has all [prime filters](../../../mathematical-logic.md#prime-filter-of-a-distributive-lattice) of $L$ as its points. Its order is inclusion. For each $a\in L$, put

$$
a^*=\{P\in\widehat L:a\in P\}.
$$

The topology is generated by the sets $a^*$ and their complements. Each $a^*$ is therefore a [clopen up-set](../../../mathematical-logic.md#clopen-up-set), and these sets separate points and order. With this topology and order, $\widehat L$ is a compact totally order-disconnected ordered space.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Stone prime filter theorem](../../../mathematical-logic.md#stone-prime-filter-theorem) says that if a [lattice filter](../../../mathematical-logic.md#lattice-filter) $F$ and a [lattice ideal](../../../mathematical-logic.md#lattice-ideal) $I$ of a [distributive lattice](../../../mathematical-logic.md#distributive-lattice) are disjoint, then there is a [prime filter of a distributive lattice](../../../mathematical-logic.md#prime-filter-of-a-distributive-lattice) $P$ such that

$$
F\subseteq P
\quad\text{and}\quad
P\cap I=\varnothing.
$$

Equivalently, whenever $a\nleq b$, there is a prime filter containing $a$ and omitting $b$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For a prime filter $P\in\widehat H$, first suppose $a\Rightarrow b\in P$. If $Q\supseteq P$ and $a\in Q$, then $a\Rightarrow b\in Q$ and

$$
a\wedge(a\Rightarrow b)\leq b,
$$

so $b\in Q$. Thus no prime filter above $P$ belongs to $a^*\setminus b^*$, and

$$
P\notin\uparrow(a^*\setminus b^*).
$$

Conversely, suppose $a\Rightarrow b\notin P$. The [lattice filter](../../../mathematical-logic.md#lattice-filter) generated by $P\cup\{a\}$ is disjoint from the principal [lattice ideal](../../../mathematical-logic.md#lattice-ideal) $\mathord\downarrow b$. Indeed, an intersection would give some $p\in P$ with $p\wedge a\leq b$, whence $p\leq a\Rightarrow b$ and then $a\Rightarrow b\in P$, a contradiction. The [Stone prime filter theorem](../../../mathematical-logic.md#stone-prime-filter-theorem) therefore extends this filter to a prime filter $Q\supseteq P$ that omits $b$. Then $Q\in a^*\setminus b^*$, so $P\in\uparrow(a^*\setminus b^*)$.

We have proved, for every $P$,

$$
P\in(a\Rightarrow b)^*
\quad\Longleftrightarrow\quad
P\notin\uparrow(a^*\setminus b^*),
$$

which is the required identity

$$
\boxed{(a\Rightarrow b)^*=\bigl(\uparrow(a^*\setminus b^*)\bigr)^{\mathcal C}.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $L$ be any [distributive lattice](../../../mathematical-logic.md#distributive-lattice). Its [Stone map of a distributive lattice](../../../mathematical-logic.md#stone-map-of-a-distributive-lattice)

$$
a\longmapsto a^*
$$

is an injective lattice homomorphism from $L$ into the lattice of [clopen up-sets](../../../mathematical-logic.md#clopen-up-set) of its [Priestley dual space](../../../mathematical-logic.md#priestley-dual-space). In particular these images are open subsets of the underlying [topological space](../../../topology.md#topological-space), and the map preserves $\bot$, $\top$, finite meets and finite joins.

Now assume that an implication-free formula $\phi$ is valid under every lattice valuation in every topological space. Given any valuation of its variables in any distributive lattice $L$, compose it with the Stone map. Topological validity says that the resulting value of $\phi$ is the whole Priestley space. Injectivity of the Stone map then says that the original value of $\phi$ was $1_L$. Hence $\phi$ is valid in every distributive lattice.

By [completeness of implication-free intuitionistic propositional logic for distributive lattices](../../../mathematical-logic.md#completeness-of-implication-free-intuitionistic-propositional-logic-for-distributive-lattices), $\phi$ is provable in the [implication-free fragment of intuitionistic propositional logic](../../../mathematical-logic.md#implication-free-fragment-of-intuitionistic-propositional-logic).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
