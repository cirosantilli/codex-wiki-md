# Two-factor tensor rank

↑ **Parent:** [Tensor product](tensor-product.md)

The [two-factor tensor rank](two-factor-tensor-rank.md) is the smallest number of [pure tensors](pure-tensor.md) whose sum equals $t$, with zero allowed as the empty sum. For two [finite-dimensional vector spaces](finite-dimensional-vector-space.md) over the same [field](field.md), it equals the [matrix rank](matrix-rank.md) of the [tensor-product coefficient matrix](tensor-product-coefficient-matrix.md). A sum of $r$ [outer products](outer-product.md) has [column space](column-space.md) contained in the span of their $r$ first factors, so its [matrix rank](matrix-rank.md) is at most $r$. Conversely, choose a [basis](basis.md) $u_1,\ldots,u_r$ for the [column space](column-space.md), express each column in that [basis](basis.md), and collect the coefficients into row [vectors](vector.md) $w_k^T$. This yields $C=\sum_{k=1}^ru_kw_k^T$, hence a sum of $r$ [pure tensors](pure-tensor.md).

The [pure tensor](pure-tensor.md) $(2,1)\otimes(-1,3)$ therefore has [two-factor tensor rank](two-factor-tensor-rank.md) one, whereas $e_1\otimes f_1+e_2\otimes f_2$ has [two-factor tensor rank](two-factor-tensor-rank.md) two. Both have two factors: the number of factors and the minimum number of product summands are different counts. Over the [real numbers](real-number.md), the [singular value decomposition](singular-value-decomposition.md) supplies a useful decomposition $C=\sum_k\sigma_ku_kv_k^T$, with one nonzero term per [matrix rank](matrix-rank.md). The two-factor rank equality does not extend to three or more factors by merely choosing one [matrix](matrix.md) layout.

## ↑ Ancestors (7)

1. [Tensor product](tensor-product.md)
2. [Multilinear algebra](multilinear-algebra.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Two-factor tensor rank](two-factor-tensor-rank.md)
