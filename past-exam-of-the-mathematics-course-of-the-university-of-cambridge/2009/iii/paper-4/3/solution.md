<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [integer partitions](../../../../../integer-partition.md) $\lambda,\mu$ of $n$, padded by zero parts, the [dominance order on partitions](../../../../../dominance-order-on-partitions.md) is

$$
\boxed{\lambda\unrhd\mu\iff\sum_{i=1}^r\lambda_i\geq\sum_{i=1}^r\mu_i\quad\text{for every }r\geq1.}
$$

A $\lambda$-tableau fills the [Young diagram](../../../../../young-diagram.md) of $\lambda$ with $1,\ldots,n$, each once. A [tabloid](../../../../../tabloid.md) $[t]$ remembers the sets of entries in each row, ignoring their order within that row. The [Young permutation module](../../../../../young-permutation-module.md) $M^\lambda=\mathbb CX_\lambda$ has these [tabloids](../../../../../tabloid.md) as basis, with $S_n$ acting by permuting the entries.

The [row and column stabilizers](../../../../../row-and-column-stabilizers-of-a-young-tableau.md) $R_t,C_t$ independently permute entries within the rows and columns of $t$. The [column antisymmetrizer](../../../../../column-antisymmetrizer-of-a-young-tableau.md) is $\kappa_t=\sum_{c\in C_t}\operatorname{sgn}(c)c$, and $e_t=\kappa_t[t]$ is the associated [polytabloid](../../../../../polytabloid.md). Since $C_{gt}=gC_tg^{-1}$ and conjugation preserves permutation sign,

$$
\kappa_{gt}=g\kappa_tg^{-1},\qquad e_{gt}=\kappa_{gt}[gt]=g\kappa_t[t],\qquad \boxed{ge_t=e_{gt}.}
$$

Thus the [Specht module](../../../../../specht-module.md) is the submodule

$$
\boxed{S^\lambda=\operatorname{span}_{\mathbb C}\{e_t:t\text{ is a }\lambda\text{-tableau}\}\subseteq M^\lambda.}
$$

Every tableau is $gt$ for a fixed $t$, so any single $e_t$ generates it under $S_n$. Also $C_t\cap R_t=\{1\}$, since a permutation preserving both rows and columns must fix every cell. The [tabloids](../../../../../tabloid.md) $[ct]$ for $c\in C_t$ are consequently distinct, and $e_t$ has coefficient $1$ at $[t]$; in particular $e_t\ne0$.

We use the following precise [column antisymmetrizer](../../../../../column-antisymmetrizer-of-a-young-tableau.md) facts. If some row of a $\mu$-tableau $s$ contains two entries from one column of $t$, the transposition interchanging them pairs equal [tabloids](../../../../../tabloid.md) with opposite signs in $\kappa_t[s]$, so $\kappa_t[s]=0$. Otherwise each row of $s$ meets each column of $t$ at most once. The first $r$ rows of $s$ therefore contain at most $\min(r,\lambda'_j)$ entries from column $j$ of $t$, whence

$$
\sum_{i=1}^r\mu_i\leq\sum_j\min(r,\lambda'_j)=\sum_{i=1}^r\lambda_i.
$$

This states and explains [dominance from a nonzero column antisymmetrizer](../../../../../dominance-from-a-nonzero-column-antisymmetrizer.md): $\kappa_t[s]\ne0$ implies $\lambda\unrhd\mu$.

When $\mu=\lambda$, the [nonzero column antisymmetrizer criterion](../../../../../nonzero-column-antisymmetrizer-criterion.md) says more: either $\kappa_t[s]=0$, or a column permutation takes $[s]$ to $[t]$, and $\kappa_t[s]=\pm e_t$. Thus $\kappa_tM^\lambda=\mathbb Ce_t$. This follows by matching the row positions within each column when all intersections have size at most one; the equal row and column sizes force the Ferrers incidence pattern.

For the [inner product](../../../../../inner-product.md), use the positive Hermitian extension of the orthonormal [tabloid](../../../../../tabloid.md) basis, linear in its first argument. It has the supplied self-adjointness of $\kappa_t$. Its orthogonal complement of $S^\lambda$ agrees with that obtained from the complex [tabloid bilinear form](../../../../../tabloid-bilinear-form.md), since the spanning [polytabloids](../../../../../polytabloid.md) have real coefficients. Because the coefficient of $[t]$ in $e_t$ is $1$, self-adjointness and the one-dimensional image give the useful identity

$$
\boxed{\kappa_tu=\langle u,e_t\rangle e_t\qquad(u\in M^\lambda).}
$$

Indeed, the scalar multiplying $e_t$ is the $[t]$-coefficient of $\kappa_tu$, which is $\langle\kappa_tu,[t]\rangle=\langle u,\kappa_t[t]\rangle=\langle u,e_t\rangle$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
