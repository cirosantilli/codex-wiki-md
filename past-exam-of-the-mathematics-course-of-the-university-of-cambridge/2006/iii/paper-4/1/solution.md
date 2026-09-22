<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [representation](../../../../../group-representation.md) over $F$ is a homomorphism $G\to\operatorname{GL}(V)$ on a [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md). It is [irreducible](../../../../../irreducible-representation.md) if it has no nonzero proper [invariant subspace](../../../../../invariant-subspace.md), and has [absolute irreducibility of a group representation](../../../../../absolute-irreducibility-of-a-group-representation.md) if it remains [irreducible](../../../../../irreducible-representation.md) after every [field extension](../../../../../field-extension.md). A [representation over the rational numbers](../../../../../representation-over-the-rational-numbers.md) is one over $\mathbb Q$; an [ordinary character](../../../../../ordinary-character.md) is the [trace](../../../../../matrix-trace.md) of a characteristic-zero [representation](../../../../../group-representation.md).

A [partition of an integer](../../../../../partition-of-an-integer.md) $n$ is a finite weakly decreasing sequence $\lambda=(\lambda_1,\lambda_2,\ldots)$ of positive integers of sum $n$, extended by zero parts when convenient. Its [Young diagram](../../../../../young-diagram.md) has $\lambda_i$ cells in row $i$; its [conjugate partition](../../../../../conjugate-partition.md) $\lambda'$ has $\lambda'_j$ cells in column $j$. [Conjugacy classes](../../../../../conjugacy-class.md) of $S_n$ are indexed by cycle lengths, hence by [partitions of an integer](../../../../../partition-of-an-integer.md). The number of ordinary [irreducible characters](../../../../../irreducible-character.md) equals the number of [conjugacy classes](../../../../../conjugacy-class.md); we now construct that many mutually distinct [representations over the rational numbers](../../../../../representation-over-the-rational-numbers.md).

A [Young tableau](../../../../../young-tableau.md) $t$ of shape $\lambda$ bijectively labels its cells by $1,\ldots,n$. Its [tabloid](../../../../../tabloid.md) $\{t\}$ remembers the set of labels in each distinguished row, not their order. The [Young permutation module](../../../../../young-permutation-module.md) $M_F^\lambda$ is the [vector space](../../../../../vector-space-split.md) on these [tabloids](../../../../../tabloid.md), with $S_n$ acting by relabeling. Its [tabloid bilinear form](../../../../../tabloid-bilinear-form.md) makes the [tabloid](../../../../../tabloid.md) basis orthonormal. Let $C_t$ be the subgroup permuting labels within each column and put

$$
\kappa_t=\sum_{g\in C_t}\operatorname{sgn}(g)g,\qquad e_t=\kappa_t\{t\},\qquad S_F^\lambda=\operatorname{span}_F\{e_t:t\text{ has shape }\lambda\}.
$$

Thus $e_t$ is a [polytabloid](../../../../../polytabloid.md) and $S_F^\lambda$ is a [Specht module](../../../../../specht-module.md). Relabeling takes $e_t$ to $e_{gt}$, so any [polytabloid](../../../../../polytabloid.md) generates the [module](../../../../../module-mathematics.md). It is nonzero over every [field](../../../../../field.md): the coefficient of $\{t\}$ in $e_t$ is one, since the [row and column stabilizers of a Young tableau](../../../../../row-and-column-stabilizers-of-a-young-tableau.md) intersect trivially.

Here is the elementary identity behind irreducibility. If a row of a [tabloid](../../../../../tabloid.md) contains two entries from one column of $t$, their [transposition](../../../../../transposition-permutation.md) pairs and cancels the terms in $\kappa_t$, including in [characteristic](../../../../../characteristic-of-a-field.md) two. Otherwise, for a [tabloid](../../../../../tabloid.md) of the same shape, its rows can be matched to those of $t$ by a column [permutation](../../../../../permutation.md), and $\kappa_t\{u\}=\pm e_t$. Looking at the coefficient of $\{t\}$ gives, for every $v\in M_F^\lambda$,

$$
\kappa_tv=\langle v,e_t\rangle e_t.
$$

Consequently a [submodule](../../../../../submodule.md) $U$ of $M_F^\lambda$ either contains $S_F^\lambda$, if one of these pairings is nonzero, or lies in $(S_F^\lambda)^\perp$. This proves the [James submodule theorem](../../../../../james-submodule-theorem.md) used below.

Over $\mathbb Q$, the restricted form on $S_\mathbb Q^\lambda$ is positive definite, so its [Gram determinant](../../../../../gram-determinant.md) in a rational basis is nonzero. Extending scalars to any characteristic-zero [field](../../../../../field.md) preserves that nonzero [determinant](../../../../../determinant.md) and hence keeps the restricted form a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md). The [James submodule theorem](../../../../../james-submodule-theorem.md) applied to a [submodule](../../../../../submodule.md) of $S^\lambda$ now forces it to be zero or the whole [module](../../../../../module-mathematics.md). Therefore **$S_\mathbb Q^\lambda$ is absolutely [irreducible](../../../../../irreducible-representation.md)**, not merely [irreducible](../../../../../irreducible-representation.md) over $\mathbb Q$.

