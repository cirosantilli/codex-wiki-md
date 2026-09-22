# Paper 116

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_116.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_116.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)

## 1

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) is an uncountable [regular cardinal](../../../set-theory.md#regular-cardinal) $\kappa$ that is also a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal):

$$
\boxed{\lambda<\kappa\quad\Longrightarrow\quad2^\lambda<\kappa.}
$$

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

A theory is [$\kappa$-satisfiable](../../../set-theory.md#kappa-satisfiable-theory) when every subtheory of size below $\kappa$ has a model. An uncountable cardinal $\kappa$ is [weakly compact](../../../set-theory.md#weakly-compact-cardinal) when every $\kappa$-satisfiable theory in an infinitary language $L_{\kappa,\kappa}$ with at most $\kappa$ nonlogical symbols is satisfiable.

Equivalently, $\kappa\to(\kappa)^2_2$: every coloring $c:[\kappa]^2\to2$ has a homogeneous subset of cardinality $\kappa$.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

A filter $U$ is [$\kappa$-complete](../../../set-theory.md#kappa-complete-filter) when intersections of fewer than $\kappa$ members remain in $U$. An uncountable cardinal $\kappa$ is a [measurable cardinal](../../../set-theory.md#measurable-cardinal) when it carries a $\kappa$-complete [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter).

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

An uncountable cardinal $\kappa$ is a [strongly compact cardinal](../../../set-theory.md#strongly-compact-cardinal) when every $\kappa$-satisfiable theory in any $L_{\kappa,\kappa}$ language is satisfiable. Unlike weak compactness, there is no cardinality bound on the language.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $U$ witness that $\kappa$ is [measurable](../../../set-theory.md#measurable-cardinal). Regularity is given, so it remains to prove the [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) property. First, every $A\in U$ has cardinality $\kappa$: if $|A|<\kappa$, then

$$
\kappa\setminus A=\bigcap_{\alpha\in A}(\kappa\setminus\{\alpha\})\in U
$$

by nonprincipality and $\kappa$-completeness, contradicting $A\in U$.

Suppose $\lambda<\kappa$ and $2^\lambda\geq\kappa$. Choose an injection $f:\kappa\to\mathcal P(\lambda)$. For each $\xi<\lambda$, exactly one of

$$
A_\xi=\{\alpha<\kappa:\xi\in f(\alpha)\},
\qquad \kappa\setminus A_\xi
$$

lies in $U$. Their chosen intersection lies in $U$ by $\kappa$-completeness. On that intersection every $f(\alpha)$ is the same subset of $\lambda$, contradicting injectivity because every member of $U$ has size $\kappa$. Thus $2^\lambda<\kappa$, and $\kappa$ is strongly inaccessible.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $F$ be a $\kappa$-complete filter on $\kappa$. Use an $L_{\kappa,\kappa}$ propositional language with a sentence $P_A$ for every $A\subseteq\kappa$. Form a theory containing $P_A$ for $A\in F$, the Boolean identities

$$
P_{\kappa\setminus A}\leftrightarrow\neg P_A,
$$

and, for every $\delta<\kappa$,

$$
P_{\bigcap_{i<\delta}A_i}\leftrightarrow\bigwedge_{i<\delta}P_{A_i}.
$$

Every subtheory of size below $\kappa$ mentions fewer than $\kappa$ required members of $F$. Their intersection is nonempty by $\kappa$-completeness; choosing a point in it and interpreting $P_A$ as membership of that point satisfies the subtheory. The theory is therefore $\kappa$-satisfiable. [Strong compactness](../../../set-theory.md#strongly-compact-cardinal) supplies a model. Then

$$
U=\{A\subseteq\kappa:P_A\text{ holds in the model}\}
$$

is an ultrafilter, contains $F$, and is $\kappa$-complete by the infinitary intersection axioms.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For regular $\kappa$, the [cobounded filter on a regular cardinal](../../../set-theory.md#cobounded-filter-on-a-regular-cardinal) is $\kappa$-complete. Part (c) extends it to a $\kappa$-complete ultrafilter $U$. Since $\kappa\setminus\{\alpha\}$ is cobounded for every $\alpha<\kappa$, no singleton belongs to $U$; hence $U$ is nonprincipal. Thus every strongly compact cardinal is [measurable](../../../set-theory.md#measurable-cardinal).

## 2

↑ **Parent:** [Paper 116](paper-116.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\lambda$ be inaccessible and let $j:V_\lambda\to M$ be an elementary embedding into a transitive set with critical point $\kappa$. It is [$\beta$-strong](../../../set-theory.md#beta-strong-elementary-embedding) when

$$
V_{\kappa+\beta}\subseteq M.
$$

A formula $\Phi(x,\kappa)$ is a [beta-stable cardinal property](../../../set-theory.md#beta-stable-cardinal-property) when it is absolute between the universe and every transitive set containing $V_{\kappa+\beta}$.

To say that the embedding reflects such a property means that whenever $\Phi(\kappa)$ holds,

$$
\{\mu<\kappa:\Phi(\mu)\}
$$

is unbounded in $\kappa$: for every $\gamma<\kappa$ there is such a $\mu$ with $\gamma<\mu<\kappa$. Indeed, stability gives $M\models\Phi(\kappa)$, so $M$ sees the witness $\kappa$ between $\gamma$ and $j(\kappa)$. Elementarity reflects a witness between $\gamma$ and $\kappa$. This is [reflection by a beta-strong embedding](../../../set-theory.md#reflection-by-a-beta-strong-embedding).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The standard closure lemma for the [ultrapower embedding](../../../set-theory.md#ultrapower-embedding) says that every $\kappa$-sequence of members of $M$ which belongs to $V_\lambda$ is itself in $M$. If $\kappa<\alpha<\kappa^+$, choose in $V_\lambda$ a surjection

$$
s:\kappa\longrightarrow\alpha.
$$

All ordinal values of $s$ belong to the transitive model $M$, so closure gives $s\in M$. Therefore

$$
M\models|\alpha|\leq\kappa<\alpha,
$$

and $M$ does not regard $\alpha$ as a cardinal.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Every ordinal below

$$
\eta=(j(\kappa)^+)^M
$$

has an ultrapower representative $f:\kappa\to\kappa^+$: by [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem), a representative below the successor of $j(\kappa)$ may be chosen below $\kappa^+$ on a set in the ultrafilter. Hence, in $V_\lambda$,

$$
|\eta|\leq(\kappa^+)^\kappa=2^\kappa.
$$

The ultrapower is closed under $\kappa$-sequences, so it contains every subset of $\kappa$ and computes $2^\kappa$ correctly. By elementarity $M$ regards $j(\kappa)$ as measurable, hence strongly inaccessible by Question 1(b). Consequently

$$
2^\kappa<j(\kappa)<\eta.
$$

Thus $V_\lambda$ has a set of cardinality at most $2^\kappa$ whose order type is $\eta>2^\kappa$, so

$$
\boxed{V_\lambda\models\text{“$\eta$ is not a cardinal”.}}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let

$$
\widehat\kappa=\sup_{n<\omega}j^n(\kappa)
$$

be the supremum of the [Kunen critical sequence](../../../set-theory.md#kunen-critical-sequence), and put

$$
X=j^{\prime\prime}\widehat\kappa
=\{j(\xi):\xi<\widehat\kappa\}.
$$

The required choices are

$$
\boxed{\beta=\widehat\kappa+2,\qquad
\gamma=\widehat\kappa+1,\qquad
X=j^{\prime\prime}\widehat\kappa.}
$$

Indeed $X$ has rank $\widehat\kappa$, so $X\in V_{\widehat\kappa+1}$, while the [Kunen lemma](../../../set-theory.md#kunen-lemma) gives $X\notin M$ once the domain contains the omega-Jonsson function required by the proof, which is ensured by $\alpha\geq\widehat\kappa+2$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $\widehat\kappa=\sup_{n<\omega}j^n(\kappa)$. Every term of the critical sequence is below $\delta$. If $\operatorname{cf}(\delta)>\aleph_0$, then its countable supremum also satisfies $\widehat\kappa<\delta$, and because $\delta$ is a limit ordinal,

$$
\widehat\kappa+2<\delta.
$$

Apply the [Kunen lemma](../../../set-theory.md#kunen-lemma) to the restriction available inside $V_\delta$. It gives

$$
j^{\prime\prime}\widehat\kappa\in
V_{\widehat\kappa+1}\setminus V_\delta,
$$

which is impossible because $V_{\widehat\kappa+1}\subseteq V_\delta$. Hence $\operatorname{cf}(\delta)\leq\aleph_0$. A nonzero limit ordinal has infinite cofinality, so

$$
\boxed{\operatorname{cf}(\delta)=\aleph_0.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
