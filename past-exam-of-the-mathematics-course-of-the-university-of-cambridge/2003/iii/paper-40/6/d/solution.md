<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the prespecified excess-sharing alternative: affected [full siblings](../../../../../../full-sibling.md) linked to a disease [genetic locus](../../../../../../genetic-locus.md) are expected to share more marker copies [identical by descent](../../../../../../identity-by-descent.md). The total sharing count is $0(42)+1(98)+2(60)=218$, so $\bar J=218/200=1.09$. Under the no-linkage null, independent sibling pairs have $E[J]=1$ and $\operatorname{Var}(J)=1/2$, giving the [mean allele-sharing test for affected siblings](../../../../../../mean-allele-sharing-test-for-affected-siblings.md)

$$
\boxed{Z=\frac{1.09-1}{\sqrt{(1/2)/200}}=1.8.}
$$

The upper 5% [standard normal](../../../../../../standard-normal-distribution.md) critical value is approximately $1.64$, so **there is evidence of excess sharing, and hence linkage, at the one-sided 5% level**. The [normal approximation](../../../../../../normal-approximation.md) gives upper-tail [p-value](../../../../../../p-value.md) $1-\Phi(1.8)\simeq0.0359$.

The conclusion depends on the intended directional test. A [two-sided test](../../../../../../two-sided-hypothesis-test.md) of the sharing mean uses $1.96$, so it would not reject at 5%. An omnibus [Pearson chi-squared goodness-of-fit test](../../../../../../pearson-chi-squared-goodness-of-fit-test.md) of the three counts against $(50,100,50)$ gives $64/50+4/100+100/50=3.32$ with two [degrees of freedom](../../../../../../degree-of-freedom.md) and also would not reject. The directional mean-sharing test targets the scientifically specified excess-sharing alternative; these different tests should not be selected after seeing which rejects. Independence of the 200 pairs is assumed: if pairs overlap within families, the [standard error](../../../../../../standard-error.md) needs adjustment.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
