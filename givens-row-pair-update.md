# Givens row-pair update

↑ **Parent:** [Givens rotation](givens-rotation.md)

Left [matrix multiplication](matrix-multiplication.md) by a [Givens rotation](givens-rotation.md) replaces rows $i,j$ of a [matrix](matrix.md) by

$$
A'_{ik}=cA_{ik}+sA_{jk},\qquad
A'_{jk}=-sA_{ik}+cA_{jk}.
$$

Both right-hand sides use the old entries. An in-place [algorithm](algorithm.md) must save the first result temporarily, update the second entry, and only then overwrite the first. The reference BLAS `DROT` implementation follows this order with its temporary `DTEMP`.[DROT source, lines 116–120 and 130–134: temporary first-row value and second-row update](drot-reference-blas-lapack-3-12-1-by-lapack-project.md)

For elimination in column $k$, construct $(c,s)$ from $(A_{ik},A_{jk})$. This sets the lower component to zero in exact arithmetic. In [floating-point arithmetic](floating-point-arithmetic.md) the computed expression can leave a small remainder; after computing the other updated entries, explicitly store $A'_{jk}=0$ and $A'_{ik}=r$. Previously eliminated columns stay zero if both participating rows are already zero there. This is why the ordering in [QR decomposition by Givens rotations](qr-decomposition-by-givens-rotations.md) matters.

## ↑ Ancestors (6)

1. [Givens rotation](givens-rotation.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [QR decomposition by Givens rotations](qr-decomposition-by-givens-rotations.md)
