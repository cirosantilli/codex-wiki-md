# Paper 128

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20128.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20128.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)

## 1

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Lévy reflection theorem](../../../set-theory.md#levy-reflection-theorem) says that for every finite collection $\Phi$ of [first-order formulas](../../../mathematical-logic.md#first-order-formula) there are arbitrarily large [ordinals](../../../set-theory.md#ordinal) $\alpha$ such that, for every $\varphi\in\Phi$ and every tuple of parameters $a_1,\ldots,a_n\in V_\alpha$,

$$
V_\alpha\models\varphi(a_1,\ldots,a_n)
\quad\Longleftrightarrow\quad
V\models\varphi(a_1,\ldots,a_n).
$$

Equivalently, the ordinals simultaneously reflecting all formulas in $\Phi$ form a closed unbounded class.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $S$ be a finite subset of $\mathrm{ZFC}+\varphi$, and let $T$ be the finite collection of axioms of $\mathrm{ZFC}$ occurring in $S$. Choose the finite fragment $T^*$ supplied by the hypothesis. The [Lévy reflection theorem](../../../set-theory.md#levy-reflection-theorem) gives a level $V_\alpha$ satisfying $T^*$; the [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) gives a countable elementary substructure of that level, and the [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) turns it into a [countable transitive model](../../../forcing.md#countable-transitive-model) $M$ of $T^*$. By the assumed extension property, $M$ is contained in a countable transitive model $N$ of $T+\varphi$, so $N$ satisfies $S$.

This argument is formalizable over $\mathrm{ZFC}$ for each finite $T$. Hence, if $\mathrm{ZFC}$ is consistent, every finite subset of $\mathrm{ZFC}+\varphi$ is consistent. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) now gives

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})
\quad\Longrightarrow\quad
\operatorname{Con}(\mathrm{ZFC}+\varphi).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take $\lambda=\omega\cdot2$. This is a [limit ordinal](../../../set-theory.md#limit-ordinal) greater than $\omega$. There is a recursive [well-order code](../../../definable-power-set.md#well-order-code) $R$ for $\omega^2$: for example, use a recursive pairing of the [natural numbers](../../../arithmetic.md#natural-number) with $\omega\times\omega$ and the lexicographic order consisting of $\omega$ successive blocks of order type $\omega$. Since $R$ is definable over $L_\omega$, it belongs to $L_{\omega+1}$ and hence to $L_{\omega\cdot2}$.

The representation of $R$ is $\omega^2$, but

$$
\omega^2>\omega\cdot2
$$

and the [ordinals](../../../set-theory.md#ordinal) belonging to $L_\lambda$ are exactly those below $\lambda$. Thus $R\in L_\lambda$ while its representation is not in $L_\lambda$, violating the second requirement for a [coding level of the constructible hierarchy](../../../definable-power-set.md#coding-level-of-the-constructible-hierarchy).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Under $V=L$, the structure $L_{\omega_1}$ contains a [well-order code](../../../definable-power-set.md#well-order-code) for every [countable ordinal](../../../set-theory.md#countable-ordinal) and the representation of every well-order code that it contains. Given any $\alpha<\omega_1$, apply the [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) to choose a countable elementary substructure

$$
X\prec L_{\omega_1}
$$

containing $\alpha$. The [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) and condensation identify the transitive collapse of $X$ with $L_\lambda$, where $\lambda=X\cap\omega_1$ is a [limit ordinal](../../../set-theory.md#limit-ordinal) greater than $\alpha$.

Elementarity now verifies both coding properties. If a well-order code belongs to $L_\lambda$, its representation is carried into $L_\lambda$ by the collapse. Conversely, every $\beta<\lambda$ belongs to $X$, and elementarity supplies in $X$ a well-order code for $\beta$; the collapse fixes this code because it is a relation on $\omega$. Hence $L_\lambda$ is a [coding level of the constructible hierarchy](../../../definable-power-set.md#coding-level-of-the-constructible-hierarchy). Such $\lambda$ occur unboundedly below $\omega_1$, so $\Gamma$ has at least $\aleph_1$ elements; since $\Gamma\subseteq\omega_1$, it has exactly

$$
|\Gamma|=\aleph_1.
$$

## 2

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The two conventions reverse the order relation. In [standard notation for forcing](../../../forcing.md#standard-notation-for-forcing), $q\leq p$ means that $q$ is stronger than $p$. Thus $p$ and $q$ are [incompatible forcing conditions](../../../forcing.md#incompatible-forcing-conditions) when there is no $r$ with $r\leq p$ and $r\leq q$, while $D\subseteq\mathbb P$ is a [dense set](../../../forcing.md#dense-subset-of-a-forcing-order) when

$$
\forall p\in\mathbb P\ \exists q\in D\ (q\leq p).
$$

In [Jerusalem notation for forcing](../../../forcing.md#jerusalem-notation-for-forcing), $p\leq q$ means that $q$ is stronger than $p$. Incompatibility therefore means that there is no $r$ with $p\leq r$ and $q\leq r$, and density means

$$
\boxed{\forall p\in\mathbb P\ \exists q\in D\ (p\leq q).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $a,p\in M[G]$, and suppose a [first-order formula](../../../mathematical-logic.md#first-order-formula) $\psi(x,y,p)$ defines exactly one $y$ for every $x\in a$. Apply the [Lévy reflection theorem](../../../set-theory.md#levy-reflection-theorem) to the formulas needed to express this assertion, choosing an [ordinal](../../../set-theory.md#ordinal) $\alpha$ with $a,p\in V_\alpha^{M[G]}$ such that

$$
M[G]\models\exists y\,\psi(x,y,p)
\quad\Longleftrightarrow\quad
V_\alpha^{M[G]}\models\exists y\,\psi(x,y,p)
$$

for every $x\in a$. Therefore every required value lies in the [set](../../../set.md) $V_\alpha^{M[G]}$.

The already established [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) forms the set

$$
b=\{y\in V_\alpha^{M[G]}:\exists x\in a\,\psi(x,y,p)\}.
$$

Functionality makes $b$ exactly the range of the definable function on $a$. This proves every instance of the [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) in the [generic extension](../../../forcing.md#generic-extension) $M[G]$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let

$$
d=\bigcup\{s:(s,f)\in G\}.
$$

For each [natural number](../../../arithmetic.md#natural-number) $m$, conditions whose stem has length at least $m$ form a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order), so the [generic filter](../../../forcing.md#generic-filter) meets all of them and $d\in\omega^\omega$.

Fix $h\in\omega^\omega\cap M$. The set

$$
D_h=\{(s,f):f(n)>h(n)\text{ for every }n\}
$$

is dense: from $(s,f)$ replace $f$ by $n\mapsto\max\{f(n),h(n)+1\}$. Choose $(s,f)\in G\cap D_h$. Every stronger condition must put each newly added stem value $d(n)$ above $f(n)$, so

$$
d(n)>h(n)
$$

for every $n\geq|s|$. Thus $d$ is a [dominating real](../../../forcing.md#dominating-real) over $M$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Conditions with the same finite stem in [Hechler forcing](../../../forcing.md#hechler-forcing) are compatible: $(s,f)$ and $(s,g)$ have the common stronger condition $(s,\max\{f,g\})$. Since there are only countably many finite stems, Hechler forcing is [sigma-centered](../../../forcing.md#sigma-centered-forcing) and hence has the [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing). It therefore preserves $\aleph_1^M$.

In $M$, the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis) gives

$$
|\mathbb D|=|\omega^\omega|=\aleph_1.
$$

Every real in $M[G]$ has a [nice name for a real](../../../forcing.md#nice-name-for-a-real), and the countable chain condition bounds the number of such names by

$$
|\mathbb D|^{\aleph_0}=\aleph_1^{\aleph_0}=\aleph_1,
$$

where the last equality uses the ground-model continuum hypothesis. The extension still contains all ground-model reals, already $\aleph_1$ many, so

$$
M[G]\models 2^{\aleph_0}=\aleph_1.
$$

**Thus forcing once with $\mathbb D$ preserves the continuum hypothesis.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
