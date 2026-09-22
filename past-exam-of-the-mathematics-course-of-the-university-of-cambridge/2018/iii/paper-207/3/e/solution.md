<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the electronic-record [observational study](../../../../../../observational-study.md), three strengths are:

- The large dataset improves precision of the estimated [statistical association](../../../../../../statistical-association.md) and allows detection of associations too small for a modest study.
- Adjusting for age, sex, and ancestry addresses specified measured sources of [confounding](../../../../../../confounding.md).
- Routinely collected [hypercalcaemia](../../../../../../hypercalcaemia.md) and [migraine](../../../../../../migraine.md) diagnoses give evidence from clinical practice, rather than depending solely on recalled [calcium intake](../../../../../../calcium-intake.md).

Three weaknesses are:

- Residual [confounding](../../../../../../confounding.md) remains possible: for example, other diseases, medicines, or health behaviours may affect both [serum calcium](../../../../../../serum-calcium.md) and [migraine](../../../../../../migraine.md).
- Co-occurrence does not establish temporal order, leaving [reverse causality](../../../../../../reverse-causality.md) possible. [Migraine](../../../../../../migraine.md), its management, or the decision to investigate it may alter recorded [serum calcium](../../../../../../serum-calcium.md).
- [Selection bias](../../../../../../selection-bias.md) and diagnostic misclassification can arise because patients enter health records and receive testing nonrandomly. Moreover, [hypercalcaemia](../../../../../../hypercalcaemia.md) is not a direct measure of dietary [calcium intake](../../../../../../calcium-intake.md), limiting the claimed intervention's interpretation.

For [two-sample Mendelian randomization](../../../../../../two-sample-mendelian-randomization.md), three strengths are:

- [Genetic variants](../../../../../../genetic-variant.md) are inherited before adult [migraine](../../../../../../migraine.md) develops, making ordinary disease-to-genotype [reverse causality](../../../../../../reverse-causality.md) implausible.
- Under [instrumental-variable independence](../../../../../../instrumental-variable-independence.md), genetic assignment reduces the environmental [confounding](../../../../../../confounding.md) that undermines a conventional [observational study](../../../../../../observational-study.md).
- The large outcome sample and combined [genetic risk score](../../../../../../genetic-risk-score.md) improve precision, while concordant [weighted-median Mendelian randomization estimator](../../../../../../weighted-median-mendelian-randomization-estimator.md) and [MR-Egger regression](../../../../../../mr-egger-regression.md) results offer checks under different assumptions about [horizontal pleiotropy](../../../../../../horizontal-pleiotropy.md).

Three weaknesses are:

- [Horizontal pleiotropy](../../../../../../horizontal-pleiotropy.md) can violate the [exclusion restriction](../../../../../../exclusion-restriction.md), while [population stratification](../../../../../../population-stratification.md) or inherited family effects can violate [instrumental-variable independence](../../../../../../instrumental-variable-independence.md). In the supplied figure, one variant has a much larger [serum calcium](../../../../../../serum-calcium.md) association than the others, motivating a check for dependence on that single variant.
- The score explains only 1.25% of [serum calcium](../../../../../../serum-calcium.md) [variance](../../../../../../variance-split.md), so instrument strength must be assessed rather than assumed. Different populations in the two samples can also undermine transport of genetic associations. A small variance fraction is not itself proof of a [weak instrument](../../../../../../weak-instrument.md) in a large sample.
- A lifelong genetically influenced shift in [serum calcium](../../../../../../serum-calcium.md) is not equivalent to changing dietary [calcium intake](../../../../../../calcium-intake.md). The robustness methods also need assumptions: the [weighted-median Mendelian randomization estimator](../../../../../../weighted-median-mendelian-randomization-estimator.md) needs more than half of the weight from valid instruments, and [MR-Egger regression](../../../../../../mr-egger-regression.md) needs the [InSIDE assumption](../../../../../../inside-assumption.md). The nonsignificant [MR-Egger regression](../../../../../../mr-egger-regression.md) intercept is compatible with zero average directional [horizontal pleiotropy](../../../../../../horizontal-pleiotropy.md), but with eight variants it cannot prove all instruments valid.

Thus **the agreement supports the hypothesis, but does not establish the effect of a dietary intervention**.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
