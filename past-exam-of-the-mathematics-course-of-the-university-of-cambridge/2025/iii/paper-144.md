# Paper 144

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_144.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_144.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)

## 1

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A complete theory $T$ is [categorical theory](../../../foundations-of-mathematics.md#categorical-theory) in the infinite cardinal $\kappa$, or $\kappa$-categorical, when it has a model of cardinality $\kappa$ and any two of its models of cardinality $\kappa$ are [isomorphic](../../../algebra.md#isomorphism). Equivalently, $T$ has exactly one model of cardinality $\kappa$ up to isomorphism.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The theory $\operatorname{Th}(\mathbb Z,+,0)$ is not [aleph-zero-categorical](../../../foundations-of-mathematics.md#omega-categorical-theory). Introduce a constant $c$ and add the formulas

$$
c\ne0,
\qquad
\exists y\;(ny=c)quad(n=1,2,\ldots).
$$

Every finite subset is realized in $\mathbb Z$ by taking $c$ to be a nonzero common multiple of the finitely many displayed integers. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) therefore gives a model of $\operatorname{Th}(\mathbb Z,+,0)$ containing a nonzero [infinitely divisible element of an abelian group](../../../group.md#infinitely-divisible-element-of-an-abelian-group). The [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) gives such a model that is countable.

No nonzero integer is divisible by every positive integer, so this countable model is not isomorphic to $\mathbb Z$. This is the [nonstandard model of the additive integers](../../../foundations-of-mathematics.md#nonstandard-model-of-the-additive-integers) obstruction to categoricity.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The group $B$ is a [vector space over a finite field](../../../vector-space.md#vector-space-over-a-finite-field), namely $\mathbb F_2$, because every element has order at most two. It is infinite-dimensional. The complete first-order theory of infinite-dimensional $\mathbb F_2$-vector spaces says, for each $n$, that there are $n$ linearly independent vectors; the usual elimination argument for vector spaces shows that all infinite-dimensional $\mathbb F_2$-vector spaces are elementarily equivalent.

Every countably infinite model of this theory has dimension $\aleph_0$: finite dimension would make it finite, while uncountable dimension would make its underlying set uncountable. Any two vector spaces over the same field with the same dimension are isomorphic. Therefore $\operatorname{Th}(B,+,0)$ is aleph-zero-categorical, as recorded by the [aleph-zero-categoricity of an infinite-dimensional vector space over a finite field](../../../foundations-of-mathematics.md#aleph-zero-categoricity-of-an-infinite-dimensional-vector-space-over-a-finite-field).

## 2

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A [filter on a set](../../../set-theory.md#filter-set-theory) $\mathcal U$ on $\mathbb N$ is a nonempty family of subsets of $\mathbb N$ such that:

- $\varnothing\notin\mathcal U$;
- if $A,B\in\mathcal U$, then $A\cap B\in\mathcal U$;
- if $A\in\mathcal U$ and $A\subseteq B\subseteq\mathbb N$, then $B\in\mathcal U$.

These conditions imply $\mathbb N\in\mathcal U$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

An [ultrafilter](../../../set-theory.md#ultrafilter) is a proper filter maximal under inclusion. Equivalently, for every $A\subseteq\mathbb N$, exactly one of $A$ and $\mathbb N\setminus A$ belongs to $\mathcal U$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

If $\mathcal U$ contains no finite set, then every cofinite set belongs to it: for a finite $F$, one has $F\notin\mathcal U$, so the ultrafilter alternative forces $\mathbb N\setminus F\in\mathcal U$. Thus $\mathcal U$ contains the [cofinite filter](../../../set-theory.md#cofinite-filter).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Suppose instead that a finite set $F$ belongs to $\mathcal U$. If none of its singleton subsets belonged to $\mathcal U$, all their complements would belong to $\mathcal U$, and intersecting those complements with $F$ would put the empty set in $\mathcal U$. Hence $\{n\}\in\mathcal U$ for some $n\in F$.

Upward closure then puts every subset containing $n$ in $\mathcal U$, while no subset omitting $n$ can belong to it. Therefore

$$
\mathcal U=\{A\subseteq\mathbb N:n\in A\},
$$

the [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) at $n$. Together with part i, this proves the dichotomy.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

**Yes.** Choose the principal ultrafilter at any $j\geq2$. Evaluation at the $j$th coordinate gives

$$
\prod_{i\in\mathbb N}\mathcal C_i/\mathcal U\cong\mathcal C_j,
$$

which is a finite [cyclic group](../../../group.md#cyclic-group) of order $j$.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

**No.** Suppose a formula with parameters defined a function $f:\mathcal C\to\mathcal C$ that was surjective and not injective. The assertions that the formula defines a function, that the function is surjective, and that it is not injective are all first-order statements about that formula and those parameters. By [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem), they would hold simultaneously in $\mathcal C_i$ for $\mathcal U$-almost every $i$.

Every surjective self-map of a finite set is injective, so no finite factor can satisfy those statements. This contradiction shows that the ultraproduct has no such definable function.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

**Yes.** Choose a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) on $\mathbb N$ and let

$$
a=[(1\bmod i)_{i\in\mathbb N}]_{\mathcal U}\in\mathcal C.
$$

For each fixed positive integer $n$, the equality $na=0$ holds in the $i$th factor exactly when $i$ divides $n$. Only finitely many positive integers divide $n$, so the cofinite set of indices for which $na\ne0$ belongs to $\mathcal U$. [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) gives $na\ne0$ in $\mathcal C$ for every $n>0$. Thus $a$ has infinite [order of a group element](../../../group-theory.md#order-of-a-group-element).

## 3

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the finite-partial-isomorphism criterion for [quantifier elimination](../../../foundations-of-mathematics.md#quantifier-elimination). Let $M,N\models\mathrm{DLO}$ and let $h:A\to B$ be an isomorphism between finite suborders. For $a\in M\setminus A$, its position relative to $A$ is one of the finitely many open intervals determined by $A$, or one of the two exterior rays. The corresponding interval or ray determined by $B$ is nonempty because the orders are dense and have no endpoints. Choose $b$ there. Then $h\cup\{(a,b)\}$ remains a partial order isomorphism.

The same argument extends in the other direction. The [back-and-forth method](../../../foundations-of-mathematics.md#back-and-forth-method) criterion therefore applies, proving [quantifier elimination for dense linear orders without endpoints](../../../foundations-of-mathematics.md#quantifier-elimination-for-dense-linear-orders-without-endpoints). Hence [DLO](../../../foundations-of-mathematics.md#dense-linear-order-without-endpoints) eliminates quantifiers.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The [type space](../../../foundations-of-mathematics.md#type-space) $S_1^{\mathcal Q}(\mathbb N)$ is the set of all [complete types](../../../foundations-of-mathematics.md#complete-type) in one free variable over the parameter set $\mathbb N\subseteq\mathbb Q$ that are consistent with $\operatorname{Th}(\mathcal Q)$ together with the diagram of those parameters. Thus each member chooses, for every formula $\varphi(x,\bar n)$ with $\bar n$ from $\mathbb N$, exactly one of $\varphi$ and $\neg\varphi$, consistently and completely.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

A type $p\in S_1^{\mathcal Q}(\mathbb N)$ is an [isolated type](../../../foundations-of-mathematics.md#isolated-type) when some formula $\varphi(x,\bar n)\in p$ isolates it: $p$ is the unique complete type containing $\varphi$. Equivalently, $\varphi$ implies every formula in $p$ modulo the complete theory with the named parameters.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

By quantifier elimination, a one-type is determined entirely by the position of $x$ relative to the natural-number parameters. Assuming $\mathbb N=\{0,1,2,\ldots\}$, the isolated types and isolating formulas are:

- $x=n$, for each $n\in\mathbb N$;
- $x<0$;
- $n<x<n+1$, for each $n\in\mathbb N$.

Each formula fixes every comparison of $x$ with every natural number, so it determines a complete type. These are precisely the isolated members of the [one-types over the natural numbers in the rational order](../../../foundations-of-mathematics.md#one-types-over-the-natural-numbers-in-the-rational-order).

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

There is exactly one non-isolated type:

$$
p_\infty(x)=\{n<x:n\in\mathbb N\}.
$$

It is consistent by the [compactness theorem](../../../mathematical-logic.md#compactness-theorem), since every finite subset is realized by a sufficiently large rational number. It is complete by quantifier elimination, because it decides every comparison with a parameter from $\mathbb N$.

**No formula isolates it.** Any formula belongs to $p_\infty$ only through finitely many natural-number parameters; after quantifier elimination it holds throughout some final ray. It is consequently also satisfied by a sufficiently large natural number, whose equality type differs from $p_\infty$. Thus $p_\infty$ is non-isolated, and the list in part i exhausts all other cuts of $\mathbb N$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
