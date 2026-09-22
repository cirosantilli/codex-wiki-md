<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Each diploid individual contributes two marker [alleles](../../../../../../allele.md). Count $A$ copies as twice the $AA$ count plus the $Aa$ count, and count $a$ copies analogously. The observed chromosome-level [contingency table](../../../../../../contingency-table.md), followed by its null expected table, is

$$
\boxed{\begin{array}{c|rr}
O&\text{cases}&\text{controls}\\\hline
A&20&120\\a&180&80
\end{array}\qquad
\begin{array}{c|rr}
E&\text{cases}&\text{controls}\\\hline
A&70&70\\a&130&130
\end{array}.}
$$

There are 200 [chromosomes](../../../../../../chromosome.md) in each group; pooled totals are 140 $A$ and 260 $a$. The usual allelic [Pearson chi-squared test of independence](../../../../../../pearson-chi-squared-test-of-independence.md) gives

$$
X^2=2\left(\frac{50^2}{70}+\frac{50^2}{130}\right)=\frac{10000}{91}\simeq109.89.
$$

With the ordinary independent-chromosome null model, use one [degree of freedom](../../../../../../degree-of-freedom.md); its [p-value](../../../../../../p-value.md) is about $1.04\times10^{-25}$, providing very strong evidence of [genetic association](../../../../../../genetic-association.md).

The two [alleles](../../../../../../allele.md) from the same person are not automatically two independent observations. The usual one-degree-of-freedom calibration is justified, for example, for unrelated individuals with [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md) under the null. If that assumption is not suitable, retain individuals as the sampling units and test their allele dosages using an appropriate variance or permutation of case-control labels, or use the genotype-level test from part (iii). No [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md) assumption was needed for that genotype-level test.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
