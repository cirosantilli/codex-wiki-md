<h1 id="5e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $f:S\to\mathcal P(S)$ were a [surjective function](../../../../../../surjective-function.md). Form the [subset](../../../../../../subset.md)

$$
D=\{s\in S:s\notin f(s)\}.
$$

Since $D$ belongs to the [power set](../../../../../../power-set.md), surjectivity would give $D=f(d)$ for some $d\in S$. But then $d\in D$ holds if and only if $d\notin f(d)=D$, a contradiction. Thus no such function is surjective, and in particular **there is no [bijection](../../../../../../bijection.md) from $S$ to its [power set](../../../../../../power-set.md)**. This is [Cantor theorem](../../../../../../cantor-s-theorem.md); the argument also applies when $S$ is empty.

For infinite [binary sequences](../../../../../../bitstream.md), use the [bijection](../../../../../../bijection.md)

$$
(x_n)_{n\geq1}\longmapsto\{n\in\mathbb N:x_n=1\}
$$

with $\mathcal P(\mathbb N)$, taking $\mathbb N=\{1,2,\ldots\}$. Conversely, a subset determines its sequence of membership indicators. The [power set](../../../../../../power-set.md) is infinite, since it contains all singletons, and [Cantor theorem](../../../../../../cantor-s-theorem.md) rules out a bijection with $\mathbb N$. Hence it is an [uncountable set](../../../../../../uncountable-set.md), as is the set of infinite [binary sequences](../../../../../../bitstream.md). Equivalently, a proposed enumeration $(x_n^{(j)})_{n\geq1}$ is defeated by the sequence $y_j=1-x_j^{(j)}$, which differs from its $j$th listed sequence at position $j$. This is the [Cantor diagonal argument](../../../../../../cantor-diagonal-argument.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
