# Paper 120

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_120.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_120.pdf)

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

## 1

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Expand $L$ to $L(M)$ by a constant $c_m$ for each $m\in M$. The [diagram of a structure](../../../foundations-of-mathematics.md#diagram-mathematical-logic) $\operatorname{Diag}(M)$ contains all atomic and negated atomic $L(M)$-sentences true in $M$. The elementary diagram $\operatorname{ElDiag}(M)$ contains every $L(M)$-sentence true in $M$.

The [method of diagrams](../../../foundations-of-mathematics.md#method-of-diagrams) combines one of these sets with another theory and applies the [compactness theorem](../../../mathematical-logic.md#compactness-theorem). A model of $\operatorname{Diag}(M)$ yields an embedding of $M$ by $m\mapsto c_m$, while a model of $\operatorname{ElDiag}(M)$ yields an [elementary embedding](../../../set-theory.md#elementary-embedding).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

On $A=\bigcup_iA_i$, interpret a constant at its common value, a function on a tuple by choosing one $A_i$ containing the tuple, and a relation similarly. Total ordering of the indices and compatibility of substructures make these definitions independent of the chosen stage. Every $A_i$ is then a substructure of $A$.

For an elementary chain, induction on formulas proves

$$
A_i\models\varphi(\bar a)\Longleftrightarrow A\models\varphi(\bar a)
\qquad(\bar a\in A_i).
$$

The atomic step follows from the induced structure, Boolean steps are immediate, and for an existential formula any witness in the union lies in a later $A_j$ containing the parameters; elementarity between $A_i$ and $A_j$ moves existence back to $A_i$. This is the [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A sentence $\forall\bar x\,\exists\bar y\,\varphi(\bar x,\bar y)$ with quantifier-free $\varphi$ is preserved by a union of an embedding chain: a tuple $\bar a$ occurs at some stage, a witness $\bar b$ exists at that stage, and quantifier-free formulas are preserved in the union. Thus every forall-exists axiomatized theory is [inductive](../../../foundations-of-mathematics.md#inductive-first-order-theory).

Conversely, let $T_0$ contain all forall-exists consequences of $T$ and suppose $M\models T_0$. The diagram-and-compactness sandwich lemma says that one can construct

$$
M=M_0\subseteq N_0\subseteq M_1\subseteq N_1\subseteq\cdots
$$

where every $N_i\models T$ and every $M_i\preccurlyeq M_{i+1}$. For completeness, the first extension is obtained by adding to $T$ the diagram of $M_i$ together with all universal formulas over $M_i$ true there. A finite inconsistency would give a forall-exists consequence of $T$ false in $M_i$. The resulting extension embeds into an elementary extension $M_{i+1}$ by the method of diagrams.

The $N_i$ form an embedding chain and have the same union $N$ as the $M_i$. By the assumed preservation, $N\models T$; by the [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem), $M\preccurlyeq N$. Hence $M\models T$, so $T_0\models T$. The two theories are equivalent, proving the characterization.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

A [model-complete theory](../../../foundations-of-mathematics.md#model-complete-theory) is one for which every embedding between models is elementary. If $(M_i)$ is an embedding chain of models, all transition embeddings are therefore elementary. The [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem) shows that the union is a model elementarily extending every $M_i$, so the theory is preserved under unions of embedding chains. Part (c) then gives an axiomatization by forall-exists sentences.

## 2

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A complete $n$-type over $X\subseteq M$ is a maximal set $p(\bar x)$ of $L(X)$-formulas consistent with the theory of $M$ with parameters from $X$. Equivalently, for every formula $\varphi(\bar x)$, exactly one of $\varphi,\neg\varphi$ belongs to $p$.

The [type space](../../../foundations-of-mathematics.md#type-space) $S_n^M(X)$ has these types as points and basic open sets

$$
[\varphi]=\{p:\varphi\in p\}.
$$

Since $[\varphi]^c=[\neg\varphi]$, these sets are clopen. An [isolated type](../../../foundations-of-mathematics.md#isolated-type) is a point $\{p\}=[\varphi]$ for some formula $\varphi\in p$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Add new constants $\bar c$ and consider

$$
\operatorname{ElDiag}(M)\cup\{\varphi(\bar c):\varphi\in p\}.
$$

Every finite subset is satisfiable because $p$ is consistent over $M$. By the [compactness theorem](../../../mathematical-logic.md#compactness-theorem) it has a model $N'$. The constants naming $M$ give an elementary embedding $M\to N'$, and $\bar c^{N'}$ realizes $p$. Replacing $N'$ by an isomorphic copy containing $M$ gives the required [realization of a type in an elementary extension](../../../foundations-of-mathematics.md#realization-of-a-type-in-an-elementary-extension).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

If $p\neq q$, completeness gives a formula $\varphi$ with $\varphi\in p$ and $\neg\varphi\in q$. Then

$$
p\in[\varphi],\qquad q\in[\neg\varphi],
$$

and these two disjoint open sets cover $S_n^M(X)$. This proves the [total disconnectedness of a type space](../../../foundations-of-mathematics.md#total-disconnectedness-of-a-type-space).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write the [Ehrenfeucht-Mostowski model](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-model) as the Skolem hull of its order-indiscernible skeleton $(a_i)_{i\in\eta}$. Every element is $t(a_{i_1},\ldots,a_{i_r})$ for a Skolem term $t$. Choose supports for the elements of $X$ and let $J\subseteq\eta$ be their union. Then

$$
|J|\leq |L|+|X|.
$$

When $\eta$ is well ordered, the type over $X$ of $t(a_{i_1},\ldots,a_{i_r})$ is determined by $t$ and the finite order pattern of the indices $i_k$ relative to $J$. There are at most $|L|$ terms and at most $|J|$ such finite patterns. Therefore the number of realized complete one-types is at most

$$
\boxed{|L|+|X|}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Assume $M$ is a [prime model](../../../foundations-of-mathematics.md#prime-model). By the downward Lowenheim-Skolem theorem, $T$ has a countable model, and the elementary embedding of $M$ into it makes $M$ countable. If a tuple $\bar a\in M$ had a nonisolated type, the omitting types theorem would give a countable model of $T$ omitting that type. An elementary embedding of $M$ into this model would realize it, a contradiction. Thus $M$ is [atomic](../../../foundations-of-mathematics.md#atomic-model).

Conversely, let $M$ be countable and atomic, enumerate it as $(a_i)_{i<\omega}$, and let $N\models T$. Construct an elementary embedding recursively. Suppose $a_0,\ldots,a_{n-1}$ have been mapped to $\bar b$. Let $\psi(\bar x)$ isolate the type of $(a_0,\ldots,a_{n-1})$ and let $\theta(\bar x,y)$ isolate the type of $(a_0,\ldots,a_n)$. Since the latter extends the former and is realized in $M$, completeness gives

$$
T\models\forall\bar x\,
\bigl(\psi(\bar x)\to\exists y\,\theta(\bar x,y)\bigr).
$$

The tuple $\bar b$ realizes $\psi$, so a suitable image of $a_n$ exists in $N$. The union of the finite partial elementary maps is an elementary embedding $M\to N$. Hence $M$ is prime.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Let $M$ be a prime model and let $[\varphi]\subseteq S_n(T)$ be a nonempty basic open set. Some model of $T$ realizes $\varphi$, so completeness of $T$ gives

$$
T\models\exists\bar x\,\varphi(\bar x).
$$

Therefore $M$ realizes $\varphi$ by some tuple $\bar a$. The prime-model characterization in part (e) says $\operatorname{tp}^M(\bar a/\varnothing)$ is isolated, and it lies in $[\varphi]$. Every nonempty basic open set thus contains an isolated point, proving [density of isolated types from a prime model](../../../foundations-of-mathematics.md#density-of-isolated-types-from-a-prime-model).

## 3

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Under the [Implicational Curry-Howard correspondence](../../../mathematical-logic.md#implicational-curry-howard-correspondence), propositions are simple types and assumptions are typed variables. The natural-deduction rules

$$
\frac{\Gamma,A\vdash B}{\Gamma\vdash A\to B}
\qquad\text{and}\qquad
\frac{\Gamma\vdash A\to B\quad\Gamma\vdash A}{\Gamma\vdash B}
$$

correspond respectively to the typing rules

$$
\frac{\Gamma,x:A\vdash M:B}{\Gamma\vdash\lambda x.M:A\to B},
\qquad
\frac{\Gamma\vdash M:A\to B\quad\Gamma\vdash N:A}{\Gamma\vdash MN:B}.
$$

An assumption $x:A$ corresponds to the variable rule. Induction on a proof converts each rule into the matching typing construction; induction on a typing derivation reverses the process. Thus derivability of an implicational formula from assumptions is equivalent to inhabitation of its corresponding type.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

By part (a), such a term would prove

$$
((\sigma\to\tau)\to\sigma)\to\sigma
$$

in intuitionistic propositional logic. Consider the two-world [Kripke model for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-model-for-intuitionistic-propositional-logic) $r<s$. Let $\sigma$ hold only at $s$ and let $\tau$ hold nowhere. At both worlds $\sigma\to\tau$ fails, so $(\sigma\to\tau)\to\sigma$ holds at $r$ vacuously, while $\sigma$ does not hold at $r$. The displayed formula therefore fails at $r$. By the [Kripke completeness theorem for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-completeness-theorem-for-intuitionistic-propositional-logic), it is not derivable, so no simply typed lambda term inhabits that type.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**No such first-order theory exists.** Suppose $T$ axiomatized the Heyting algebras having only finitely many [regular elements](../../../mathematical-logic.md#regular-element-of-a-heyting-algebra). Expand the language by constants $c_n$ and add

$$
\neg\neg c_n=c_n,\qquad c_n\neq c_m\quad(n\neq m).
$$

Every finite subset has a model: take a sufficiently large finite Boolean algebra, in which every element is regular. By the [compactness theorem](../../../mathematical-logic.md#compactness-theorem), the entire expanded theory has a model. Its reduct is a model of $T$ with infinitely many distinct regular elements, contradicting the proposed axiomatization.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
