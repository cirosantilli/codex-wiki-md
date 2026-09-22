# Paper 128

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_128.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_128.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

First form the [singleton set](../../../set.md#singleton-mathematics) $\{b\}=F_1(b,b)$ and then use $F_2$ to take a [set union](../../../set.md#set-union):

$$
U(a,b)=F_2\bigl(F_1(a,F_1(b,b)),a\bigr)=\bigcup\{a,\{b\}\}=a\cup\{b\}.
$$

The unused second argument of $F_2$ may be any term. Since $x\cap c=x\setminus(x\setminus c)$, a term using only the prescribed operation symbols is

$$
\boxed{G(a,b,c)=F_3\bigl(U(a,b),F_3(U(a,b),c)\bigr).}
$$

After substituting the displayed term for both occurrences of $U$, this is literally a term in $F_1,F_2,F_3$, and its value is $(a\cup\{b\})\cap c$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Work in the ambient universe and let $a,u\in L$. Suppose

$$
L\models\forall x\in a\;\exists!y\;\varphi(x,y,u).
$$

For each $x\in a$, let $y_x$ be this unique witness. The relativization $\varphi^L$ is a first-order formula, so the ambient [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) collects the witnesses $y_x$ into a set. Every witness lies in the [constructible hierarchy](../../../definable-power-set.md#constructible-hierarchy), hence there is an ordinal $\alpha$ such that

$$
\{y_x:x\in a\}\subseteq L_\alpha.
$$

For example, take the supremum of one constructible rank for each witness and then increase it by one.

The set $L_\alpha$ itself belongs to $L_{\alpha+1}\subseteq L$. Taking $b=L_\alpha$, every $x\in a$ has a witness $y\in b$ satisfying $\varphi^L(x,y,u)$. Therefore

$$
L\models\exists b\;\forall x\in a\;\exists y\in b\;\varphi(x,y,u),
$$

which is the stated instance of Replacement.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Suppose $V=L$. If $x\in L_{\omega_1}$, then $x\in L_\alpha$ for some [countable ordinal](../../../set-theory.md#countable-ordinal) $\alpha$. The set $L_\alpha$ is transitive and countable, so the [transitive closure](../../../set-theory.md#transitive-closure) of $x$ lies in a countable set. Thus $x$ is [hereditarily countable](../../../set-theory.md#hereditarily-countable-set), proving

$$
L_{\omega_1}\subseteq H_{\aleph_1}.
$$

Conversely, let $x\in H_{\aleph_1}$ and choose a sufficiently large $L_\theta$ containing $x$. By the [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem), there is a countable elementary substructure $N\prec L_\theta$ that contains every member of $\operatorname{TC}(\{x\})$. The [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) gives a transitive collapse of $N$, and the [condensation lemma for the constructible universe](../../../definable-power-set.md#condensation-lemma-for-the-constructible-universe) identifies it with $L_\beta$ for a countable ordinal $\beta$. Because $N$ contains the transitive closure of $x$ pointwise, the collapse fixes $x$. Thus $x\in L_\beta\subseteq L_{\omega_1}$. Hence

$$
\boxed{L_{\omega_1}=H_{\aleph_1}.}
$$

## 2

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The [Fn forcing](../../../forcing.md#fn-forcing) order is

$$
\operatorname{Fn}(I,J)=\{p:p\text{ is a finite partial function }I\rightharpoonup J\}.
$$

It is ordered by reverse inclusion:

$$
q\le p\iff q\supseteq p,
$$

so a stronger condition specifies more values. Its maximal, or weakest, element is the empty function $\varnothing$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

For a [regular cardinal](../../../set-theory.md#regular-cardinal) $\kappa$,

$$
\operatorname{Fn}_\kappa(I,J)=\{p:p:I\rightharpoonup J,\ |\operatorname{dom}p|<\kappa\}.
$$

Again $q\le p$ means $q\supseteq p$, and the maximal element is the empty function. The regularity of $\kappa$ ensures that the union of a descending sequence of fewer than $\kappa$ conditions still has domain of cardinality below $\kappa$ whenever the conditions form a compatible increasing chain of partial functions.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $A\subseteq\operatorname{Fn}(I,J)$ be uncountable. Apply the [Delta-system lemma](../../../set-theory.md#delta-system-lemma) to the finite sets $\operatorname{dom}p$ for $p\in A$. After passing to an uncountable subset $A'$, there is a fixed finite root $R$ such that

$$
\operatorname{dom}p\cap\operatorname{dom}q=R
$$

for distinct $p,q\in A'$. Because $J$ is countable and $R$ is finite, there are only countably many functions $R\to J$. A further uncountable subset $A''\subseteq A'$ therefore has the same restriction to $R$.

Any two conditions in $A''$ agree on the intersection of their domains, so their union is a common stronger condition. Thus every uncountable family contains two compatible conditions, and no uncountable antichain exists. Therefore

$$
\boxed{\operatorname{Fn}(I,J)\text{ has the countable chain condition}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $c=\bigcup G$ and $d(n)=c(2n)$. Define

$$
H=\{p\in\operatorname{Fn}(\omega,2)^M:p\subseteq d\}.
$$

This is a filter: restrictions of finite pieces of $d$ remain in $H$, and the union of two members is a common stronger condition.

To prove genericity, take a dense set $D\in M$. Let $E_D$ consist of conditions $q\in\operatorname{Fn}(\omega,2)$ for which some $p\in D$ satisfies

$$
p(n)=q(2n)\qquad(n\in\operatorname{dom}p).
$$

The set $E_D$ is dense. Indeed, given $q$, first read its finitely many assigned even coordinates as a condition $p_0$ on $\omega$. Choose $p\le p_0$ in $D$, and extend $q$ by setting $q(2n)=p(n)$ at the remaining coordinates of $p$. Since $E_D\in M$, the [generic filter](../../../forcing.md#generic-filter) $G$ meets it. For $q\in G\cap E_D$, the corresponding $p\in D$ is a finite subfunction of $d$, so $p\in H\cap D$.

Thus $H$ meets every dense subset belonging to $M$. Moreover, each singleton $\{(n,d(n))\}$ belongs to $H$, and hence

$$
\boxed{H\text{ is }\operatorname{Fn}(\omega,2)\text{-generic over }M,qquad\bigcup H=d.}
$$

## 3

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [forcing theorem](../../../forcing.md#forcing-theorem) has two parts. The definability lemma says that for every formula $\varphi$, the relation

$$
p\Vdash_M\varphi(\tau_1,\ldots,\tau_n)
$$

is definable in $M$. The truth lemma says that if $G$ is generic over $M$, then

$$
\boxed{M[G]\models\varphi(\tau_1^G,\ldots,\tau_n^G)
\iff
\exists p\in G\;p\Vdash_M\varphi(\tau_1,ldots,\tau_n).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume the forcing relation and the forcing theorem have been constructed for $\varphi(x,\vec y)$. Define

$$
p\Vdash\exists x\,\varphi(x,\vec\tau)
$$

to mean that

$$
D_p=\{q\le p:\exists\sigma\in M\;q\Vdash\varphi(\sigma,\vec\tau)\}
$$

is dense below $p$. This definition is first-order over $M$, so the definability lemma is preserved.

Suppose $p\in G$ forces the existential statement. Genericity below $p$ gives $q\in G\cap D_p$ and a name $\sigma$ with $q\Vdash\varphi(\sigma,\vec\tau)$. The truth lemma for $\varphi$ yields

$$
M[G]\models\varphi(\sigma^G,\vec\tau^G),
$$

so the existential statement is true. Conversely, if $M[G]\models\exists x\,\varphi(x,\vec\tau^G)$, choose a name $\sigma$ for a witness. The truth lemma for $\varphi$ gives $q\in G$ with $q\Vdash\varphi(\sigma,\vec\tau)$, and then $q\Vdash\exists x\,\varphi(x,\vec\tau)$. This proves both directions of the forcing theorem for the existential formula.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Conditions in $G$ are compatible finite functions, so their union $F=\bigcup G$ is a function $(\omega_1)^M\rightharpoonup(\omega_1)^M$. For each $\alpha<\omega_1$, the set

$$
D_\alpha=\{p:\alpha\in\operatorname{dom}p\}
$$

is dense: choose a normal function extending $p$ and add its value at $\alpha$. Genericity makes $F$ total.

If $\alpha<\beta$, choose a condition in the filter extending conditions that decide both values. It is contained in a [normal function on an ordinal](../../../set-theory.md#normal-function-on-an-ordinal), so $F(\alpha)<F(\beta)$. Thus $F$ is strictly increasing.

It remains to prove continuity. For every limit $\delta<\omega_1$ and $\gamma<\omega_1$, let $D_{\delta,\gamma}$ contain the conditions $p$ such that $\delta\in\operatorname{dom}p$ and either

$$
p(\delta)\le\gamma
$$

or there is some $\alpha<\delta$ in $\operatorname{dom}p$ with $p(\alpha)>\gamma$. This set is dense. Given $p$, extend it to a normal function $f$ and add $(\delta,f(\delta))$; if $f(\delta)>\gamma$, continuity of $f$ supplies an $\alpha<\delta$ with $f(\alpha)>\gamma$, which may also be added.

Now fix $\gamma<F(\delta)$. Since $G$ meets $D_{\delta,\gamma}$, compatibility with the condition deciding $F(\delta)$ rules out the first alternative and gives $\alpha<\delta$ with $F(\alpha)>\gamma$. Therefore values below $\delta$ are cofinal in $F(\delta)$. Strict increase supplies the reverse bound, so

$$
\boxed{F(\delta)=\sup_{\alpha<\delta}F(\alpha).}
$$

**Hence $F$ is normal on $(\omega_1)^M$ in $M[G]$.**

## 4

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Lévy reflection theorem](../../../set-theory.md#levy-reflection-theorem) states that for every finite collection $\Phi$ of formulas and every ordinal $\gamma$, there is an ordinal $\alpha>\gamma$ such that, for every $\varphi\in\Phi$ and all parameters $\vec a\in V_\alpha$,

$$
\boxed{V\models\varphi(\vec a)\iff V_\alpha\models\varphi(\vec a).}
$$

Indeed, the ordinals $\alpha$ reflecting all formulas in $\Phi$ form a closed unbounded class.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Let $\alpha=(\omega_1)^M$ and take

$$
\varphi_1(\alpha)\equiv\text{“there exists a function }f\text{ with }\operatorname{dom}f=\omega\text{ and }\operatorname{ran}f=\alpha\text{.”}
$$

This formula is [upward absolute](../../../set-theory.md#upward-absolute-formula) between transitive models: if the smaller model contains such an $f$, the assumed absoluteness of “function”, domain, range, and $\omega$ shows that the same witness works in the larger model.

The generic union $g=\bigcup G$ is a total map $\omega\to\alpha$, because the conditions deciding each input form a dense set. For every $\beta<\alpha$, the conditions putting $\beta$ somewhere in the range are also dense, so $g$ is surjective. Thus $M[G]\models\varphi_1(\alpha)$. But $M\not\models\varphi_1(\alpha)$ because $M$ regards $\alpha$ as its first uncountable ordinal. Hence $\varphi_1$ is not downward absolute between $M$ and $M[G]$.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

With the same parameter $\alpha=(\omega_1)^M$, let

$$
\varphi_2(\alpha)\equiv\text{“there is no function }f\text{ with }\operatorname{dom}f=\omega\text{ and }\operatorname{ran}f=\alpha\text{.”}
$$

This formula is [downward absolute](../../../set-theory.md#downward-absolute-formula): if the larger transitive model has no such function, then neither can the smaller model, since any witness in the smaller model would remain a witness in the larger one. The model $M$ satisfies $\varphi_2(\alpha)$, while the generic surjection $\bigcup G$ makes it false in $M[G]$. Therefore it is not upward absolute.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Assume $\varphi(\vec a)$ is a [Delta-one formula in set theory](../../../set-theory.md#delta-one-formula-in-set-theory). Thus ZF proves it equivalent to a $\Sigma_1$ formula $\sigma$ and to a $\Pi_1$ formula $\pi$. Only finitely many axioms of ZF occur in these two formal proofs; collect them, together with the finite fragment needed for bounded-formula absoluteness, into $T$.

Let $M$ be a transitive class containing $\vec a$ and satisfying $T$. If $M\models\varphi$, then $M\models\sigma$, and upward absoluteness of $\Sigma_1$ formulas gives $V\models\sigma$, hence $V\models\varphi$. If $V\models\varphi$, then $V\models\pi$, and downward absoluteness of $\Pi_1$ formulas gives $M\models\pi$, hence $M\models\varphi$. Therefore ZF proves that $\varphi$ is absolute for every such $M$.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Conversely, suppose a finite $T\subseteq\mathrm{ZF}$ has the stated absoluteness property. Let

$$
\sigma(\vec a)\equiv\exists N\,[N\text{ is a transitive set},\ \vec a\in N,\ N\models T,\ N\models\varphi(\vec a)].
$$

Because $T$ is finite, every satisfaction assertion here can be replaced by the corresponding [formula relativization to a class](../../../set-theory.md#formula-relativization-to-a-class). All quantifiers in the matrix are bounded by $N$, so $\sigma$ is $\Sigma_1$. Define the $\Pi_1$ formula

$$
\pi(\vec a)\equiv\neg\exists N\,[N\text{ is a transitive set},\ \vec a\in N,\ N\models T,\ N\models\neg\varphi(\vec a)].
$$

By the [Lévy reflection theorem](../../../set-theory.md#levy-reflection-theorem), ZF proves that for any parameters $\vec a$ there is a level $V_\alpha$ containing them and satisfying the finite fragment $T$. The assumed absoluteness says that every such transitive set agrees with $V$ about $\varphi$. Consequently ZF proves

$$
\varphi(\vec a)\leftrightarrow\sigma(\vec a)
\qquad\text{and}\qquad
\varphi(\vec a)\leftrightarrow\pi(\vec a).
$$

**Thus $\varphi$ is both $\Sigma_1^{\mathrm{ZF}}$ and $\Pi_1^{\mathrm{ZF}}$, so it is $\Delta_1^{\mathrm{ZF}}$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
