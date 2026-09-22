<h1 id="5d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [set](../../../../../../set-split.md) is countable if it admits an [injection](../../../../../../injective-function.md) into the [natural numbers](../../../../../../natural-number.md); this includes [finite sets](../../../../../../finite-set.md) and the empty [set](../../../../../../set-split.md). Use $\mathbb N_0=\{0,1,2,\ldots\}$ for the enumeration. The [Cantor pairing function](../../../../../../cantor-pairing-function.md)

$$
\Pi(i,j)=\frac{(i+j)(i+j+1)}2+j
$$

is a [bijection](../../../../../../bijection.md) $\mathbb N_0^2\to\mathbb N_0$. Indeed, on the diagonal $i+j=s$, its values are the consecutive [integers](../../../../../../integer.md) from $s(s+1)/2$ through $s(s+1)/2+s$. These intervals are disjoint, and the next starts one beyond the preceding endpoint. Every nonnegative [integer](../../../../../../integer.md) therefore determines exactly one diagonal $s$, then exactly one $j$, and finally $i=s-j$. If one's convention starts the [natural numbers](../../../../../../natural-number.md) at one, translate both coordinates by one. Thus **$\mathbb N\times\mathbb N$ is a [countable set](../../../../../../countable-set.md)**.

For [countable sets](../../../../../../countable-set.md) $X,Y$, choose [injections](../../../../../../injective-function.md) $e_X:X\to\mathbb N_0$ and $e_Y:Y\to\mathbb N_0$. The map $(x,y)\mapsto\Pi(e_X(x),e_Y(y))$ is an [injection](../../../../../../injective-function.md), proving their [Cartesian product](../../../../../../cartesian-product.md) is countable. Repeating this proves that every [finite Cartesian power of a countable set](../../../../../../finite-cartesian-power-of-a-countable-set.md) is countable.

For a sequence of [countable sets](../../../../../../countable-set.md) $X_n$, choose an [injection](../../../../../../injective-function.md) $e_n:X_n\to\mathbb N_0$ for each $n$. For $x\in\bigcup_nX_n$, let $n(x)$ be the least index containing $x$. The map

$$
x\longmapsto\Pi\bigl(n(x),e_{n(x)}(x)\bigr)
$$

is an [injection](../../../../../../injective-function.md): its value recovers $n(x)$ and then $x$. This proves the **[countable union of countable sets](../../../../../../countable-union-of-countable-sets.md) theorem**. Selecting all $e_n$ uses the usual [axiom of countable choice](../../../../../../axiom-of-countable-choice.md); if enumerations are already supplied, the construction itself needs no additional choices.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
