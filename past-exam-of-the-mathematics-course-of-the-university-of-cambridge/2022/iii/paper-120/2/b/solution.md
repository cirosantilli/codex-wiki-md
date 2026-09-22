<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathcal U$ be a [nonprincipal ultrafilter](../../../../../../nonprincipal-ultrafilter.md) on an infinite set $I$. It contains no finite set, so a finite $X\subseteq I$ does not belong to $\mathcal U$. An [ultrafilter](../../../../../../ultrafilter.md) contains exactly one of a set and its complement; hence $I\setminus X\in\mathcal U$. Equivalently, every nonprincipal ultrafilter contains the [cofinite filter](../../../../../../cofinite-filter.md).

For structures $(M_i)_{i\in I}$ and a first-order formula $\varphi$, the [Łoś theorem](../../../../../../los-theorem.md) says

$$
\prod_{i\in I}M_i/\mathcal U\models\varphi([a_i^1],\ldots,[a_i^k])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(a_i^1,\ldots,a_i^k)\}\in\mathcal U.
$$

Fix a [prime number](../../../../../../prime-number.md) $p$, take $I=\mathbb N_{>0}$, and choose a nonprincipal ultrafilter on $I$. The [ultraproduct](../../../../../../ultraproduct.md)

$$
K=\prod_{n\geq1}\mathbb F_{p^n}/\mathcal U
$$

is a [field](../../../../../../field.md) because each factor is a [finite field](../../../../../../finite-field.md), and it has [characteristic](../../../../../../characteristic-of-a-field.md) $p$ because each factor satisfies $p\cdot1=0$ and $m\cdot1\ne0$ for $1\leq m<p$. For every natural number $r$, all sufficiently large factors contain at least $r$ distinct elements. The first-order sentence asserting the existence of $r$ distinct elements therefore holds in $K$. Thus $K$ is infinite, as summarized by [infinite field of positive characteristic from an ultraproduct](../../../../../../infinite-field-of-positive-characteristic-from-an-ultraproduct.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
