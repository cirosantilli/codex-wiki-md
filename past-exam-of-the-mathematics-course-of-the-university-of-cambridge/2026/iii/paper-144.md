# Paper 144

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20144.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20144.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A model of cardinality $\kappa$ is determined up to isomorphism by the unordered pair of cardinalities of its two equivalence classes. At cardinality $\aleph_0$, both infinite classes must be countable, so there is one isomorphism type. Thus $T_1$ is [categorical theory](../../../foundations-of-mathematics.md#categorical-theory) in $\aleph_0$.

For every uncountable $\kappa$, a model with class sizes $(\aleph_0,\kappa)$ is not isomorphic to one with sizes $(\kappa,\kappa)$. Hence $T_1$ is not $\kappa$-categorical for any uncountable $\kappa$; it has no finite models.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The theory is not categorical in any infinite cardinal. In cardinality $\aleph_0$, one may add no infinite equivalence class or one countably infinite class; these models are not isomorphic. For uncountable $\kappa$, one can vary the number and cardinalities of infinite classes while retaining infinitely many classes of every finite size. These choices are isomorphism invariants.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Every finite partial isomorphism between models of $T_1$ extends by one point. If the new point belongs to a class already represented in the domain, choose an unused point in the corresponding target class. Otherwise choose an unused point in the other target class. Both classes are infinite, so the choice is always possible. The [back-and-forth method](../../../foundations-of-mathematics.md#back-and-forth-method) shows that tuples with the same quantifier-free type have the same complete type. Therefore $T_1$ has [quantifier elimination](../../../foundations-of-mathematics.md#quantifier-elimination).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The formula saying that the $E$-class of $x$ has exactly $n$ elements uses quantifiers and distinguishes elements in differently sized classes. No quantifier-free one-variable formula in the language $\{E\}$ can do so, since its only atomic information is $x=x$ and $E(x,x)$. Thus $T_2$ does not eliminate quantifiers.

Expand the language by unary predicates $P_n(x)$, one for each positive integer $n$, interpreted as “the $E$-class of $x$ has size $n$”. In this definitional expansion, back-and-forth on finite substructures gives quantifier elimination.

## 2

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Fix an index $j$ and take the [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) $\mathcal U_1=\{A\subseteq\omega:j\in A\}$. Evaluation at the $j$th coordinate gives

$$
\prod_i\mathbb F_i/\mathcal U_1\cong\mathbb F_j,
$$

so the ultraproduct has characteristic $p_j$. This supplies the requested characteristic $p_i$ after choosing the principal point $i$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix $n\geq1$ and let $\mathbb E_i/\mathbb F_i$ be the unique degree-$n$ finite-field extension. [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) shows that

$$
\mathbb E=\prod_i\mathbb E_i/\mathcal U_2
$$

is a field extension of $\mathcal F$ of degree $n$: ultraproducts of chosen bases satisfy the first-order linear-independence and spanning statements.

Conversely, let $\mathcal F(\alpha)/\mathcal F$ have degree $n$, with irreducible minimal polynomial $f$. Represent its coefficients by polynomials $f_i$. Irreducibility in fixed degree is first-order, so $f_i$ is irreducible of degree $n$ for $\mathcal U_2$-almost every $i$. Its root generates $\mathbb E_i$, and the ultraproduct of these roots induces an $\mathcal F$-isomorphism $\mathcal F(\alpha)\cong\mathbb E$. Hence the degree-$n$ algebraic extension exists and is unique.

## 3

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A model $M$ is [aleph-zero-homogeneous model](../../../foundations-of-mathematics.md#aleph-zero-homogeneous-model) when, for finite tuples $\bar a,\bar b$ with the same complete type and every $c\in M$, there is $d\in M$ such that

$$
\operatorname{tp}(\bar a,c)=\operatorname{tp}(\bar b,d).
$$

Equivalently, every finite partial elementary map extends by one more element.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Start with the countable model $M_0$. There are countably many finite tuples and formulas. For every pair $\bar a,\bar b\in M_i$ having the same type and every $c\in M_i$, use compactness to realize over $\bar b$ the transported type $\operatorname{tp}(c/\bar a)$. Realize all these countably many requirements in an elementary extension and use the [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) to choose it countable; call it $M_{i+1}$.

The elementary union $M_\omega=\bigcup_{i<\omega}M_i$ is countable. Any finite tuples and element in it occur at one stage, and their required matching element appears at the next. Thus $M_\omega$ is an aleph-zero-homogeneous [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) of $M_0$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let

$$
M=\mathbb Z+(\mathbb Q\times\mathbb Z)
$$

with the lexicographic order, where the initial $\mathbb Z$ is one discrete block. This is a countable model of $\operatorname{Th}(\mathbb Z,<)$: it is a discrete order without endpoints, and every interval is either of its prescribed finite length or contains arbitrarily long finite chains.

An element $a$ in the initial block and an element $b$ in a later block have the same one-type. There is, however, a $c<b$ with infinitely many points between $c$ and $b$, whereas no such $c<a$ exists because every predecessor of $a$ lies at finite distance within the initial block. The type of $(b,c)$ therefore cannot be transported over $a$, so $M$ is not aleph-zero-homogeneous.

## 4

↑ **Parent:** [Paper 144](paper-144.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A complete theory $T$ is [strongly minimal](../../../foundations-of-mathematics.md#strongly-minimal-theory) when, in every model of $T$, every definable subset of the home sort in one variable, allowing parameters, is finite or cofinite.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In a strongly minimal theory, model-theoretic algebraic closure is a [pregeometry](../../../foundations-of-mathematics.md#pregeometry). Given finite tuples $\bar a,\bar b$ of the same type, the induced correspondence extends to an isomorphism between their algebraic closures. If $c\in\operatorname{acl}(\bar a)$, transport it through this isomorphism. If $c\notin\operatorname{acl}(\bar a)$, its type is the unique generic one over $\bar a$; choose a corresponding element outside $\operatorname{acl}(\bar b)$. Exchange ensures that this choice has the transported type. Hence every finite partial elementary map extends, and every model is aleph-zero-homogeneous.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The theory $\operatorname{ACF}_0$ of [algebraically closed fields](../../../algebra.md#algebraically-closed-field) of characteristic zero is strongly minimal in its field sort. Let

$$
M=\overline{\mathbb Q(t_0,t_1,\ldots)}
$$

and take $\kappa=\aleph_1$. The countable tuples

$$
\bar a=(t_1,t_2,\ldots),\qquad
\bar b=(t_0,t_1,\ldots)
$$

have the same type because both are algebraically independent sequences. The element $t_0$ is independent from $\bar a$, but there is no element of $M$ independent from $\bar b$, since $\bar b$ is a transcendence basis and $M=\operatorname{acl}(\bar b)$. Thus the partial elementary map $\bar a\mapsto\bar b$ cannot be extended to $t_0$, so $M$ is not $\aleph_1$-homogeneous.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
