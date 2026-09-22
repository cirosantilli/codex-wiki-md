<h1 id="5d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $X^2\equiv-1\pmod p$. Then $X$ is a [unit modulo n](../../../../../../unit-modulo-n.md) for modulus $p$, and [Fermat's little theorem](../../../../../../fermat-little-theorem.md) implies

$$
1\equiv X^{p-1}=(X^2)^{(p-1)/2}\equiv(-1)^{(p-1)/2}\pmod p.
$$

Since $p$ is an odd [prime number](../../../../../../prime-number.md), $1$ and $-1$ are distinct [residue classes](../../../../../../residue-class.md). Therefore $(p-1)/2$ is even, and $p\equiv1\pmod4$.

Conversely, put $q=(p-1)/2$. Pair each [integer](../../../../../../integer.md) $j\in\{1,\ldots,q\}$ with $p-j$ in the [factorial](../../../../../../factorial.md). [Wilson theorem](../../../../../../wilson-s-theorem.md) yields

$$
-1\equiv(p-1)!=\prod_{j=1}^q j(p-j)\equiv(-1)^q(q!)^2\pmod p.
$$

When $p\equiv1\pmod4$, $q$ is even, so $X=q!$ satisfies $X^2\equiv-1\pmod p$. This proves the [first supplementary law for quadratic reciprocity](../../../../../../first-supplementary-law-for-quadratic-reciprocity.md) without assuming a primitive root. Hence

$$
\boxed{X^2\equiv-1\pmod p\text{ is solvable exactly when }p\equiv1\pmod4.}
$$

The two solutions are $q!$ and $-q!$ modulo $p$: their difference is nonzero, and factoring $X^2-Y^2$ shows that a degree-two [polynomial](../../../../../../polynomial-split.md) over the [field](../../../../../../field.md) of residues modulo $p$ has no further roots.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
