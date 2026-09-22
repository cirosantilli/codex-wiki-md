# Finite-difference Jacobian

↑ **Parent:** [Jacobian matrix](jacobian-matrix.md)

An approximation to a [Jacobian matrix](jacobian-matrix.md) obtained using [finite differences](finite-difference-split.md) instead of analytic partial derivatives. For a vector-valued function $F$, the forward-difference entry is $J_{ij}\approx(F_i(x+h e_j)-F_i(x))/h$, where $e_j$ is a coordinate [basis vector](basis-vector.md). The step $h$ balances truncation and rounding errors; the resulting matrix can be used in a [Newton root-finding iteration](newton-root-finding-iteration.md).

## ↑ Ancestors (9)

1. [Jacobian matrix](jacobian-matrix.md)
2. [Jacobian matrix and determinant](jacobian-matrix-and-determinant.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
