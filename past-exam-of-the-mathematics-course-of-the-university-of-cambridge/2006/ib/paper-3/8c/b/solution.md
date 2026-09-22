<h1 id="8c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Pearson chi-squared test of homogeneity](../../../../../../pearson-chi-squared-test-of-homogeneity.md) for two multinomial samples. Under equal preference distributions, estimate the common probabilities from pooled counts, giving $(1/4,1/4,1/2)$. With row totals forty and sixty, the expected table is

$$
E=\begin{pmatrix}10&10&20\\15&15&30\end{pmatrix}.
$$

The [Pearson chi-squared statistic for contingency tables](../../../../../../pearson-chi-squared-statistic-for-contingency-tables.md) is

$$
\begin{aligned}
X^2&=\frac4{10}+\frac1{10}+\frac9{20}+\frac4{15}+\frac1{15}+\frac9{30}\\
&=\frac{19}{12}\simeq1.58333.
\end{aligned}
$$

There are $(2-1)(3-1)=2$ degrees of freedom, after fitting the common category probabilities. All expected counts exceed five. Thus

$$
\boxed{p=e^{-19/24}\simeq0.4531.}
$$

At five percent, **do not reject the common preference distribution**. These data are consistent with that hypothesis; failure to reject does not prove equality. This conclusion differs from part a because a common nonuniform distribution, especially an overall preference for chocolate, is allowed here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8C](../../8c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
