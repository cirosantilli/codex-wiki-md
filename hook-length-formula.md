# Hook-length formula

↑ **Parent:** [Specht module](specht-module.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hook-length_formula)

For any [partition of an integer](partition-of-an-integer.md) $\lambda\vdash n$, the number $f^\lambda$ of [standard Young tableaux](standard-young-tableau.md) of shape $\lambda$ is

$$
f^\lambda=|\operatorname{SYT}(\lambda)|
=\frac{n!}{\displaystyle\prod_{(i,j)\in Y(\lambda)}h_{i,j}(\lambda)}.
$$

The numerator is a [factorial](factorial.md), and the denominator is the [hook product of a partition](hook-product-of-a-partition.md), using every cell's [hook length](hook-length.md) once. The empty shape has one empty [standard Young tableau](standard-young-tableau.md), and the formula still holds with $0!=1$ and an empty product equal to one. By the [standard polytabloid basis](standard-polytabloid-basis.md), $f^\lambda$ is also the [dimension](dimension-vector-space.md) of the [Specht module](specht-module.md) $S^\lambda$ over the [complex numbers](complex-number.md), or equivalently the degree $\chi^\lambda(1)$ of its [irreducible character](irreducible-character.md). For a teaching derivation of this [dimension](dimension-vector-space.md) formula, see [Etingof et al., Introduction to Representation Theory, §5.17, Theorem 5.17.1](https://math.mit.edu/~etingof/representationtheorybook.pdf).

In the [Young diagram](young-diagram.md) of $(3,2)$, the [hook length](hook-length.md) array $[[4,3,1],[2,1]]$ gives

$$
H_{(3,2)}=4\cdot3\cdot1\cdot2\cdot1=24,\qquad
f^{(3,2)}=\frac{5!}{24}=\frac{120}{24}=5
=\dim_{\mathbb C}S^{(3,2)}.
$$

This agrees with the five explicit fillings in [standard Young tableau](standard-young-tableau.md). Its [conjugate partition](conjugate-partition.md) $(2,2,1)$ has the same [hook lengths](hook-length.md) after transposition, hence also gives [dimension](dimension-vector-space.md) five. At the extremes, for $n\geq1$, a single row $(n)$ and a single column $(1^n)$ each have [hook product](hook-product-of-a-partition.md) $n!$ and exactly one [standard Young tableau](standard-young-tableau.md); their [Specht modules](specht-module.md) over the [complex numbers](complex-number.md) are the [trivial representation](trivial-representation.md) and [sign representation](sign-representation.md), respectively.

Why the formula is beautiful: global compatibility of all the row and column inequalities reduces to a product of local [hook lengths](hook-length.md). It is useful when enumeration is already expensive: computing one [hook length](hook-length.md) per cell replaces testing up to $n!$ numbered [Young tableaux](young-tableau.md). For $(3,2)$, the proportion of the $120$ bijective fillings that are [standard Young tableaux](standard-young-tableau.md) is $5/120=1/24$, the reciprocal of the [hook product](hook-product-of-a-partition.md). This product does not justify treating overlapping hook conditions as independent; Grinberg explains that tempting but invalid argument in [§1.3 of his teaching slides](https://www.cip.ifi.lmu.de/~grinberg/t/24s/hooktalk.pdf).

Historically, the modern hook-product statement was published by J. S. Frame, G. de B. Robinson and R. M. Thrall in 1954: [The Hook Graphs of the Symmetric Group, Canadian Journal of Mathematics 6, 316–324, Theorem 1](https://doi.org/10.4153/CJM-1954-030-1). Their manuscript was received on 1 September 1953, and their proof reorganizes an earlier [irreducible character](irreducible-character.md) degree formula into the product of the [hook lengths](hook-length.md). The theorem unifies the counting and [representation](group-representation.md) viewpoints developed earlier by Young. For proof routes within this wiki, see [trace computation of Specht module dimension](trace-computation-of-specht-module-dimension.md), [determinant formula for Specht module dimension](determinant-formula-for-specht-module-dimension.md), and [Greene–Nijenhuis–Wilf hook walk](greene-nijenhuis-wilf-hook-walk.md).

**Table of contents**

- [Least non-linear ordinary degree of a symmetric group](least-non-linear-ordinary-degree-of-a-symmetric-group.md)
- [Trace computation of Specht module dimension](trace-computation-of-specht-module-dimension.md)
- [Determinant formula for Specht module dimension](determinant-formula-for-specht-module-dimension.md)
- [Greene–Nijenhuis–Wilf hook walk](greene-nijenhuis-wilf-hook-walk.md)
  - [Hook walk terminal probability](hook-walk-terminal-probability.md)

## ↑ Ancestors (11)

1. [Specht module](specht-module.md)
2. [Polytabloid](polytabloid.md)
3. [Tabloid](tabloid.md)
4. [Young tableau](young-tableau.md)
5. [Partition of an integer](partition-of-an-integer.md)
6. [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group-split.md)
7. [Representation theory](representation-theory-split.md)
8. [Algebra](algebra-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Beta-set hook-product identity](beta-set-hook-product-identity.md)
- [Conjugate partition](conjugate-partition.md)
- [Determinant formula for Specht module dimension](determinant-formula-for-specht-module-dimension.md)
- [Greene–Nijenhuis–Wilf hook walk](greene-nijenhuis-wilf-hook-walk.md)
- [Hook graph of a partition](hook-graph-of-a-partition.md)
- [Hook length](hook-length.md)
- [Hook of a Young diagram](hook-of-a-young-diagram.md)
- [Hook product of a partition](hook-product-of-a-partition.md)
- [Least non-linear ordinary degree of a symmetric group](least-non-linear-ordinary-degree-of-a-symmetric-group.md)
- [P-adic valuation of a symmetric-group character degree from the core tower](p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-3/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-3/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-3/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-3/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-5/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-103/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-103/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-103/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-160/1/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-160/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-160/2/b/solution.md)
- [Smallest non-linear ordinary degree of an alternating group](smallest-non-linear-ordinary-degree-of-an-alternating-group.md)
- [Standard Young tableau](standard-young-tableau.md)
- [Symmetric-group character co-degree vanishing criterion](symmetric-group-character-co-degree-vanishing-criterion.md)
- [Vandermonde shift identity](vandermonde-shift-identity.md)
- [Young tableau](young-tableau.md)
