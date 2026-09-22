# Pivoted LU decomposition

↑ **Parent:** [LU decomposition](lu-decomposition.md)

We fix the convention $PA=LU$: the [permutation matrix](permutation-matrix.md) $P$ acts on the rows of $A$, and the same row ordering must be applied to $b$ before the [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md). Equivalently, $A=P^TLU$, since $P^{-1}=P^T$. LAPACK documents its factors as $A=PLU$ instead, so check the defining equation rather than just the letter $P$.[LAPACK DGETRS, A argument: factors from DGETRF satisfy $A=PLU$](dgetrs-lapack-3-3-1-by-lapack-project.md) [Partial pivoting](columnwise-partial-pivoting.md) selects the largest absolute candidate in the current column, among rows $k,\ldots,n$, before forming [elimination multipliers](elimination-multiplier.md).[§2.6.1, Definition 2.6.1; §2.6.2, Definition 2.6.2 and equation (2.6.1): pivot selection and reordered-row factorization](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

A zero first [pivot element](pivot-element.md) does not imply a [singular matrix](singular-matrix.md). For example,

$$
A_0=\begin{pmatrix}0&1\\2&3\end{pmatrix},\qquad \det A_0=-2,\qquad P=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad PA_0=\underbrace{\begin{pmatrix}1&0\\0&1\end{pmatrix}}_{L}\underbrace{\begin{pmatrix}2&3\\0&1\end{pmatrix}}_{U}.
$$

Unpivoted [Gaussian elimination](gaussian-elimination.md) would divide $2$ by zero. Indeed, no $A_0=LU$ with a unit [lower triangular matrix](lower-triangular-matrix.md) $L$ exists: $u_{11}=0$ would force $(LU)_{21}=l_{21}u_{11}=0$, contradicting $(A_0)_{21}=2$. One row interchange resolves the obstruction. For $b_0=(1,5)^T$, use $Pb_0=(5,1)^T$; [back substitution](back-substitution.md) then gives $x=(1,1)^T$. Using the original $b_0$ with these factors would solve a different [linear system](system-of-linear-equations.md).

[Partial pivoting](columnwise-partial-pivoting.md) bounds each [elimination multiplier](elimination-multiplier.md) by one in absolute value in exact arithmetic. This helps control [roundoff error](round-off-error.md), but intermediate entries can still grow; it is not an unconditional guarantee of [numerical stability](stability-of-a-numerical-method.md) for every [matrix](matrix.md).[§2.6.4, Example 2.6.6 and the concluding discussion: stability of unpivoted and pivoted factorization](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md) It also does not remove the original problem's [condition number](condition-number.md). For the [diagonal matrix](diagonal-matrix.md) $D=\operatorname{diag}(1,\varepsilon)$ with $0<\varepsilon<1$, the [condition number](condition-number.md) in the [Euclidean norm](euclidean-norm.md) is $\kappa_2(D)=1/\varepsilon$. Row permutations preserve this [condition number](condition-number.md), because they preserve [Euclidean norms](euclidean-norm.md). Even an exact solve changes from $(1,1)^T$ to $(1,1+\eta/\varepsilon)^T$ when the right-hand side changes from $(1,\varepsilon)^T$ to $(1,\varepsilon+\eta)^T$. This sensitivity is a property of the [linear system](system-of-linear-equations.md), not a zero-[pivot element](pivot-element.md) failure.[§2.8, Definition 2.8.1, and §2.8.1, Theorem 2.8.1, equations (2.8.5)–(2.8.6): condition number and right-hand-side sensitivity](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

## ↑ Ancestors (7)

1. [LU decomposition](lu-decomposition.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Choosing a different block pivot](choosing-a-different-block-pivot.md)
- [LU decomposition](lu-decomposition.md)
- [Pivot element](pivot-element.md)
- [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md)
- [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
