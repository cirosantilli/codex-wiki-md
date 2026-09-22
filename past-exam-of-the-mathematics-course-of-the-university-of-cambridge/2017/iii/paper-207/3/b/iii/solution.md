<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Visits can be missed or rescheduled because of illness, clinic availability or patient choice; follow-up may end through dropout or [right censoring](../../../../../../../right-censoring.md). The correct [panel-observed multi-state likelihood](../../../../../../../panel-observed-multi-state-likelihood.md) uses each observed interval length $\Delta_{ik}$:

$$
\boxed{\ell(\lambda,\mu)=\sum_{i,k}\log p_{x_{ik},x_{i,k+1}}(\Delta_{ik};\lambda,\mu).}
$$

Thus the four aggregated one-year counts are generally no longer sufficient; records must retain actual durations. Numerical [maximum likelihood estimation](../../../../../../../maximum-likelihood-estimation.md) uses the corresponding [transition probabilities](../../../../../../../transition-probability.md), or a [matrix exponential](../../../../../../../matrix-exponential.md) of the generator when a larger model is fitted. One must not treat a two-year interval as a single one-year transition or as two known transitions through an unobserved intermediate state.

This conditional calculation is valid when visit scheduling and loss to follow-up are ignorable given the modeled information. If symptomatic patients are systematically examined earlier or leave the study differently, observation itself may be informative; the visit or dropout process may require a joint [statistical model](../../../../../../../statistical-model-split.md). Simply replacing one year by the actual interval does not correct informative observation.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
