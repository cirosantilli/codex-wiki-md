<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

Associate to $c=(c_1,\ldots,c_n)^T$ the [polynomial](../../../../../polynomial-split.md) $p(t)=\sum_{j=1}^nc_jt^{j-1}$. The $i$th component of $Ac$ is exactly $p(a_i)$. If $Ac=0$, this [polynomial](../../../../../polynomial-split.md) of degree at most $n-1$ has $n$ distinct roots. Repeated use of the factor theorem would make $\prod_{i=1}^n(t-a_i)$ divide any nonzero such [polynomial](../../../../../polynomial-split.md), contradicting its degree. Hence $p$ is the zero [polynomial](../../../../../polynomial-split.md) and all $c_j=0$. The converse is immediate, proving **$\ker A=\{0\}$**.

A square [matrix](../../../../../matrix.md) has full column [rank](../../../../../rank-one-quadratic-form.md) if and only if its [kernel](../../../../../kernel-of-a-linear-map.md) is zero, by [rank-nullity theorem](../../../../../rank-nullity-theorem.md). Its row [rank](../../../../../rank-one-quadratic-form.md) equals its column [rank](../../../../../rank-one-quadratic-form.md). Therefore this [Vandermonde matrix](../../../../../vandermonde-matrix.md) has row [rank](../../../../../rank-one-quadratic-form.md) $n$, and its rows $v_1,\ldots,v_n$ are a [basis](../../../../../basis.md) and **span $\mathbb R^n$**.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
