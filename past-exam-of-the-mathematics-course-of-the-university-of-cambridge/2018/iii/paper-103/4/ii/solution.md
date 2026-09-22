<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We use the [core-quotient bijection for partitions](../../../../../../core-quotient-bijection-for-partitions.md): an ordered $p$-tuple $(\nu_0,\ldots,\nu_{p-1})$ and a fixed $p$-core determine a unique [partition of an integer](../../../../../../partition-of-an-integer.md), with

$$
|\lambda|=|C_p(\lambda)|+p\sum_i|\nu_i|.
$$

The [irreducible characters](../../../../../../irreducible-character.md) in both $B$ and $C$ therefore correspond to the same ordered tuples of total size $w$. Replacing the empty [core of a partition](../../../../../../core-of-a-partition.md) by $\gamma$ while keeping the [quotient of a partition](../../../../../../quotient-of-a-partition.md) fixed gives a [bijection](../../../../../../bijection.md) $\chi^\lambda\mapsto\chi^\mu$ from $B$ to $C$. In particular $|B|=|C|$.

For such a pair, all levels of the [core tower of a partition](../../../../../../core-tower-of-a-partition.md) above level zero agree. At level zero, their sizes are $0$ and $m$, respectively. Put $D=\sum_{r\geq1}|T^C(\lambda)_r|=\sum_{r\geq1}|T^C(\mu)_r|$. When $0\leq m<p$, the [base-p digit sum](../../../../../../base-p-digit-sum.md) satisfies

$$
d_p(wp)=d_p(w),\qquad d_p(wp+m)=d_p(w)+m.
$$

The [P-adic valuation of a symmetric-group character degree from the core tower](../../../../../../p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower.md) then gives

$$
\nu_p(\chi^\lambda(1))=\frac{D-d_p(w)}{p-1}
=\frac{m+D-[d_p(w)+m]}{p-1}
=\nu_p(\chi^\mu(1)).
$$

Thus the same bijection preserves degree coprimality to $p$ and restricts to a bijection between the indicated sets of [irreducible characters of degree coprime to p](../../../../../../irreducible-characters-of-degree-coprime-to-p.md). Consequently

$$
\boxed{|B|=|C|,\qquad
|B\cap\operatorname{Irr}_{p'}(S_{wp})|=|C\cap\operatorname{Irr}_{p'}(S_n)|.}
$$

For $m=0$, take $\gamma$ to be the empty partition; the construction becomes the identity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
