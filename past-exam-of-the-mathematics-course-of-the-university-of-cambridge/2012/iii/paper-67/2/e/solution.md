<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a [Boolean function](../../../../../../boolean-function.md) $f$, its [block sensitivity](../../../../../../block-sensitivity.md) at $x$ is the maximum number of pairwise disjoint nonempty index sets $B_j$ such that flipping all bits in each $B_j$ individually changes $f(x)$. Maximize over $x$ to obtain $\operatorname{bs}(f)$.

Choose $x=(110)(110)\cdots(110)$, so every three-bit block has majority one and the conjunction is one. In each block, flipping either of its two one bits alone changes that block's majority to zero and therefore changes the conjunction to zero. These $2n$ singleton index sets are all disjoint, so

$$
\operatorname{bs}(\operatorname{MAJ}_n)\ge2n.
$$

The supplied bounded-error [quantum query complexity](../../../../../../quantum-query-complexity.md) lower bound now gives

$$
\boxed{Q_2(\operatorname{MAJ}_n)=\Omega(\sqrt n).}
$$

Here $Q_2$ denotes a fixed two-sided error bound below $1/2$, such as $1/3$.

In fact the [block sensitivity](../../../../../../block-sensitivity.md) is exactly $2n$. At a one-input, selecting two one bits from each triple gives a size-$2n$ certificate: any block flip changing the output must touch it, so disjoint sensitive sets number at most $2n$. At a zero-input, one failing triple contains at least two zero bits; fixing those two zeros certifies zero, so at most two disjoint sensitive sets can change the output. The lower-bound witness above attains $2n$. The [certificate complexity of a Boolean function](../../../../../../certificate-complexity-of-a-boolean-function.md) supplies these upper bounds, though only the witness is needed for the requested result.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
