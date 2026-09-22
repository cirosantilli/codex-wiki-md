<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The episodes from one patient share treatment, biological susceptibility and prior history, so they are not independent observations. Treating every row as an unrelated subject can substantially understate uncertainty. Two approaches address this [within-patient recurrent-event dependence](../../../../../within-patient-recurrent-event-dependence.md):

- A patient-clustered [sandwich covariance matrix](../../../../../sandwich-covariance-matrix.md) retains a suitable working Cox mean/intensity model but groups score contributions by patient. If $U_i$ is the patient's score contribution and $A$ the observed information, its form is $A^{-1}(\sum_iU_iU_i^{\mathsf T})A^{-1}$. Independent patients, rather than independent rows, determine the sampling units. This corrects uncertainty for within-patient dependence when the working estimating equation is appropriate; it does not repair an incorrect mean model.
- A [shared frailty model](../../../../../shared-frailty-model.md) introduces a common latent positive multiplier $V_i$ for all of patient $i$'s episode hazards, often with a specified gamma or lognormal distribution. Given frailty and the relevant history, the event mechanism is modeled through that patient's intensity. Estimate treatment and frailty parameters by integrating or profiling the latent effect. This models persistent heterogeneity directly, but relies on the frailty assumptions and generally gives a conditional treatment-effect interpretation.

A patient-level [bootstrap](../../../../../bootstrapping-statistics.md) is another way to retain dependence: resample complete histories, not individual episode rows. It is not necessary to assume that robust marginal/working and frailty-conditional effect estimates target exactly the same parameter.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
