# Paper 128

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20128.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20128.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [definable power set](../../../definable-power-set.md) of a set $X$ is

$$
\mathcal D(X)=
\left\{
\{x\in X:(X,\in)\models\varphi(x,a_1,\ldots,a_n)\}:
\varphi\text{ is a formula and }a_1,\ldots,a_n\in X
\right\}.
$$

**Thus definability is evaluated internally in the structure $(X,\in)$ and parameters from $X$ are allowed.**

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [constructible hierarchy](../../../definable-power-set.md#constructible-hierarchy) is defined by transfinite recursion:

$$
L_0=\varnothing,
\qquad
L_{\beta+1}=\mathcal D(L_\beta),
\qquad
L_\lambda=\bigcup_{\beta<\lambda}L_\beta
$$

when $\lambda$ is a [limit ordinal](../../../set-theory.md#limit-ordinal). Its union over all ordinals is the constructible universe $L$.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

A [condensation sentence for the constructible hierarchy](../../../definable-power-set.md#condensation-sentence-for-the-constructible-hierarchy) may be obtained by taking a single conjunction $\sigma$ that expresses a sufficiently strong finite fragment of set theory, the assertion $V=L$, and that the ordinals have no largest member. The finite fragment is chosen strong enough to define the satisfaction relation needed for the $L$-construction and to prove its absoluteness for transitive sets.

If a [transitive set](../../../set-theory.md#transitive-set) $X$ satisfies $\sigma$, let $\lambda=X\cap\operatorname{Ord}$. The absence of a largest ordinal makes $\lambda$ a limit ordinal. Internal $V=L$ says every $x\in X$ belongs to some internally constructed $L_\beta$, while transitivity and absoluteness identify that level with the actual $L_\beta$. Conversely the finite closure axioms ensure that every $L_\beta$, $\beta<\lambda$, belongs to $X$. Hence $X=L_\lambda$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Choose a successor ordinal $\beta=\delta+1>\alpha$, and then choose a limit ordinal $\gamma>\beta$. The level $L_\gamma$ satisfies the [condensation sentence for the constructible hierarchy](../../../definable-power-set.md#condensation-sentence-for-the-constructible-hierarchy). The level $L_\beta$ cannot satisfy it: otherwise condensation would give $L_\beta=L_\lambda$ for a limit $\lambda$, but

$$
L_\xi\cap\operatorname{Ord}=\xi
$$

would imply the impossible equality $\beta=\lambda$. Thus the condensation sentence belongs to $T_\gamma$ but not to $T_\beta$, and $T_\beta\ne T_\gamma$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The language of set theory has only countably many [sentences](../../../mathematical-logic.md#first-order-sentence), so there are at most $2^{\aleph_0}$ possible complete sets of sentences $T_\xi$. Choose $(2^{\aleph_0})^++1$ ordinals above $\alpha$. By cardinal pigeonhole, two of their theories agree. Hence some $\gamma>\beta>\alpha$ satisfy $T_\beta=T_\gamma$.

## 2

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

With the convention that $p\leq q$ means that $p$ is stronger, a set $G\subseteq\mathbb P$ is a [generic filter](../../../forcing.md#generic-filter) over $M$ when it is a filter and meets every [dense set](../../../forcing.md#dense-subset-of-a-forcing-order) $D\subseteq\mathbb P$ with $D\in M$. Explicitly, $G$ is upward closed toward weaker conditions, every two members have a common stronger member in $G$, and $G\cap D\ne\varnothing$ for every such $D$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $g\in\mathbb N^{\mathbb N}\cap M$ and $n\in\mathbb N$, the set

$$
D_{g,n}=\{s:\text{some }k\geq n\text{ below }|s|\text{ satisfies }s(k)=g(k)\}
$$

is dense in $\mathbb Q_0$: extend any finite sequence at one fresh coordinate with the corresponding value of $g$. The generic union $x_0$ meets every $D_{g,n}$, so it agrees infinitely often with every ground-model $g$. Thus $x_0$ is infinitely equal over $M$ and is not eventually different over $M$.

For $g\in\mathbb N^{\mathbb N}\cap M$, conditions of $\mathbb Q_1$ whose side set contains $g$ form a dense set. Once such a condition enters $G_1$, every later coordinate added to its stem must avoid $g$. Hence the generic union $x_1$ is eventually different from every ground-model $g$, and consequently is not infinitely equal over $M$.

The four answers are therefore

$$
\begin{array}{c|cc}
&\text{eventually different}&\text{infinitely equal}\\ \hline
x_0&\text{no}&\text{yes}\\
x_1&\text{yes}&\text{no}.
\end{array}
$$

## 3

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The [Hausdorff formula for cardinal exponentiation](../../../set-theory.md#hausdorff-formula-for-cardinal-exponentiation) states that for infinite cardinals $\kappa$ and $\lambda$,

$$
(\kappa^+)^\lambda
=\kappa^\lambda\cdot\kappa^+
=\max\{\kappa^\lambda,\kappa^+\}.
$$

Equivalently,

$$
\aleph_{\alpha+1}^{\aleph_\beta}
=\aleph_\alpha^{\aleph_\beta}\cdot\aleph_{\alpha+1}.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The [Fn forcing](../../../forcing.md#fn-forcing) $\operatorname{Fn}(X,Y,\kappa)$ consists of partial functions $p:X\rightharpoonup Y$ such that

$$
|\operatorname{dom}p|<\kappa.
$$

It is ordered by reverse inclusion: $p\leq q$ exactly when $p\supseteq q$, so a stronger condition supplies more values.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

If $M$ regards $\mathbb P$ as satisfying the [$\kappa$-chain condition](../../../forcing.md#chain-condition-for-forcing), then forcing with $\mathbb P$ preserves every cardinal and cofinality at least $\kappa$. If $M$ regards $|\mathbb P|$ as $\mu$, then every antichain has size at most $\mu$, so $\mathbb P$ has the $\mu^+$-chain condition. It follows that every cardinal and cofinality at least $\mu^+$ is preserved in a $\mathbb P$-generic extension.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

If $\mathbb P$ is [$\aleph_1$-closed](../../../forcing.md#closed-forcing) in $M$, a descending sequence deciding successively all entries of a proposed function $\mathbb N\to M$ has a common lower bound. Thus the extension contains no new countable sequences of ground-model elements and in particular

$$
\wp(\mathbb N)^{M[G]}=\wp(\mathbb N)^M.
$$

It follows that $\aleph_1^M$ remains uncountable and hence is preserved. More generally such closure preserves cardinals at most $\aleph_1$, but closure alone need not preserve larger cardinals.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The forcing

$$
\mathbb P=\operatorname{Fn}(\aleph_1^M\times\mathbb N,2,\aleph_1^M)
$$

is $\aleph_1^M$-closed, so by [closed forcing](../../../forcing.md#closed-forcing) it adds no new real numbers. Its generic union can be viewed as a sequence

$$
\langle r_\xi:\xi<\aleph_1^M\rangle,
\qquad r_\xi(n)=\bigcup G(\xi,n),
$$

of old reals. For every $r\in\wp(\mathbb N)^M$, conditions asserting that some unused row equals $r$ are dense: assigning all countably many values of that row is a legitimate condition. Thus the generic sequence surjects $\aleph_1^M$ onto the old set of reals.

In $M$, that set had cardinality $\aleph_2^M$. The forcing therefore collapses $\aleph_2^M$ to $\aleph_1^M$, while adding no reals and preserving $\aleph_1^M$. Consequently

$$
\boxed{M[G]\models 2^{\aleph_0}=\aleph_1.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The forcing $\mathbb P=\operatorname{Fn}(\aleph_1^N,2,\aleph_1^N)$ is $\aleph_1^N$-closed, so it adds no reals:

$$
\wp(\mathbb N)\cap N[G]=\wp(\mathbb N)\cap N.
$$

By contrast, $\aleph_1^M$ is countable in $N$. The union of the $\mathbb Q$-generic filter is a total binary function

$$
h:\aleph_1^M\longrightarrow2.
$$

Fix in $N$ a bijection $e:\mathbb N\to\aleph_1^M$. Then $r(n)=h(e(n))$ is a real in $N[H]$. It is not in $N$: for any ground-model real $r_0$ and any $p\in\mathbb Q$, some coordinate of $\aleph_1^M$ is outside $\operatorname{dom}p$, and extending there forces $r$ to differ from $r_0$. Hence $\mathbb Q$ adds a new real, and

$$
\boxed{\wp(\mathbb N)\cap N[G]\ne\wp(\mathbb N)\cap N[H].}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
