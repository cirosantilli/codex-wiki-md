<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Use the inclusive convention: a [set](../../../../../set-split.md) is [countable](../../../../../countable-set.md) if it admits an [injective function](../../../../../injective-function.md) into $\mathbb N=\{1,2,\ldots\}$. This includes every [finite set](../../../../../finite-set.md) and the empty set. If $j:X\to\mathbb N$ is injective and $Y\subseteq X$, its restriction to $Y$ is still injective, proving directly that every subset of a [countable set](../../../../../countable-set.md) is countable.

Enumerate pairs by diagonals. The positive-integer [Cantor pairing function](../../../../../cantor-pairing-function.md)

$$
\pi(a,b)=\frac{(a+b-2)(a+b-1)}2+b
$$

is a [bijection](../../../../../bijection.md) $\mathbb N^2\to\mathbb N$: on the diagonal $a+b-2=d$, its values are $d(d+1)/2+1$ through $(d+1)(d+2)/2$, each once, and these consecutive blocks partition $\mathbb N$. This proves countability without assuming any product theorem.

For a sequence of [countable sets](../../../../../countable-set.md) $X_1,X_2,\ldots$, choose injections $j_i:X_i\to\mathbb N$. For $x$ in their union, let $i(x)$ be the least index containing $x$. The map

$$
x\longmapsto\pi\bigl(i(x),j_{i(x)}(x)\bigr)
$$

is injective: its encoded index and the injective within-set code recover $x$. Thus a [countable union of countable sets](../../../../../countable-union-of-countable-sets.md) is countable. Selecting the injections for an arbitrary given family uses the usual [axiom of countable choice](../../../../../axiom-of-countable-choice.md); when the encodings are supplied, the displayed construction is entirely explicit.

For finite Cartesian powers, start with the identity injection on $\mathbb N$ and recursively encode $(a_1,\ldots,a_n)$ as $\pi(j_{n-1}(a_1,\ldots,a_{n-1}),a_n)$. This proves that $\mathbb N^n$ is countable for every [positive integer](../../../../../positive-integer.md) $n$ and is the constructive proof of the [finite Cartesian power of a countable set](../../../../../finite-cartesian-power-of-a-countable-set.md) property.

For each [positive integer](../../../../../positive-integer.md) $m$, let $P_m$ consist of the functions for which $m$ is a period. Restriction to the residues $0,1,\ldots,m-1$ is a [bijection](../../../../../bijection.md) $P_m\to\mathbb N^m$: any tuple extends uniquely to all of $\mathbb Z$ by taking residues modulo $m$, including negative arguments. Hence $P_m$ is countable. Every [periodic function](../../../../../periodic-function.md) belongs to some $P_m$, so

$$
\boxed{\{f:\mathbb Z\to\mathbb N:f\text{ is periodic}\}=\bigcup_{m\geq1}P_m\text{ is countable}}.
$$

There is no need to assume the chosen period is minimal; multiple descriptions only create overlap, which does not invalidate the union argument. This is an instance of the [cardinality of integer-periodic function spaces](../../../../../cardinality-of-integer-periodic-function-spaces.md) principle.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
