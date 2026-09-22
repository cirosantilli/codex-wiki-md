# Safe pivots for tridiagonal elimination

↑ **Parent:** [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)

The displayed [Thomas algorithm](tridiagonal-matrix-algorithm.md) requires every modified [pivot element](pivot-element.md) to be nonzero in exact [arithmetic](arithmetic-split.md). Nonzero original diagonal entries alone are insufficient: later [pivot elements](pivot-element.md) can vanish after elimination. Two useful sufficient contexts are a real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md), and [strict diagonal dominance](strictly-diagonally-dominant-matrix.md) by rows:

$$
|b_i|>|a_i|+|c_i|\quad(1\leq i\leq n),\qquad a_1=c_n=0.
$$

For the [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) case, elimination leaves positive-definite remaining blocks by the [Schur complement](schur-complement.md), so each $p_i>0$. Equivalently, the initial [principal minors](principal-minor.md) $\Delta_i=\det A_{1:i,1:i}$ are positive, and $p_i=\Delta_i/\Delta_{i-1}$ with $\Delta_0=1$.

For [strict diagonal dominance](strictly-diagonally-dominant-matrix.md), a short induction shows $|p_i|>|c_i|$. The first row gives $|p_1|=|b_1|>|c_1|$. Assuming the preceding bound, the [triangle inequality](triangle-inequality.md) gives

$$
|p_i|\geq|b_i|-\frac{|a_i|\,|c_{i-1}|}{|p_{i-1}|}\geq|b_i|-|a_i|>|c_i|.
$$

In particular $p_n\ne0$. These are structural guarantees against a zero [pivot element](pivot-element.md), not universal bounds on forward error in [floating-point arithmetic](floating-point-arithmetic.md). A poorly conditioned [linear system](system-of-linear-equations.md) can still amplify [roundoff error](round-off-error.md); [numerical stability](stability-of-a-numerical-method.md) and the [condition number](condition-number.md) must be distinguished.

## ↑ Ancestors (6)

1. [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Dirichlet Poisson solution by tridiagonal elimination](dirichlet-poisson-solution-by-tridiagonal-elimination.md)
