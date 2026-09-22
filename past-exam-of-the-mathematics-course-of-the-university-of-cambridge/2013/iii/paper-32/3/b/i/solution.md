<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Conditioning on continuation selects the upper part of the stage-1 [estimator](../../../../../../../estimator.md)'s distribution, since $C=\{\widehat\delta_1\geq f_1/\sqrt{I_1}\}$. Thus $\mathbb E_\delta(\widehat\delta_1\mid C)>\delta$ for every finite threshold. The fresh stage-2 estimate $\widehat\delta_2^*$ is independent of $C$ and remains unbiased for $\delta$. The pooled [estimator](../../../../../../../estimator.md) retains a positive weight on the selected stage-1 data, giving

$$
\mathbb E_\delta(\widehat\delta_2\mid C)-\delta
=\frac{n_1}{n_2}\left[\mathbb E_\delta(\widehat\delta_1\mid C)-\delta\right]>0.
$$

**Conditional on full enrollment, the ordinary pooled [MLE](../../../../../../../maximum-likelihood-estimator.md) overestimates the treatment effect.** This is [conditional selection bias after futility continuation](../../../../../../../conditional-selection-bias-after-futility-continuation.md). Randomization of treatment assignments does not undo selection on the interim outcome.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
