<h1 id="10f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For every nonnegative integer $k$,

$$
(BA)^{k+1}=B(AB)^kA.
$$

Consequently, if $m_{AB}(AB)=0$, then

$$
(BA)m_{AB}(BA)=B\,m_{AB}(AB)A=0.
$$

By the divisibility characterization of the [minimal polynomial](../../../../../../minimal-polynomial.md),

$$
m_{BA}(t)\mid t,m_{AB}(t).
$$

Interchanging $A$ and $B$ also gives $m_{AB}(t)\mid t,m_{BA}(t)$. Therefore the [Minimal polynomials of AB and BA](../../../../../../minimal-polynomials-of-ab-and-ba.md) can differ only in the exponent of the factor $t$, and that exponent differs by at most one.

If $AB$ is [diagonalizable](../../../../../../diagonalizable-matrix.md), its minimal polynomial has no repeated roots. The preceding divisibility says that every nonzero [Jordan block](../../../../../../jordan-block.md) of $BA$ has size one and every zero-eigenvalue block has size at most two. Squaring $BA$ preserves the one-dimensional nonzero blocks and sends every size-at-most-two nilpotent block to zero. Thus the [Jordan normal form](../../../../../../jordan-normal-form.md) of $(BA)^2$ is diagonal, so

$$
\boxed{AB\text{ diagonalizable}\ \Longrightarrow\ (BA)^2\text{ diagonalizable}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
