# Tridiagonal solve costs

↑ **Parent:** [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)

For the displayed unpivoted [Thomas algorithm](tridiagonal-matrix-algorithm.md) with one right-hand side, count each scalar [addition](addition.md), [subtraction](subtraction.md), [multiplication](multiplication.md) or [division](division-mathematics.md) as one [arithmetic operation](arithmetic-operation.md). Forming $m_i,p_i,g_i$ takes five [arithmetic operations](arithmetic-operation.md) per forward step. The last unknown takes one [division](division-mathematics.md); each remaining [back substitution](back-substitution.md) step takes three [arithmetic operations](arithmetic-operation.md). Thus

$$
5(n-1)+1+3(n-1)=8n-7.
$$

This is an operation-count model, excluding assignments, indexing, pivot checks and any special simplifications of the coefficients. It is not a timing benchmark. The original [tridiagonal matrix](tridiagonal-matrix.md) needs $3n-2$ scalar entries, and its right-hand side another $n$. Overwriting $b_i$ with $p_i$ and $d_i$ with $g_i$, then with $x_i$, keeps storage $O(n)$; the arrays, rather than the few loop temporaries, determine the total [space complexity](space-complexity.md).

For repeated right-hand sides, retain the [LU decomposition](lu-decomposition.md): computing $m_i,p_i$ once costs $3(n-1)$ [arithmetic operations](arithmetic-operation.md), and each subsequent pair of [forward substitution](forward-substitution.md) and [back substitution](back-substitution.md) sweeps costs $5n-4$. Hence $r$ right-hand sides cost $3(n-1)+r(5n-4)$ [arithmetic operations](arithmetic-operation.md). This is the banded counterpart of [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md).

## ↑ Ancestors (6)

1. [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
