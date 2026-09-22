<h1 id="7e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use “countable” to include finite and empty sets: a [countable set](../../../../../../countable-set.md) admits an [injection](../../../../../../injective-function.md) into $\mathbb N_0$. If $B\subseteq A$ and $j:A\to\mathbb N_0$ is [injective](../../../../../../injective-function.md), restricting $j$ to $B$ proves that $B$ is a [countable set](../../../../../../countable-set.md).

For a [countable union of countable sets](../../../../../../countable-union-of-countable-sets.md), index the family as $A_0,A_1,\ldots$ and choose an [injection](../../../../../../injective-function.md) $j_i:A_i\to\mathbb N_0$ for each member. For an element $a$ of the union, let $i(a)$ be the least index containing it, and assign

$$
a\longmapsto\bigl(i(a),j_{i(a)}(a)\bigr).
$$

This is [injective](../../../../../../injective-function.md): equality of the pair gives the same set index and then the same element. Finally the [Cantor pairing function](../../../../../../cantor-pairing-function.md)

$$
(i,j)\longmapsto\frac{(i+j)(i+j+1)}2+j
$$

injects $\mathbb N_0^2$ into $\mathbb N_0$. **The union is therefore countable.** The proof uses chosen injections for the family, as in the usual set-theoretic framework with [axiom of countable choice](../../../../../../axiom-of-countable-choice.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
