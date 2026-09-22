# Paper 144

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_144.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_144.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [i](#8/i)
    - [Solution](#8/i/solution)
  - [ii](#8/ii)
    - [Solution](#8/ii/solution)

## 1

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let tuples $\bar a\in M\models T$ and $\bar b\in N\models T$ have the same quantifier-free type. The map $\bar a\mapsto\bar b$ extends to an isomorphism between the substructures they generate. Identify these substructures with one structure $A$. Both expanded models satisfy $T\cup D(A)$, which is complete by hypothesis, so they satisfy the same formulas with parameters from $A$. Thus $\bar a$ and $\bar b$ have the same complete type.

Therefore every isomorphism between substructures of models of $T$ is partial elementary. By compactness, this implies that every formula is equivalent modulo $T$ to a quantifier-free formula: otherwise two tuples with the same quantifier-free type but different truth values could be constructed. This is the [common-substructure test for quantifier elimination](../../../foundations-of-mathematics.md#common-substructure-test-for-quantifier-elimination), so $T$ admits [quantifier elimination](../../../foundations-of-mathematics.md#quantifier-elimination).

## 2

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Apply the test from Question 1. If two algebraically closed fields of the same characteristic contain a common subring $A$, they contain its fraction field and agree on all algebraic equations over it. Algebraic elements can be matched through their minimal polynomials, while transcendental elements can be matched by extending transcendence bases; an algebraic closure then gives a common extension. Thus the theory with $D(A)$ is complete. Hence the theory of [algebraically closed fields](../../../algebra.md#algebraically-closed-field) of each fixed characteristic has [quantifier elimination for algebraically closed fields](../../../foundations-of-mathematics.md#quantifier-elimination-for-algebraically-closed-fields) in the ring language.

For $F\subseteq K$ and a tuple $a$ in an elementary extension, associate

$$
I(a/F)=\{P\in F[X_1,\ldots,X_n]:P(a)=0\}.
$$

This is a prime ideal. Conversely, the fraction field of $F[X]/\mathfrak p$ embeds into an algebraically closed extension, producing a tuple with relation ideal $\mathfrak p$. Quantifier elimination says this ideal determines the complete type. Thus $S_n^K(F)$ is the set of prime ideals of $F[X_1,\ldots,X_n]$. A basic formula consisting of polynomial equalities and inequalities gives a constructible subset of the prime spectrum, and these sets are clopen. This is the [type space of an algebraically closed field over a subfield](../../../foundations-of-mathematics.md#type-space-of-an-algebraically-closed-field-over-a-subfield) with its constructible topology.

## 3

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In a real closed field, the formula $\exists z\,(z^2=x)$ defines the nonnegative elements. A quantifier-free formula in one variable over the prime field is a Boolean combination of polynomial equations, so in an infinite field it defines a finite or cofinite set. The nonnegative cone is neither finite nor cofinite. Hence the [Theory of real closed fields](../../../foundations-of-mathematics.md#theory-of-real-closed-fields) does not eliminate quantifiers in the pure ring language.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Expand RCF by a constant $c$ and the sentences $c>n$ for all natural numbers $n$. Every finite subset is realized in $\mathbb R$. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) gives a model realizing all of them, hence a [Non-Archimedean real closed field](../../../foundations-of-mathematics.md#non-archimedean-real-closed-field).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

RCF is not aleph-zero-categorical: the real algebraic numbers and a countable real closure of $\mathbb Q(t)$ are countable models with different transcendence degrees. It is not categorical in any uncountable cardinal either. At cardinality $2^{\aleph_0}$, for example, $\mathbb R$ is Archimedean whereas the real closure of $\mathbb R(t)$ with $t$ infinitely large is non-Archimedean. If RCF were categorical in any uncountable cardinal, the [Morley categoricity theorem](../../../foundations-of-mathematics.md#morley-categoricity-theorem) would make it categorical in every uncountable cardinal, contradicting this pair.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Let $f\in\mathbb R(X_1,\ldots,X_n)$ be positive semidefinite. The assertion that $f(x)\geq0$ wherever its denominator is nonzero is first-order in ordered fields and holds in $\mathbb R$. Since RCF is model-complete, it holds in every real closed extension of $\mathbb R$.

If $f$ were not a sum of squares, the Artin-Schreier ordering criterion would give an ordering of $\mathbb R(X_1,\ldots,X_n)$ in which $f<0$. Its real closure is a real closed extension of $\mathbb R$, contradicting the transferred assertion at the generic tuple $(X_1,ldots,X_n)$. Hence $f$ is a sum of squares. This is the [Model-theoretic proof of Hilbert's seventeenth problem](../../../foundations-of-mathematics.md#model-theoretic-proof-of-hilbert-s-seventeenth-problem).

## 4

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

An [atomic model](../../../foundations-of-mathematics.md#atomic-model) is a model in which the type over the empty set of every finite tuple is isolated. Let $\bar a\mapsto\bar b$ be partial elementary and take $c\in M$. Choose a formula $\theta(\bar x,y)$ isolating $\operatorname{tp}(\bar a,c)$. Since $M\models\exists y\,\theta(\bar a,y)$, elementarity gives $N\models\exists y\,\theta(\bar b,y)$. Any witness $d$ realizes the isolated joint type, so $\bar a,c\mapsto\bar b,d$ is partial elementary. This is the [one-point extension between atomic models](../../../foundations-of-mathematics.md#one-point-extension-between-atomic-models).

Alternately applying this extension property in the two directions to enumerations of countable atomic models constructs a [back-and-forth](../../../foundations-of-mathematics.md#back-and-forth-method) isomorphism.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Suppose first that $T$ is aleph-zero-categorical. If a type in some $S_n(T)$ were nonisolated, the [omitting types theorem](../../../foundations-of-mathematics.md#omitting-types-theorem) would produce a countable model omitting it, while a countable elementary submodel of a model realizing it would be another countable model. This contradicts categoricity. Thus every type is isolated. The compact Stone space $S_n(T)$ is then discrete and therefore finite.

Conversely, if every $S_n(T)$ is finite, every type is isolated. Every countable model is consequently atomic, and part i says that any two countable models are isomorphic. This proves the [Ryll-Nardzewski theorem](../../../foundations-of-mathematics.md#ryll-nardzewski-theorem).

## 5

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The theory RG says that the edge relation is irreflexive and symmetric and includes, for every $m,n$, the extension axiom asserting that for disjoint vertices $u_1,\ldots,u_m,v_1,\ldots,v_n$ there is a new vertex adjacent to every $u_i$ and no $v_j$. Every finite subset of these axioms has a finite model by choosing a sufficiently large random graph, so compactness proves consistency. Equivalently, the countable Rado graph is an explicit model.

Any finite partial graph isomorphism extends by one vertex using the extension axiom. Back-and-forth therefore makes every partial embedding elementary, proving [quantifier elimination for the random graph](../../../foundations-of-mathematics.md#quantifier-elimination-for-the-random-graph).

By quantifier elimination, a three-type is determined by equality and adjacency. There is one type with all variables equal. If exactly two are equal, there are three choices of the equal pair and two choices for adjacency to the third vertex, giving six. If all are distinct, the three possible edges can be chosen independently, giving eight. Thus the [three-type space of the random graph](../../../foundations-of-mathematics.md#three-type-space-of-the-random-graph) has

$$
1+6+8=15
$$

elements, with the discrete Stone topology.

## 6

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

A structure $M$ is $\kappa$-saturated when every type over a parameter set of cardinality below $\kappa$ is realized in $M$. It is $\kappa$-homogeneous when every partial elementary map of size below $\kappa$ has the one-point extension property.

Let $f:A\to B$ be such a map and $c\in M$. Transport $\operatorname{tp}(c/A)$ through $f$ to a type over $B$. Its parameter set has size below $\kappa$, so saturation supplies a realization $d$. Then $f\cup\{(c,d)\}$ is partial elementary. This proves that [saturation implies homogeneity](../../../foundations-of-mathematics.md#saturation-implies-homogeneity).

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Let $A=\{a_1,\ldots,a_n\}\subseteq M$ and let $p(x/A)$ be a type. In an elementary extension choose $c$ realizing it and consider the empty-set type $q=\operatorname{tp}(a_1,\ldots,a_n,c)$. By hypothesis, $M$ contains a tuple $(b_1,\ldots,b_n,d)$ realizing $q$. The map $b_i\mapsto a_i$ is partial elementary, so omega-homogeneity extends it to include $d\mapsto d'$. Then $d'$ realizes $p$. Hence $M$ is omega-saturated, as stated by [homogeneity plus realization of empty-set types implies saturation](../../../foundations-of-mathematics.md#homogeneity-plus-realization-of-empty-set-types-implies-saturation).

## 7

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

An omega-stable countable theory is totally transcendental. The resulting definability and finite-base theorem for types says that every type over a parameter set $A$ is based on a finite tuple from $A$ and is determined by a countable choice of formulas over that tuple. For infinite $|A|=\kappa$, there are only $\kappa$ finite tuples from $A$ and only countably many formulas, so

$$
|S_n(A)|\leq\kappa\cdot\aleph_0=\kappa.
$$

**Thus $T$ is $\kappa$-stable for every infinite cardinal $\kappa$. This is [omega-stability implies stability in every infinite cardinal](../../../foundations-of-mathematics.md#omega-stability-implies-stability-in-every-infinite-cardinal).**

## 8

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="8/i">i</h3>

↑ **Parent:** [8](#8)

<h4 id="8/i/solution">Solution</h4>

↑ **Parent:** [I](#8/i)

Take $f<g$ in $I=\mathbb Q^\lambda$ and let $\alpha$ be their first differing coordinate. Choose $r\in\mathbb Q$ with $f(\alpha)<r<g(\alpha)$, copy their common initial segment below $\alpha$, put $r$ at $\alpha$, and put zero at every later coordinate. The resulting eventually zero element lies strictly between $f$ and $g$, so $J$ is dense.

For each $\mu<\lambda$, the eventually zero functions supported below $\mu$ number at most

$$
|\mathbb Q|^{|\mu|}=2^{|\mu|}.
$$

Minimality of $\lambda$ gives $2^{|\mu|}\leq\kappa$ for every $\mu<\lambda$. Also $\lambda\leq\kappa$, since $2^\kappa>\kappa$. Taking the union over $\mu<\lambda$ therefore gives $|J|\leq\kappa$.

<h3 id="8/ii">ii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8/ii)

A formula $\phi(\bar x,\bar y)$ has the [order property](../../../foundations-of-mathematics.md#order-property) for $T$ when, for every finite $n$, some model contains tuples $a_i,b_j$ with

$$
\phi(a_i,b_j)\quad\Longleftrightarrow\quad i<j.
$$

Compactness realizes this pattern indexed by any linear order.

Fix $\kappa\geq|T|$ and let $\lambda$ be least with $2^\lambda>\kappa$. Use the order property along $I=\mathbb Q^\lambda$, and take parameters

$$
B=\{b_j:j\in J\},
$$

where part i gives $|B|\leq\kappa$. For distinct $i,i'\in I$, choose $j\in J$ strictly between them. Then $\phi(a_i,b_j)$ and $\phi(a_{i'},b_j)$ have different truth values, so the types $\operatorname{tp}(a_i/B)$ are distinct. There are $|I|=2^\lambda>\kappa$ such types over at most $\kappa$ parameters. Enlarging $B$ to size exactly $\kappa$ if necessary preserves them. Hence $T$ is not $\kappa$-stable. This is the [order property implies instability](../../../foundations-of-mathematics.md#order-property-implies-instability) argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
