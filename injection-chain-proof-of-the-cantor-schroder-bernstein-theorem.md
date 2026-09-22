<h1 id="injection-chain-proof-of-the-cantor-schroder-bernstein-theorem">Injection-chain proof of the Cantor-Schröder-Bernstein theorem</h1>

↑ **Parent:** [Cantor-Schröder-Bernstein theorem](cantor-schroder-bernstein-theorem.md)

Given [injections](injective-function.md) $f:X\to Y$ and $g:Y\to X$, start with the [set difference](set-difference.md) $A_0=X\setminus g(Y)$: these are exactly the inputs for which $g^{-1}$ is unavailable. Follow both [functions](function-split.md) repeatedly, using the [natural-number recursion theorem](natural-number-recursion-theorem.md) to define

$$
A_{k+1}=g(f(A_k)),\qquad
A=\bigcup_{k=0}^{\infty}A_k.
$$

Thus $A$ contains all the $X$ members reachable from any starting point in $A_0$. The notation $f(A_k)$ and $g(f(A_k))$ denotes [images of a function](image-of-a-function.md). If $A_0$ is the [empty set](empty-set.md), then every $A_k$ is empty and $g^{-1}$ alone gives the desired [bijection](bijection.md).

<a id="image-the-injection-chain-proof-of-the-cantor-schroder-bernstein-theorem-partitions-the-inputs-into-two-matching-rules"></a>
![](cantor-schroder-bernstein-injection-chain-partition.png)

**[Figure 4](#image-the-injection-chain-proof-of-the-cantor-schroder-bernstein-theorem-partitions-the-inputs-into-two-matching-rules). The Injection-chain proof of the Cantor-Schröder-Bernstein theorem partitions the inputs into two matching rules**. The upper row shows a chain seeded in $A_0$, where the [bijection](bijection.md) follows $f$. The lower row shows a chain beginning in $Y$, where the [bijection](bijection.md) reverses $g$. The same rule $g^{-1}$ also handles chains with no starting point and closed loops. Separate $X$ and $Y$ copies are used even if the original [sets](set-split.md) overlap.

Define a [function](function-split.md) on all of $X$ by

$$
h(x)=\begin{cases}
f(x),&x\in A,\\
g^{-1}(x),&x\in X\setminus A.
\end{cases}
$$

Here $g^{-1}$ is the [inverse function](inverse-function.md) from $g(Y)$ to $Y$, obtained by restricting the [codomain](codomain.md) of $g$ to its [image](image-of-a-function.md). It is well defined because $g$ is [injective](injective-function.md). Every $x\notin A$ belongs to $g(Y)$, since $A_0\subseteq A$, so the second rule is always available where it is used.

The decisive [set](set-split.md) identity is

$$
g(f(A))=\bigcup_{k=0}^{\infty}g(f(A_k))
=\bigcup_{k=1}^{\infty}A_k
=A\setminus A_0.
$$

The last equality holds because every $A_k$ with $k\geq1$ lies in $g(Y)$, whereas $A_0$ is disjoint from $g(Y)$. Consequently, for any $y\in Y$,

$$
g(y)\in A\quad\Longleftrightarrow\quad y\in f(A).
$$

Indeed, $g(y)$ cannot belong to $A_0$; if it lies in $A$, the identity gives $g(y)=g(f(a))$ for some $a\in A$, and [injectivity](injective-function.md) gives $y=f(a)$. The converse follows directly by applying $g$.

Now $f$ restricts to a [bijection](bijection.md) from $A$ onto $f(A)$. The displayed equivalence says that $g$ restricts to a [bijection](bijection.md) from $Y\setminus f(A)$ onto $X\setminus A$, so its [inverse function](inverse-function.md) bijects the remaining inputs with the remaining outputs. The two input [sets](set-split.md) partition $X$ and the two output [sets](set-split.md) partition $Y$. Their combined [function](function-split.md) $h$ is therefore both [injective](injective-function.md) and [surjective](surjective-function.md).

No [choice function](choice-function.md) is needed: $A$ is fixed by the given [injections](injective-function.md), and each required $g^{-1}(x)$ is unique. We neither choose a representative from each chain nor enumerate $X$. This is a proof in ordinary classical [ZF](zermelo-fraenkel-set-theory.md), even when no [well-ordering](well-order.md) of the [sets](set-split.md) exists there.[Paul Garrett, Cantor-Schroeder-Bernstein Theorem, pp. 1–2, chain construction and pairings; p. 1, no invocation of the axiom of choice](cantor-schroeder-bernstein-theorem-by-paul-garrett.md)

## ↑ Ancestors (7)

1. [Cantor-Schröder-Bernstein theorem](cantor-schroder-bernstein-theorem.md)
2. [Cardinal number](cardinal-number-split.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cantor-Schröder-Bernstein theorem](cantor-schroder-bernstein-theorem.md)
- [Injection-chain proof of the Cantor-Schröder-Bernstein theorem](injection-chain-proof-of-the-cantor-schroder-bernstein-theorem.md)
