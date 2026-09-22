# Paper 116

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_116.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_116.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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

## 1

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An uncountable [cardinal number](../../../set-theory.md#cardinal-number) $\kappa$ is [weakly compact](../../../set-theory.md#weakly-compact-cardinal) when every $\kappa$-satisfiable theory in an [infinitary language](../../../mathematical-logic.md#infinitary-language) $L_{\kappa,\kappa}$ with at most $\kappa$ nonlogical symbols is satisfiable. A cardinal is [inaccessible](../../../set-theory.md#strongly-inaccessible-cardinal) when it is uncountable, [regular](../../../set-theory.md#regular-cardinal), and a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal).

Two standard results supply the proof. First, every weakly compact cardinal is inaccessible. Second, every weakly compact $\kappa$ has the [Keisler extension property](../../../set-theory.md#keisler-extension-property): there is a transitive set $X\supsetneq V_\kappa$ such that

$$
(V_\kappa,\in)\prec(X,\in)
$$

and $\kappa\in X$. Since $\kappa$ is inaccessible, the relevant [downward absoluteness](../../../set-theory.md#set-theoretic-absoluteness) makes $X\models$ “$\kappa$ is inaccessible”. Hence $X$ satisfies “there is an inaccessible cardinal”. By [elementarity](../../../mathematical-logic.md#elementary-substructure), $V_\kappa$ satisfies the same sentence, so it contains some inaccessible $\lambda$. Every [ordinal](../../../set-theory.md#ordinal) in $V_\kappa$ is below $\kappa$, and inaccessibility is absolute here, giving

$$
\boxed{\lambda<\kappa\text{ and }\lambda\text{ is inaccessible}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

An uncountable cardinal $\kappa$ is [measurable](../../../set-theory.md#measurable-cardinal) when it carries a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) $U$ that is [$\kappa$-complete](../../../set-theory.md#kappa-complete-filter). For an inaccessible $\lambda>\kappa$, the cardinal $\kappa$ is [1-strong](../../../set-theory.md#one-strong-cardinal) when there is an [elementary embedding](../../../set-theory.md#elementary-embedding)

$$
j:V_\lambda\longrightarrow M
$$

into a transitive model, with [critical point](../../../set-theory.md#critical-point-of-an-elementary-embedding) $\kappa$ and $V_{\kappa+1}\subseteq M$.

The fundamental theorem on measurable cardinals constructs from $U$ the well-founded [ultrapower](../../../foundations-of-mathematics.md#ultrapower) and its [ultrapower embedding](../../../set-theory.md#ultrapower-embedding) $j:V_\lambda\to M$, whose critical point is $\kappa$. The embedding fixes $V_\kappa$. If $A\in V_{\kappa+1}$, then $A\subseteq V_\kappa$, and [elementarity](../../../set-theory.md#elementary-embedding) gives

$$
A=j(A)\cap V_\kappa.
$$

Both $j(A)$ and $V_\kappa$ belong to the transitive target, so $A\in M$. Thus $V_{\kappa+1}\subseteq M$, proving that every measurable cardinal is [1-strong](../../../set-theory.md#measurable-cardinal-is-one-strong).

## 2

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $U$ be a nonprincipal $\kappa$-complete [ultrafilter](../../../set-theory.md#ultrafilter) on the measurable cardinal $\kappa$, and fix $\lambda<\kappa$. Suppose for a contradiction that $2^\lambda\geq\kappa$. Choose distinct subsets $A_\alpha\subseteq\lambda$ for $\alpha<\kappa$. For each $\xi<\lambda$, the [ultrafilter](../../../set-theory.md#ultrafilter) property chooses exactly one of

$$
S_\xi=\{\alpha<\kappa:\xi\in A_\alpha\},
\qquad
\kappa\setminus S_\xi
$$

as a member $H_\xi$ of $U$. Since $\lambda<\kappa$, [$\kappa$-completeness](../../../set-theory.md#kappa-complete-filter) gives $H=\bigcap_{\xi<\lambda}H_\xi\in U$.

Any two indices in $H$ give subsets having the same membership decision at every $\xi<\lambda$, so they give the same $A_\alpha$. The chosen subsets were distinct, hence $|H|\leq1$. This contradicts the fact that a [small set is absent from a complete nonprincipal ultrafilter](../../../set-theory.md#small-set-is-absent-from-a-complete-nonprincipal-ultrafilter). Therefore $2^\lambda<\kappa$ for every $\lambda<\kappa$, which is precisely the [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) condition. This is the [measurable cardinal is a strong limit cardinal](../../../set-theory.md#measurable-cardinal-is-a-strong-limit-cardinal) argument.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Suppose that a [first-order formula](../../../mathematical-logic.md#first-order-formula) $\varphi$ described the inaccessible cardinal $\kappa$, so that $\kappa$ were the least ordinal with $V_\kappa\models\varphi$. Since $\kappa$ is inaccessible, $V_\kappa$ is a [model](../../../mathematical-logic.md#model-of-a-first-order-theory) of ZFC. Apply the [Lévy reflection theorem](../../../set-theory.md#levy-reflection-theorem) inside this model to the single formula $\varphi$. There is some $\alpha<\kappa$ for which

$$
V_\alpha\models\varphi
\quad\Longleftrightarrow\quad
V_\kappa\models\varphi.
$$

The right side holds, so the left side contradicts the asserted minimality of $\kappa$. Hence no first-order formula describes an inaccessible cardinal, as recorded by [ordinal described by a first-order formula](../../../set-theory.md#ordinal-described-by-a-first-order-formula).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $I(\kappa)$, $W(\kappa)$, and $M(\kappa)$ mean respectively that $\kappa$ is inaccessible, weakly compact, and measurable. Define a fourth cardinal property

$$
\Theta(\kappa)
\quad\Longleftrightarrow\quad
\bigl(W\mathbf C\land M(\kappa)\bigr)
\lor
\bigl(\neg W\mathbf C\land I(\kappa)\bigr).
$$

Take $\Phi_0=I$, $\Phi_1=W$, and $\Phi_2=\Theta$.

If inaccessible and weakly compact cardinals exist, Question 1a shows that an inaccessible lies below every weakly compact cardinal. Thus $I<_1W$. If $W\mathbf C$ and $\Theta\mathbf C$ both hold, then $\Theta$ is exactly measurability. Every measurable cardinal is weakly compact, and the usual ultrapower reflection theorem gives weakly compact cardinals below every measurable cardinal. Therefore $W<_1\Theta$.

Now assume the consistency of ZFC with an inaccessible cardinal but no weakly compact cardinal. In such a model $\Theta(\kappa)$ is exactly $I(\kappa)$, so

$$
\iota_\Theta=\iota_I.
$$

**Consequently $I\not<_1\Theta$. This is an explicit [nontransitivity of the least-occurrence order on cardinal properties](../../../set-theory.md#nontransitivity-of-the-least-occurrence-order-on-cardinal-properties), even though $I<_1W$ and $W<_1\Theta$.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write

$$
T=\mathrm{ZFC}+\text{“there is a worldly cardinal”},
\qquad
T^*=\mathrm{ZFC}+\operatorname{Con}(\mathrm{ZFC}).
$$

If $\kappa$ is a [worldly cardinal](../../../set-theory.md#worldly-cardinal), then $V_\kappa\models\mathrm{ZFC}$. The existence of this set model proves $\operatorname{Con}(\mathrm{ZFC})$ in the universe. By [arithmetic absoluteness for a rank-initial model](../../../set-theory.md#arithmetic-absoluteness-for-a-rank-initial-model), the same formal consistency statement holds in $V_\kappa$. Hence $V_\kappa\models T^*$, so $T$ proves $\operatorname{Con}(T^*)$.

Conversely, suppose $T^*$ proved $\operatorname{Con}(T)$. The theory $T$ proves every axiom of $T^*$, since a worldly cardinal proves $\operatorname{Con}(\mathrm{ZFC})$. It would therefore also prove $\operatorname{Con}(T)$, contrary to the [Gödel second incompleteness theorem](../../../mathematical-logic.md#godel-second-incompleteness-theorem) when $T$ is consistent. Thus $T^*$ cannot prove $\operatorname{Con}(T)$, and

$$
\boxed{T^*<_{\mathrm{Cons}}T.}
$$

This is the [consistency strength of a worldly cardinal](../../../mathematical-logic.md#consistency-strength-of-a-worldly-cardinal) comparison.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Because $\kappa_0<\kappa_1=\operatorname{crit}(j_1)$, the definition of the [critical point of an elementary embedding](../../../set-theory.md#critical-point-of-an-elementary-embedding) immediately gives

$$
j_1(\kappa_0)=\kappa_0.
$$

To evaluate $j_0(\kappa_1)$, first use the regularity of the measurable cardinal $\kappa_1$. Every function $f:\kappa_0\to\kappa_1$ has bounded range, so every ordinal below $j_0(\kappa_1)$ lies below $j_0(\beta)$ for some $\beta<\kappa_1$. Hence

$$
j_0(\kappa_1)=\sup_{\beta<\kappa_1}j_0(\beta).
$$

The [strong-limit property](../../../set-theory.md#measurable-cardinal-is-a-strong-limit-cardinal) of $\kappa_1$ gives $\beta^{\kappa_0}<\kappa_1$ for every $\beta<\kappa_1$. There are therefore fewer than $\kappa_1$ functions $\kappa_0\to\beta$, which implies $j_0(\beta)<\kappa_1$. On the other hand $j_0(\beta)\geq\beta$. Taking suprema yields

$$
\boxed{j_0(\kappa_1)=\kappa_1,
\qquad j_1(\kappa_0)=\kappa_0,}
$$

the [two measurable cardinals under an ultrapower embedding](../../../set-theory.md#two-measurable-cardinals-under-an-ultrapower-embedding) formula.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Fix $i\in\{0,1\}$ and write $\kappa=\kappa_i$, $j=j_i$, and $M=M_i$. Every ordinal below $j(\kappa)$ is represented in the [ultrapower](../../../foundations-of-mathematics.md#ultrapower) by a function $\kappa\to\kappa$. Consequently, in $V_\lambda$,

$$
|j(\kappa)|\leq\kappa^\kappa=2^\kappa=\kappa^+,
$$

where the last equality uses the [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis).

By [elementarity](../../../set-theory.md#elementary-embedding), $M$ regards $j(\kappa)$ as measurable and hence as a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal). Moreover $V_{\kappa+1}\subseteq M$, so $M$ and $V_\lambda$ have the same subsets of $\kappa$ and the same $\kappa^+$. It follows inside $M$ that

$$
\kappa^+=2^\kappa<j(\kappa).
$$

Thus, in the ambient $V_\lambda$, the ordinal $j(\kappa)$ is strictly larger than $\kappa^+$ but has cardinality at most $\kappa^+$. It cannot be a [cardinal number](../../../set-theory.md#cardinal-number). Applying this argument to both $i=0$ and $i=1$ proves that neither $j_0(\kappa_0)$ nor $j_1(\kappa_1)$ is a cardinal in $V_\lambda$, exactly as in [moved critical point is not an ambient cardinal under GCH](../../../set-theory.md#moved-critical-point-is-not-an-ambient-cardinal-under-gch).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
