<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [generating function](../../../../../../generating-function.md) for [integer partitions](../../../../../../integer-partition.md) is $\sum_\lambda u^{|\lambda|}=\prod_{i\ge1}(1-u^i)^{-1}$, since independently choosing the multiplicity of each part size gives a [geometric series](../../../../../../geometric-series.md). Applying the parameterization in 5(a),

$$
\sum_{n\ge0}k_n(q)t^n=\prod_{f\ne t}\prod_{i\ge1}(1-t^{i\deg(f)})^{-1}.
$$

Unique factorization of [monic polynomials](../../../../../../monic-polynomial.md) shows

$$
\prod_{f\ne t}(1-u^{\deg(f)})^{-1}
=1+\sum_{r\ge1}(q-1)q^{r-1}u^r
=\frac{1-u}{1-qu}.
$$

Indeed the left side counts [monic polynomials](../../../../../../monic-polynomial.md) with nonzero constant term; in degree $r\ge1$ there are $(q-1)q^{r-1}$ choices. Reordering the formal products is legitimate because only finitely many factors contribute to any fixed coefficient. Substituting $u=t^i$ for each $i$ gives the [conjugacy-class generating function for finite general linear groups](../../../../../../conjugacy-class-generating-function-for-finite-general-linear-groups.md):

$$
\boxed{k_n(q)=[t^n]\prod_{i\ge1}\frac{1-t^i}{1-qt^i}.}
$$

The constant term corresponds to the trivial zero-dimensional [group](../../../../../../group-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
