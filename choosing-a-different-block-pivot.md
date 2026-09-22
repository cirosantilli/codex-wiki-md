# Choosing a different block pivot

↑ **Parent:** [Block matrix inverse](block-matrix-inverse.md)

An [invertible matrix](invertible-matrix.md) need not have an invertible chosen diagonal block. For example,

$$
M=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad M^{-1}=M,
$$

has [singular matrices](singular-matrix.md) as both one-by-one diagonal blocks. Neither diagonal-block formula applies in that partition. Interchanging the two rows produces the [identity matrix](identity-matrix.md) and a usable [pivot element](pivot-element.md). This is why a failed block pivot is not proof that the full [matrix](matrix.md) is a [singular matrix](singular-matrix.md); [Pivoted LU decomposition](pivoted-lu-decomposition.md) changes the order before eliminating.

Conversely, invertible diagonal blocks do not suffice: $M=\begin{pmatrix}1&1\\1&1\end{pmatrix}$ has $A=D=1$ but [Schur complement](schur-complement.md) $S=0$, so it is a [singular matrix](singular-matrix.md). Both hypotheses in the [block matrix inverse](block-matrix-inverse.md) formula have work to do.

## ↑ Ancestors (7)

1. [Block matrix inverse](block-matrix-inverse.md)
2. [Matrix inverse](matrix-inverse-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