To distinguish shapes, the cancellation argument above works for a $\mu$-tabloid too. If $\kappa_t\{u\}\ne0$, its first $r$ rows contain at most $\min(r,\lambda'_j)$ entries from column $j$, so

$$
\sum_{i\le r}\mu_i\le\sum_j\min(r,\lambda'_j)=\sum_{i\le r}\lambda_i.
$$

Thus $\lambda$ dominates $\mu$. The operator $\kappa_t$ acts nontrivially on $S^\lambda$ because the restricted form is a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md). An isomorphism $S^\lambda\cong S^\mu$ would therefore imply $\lambda\unrhd\mu$, and reversing the roles gives equality of the [partitions of an integer](../../../../../partition-of-an-integer.md). Counting [conjugacy classes](../../../../../conjugacy-class.md) proves exhaustion. All matrices in a rational [polytabloid](../../../../../polytabloid.md) basis have rational entries, giving the requested [representations over the rational numbers](../../../../../representation-over-the-rational-numbers.md).

For positive [characteristic](../../../../../characteristic-of-a-field.md) $p$, call a [partition of an integer](../../../../../partition-of-an-integer.md) a [regular partition](../../../../../regular-partition.md) if no part is repeated $p$ or more times. Define

$$
R_F^\lambda=S_F^\lambda\cap(S_F^\lambda)^\perp,\qquad D_F^\lambda=S_F^\lambda/R_F^\lambda.
$$

The [James submodule theorem](../../../../../james-submodule-theorem.md) shows that every proper [submodule](../../../../../submodule.md) of $S_F^\lambda$ lies in $R_F^\lambda$. Whenever the restricted form is nonzero, $R_F^\lambda$ is proper and its quotient is simple.

We verify exactly when this happens. Let $m_j$ be the number of rows of length $j$. In the integral pairing $\langle e_s,e_t\rangle$, common [tabloids](../../../../../tabloid.md) are acted on freely by [permutations](../../../../../permutation.md) of equal-length rows. Such a row [permutation](../../../../../permutation.md) has sign $\operatorname{sgn}(\pi)^j$ in both [polytabloids](../../../../../polytabloid.md), so its contribution to the product of coefficients is unchanged. Each orbit has size $\prod_jm_j!$. Thus that integer divides every pairing. On the other hand, reverse each row of $t$ to obtain $t^*$. A [tabloid](../../../../../tabloid.md) common to $e_t$ and $e_{t^*}$ can only interchange entries between rows of equal length. There are $m_j!$ independent choices in each of their $j$ columns, and the two signs agree. Hence

$$
\langle e_t,e_{t^*}\rangle=\prod_j(m_j!)^j.
$$

These two products have exactly the same prime divisors. All pairings vanish modulo $p$ precisely when some $m_j\ge p$. Therefore $D_F^\lambda\ne0$ exactly for $p$-regular $\lambda$.

For such a shape, the displayed pairing gives $\kappa_te_{t^*}=h e_t$ with $h\ne0$, and $e_t$ has nonzero image in $D^\lambda$. If $D^\lambda\cong D^\mu$, the same operator must act nontrivially on a quotient of $M^\mu$, forcing $\lambda\unrhd\mu$ by the cancellation argument. Interchanging the shapes proves $\lambda=\mu$.

For exhaustion over an [algebraic closure](../../../../../algebraic-closure.md) use the general [Brauer character basis theorem](../../../../../brauer-character-basis-theorem.md): the number of [simple modules](../../../../../irreducible-module.md) over an algebraically closed [field](../../../../../field.md) of [characteristic](../../../../../characteristic-of-a-field.md) $p$ is the number of [conjugacy classes](../../../../../conjugacy-class.md) of elements of order prime to $p$. Here these are the cycle [partitions of an integer](../../../../../partition-of-an-integer.md) with no part divisible by $p$. The generating-function identity

$$
\prod_{j\ge1}(1+t^j+\cdots+t^{(p-1)j})
=\prod_{j\ge1}\frac{1-t^{pj}}{1-t^j}
=\prod_{p\nmid j}(1-t^j)^{-1}
$$

shows that their number equals the number of $p$-regular [partitions of an integer](../../../../../partition-of-an-integer.md). We have already constructed that many distinct [simple modules](../../../../../irreducible-module.md), so they exhaust all simples. The form, its radical and its quotient commute with [field extension](../../../../../field-extension.md), and the same simplicity proof holds after every extension. The [modules](../../../../../module-mathematics.md) defined over the [prime field](../../../../../prime-field.md) are therefore absolutely [irreducible](../../../../../irreducible-representation.md) and form a split complete list over arbitrary $F$ as well. In summary,

$$
\boxed{\operatorname{Irr}(FS_n)=\{D_F^\lambda:\lambda\vdash n\text{ is }p\text{-regular}\}.}
$$

For [characteristic](../../../../../characteristic-of-a-field.md) zero the list is instead all $S_F^\lambda$. In positive [characteristic](../../../../../characteristic-of-a-field.md) a [Specht module](../../../../../specht-module.md) itself need not be [irreducible](../../../../../irreducible-representation.md); the radical quotient is essential.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
