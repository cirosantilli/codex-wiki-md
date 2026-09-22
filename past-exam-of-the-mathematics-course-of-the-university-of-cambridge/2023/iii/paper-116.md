# Paper 116

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_116.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_116.pdf)

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
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $[f]$ for the equivalence class of $f:\kappa\to V_\lambda$ in the [ultrapower](../../../foundations-of-mathematics.md#ultrapower)

$$
N=(V_\lambda)^\kappa/U,
$$

and define its membership relation by

$$
[g]\mathrel E[f]
\quad\Longleftrightarrow\quad
\{\xi<\kappa:g(\xi)\in f(\xi)\}\in U.
$$

The [kappa-complete filter](../../../set-theory.md#kappa-complete-filter) property makes $E$ [well-founded](../../../set-theory.md#well-founded-relation): an infinite descending $E$-chain would give countably many members of $U$ whose intersection belongs to $U$, and every index in that intersection would yield an infinite descending membership chain, contradicting the [Axiom of foundation](../../../set-theory.md#axiom-of-regularity). The relation is [extensional](../../../set-theory.md#extensional-relation) by [Łoś's theorem](../../../foundations-of-mathematics.md#los-theorem).

The [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) therefore gives a unique isomorphism $\pi:(N,E)\to(M,\in)$ onto a [transitive set](../../../set-theory.md#transitive-set) $M$. Recursively, the notation missing from the printed formula may be defined by

$$
\pi([f])=\{\pi([g]):[g]\mathrel E[f]\}.
$$

The value is independent of the representative because it is defined on the ultrapower class $[f]$. Moreover $M\subseteq V_\lambda$: every $f:\kappa\to V_\lambda$ has its range contained in some $V_\alpha$ with $\alpha<\lambda$, since $\kappa<\lambda$ and the [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) $\lambda$ is [regular](../../../set-theory.md#regular-cardinal); induction on the resulting rank bound keeps $\pi([f])$ inside $V_\lambda$.

Define the [ultrapower embedding](../../../set-theory.md#ultrapower-embedding)

$$
j:V_\lambda\longrightarrow M,
\qquad
j(x)=\pi([\operatorname{const}_x]).
$$

The constant-function map into $N$ is [elementary](../../../set-theory.md#elementary-embedding) by Łoś's theorem, and $\pi$ is an isomorphism, so their composite $j$ is elementary.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [critical point of an elementary embedding](../../../set-theory.md#critical-point-of-an-elementary-embedding) $j$ is the least [ordinal](../../../set-theory.md#ordinal) $\alpha$ for which $j(\alpha)\ne\alpha$.

We first prove by [transfinite induction](../../../set-theory.md#transfinite-induction) that $j(\alpha)=\alpha$ for every $\alpha<\kappa$. Suppose this is known below $\alpha<\kappa$. If $[f]\mathrel E[\operatorname{const}_\alpha]$, then

$$
A=\{\xi<\kappa:f(\xi)<\alpha\}\in U.
$$

The sets $A_\beta=\{\xi\in A:f(\xi)=\beta\}$ for $\beta<\alpha$ partition $A$ into fewer than $\kappa$ pieces. A [kappa-complete filter](../../../set-theory.md#kappa-complete-filter) that is an [ultrafilter](../../../set-theory.md#ultrafilter) must contain one cell $A_\beta$: otherwise all their complements would belong to $U$, and their intersection would contradict $A\in U$. Hence $[f]=[\operatorname{const}_\beta]$. The predecessors of $j(\alpha)$ are consequently exactly the already-fixed ordinals below $\alpha$, so $j(\alpha)=\alpha$.

Now let $\operatorname{id}(\xi)=\xi$. An identical argument shows that the predecessors of $[\operatorname{id}]$ in the ultrapower are exactly $[\operatorname{const}_\beta]$ for $\beta<\kappa$, so

$$
\pi([\operatorname{id}])=\kappa.
$$

Since $\{\xi<\kappa:\xi<\kappa\}=\kappa\in U$, one has $[\operatorname{id}]\mathrel E[\operatorname{const}_\kappa]$. After collapsing, $\kappa\in j(\kappa)$, and therefore $j(\kappa)>\kappa$. Thus $\operatorname{crit}(j)=\kappa$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A property $P$ of $\kappa$ [reflects below](../../../set-theory.md#reflection-below-a-cardinal) $\kappa$ when

$$
\{\mu<\kappa:P(\mu)\}
$$

is unbounded in $\kappa$. The standard [elementary-embedding reflection argument](../../../set-theory.md#reflection-by-a-beta-strong-embedding) starts with any $\gamma<\kappa$. Since $j(\gamma)=\gamma$ and $j(\kappa)>\kappa$, the target model can use $\kappa$ itself as a witness to

$$
\exists\mu\,(\gamma<\mu<j(\kappa)\land P(\mu)).
$$

[Elementarity](../../../set-theory.md#elementary-embedding) then gives a witness $\mu$ with $\gamma<\mu<\kappa$ in the domain.

For a concrete example, the property of being a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) reflects below $\kappa$. A [measurable cardinal](../../../set-theory.md#measurable-cardinal) is strongly inaccessible, and the assumed inclusion $V_{\kappa+1}\subseteq M$ makes this assertion about $\kappa$ [absolute](../../../set-theory.md#set-theoretic-absoluteness) between $V_\lambda$ and $M$: both models have all subsets of every ordinal below $\kappa$. Thus $M$ sees that $\kappa$ is strongly inaccessible. Given $\gamma<\kappa$, it therefore satisfies

$$
\exists\mu\,(\gamma<\mu<j(\kappa)\land\mu\text{ is strongly inaccessible}).
$$

Elementarity supplies a strongly inaccessible $\mu$ between $\gamma$ and $\kappa$ in $V_\lambda$. As $\gamma$ was arbitrary, the strongly inaccessible cardinals below $\kappa$ are unbounded.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

An [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) $\kappa$ has the [Keisler extension property](../../../set-theory.md#keisler-extension-property) when there is a proper [transitive set](../../../set-theory.md#transitive-set) $X\supsetneq V_\kappa$ such that

$$
(V_\kappa,\in)\prec(X,\in).
$$

Suppose $\kappa$ is strongly inaccessible and has this property. Because $X$ properly extends the transitive set $V_\kappa$, it contains $\kappa$. Strong inaccessibility of $\kappa$ is [downward absolute](../../../set-theory.md#downward-absolute-formula) from the ambient universe to the transitive set $X$: any internal witness that $\kappa$ is countable, singular, or not a strong limit would also be an ambient witness. Hence

$$
X\models\text{“there exists a strongly inaccessible cardinal”},
$$

with $\kappa$ as a witness. Since $V_\kappa\prec X$, the same sentence holds in $V_\kappa$. Its witness is an ordinal $\mu<\kappa$. The set $V_\kappa$ contains $V_{\mu+1}$, so it computes all subsets of cardinals below $\mu$ correctly; strong inaccessibility of $\mu$ is therefore absolute between $V_\kappa$ and the universe. Thus there is a strongly inaccessible $\mu<\kappa$, and $\kappa$ cannot be the least strongly inaccessible cardinal.

## 2

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a [first-order theory](../../../mathematical-logic.md#first-order-theory) $R$ extending ZFC, let $C_R$ be its set of formal consequences and let $\mathrm{Cons}$ denote the class of [formal consistency statements](../../../mathematical-logic.md#formal-consistency-statement) $\operatorname{Con}(Q)$ for recursively axiomatized extensions $Q$ of ZFC. Using [Gödel numbering](../../../mathematical-logic.md#godel-numbering) to code proofs and theories, these objects and the following comparison are definable in the base theory ZFC.

The [consistency-strength preorder](../../../mathematical-logic.md#consistency-strength-preorder) is

$$
T\leq_{\mathrm{Cons}}S
\quad\Longleftrightarrow\quad
\mathrm{Cons}\cap C_T\subseteq\mathrm{Cons}\cap C_S.
$$

Thus every consistency assertion provable in $T$ is also provable in $S$. Its strict part is

$$
\boxed{T<_{\mathrm{Cons}}S
\quad\Longleftrightarrow\quad
T\leq_{\mathrm{Cons}}S\ \land\ \neg(S\leq_{\mathrm{Cons}}T).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\mathrm{IC}$ be the sentence asserting that a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) exists, and begin with

$$
T_0=\mathrm{ZFC}+\mathrm{IC}.
$$

Define the [iterated consistency progression](../../../mathematical-logic.md#iterated-consistency-progression)

$$
T_{n+1}=T_n+\operatorname{Con}(T_n),
\qquad
T_\infty=\bigcup_{n<\omega}T_n.
$$

The construction is effective, so every $T_n$ and $T_\infty$ is a recursively axiomatized [first-order theory](../../../mathematical-logic.md#first-order-theory) extending ZFC.

Because $T_{n+1}$ extends $T_n$, every theorem of $T_n$, including every [formal consistency statement](../../../mathematical-logic.md#formal-consistency-statement) it proves, is a theorem of $T_{n+1}$; hence $T_n\leq_{\mathrm{Cons}}T_{n+1}$. The theory $T_{n+1}$ proves $\operatorname{Con}(T_n)$ by construction, whereas a consistent $T_n$ cannot prove its own consistency by [Gödel second incompleteness theorem](../../../mathematical-logic.md#godel-second-incompleteness-theorem). Therefore

$$
T_n<_{\mathrm{Cons}}T_{n+1}.
$$

Likewise $T_\infty$ extends every $T_n$ and contains $\operatorname{Con}(T_n)$ as an axiom already at stage $n+1$, while $T_n$ does not prove it. Consequently

$$
T_0<_{\mathrm{Cons}}T_1<_{\mathrm{Cons}}T_2<_{\mathrm{Cons}}\cdots<_{\mathrm{Cons}}T_\infty,
$$

assuming the stated consistency hypotheses.

## 3

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Since the [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) $\lambda$ is inaccessible, $(V_\lambda,\in)$ is a [model](../../../mathematical-logic.md#model-of-a-first-order-theory) of ZFC. The [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) gives an [elementary substructure](../../../mathematical-logic.md#elementary-substructure)

$$
X\prec V_\lambda
$$

of [cardinality](../../../set-theory.md#cardinal-number) $\kappa$ such that

$$
V_\kappa\cup\{\kappa,U\}\subseteq X.
$$

One may obtain $X$ concretely as the [Skolem hull](../../../mathematical-logic.md#skolem-hull) of this set; its cardinality remains $\kappa$ because the language of set theory is countable and $|V_\kappa|=\kappa$.

Apply the [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) to $X$ and write $\pi:X\to M$ for the collapse. Then $M$ is a [transitive set](../../../set-theory.md#transitive-set), $|M|=\kappa$, and $\pi$ fixes $V_\kappa$ pointwise. It also fixes $\kappa$, because it fixes every ordinal below $\kappa$. By [elementarity](../../../mathematical-logic.md#elementary-substructure), $X$ satisfies ZFC and regards $U$ as a [kappa-complete filter](../../../set-theory.md#kappa-complete-filter) that is a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) on $\kappa$. Therefore, with $\bar U=\pi(U)$,

$$
(M,\in)\models\mathrm{ZFC}+\text{“$\kappa$ is a measurable cardinal, witnessed by $\bar U$.”}
$$

The internal ultrafilter $\bar U$ need not equal the original $U$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

**No.** Let

$$
\alpha=(\kappa^+)^M,
$$

the [successor cardinal](../../../set-theory.md#successor-cardinal) of $\kappa$ computed by $M$. Then $\alpha\in M$, and $M$ regards $\alpha$ as a [cardinal number](../../../set-theory.md#cardinal-number). Because $M$ is transitive, $\alpha\subseteq M$, so externally

$$
|\alpha|\leq|M|=\kappa.
$$

On the other hand $\kappa<\alpha$, hence $|\alpha|=\kappa$ in the ambient universe. A corresponding [bijection](../../../function.md#bijection) belongs to $V_\lambda$ because its [rank](../../../set-theory.md#rank-of-a-set) is below the inaccessible limit $\lambda$. Thus $V_\lambda$ regards $\alpha$ as equinumerous with $\kappa$ and therefore not as a cardinal. This is an instance of [cardinal nonabsoluteness in a small transitive model](../../../set-theory.md#cardinal-nonabsoluteness-in-a-small-transitive-model).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**Yes.** Start with the model $M_0$ constructed in part a. If $M_0$ has no internally [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) above $\kappa$, put $M=M_0$. Otherwise let $\delta$ be the least ordinal above $\kappa$ that $M_0$ regards as strongly inaccessible, and put

$$
M=(V_\delta)^{M_0}.
$$

In the second case $M\models\mathrm{ZFC}$ because $M_0$ regards $\delta$ as inaccessible. The measure witnessing that $\kappa$ is [measurable](../../../set-theory.md#measurable-cardinal) has rank below $\kappa+3<\delta$, so it still belongs to $M$. In both cases $M$ is a [transitive set](../../../set-theory.md#transitive-set) of cardinality $\kappa$, contains $V_\kappa$, and has no internally inaccessible ordinal strictly between $\kappa$ and its height.

We verify [absoluteness](../../../set-theory.md#set-theoretic-absoluteness) for every ordinal $\alpha\in M$. If $\alpha<\kappa$, then $M$ and $V_\lambda$ both contain $V_{\alpha+1}$ and therefore compute all subsets and functions relevant to strong inaccessibility in the same way. At $\alpha=\kappa$, both models see a [measurable cardinal](../../../set-theory.md#measurable-cardinal) and hence an inaccessible cardinal. Finally, if $\kappa<\alpha\in M$, then $M$ says that $\alpha$ is not inaccessible by construction. The larger model $V_\lambda$ cannot say that it is inaccessible, because strong inaccessibility is downward absolute to a transitive model of ZFC: any failure visible in the smaller model remains a failure in the larger one, while ambient inaccessibility would force internal inaccessibility. Hence “$\alpha$ is inaccessible” is absolute between $M$ and $V_\lambda$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
