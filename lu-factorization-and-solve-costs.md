# LU factorization and solve costs

↑ **Parent:** [LU decomposition](lu-decomposition.md)

For classical dense [Gaussian elimination](gaussian-elimination.md) over the [real numbers](real-number.md), count each scalar [addition](addition.md), [subtraction](subtraction.md), [multiplication](multiplication.md) or [division](division-mathematics.md) as one [arithmetic operation](arithmetic-operation.md). At step $k$, there are $n-k$ [elimination multipliers](elimination-multiplier.md) to divide out and $(n-k)^2$ remaining entries, each requiring one [multiplication](multiplication.md) and one [subtraction](subtraction.md). Thus this implementation's unpivoted factorization count is

$$
F(n)=\sum_{k=1}^{n-1}\bigl((n-k)+2(n-k)^2\bigr)=\frac{n(n-1)(4n+1)}6=\frac23n^3+O(n^2).
$$

Here $O$ uses [Big O notation](big-o-notation.md). [Partial pivoting](columnwise-partial-pivoting.md) adds $O(n^2)$ comparisons and row movement, leaving the leading arithmetic count unchanged. The leading $\tfrac23n^3$ count agrees with the standard dense [LU decomposition](lu-decomposition.md) analysis.[§2.5.2, Definition 2.5.2; §2.5, equations (2.5.7)–(2.5.8) and Theorem 2.5.1; lower-order counts depend on implementation](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

With unit $L$, [forward substitution](forward-substitution.md) uses $n(n-1)$ [arithmetic operations](arithmetic-operation.md). [Back substitution](back-substitution.md) uses another $n(n-1)$ plus $n$ diagonal divisions. Together these cost $2n^2-n$ per right-hand side; applying a stored row permutation moves $n$ entries and requires no scalar arithmetic. In [Big O notation](big-o-notation.md), [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md) therefore costs

$$
\frac23n^3+2rn^2+O(n^2+rn),
$$

whereas refactorizing for each of the $r$ right-hand sides costs $\tfrac23rn^3+O(rn^2)$. For $n=1000$ and $r=10$, the leading counts are about $6.87\times10^8$ versus $6.69\times10^9$ [arithmetic operations](arithmetic-operation.md), nearly a tenfold saving. These are operation counts, not measured runtimes: memory access and optimized [matrix multiplication](matrix-multiplication.md) also affect speed.[§2.5.2, Important note after Definition 2.5.2: flop counts are a rough runtime model; the numerical comparison here is an original calculation](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

## ↑ Ancestors (7)

1. [LU decomposition](lu-decomposition.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian elimination](gaussian-elimination.md)
- [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
