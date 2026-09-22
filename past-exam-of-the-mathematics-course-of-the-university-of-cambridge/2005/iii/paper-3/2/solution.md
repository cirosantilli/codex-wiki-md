<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [dominance order on partitions](../../../../../dominance-order-on-partitions.md) is defined by

$$
\lambda\unrhd\mu\quad\Longleftrightarrow\quad
\sum_{i=1}^r\lambda_i\ge\sum_{i=1}^r\mu_i\quad\text{for every }r.
$$

Write $\lambda\triangleright\mu$ when the shapes are distinct as well. We first explain why the nonzero $D^\lambda$ from [regular partitions](../../../../../regular-partition.md) exhaust the simple [modules](../../../../../module-mathematics.md). The argument also provides the required constraint on [composition factors](../../../../../composition-factor.md).

For a [regular partition](../../../../../regular-partition.md) $\lambda$ and a tableau $t$ of that shape, the operator $b_t$ has rank one on $D^\lambda$: on $S^\lambda$ its image lies in $Fe_t$, and the nonzero pairing with the row-reversed [polytabloid](../../../../../polytabloid.md) from Question 1 shows that this image survives in $D^\lambda$. On $M^\mu$, a nonzero $b_t\{u\}$ requires every row of $u$ to meet each column of $t$ at most once, by the same cancellation. Consequently the first $r$ rows of $u$ contain at most $\min(r,\lambda'_j)$ entries from column $j$. Summing gives

$$
\sum_{i=1}^r\mu_i\le\sum_j\min(r,\lambda'_j)
=\sum_{i=1}^r\lambda_i.
$$

Thus nonzero column action forces $\lambda\unrhd\mu$. In particular, if $D^\lambda\cong D^\mu$, its nonzero column operators applied to the realization of either simple as a [composition factor](../../../../../composition-factor.md) of the other's [Young permutation module](../../../../../young-permutation-module.md) force both dominances; hence $\lambda=\mu$.

Over an algebraic closure in characteristic $p>0$, the number of simple group [modules](../../../../../module-mathematics.md) is the number of [p-regular elements](../../../../../p-regular-element.md)' [conjugacy classes](../../../../../conjugacy-class.md), by the [Brauer character basis theorem](../../../../../brauer-character-basis-theorem.md). Such classes in $S_n$ have cycle lengths not divisible by $p$. The [Glaisher partition bijection](../../../../../glaisher-partition-bijection.md) equates their number with the number of [regular partitions](../../../../../regular-partition.md): expand a part $p^a d$, with $p\nmid d$, into $p^a$ copies of $d$, and invert by the base-$p$ expansion of each multiplicity. The distinct absolutely [irreducible](../../../../../irreducible-representation.md) $D^\lambda$ therefore form the complete list. Since they are already defined and absolutely [irreducible](../../../../../irreducible-representation.md) over the prime [field](../../../../../field.md), the same list is valid over any $F$ of characteristic $p$. In [characteristic zero](../../../../../characteristic-zero.md), the analogous count uses all [partitions of an integer](../../../../../partition-of-an-integer.md) and all [conjugacy classes](../../../../../conjugacy-class.md).

If $D^\lambda$ occurs in a [composition series](../../../../../composition-series.md) of $M^\mu$, its nonzero $b_t$ action lifts through the subquotient, so $b_tM^\mu\ne0$. The inequality above proves $\lambda\unrhd\mu$. When $\lambda=\mu$ is regular, $b_t$ has rank one on $M^\mu$ and rank one on $D^\mu$. An operator preserving a finite filtration has rank at least the sum of its ranks on the successive quotients: relative to an adapted basis its matrix is block triangular, and nonzero pivot minors of the diagonal blocks combine to a nonzero minor. Therefore $D^\mu$ can occur at most once. It occurs at least once as the quotient of $S^\mu\subset M^\mu$. We have proved

$$
\boxed{[M^\mu:D^\lambda]\ne0\Rightarrow\lambda\unrhd\mu,
\qquad [M^\mu:D^\mu]=1\text{ if }\mu\text{ is regular}.}
$$

For a nonregular $\mu$, equality is impossible because $D^\mu=0$.

Over $\mathbb Q$, [Young's rule](../../../../../young-s-rule.md) gives the exact decomposition

$$
M^\mu\cong\bigoplus_{\lambda\vdash n}(S^\lambda)^{\oplus K_{\lambda\mu}}.
$$

The [Kostka number](../../../../../kostka-number.md) $K_{\lambda\mu}$ counts [Semistandard Young tableaux](../../../../../semistandard-young-tableau.md) of shape $\lambda$ and content $\mu$: entry $i$ occurs $\mu_i$ times, rows weakly increase, and columns strictly increase. In particular $K_{\mu\mu}=1$ and nonzero multiplicity requires dominance.

For the requested induction, products mean induction of the [external tensor product of group representations](../../../../../external-tensor-product-of-group-representations.md) from $S_5\times S_2$ to $S_7$: on $V\boxtimes W$, the pair $(g,h)$ acts as $v\otimes w\mapsto gv\otimes hw$. One can compute using [Young's rule](../../../../../young-s-rule.md) alone. The two-row [permutation](../../../../../permutation.md) decompositions give

$$
[S^{(3,2)}]=[M^{(3,2)}]-[M^{(4,1)}],
$$

where subtraction is in the [ordinary character](../../../../../ordinary-character.md) group. Reordering row blocks gives isomorphic [permutation modules](../../../../../permutation-module.md). Inducing after multiplication by the trivial $S^{(2)}$ gives $[M^{(3,2,2)}]-[M^{(4,2,1)}]$. For a direct [Kostka number](../../../../../kostka-number.md) calculation, the differences $K_{\nu,(3,2,2)}-K_{\nu,(4,2,1)}$ are one for

$$
\nu=(5,2),(4,3),(4,2,1),(3,3,1),(3,2,2)
$$

and zero for every other [partition of an integer](../../../../../partition-of-an-integer.md) of seven. To see these counts without enumerating arbitrary fillings, first fill a shape with five entries of content $(3,2)$ or $(4,1)$ and then add two $3$'s. The added cells must be a [horizontal strip](../../../../../horizontal-strip.md). Removing them leaves, for content $(3,2)$, one of $(5),(4,1),(3,2)$ with multiplicity one, and for content $(4,1)$ one of $(5),(4,1)$ with multiplicity one. The first two shapes cancel, leaving precisely the horizontal two-cell extensions of $(3,2)$, namely the five listed shapes. Consequently

$$
\boxed{\operatorname{Ind}_{S_5\times S_2}^{S_7}
(S^{(3,2)}\boxtimes S^{(2)})
\cong S^{(5,2)}\oplus S^{(4,3)}\oplus S^{(4,2,1)}\oplus S^{(3,3,1)}\oplus S^{(3,2,2)}.}
$$

The [hook-length formula](../../../../../hook-length-formula.md) checks the [dimensions](../../../../../dimension-vector-space.md): $14+14+35+21+21=105=\binom75\cdot5$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
