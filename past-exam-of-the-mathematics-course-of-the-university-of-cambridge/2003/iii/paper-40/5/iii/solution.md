<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Arrange rows by marker [genotype](../../../../../../genotype.md), with cases and controls as the two columns. Both column totals are 100, and the three row totals are 100, 60 and 40. Under the null of no [genetic association](../../../../../../genetic-association.md), estimate each common row [probability](../../../../../../probability.md) from its pooled proportion. The expected count is row total times column total divided by the grand total. Thus the expected [contingency table](../../../../../../contingency-table.md) is

$$
\boxed{\begin{array}{c|rr}
&\text{cases}&\text{controls}\\\hline
aa&50&50\\Aa&30&30\\AA&20&20
\end{array}.}
$$

The [Pearson chi-squared test of independence](../../../../../../pearson-chi-squared-test-of-independence.md) uses

$$
X^2=\sum_{r,c}\frac{(O_{rc}-E_{rc})^2}{E_{rc}}=2\left(\frac{34^2}{50}+\frac{18^2}{30}+\frac{16^2}{20}\right)=93.44.
$$

Under independent sampled individuals and the no-association null, its reference [chi-squared distribution](../../../../../../chi-squared-distribution.md) has $(3-1)(2-1)=2$ [degrees of freedom](../../../../../../degree-of-freedom.md). All expected cells are well above five. **The null is overwhelmingly rejected**: the approximate [p-value](../../../../../../p-value.md) is $e^{-93.44/2}\simeq5.13\times10^{-21}$. This establishes association in the sampling model, not by itself a causal role for the marker.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
