<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First investigate what predicts dropout among variables actually observed, record reasons where possible, and seek additional outcome follow-up. Dependence on observed history alone can be [missing at random](../../../../../../missing-at-random.md); informative dependence on unseen responses or latent heterogeneity requires a [missing not at random](../../../../../../missing-not-at-random.md) analysis. Observed data do not ordinarily distinguish MAR from all MNAR explanations.

An explicit [selection model for informative longitudinal dropout](../../../../../../selection-model-for-informative-longitudinal-dropout.md) can augment a joint response model $f_\vartheta(Y_i\mid z_i,x_i)$ by dropout hazards. Define $R_{ij}$ as above and, among subjects retained through visit $j-1$, put

$$
h_{ij}(Y_i)=P(R_{ij}=0\mid R_{i,j-1}=1,Y_i,z_i,x_i),\qquad \operatorname{logit}h_{ij}=a_j+c^Tx_i+d z_i+\lambda Y_{i,j-1}+\kappa Y_{ij}.
$$

Omit the previous-response term at the first visit. A nonzero $\kappa$ makes dropout depend on the currently missing response. For monotone observation indicators $r_i$, let

$$
g_\eta(r_i\mid Y_i,z_i,x_i)=\prod_{j:r_{i,j-1}=1}h_{ij}(Y_i)^{1-r_{ij}}[1-h_{ij}(Y_i)]^{r_{ij}}.
$$

The appropriate [observed-data likelihood](../../../../../../observed-data-likelihood.md) is

$$
L(\vartheta,\eta)=\prod_i\sum_{Y_i^{\mathrm{mis}}\in\{0,1\}^{|\mathcal O_i^c|}} f_\vartheta(Y_i^{\mathrm{obs}},Y_i^{\mathrm{mis}}\mid z_i,x_i)\,g_\eta(r_i\mid Y_i,z_i,x_i).
$$

Thus a patient's dropout pattern contributes information in the model; dropping the $g_\eta$ factor is not justified under this informative mechanism.

Another option is a [shared-parameter model for informative dropout](../../../../../../shared-parameter-model-for-informative-dropout.md): retain the conditional Bernoulli response model, but let the dropout [logit](../../../../../../logit.md) contain the same latent effect, for example $a_j+c^Tx_i+d z_i+\lambda Y_{i,j-1}+\kappa_B B_i$. Conditional on the shared effect and observed history the processes can be independent, while marginally dropout remains associated with unseen responses. The joint [likelihood](../../../../../../likelihood-function.md) must integrate the response factors and dropout factors together over $B_i$. A response-only mixed-model fit does not generally account for this dependence.

Because $\kappa$ or $\kappa_B$ can be weakly identified from the observed outcomes, **report sensitivity of the treatment conclusion to plausible informative-dropout assumptions**. One can fix a range of these dependence parameters and refit, or use [pattern-mixture sensitivity analysis](../../../../../../pattern-mixture-sensitivity-analysis.md) that shifts the imputed post-dropout [log odds](../../../../../../log-odds.md) by a specified amount from the MAR prediction. Present population risks and treatment contrasts across these scenarios with their uncertainty. These are explicit identifying assumptions, not an empirical test proving which missingness mechanism is true. Neither a complete-case analysis nor carrying forward the last response supplies such a justification.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
