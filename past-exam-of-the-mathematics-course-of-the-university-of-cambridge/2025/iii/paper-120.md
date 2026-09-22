# Paper 120

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20120.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20120.pdf)

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

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [Heyting algebra](../../../mathematical-logic.md#heyting-algebra) is a bounded [distributive lattice](../../../mathematical-logic.md#distributive-lattice) $L$ in which, for every $a,b\in L$, there is an element $a\Rightarrow b$ satisfying

$$
x\leq(a\Rightarrow b)\quad\Longleftrightarrow\quad x\wedge a\leq b.
$$

**Thus $a\Rightarrow b$ is the greatest element whose meet with $a$ lies below $b$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a finite distributive lattice, define

$$
a\Rightarrow b=\bigvee\{x\in L:x\wedge a\leq b\}.
$$

Distributivity and finiteness give

$$
a\wedge(a\Rightarrow b)=\bigvee_{x\wedge a\leq b}(a\wedge x)\leq b.
$$

Every $x$ with $x\wedge a\leq b$ occurs in the join, so $x\leq a\Rightarrow b$. This proves the defining adjunction and makes $L$ a [Heyting algebra](../../../mathematical-logic.md#heyting-algebra).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Under the [Curry-Howard correspondence](../../../mathematical-logic.md#curry-howard-correspondence), the term takes a proof $p$ of $\phi\wedge\psi$, extracts proofs of $\phi$ and $\psi$, and applies $f:\phi\to(\psi\to\bot)$ to obtain a contradiction. It is therefore a proof of

$$
(\phi\wedge\psi)\to\bigl((\phi\to\neg\psi)\to\bot\bigr),
$$

equivalently $(\phi\wedge\psi)\to\neg(\phi\to\neg\psi)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**No.** Although $\neg(\phi\to\neg\psi)$ is classically equivalent to $\phi\wedge\psi$, the reverse implication $\neg(\phi\to\neg\psi)\to\phi\wedge\psi$ is not intuitionistically valid, as part e shows. More generally, the standard normal-form separation theorem for the implicational fragment with falsity says that no formula built uniformly from $\phi,\psi,\to,\bot$ has both the pairing introduction rule and the two projection elimination rules of conjunction. Hence conjunction is not definable from implication and falsity in [Intuitionistic propositional logic](../../../mathematical-logic.md#intuitionistic-propositional-logic).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Use a two-world [Kripke model for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-model-for-intuitionistic-propositional-logic) $w<v$. Force neither $\phi$ nor $\psi$ at $w$, and force both at $v$. Neither world forces $\phi\to\neg\psi$: at $v$, both $\phi$ and $\psi$ hold, while at $w$ the extension $v$ is a counterexample. Therefore every extension of $w$ fails $\phi\to\neg\psi$, so

$$
w\Vdash\neg(\phi\to\neg\psi).
$$

But $w\nVdash\phi\wedge\psi$. The implication is therefore not intuitionistically valid by [Kripke completeness theorem for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-completeness-theorem-for-intuitionistic-propositional-logic).

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

If $w$ determines an atom $p$, then either $w\Vdash p$, in which case persistence gives $u\Vdash p$ for every $u\geq w$, or $w\Vdash\neg p$, in which case no such $u$ forces $p$. Thus every relevant atom has a constant truth value throughout the cone above $w$. Structural induction on $\phi$ now shows that every subformula has the same forcing value at all worlds above $w$: conjunction and disjunction are immediate, and an implication is forced exactly when the corresponding implication between these fixed truth values holds. Hence $w\Vdash\phi$ exactly when $w'\Vdash\phi$.

## 2

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Church-Rosser theorem](../../../foundations-of-mathematics.md#church-rosser-theorem) states that if $M\twoheadrightarrow_\beta N_1$ and $M\twoheadrightarrow_\beta N_2$, then there is a term $P$ with $N_1\twoheadrightarrow_\beta P$ and $N_2\twoheadrightarrow_\beta P$. Equivalently, beta reduction is confluent.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Weak normalization theorem for simply typed lambda calculus](../../../foundations-of-mathematics.md#weak-normalization-theorem-for-simply-typed-lambda-calculus) says that every term typable in the implicational [simply typed lambda calculus](../../../foundations-of-mathematics.md#simply-typed-lambda-calculus) has a beta-normal form. Define reducibility by induction on types: a term of atomic type is reducible when it is weakly normalizing, and $M:A\to B$ is reducible when $MN$ is reducible at $B$ for every reducible $N:A$. Induction on types shows that every reducible term is weakly normalizing and that variables are reducible.

The fundamental substitution lemma is proved by induction on a typing derivation: if $\Gamma\vdash M:A$ and each variable in $\Gamma$ is replaced by a reducible term of its declared type, then the resulting term is reducible at $A$. The application case is the definition at arrow type; in the abstraction case, applying the abstraction to any reducible argument makes one beta step to the substituted body, which is reducible by induction. Substituting each free variable by itself makes every well-typed term reducible, hence weakly normalizing.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A lambda term $F$ lambda-defines $f:\mathbb N^k\to\mathbb N$ when, for all $n_1,\ldots,n_k$,

$$
F\,c_{n_1}\cdots c_{n_k}\equiv_\beta c_{f(n_1,\ldots,n_k)},
$$

where $c_n$ is the [Church numeral](../../../foundations-of-mathematics.md#church-numeral) for $n$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**No.** Let $c_0=\lambda f.\lambda x.x$ and set

$$
R=\lambda n.c_0,
\qquad
S=\lambda n.n\,(\lambda x.c_0)\,c_0.
$$

Both terms send every [Church numeral](../../../foundations-of-mathematics.md#church-numeral) to $c_0$, so both define the constant-zero function. They are distinct beta-normal forms, however, and the [Church-Rosser theorem](../../../foundations-of-mathematics.md#church-rosser-theorem) implies that distinct beta-normal forms cannot be beta-equivalent.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Take

$$
\delta=\lambda x.\lambda f.f(xf).
$$

If $L$ is a [fixed-point combinator](../../../foundations-of-mathematics.md#fixed-point-combinator), then $Lf\equiv_\beta f(Lf)$, so eta-conversion gives

$$
L\equiv_\eta\lambda f.Lf\equiv_\beta\lambda f.f(Lf)=\delta L.
$$

Conversely, if $L\equiv_{\beta\eta}\delta L$, application to an arbitrary $f$ gives $Lf\equiv_{\beta\eta}f(Lf)$, which is precisely the fixed-point-combinator property.

## 3

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [Sigma-1 formula](../../../foundations-of-mathematics.md#sigma-1-formula) is a formula equivalent in arithmetic to $\exists y_1\cdots\exists y_r\,\delta$, where $\delta$ is bounded. A [Pi-1 formula](../../../foundations-of-mathematics.md#pi-1-formula) is similarly equivalent to $\forall y_1\cdots\forall y_r\,\delta$ with $\delta$ bounded.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The total function $f:\mathbb N^k\to\mathbb N$ is Sigma-1 represented in $T$ when there is a [Sigma-1 formula](../../../foundations-of-mathematics.md#sigma-1-formula) $F(\mathbf x,y)$ such that, for every standard tuple $\mathbf n$ and $m=f(\mathbf n)$,

$$
T\vdash\forall y\bigl(F(\overline{\mathbf n},y)\leftrightarrow y=\bar m\bigr).
$$

**Thus $T$ proves the correct unique output on every standard input.**

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [diagonal lemma](../../../mathematical-logic.md#diagonal-lemma) says that for every one-variable formula $\theta(x)$ there is a sentence $\gamma$ such that

$$
T\vdash\gamma\leftrightarrow\theta(\ulcorner\gamma\urcorner).
$$

Let $d(n)$ be the computable function taking the code of a one-variable formula $\alpha(x)$ to the code of $\alpha(\bar n)$. By the assumed representation theorem, choose a Sigma-1 formula $D(x,y)$ representing $d$. Given $\theta$, put

$$
\beta(x)=\exists y\bigl(D(x,y)\wedge\theta(y)\bigr)
$$

and let $b=\ulcorner\beta\urcorner$. Taking $\gamma=\beta(\bar b)$, representability proves in $T$ that the unique relevant $y$ is $d(b)=\ulcorner\gamma\urcorner$, yielding the required equivalence.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Suppose such a formula $\theta(x)$ existed. Apply the [diagonal lemma](../../../mathematical-logic.md#diagonal-lemma) to $\neg\theta(x)$ to obtain a sentence $\sigma$ for which

$$
\mathrm{PA}^-\vdash\sigma\leftrightarrow\neg\theta(\ulcorner\sigma\urcorner).
$$

Because $M\models\mathrm{PA}^-$, the equivalence holds in $M$. But the defining property of $\theta$ says $M\models\theta(\ulcorner\sigma\urcorner)$ exactly when $M\models\sigma$, producing $M\models\sigma$ exactly when $M\not\models\sigma$, a contradiction.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [Tennenbaum theorem](../../../mathematical-logic.md#tennenbaum-s-theorem) states that no countable nonstandard model of [Peano arithmetic](../../../mathematical-logic.md#peano-arithmetic) has a presentation on $\mathbb N$ in which both its addition and multiplication operations are recursive.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Assume multiplication in $M$ were recursive. The multiplication half of Tennenbaum's coding argument says that, for a fixed nonstandard code $c$, both

$$
\{n\in\mathbb N:M\models\operatorname{Bit}(c,\bar n)\}
\quad\text{and its complement}
$$

are computably enumerable from the multiplication table. The proof uses the canonical prime-power coding in PA; bounded inequalities are replaced by existential sum-of-four-squares conditions using the [Lagrange four-square theorem](../../../number-theory.md#lagrange-s-four-square-theorem), and the resulting witnesses can be searched for effectively from multiplication. Dovetailing the two searches decides the coded set. Applied to $c$, this would make $X$ recursive, contradicting the hypothesis. Therefore multiplication in $M$ cannot be recursive.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
