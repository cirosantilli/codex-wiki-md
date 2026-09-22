<h1 id="6/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The [LOD score](../../../../../../lod-score.md) is the base-ten log [likelihood](../../../../../../likelihood-function.md) ratio against independent assortment. For the two families,

$$
\boxed{Z_{\max}=\log_{10}\frac{L_1(\widehat\theta)L_2(\widehat\theta)}{L_1(1/2)L_2(1/2)},\qquad0\leq\widehat\theta\leq\tfrac12.}
$$

For a known-phase first family this becomes

$$
Z_{\max}=r_1\log_{10}(2\widehat\theta)
+(m_1-r_1)\log_{10}(2(1-\widehat\theta))
+\log_{10}\frac{L_2(\widehat\theta)}{L_2(1/2)},
$$

with endpoint terms interpreted by limits, such as $0\log0=0$ when the corresponding count is zero. Positive values favour [genetic linkage](../../../../../../genetic-linkage.md), and the [likelihood](../../../../../../likelihood-function.md) ratio is $10^{Z_{\max}}$. A conventional large positive threshold such as 3 represents a [likelihood](../../../../../../likelihood-function.md) ratio of 1000, not automatically a posterior [probability](../../../../../../probability.md) or a universal 5% test.

For a test calibrated to this study, use the distribution of the maximized statistic under $\theta=1/2$, for example by simulating transmissions conditional on the same parental [genotype](../../../../../../genotype.md) and ascertainment scheme. Reject for sufficiently large values with the chosen significance threshold; phase uncertainty and the boundary null prevent assuming an unqualified ordinary interior Wilks reference. The missing pedigrees prevent the numerical value or their explicit [likelihood](../../../../../../likelihood-function.md) polynomial from being supplied, but the likelihood-ratio definition and testing procedure apply once those data are recovered.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
