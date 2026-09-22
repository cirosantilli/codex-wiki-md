<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Pauli matrices](../../../../../../pauli-matrices.md) obey $[X,Z]=-2iY$ and $[Y,Z]=2iX$, and operators on different tensor factors commute. Hence

$$
[X_mX_n,Z_m+Z_n]=-2i(Y_mX_n+X_mY_n),\qquad [Y_mY_n,Z_m+Z_n]=2i(X_mY_n+Y_mX_n).
$$

Adding gives $\boxed{[X_mX_n+Y_mY_n,Z_m+Z_n]=0}$. Each $Z_mZ_n$ commutes separately with both $Z_m$ and $Z_n$, so $\boxed{[Z_mZ_n,Z_m+Z_n]=0}$. Every interaction on sites $m,n$ also commutes with all $Z_\ell$ for $\ell\notin\{m,n\}$. Therefore equal $XX$ and $YY$ coefficients make their contributions cancel pair by pair, and $\boxed{[H_S,S]=0\text{ when }\alpha_{mn}=\beta_{mn}\text{ for every pair}}$. This is [Excitation-number conservation in XXZ spin chains](../../../../../../excitation-number-conservation-in-xxz-spin-chains.md): $S$ is the total [spin magnetization](../../../../../../spin-magnetization.md) in Pauli normalization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
