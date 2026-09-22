<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A case chromosome is transmitted and a pseudo-control chromosome is untransmitted. Summing the paired table by columns for cases and by rows for controls gives

$$
\begin{array}{c|rr}
\text{Allele}&\text{Case}&\text{Pseudo-control}\\\hline
1&27&33\\
2&73&67\\\hline
\text{Total}&100&100
\end{array}.
$$

For the ordinary unpaired [chi-squared test](../../../../../../chi-squared-test.md) of independence, the expected cells are 30,30,70,70. Its uncorrected Pearson statistic is

$$
\boxed{X^2=\frac{(27-30)^2}{30}+\frac{(33-30)^2}{30}
+\frac{(73-70)^2}{70}+\frac{(67-70)^2}{70}
=\frac67\approx0.8571.}
$$

For the paired [McNemar's test](../../../../../../mcnemar-s-test.md), only the discordant transmissions matter, with counts 24 and 18. Thus

$$
\boxed{X^2_{\mathrm{McN}}=\frac{(24-18)^2}{24+18}=\frac67\approx0.8571.}
$$

Both uncorrected statistics happen to coincide and have the same approximate one-degree-of-freedom [chi-squared distribution](../../../../../../chi-squared-distribution.md) reference, giving $p\approx0.355$. The data do not show persuasive transmission imbalance at the conventional 5% level.

The equality is a numerical coincidence, not a justification for ignoring pairing. To see the [equality criterion for paired and unpaired allele tests](../../../../../../equality-criterion-for-paired-and-unpaired-allele-tests.md), write the original matched cells as $a,b,c,d$ and $n=a+b+c+d$. The unpaired marginal-table statistic is

$$
\frac{2n(b-c)^2}{(2a+b+c)(2d+b+c)},
$$

whereas McNemar's is $(b-c)^2/(b+c)$. Here $n=100$, $b+c=42$, and $(2a+b+c)(2d+b+c)=60\times140=2n(b+c)$, giving equality. Changing concordant counts can change the unpaired statistic without changing McNemar's. The [transmission disequilibrium test](../../../../../../transmission-disequilibrium-test.md) should retain its conditional paired interpretation.

If a continuity correction is used, state it explicitly: McNemar's corrected statistic is $(|24-18|-1)^2/42=25/42\approx0.5952$; the corresponding Yates-corrected marginal statistic also coincides here. An exact conditional test uses $\operatorname{Binomial}(42,1/2)$ and gives the two-sided [probability](../../../../../../probability.md) $2\mathbb P(K\leq18)\approx0.4408$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
