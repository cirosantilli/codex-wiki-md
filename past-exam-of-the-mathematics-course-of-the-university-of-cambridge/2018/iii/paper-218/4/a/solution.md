<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T_i=1$ denote Progabide and $T_i=0$ placebo; write $a_i$ for age and $b_i$ for baseline count. The fitted [Poisson regression](../../../../../../poisson-regression.md) specifies independent

$$
Y_i\sim\operatorname{Poisson}(\mu_i),\qquad\eta_i=\log\mu_i=\beta_0+\beta_Aa_i+\beta_TT_i+\beta_Bb_i+\beta_{TB}T_ib_i.
$$

Its [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta)=\sum_{i=1}^{107}\{Y_i\eta_i-e^{\eta_i}-\log(Y_i!)\}.
$$

The coefficient table in the original PDF, whose TeX transcription is truncated, gives the [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md)

$$
\boxed{(\widehat\beta_0,\widehat\beta_A,\widehat\beta_T,\widehat\beta_B,\widehat\beta_{TB})=(1.1215275,0.0090311,-0.3592068,0.0186824,0.0008682).}
$$

For the [treatment interaction contrast in a Poisson regression](../../../../../../treatment-interaction-contrast-in-a-poisson-regression.md), the baseline slope of the log mean is $0.0186824$ on placebo and $0.0195506$ on Progabide. At fixed age and baseline $b$, the fitted drug-to-placebo mean ratio is $\exp(-0.3592068+0.0008682b)$. Increasing baseline by one multiplies that ratio by $e^{0.0008682}\approx1.0008686$. Thus the [interaction term](../../../../../../interaction-term.md) describes how the treatment ratio changes with baseline, rather than a uniform additive change in seizure counts. The displayed call makes clear that the source's `summary(model1)` line is an object-name typo for the epilepsy fit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
