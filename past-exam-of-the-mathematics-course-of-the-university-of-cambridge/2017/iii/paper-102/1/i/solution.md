<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [simple Lie algebra](../../../../../../simple-lie-algebra.md) is a nonabelian [Lie algebra](../../../../../../lie-algebra-split.md) whose only [Lie algebra ideals](../../../../../../ideal-of-a-lie-algebra.md) are zero and the whole algebra. Assume $n\geq2$; $\mathfrak{sl}_1=0$ is not simple. We prove the assertion by the [matrix-unit extraction lemma for special linear ideals](../../../../../../matrix-unit-extraction-lemma-for-special-linear-ideals.md), avoiding any classification theorem.

Let $I$ be a nonzero ideal in the [special linear Lie algebra](../../../../../../special-linear-lie-algebra.md) and $0\ne A\in I$. If an off-diagonal entry $A_{ji}$ is nonzero, two [commutators](../../../../../../commutator.md) with the [matrix unit](../../../../../../matrix-unit.md) $E_{ij}$ give

$$
[E_{ij},[E_{ij},A]]=-2A_{ji}E_{ij}\in I,
$$

so $E_{ij}\in I$. If $A$ is diagonal and nonscalar, choose unequal diagonal entries; $[E_{ij},A]=(A_{jj}-A_{ii})E_{ij}$ again supplies a [matrix unit](../../../../../../matrix-unit.md). A nonzero scalar matrix cannot have zero [trace](../../../../../../matrix-trace.md) over $\mathbb C$, so these cases cover every nonzero $A$.

Once $E_{ij}\in I$, its bracket with $E_{ji}$ gives $H=E_{ii}-E_{jj}$, and $[H,E_{ji}]=-2E_{ji}$ puts the reverse unit in $I$. Bracketing with the other off-diagonal [matrix units](../../../../../../matrix-unit.md) generates every off-diagonal unit: for a third index $k$, $[E_{ij},E_{jk}]=E_{ik}$ and $[E_{ki},E_{ij}]=E_{kj}$; using the reverse unit fills the remaining row and column, then $[E_{ki},E_{i\ell}]=E_{k\ell}$ fills the others. Opposite pairs generate every trace-zero diagonal matrix. These vectors span $\mathfrak{sl}_n$, so

$$
\boxed{\mathfrak{sl}_n(\mathbb C)\text{ is simple for }n\geq2.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
