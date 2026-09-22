<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The last lung-cancer failure before five years is at 4.85, where the displayed [net survival](../../../../../../../net-survival.md) estimate is 0.392. The other-death [net survival](../../../../../../../net-survival.md) estimate remains 0.498 from 4.096 until 5.065. Thus the two supplied curves imply **net five-year death estimates of $1-0.392=0.608$ for lung cancer and $1-0.498=0.502$ for other causes**. Their sum is 1.110, already showing that they cannot be probabilities of two disjoint actual causes of death.

In [competing risks](../../../../../../../competing-risks.md), let $\lambda_1(t)$ and $\lambda_2(t)$ be the [cause-specific hazards](../../../../../../../cause-specific-hazard.md) while alive, with [cumulative hazards](../../../../../../../cumulative-hazard-function.md) $\Lambda_k(t)=\int_0^t\lambda_k(u)\,du$. Treating the other cause as censored estimates the [net survival](../../../../../../../net-survival.md) $S_k^{\rm net}(t)=e^{-\Lambda_k(t)}$. The actual probability of death from cause $k$ by time $t$ is the [cumulative incidence function](../../../../../../../cumulative-incidence-function.md)

$$
\boxed{F_k(t)=\int_0^t S(u)\lambda_k(u)\,du,\qquad
S(u)=e^{-\Lambda_1(u)-\Lambda_2(u)}.}
$$

Since $S(u)\le e^{-\Lambda_k(u)}$, the net probability $1-S_k^{\rm net}(t)$ generally overstates the [cumulative incidence function](../../../../../../../cumulative-incidence-function.md): death from the other cause prevents a later death of cause $k$. This discrepancy exists even for independent latent cause-specific failure times. Moreover, Kaplan–Meier estimates are not generally exactly unbiased in finite samples even for their proper target. **The plotted complements are not unbiased estimators of $\mathbb P(T\le5,D=k)$, and are not even consistent for that target in general.**

For the desired probabilities, use the [Aalen–Johansen estimator](../../../../../../../aalen-johansen-estimator.md) $\widehat F_k(t)=\sum_{u\le t}\widehat S(u-)d_k(u)/n(u)$, with all-cause survival $\widehat S(u)=\prod_{v\le u}[1-(d_1(v)+d_2(v))/n(v)]$ and independent study censoring. Removing competing deaths from subsequent [risk sets](../../../../../../../risk-set.md) is correct for estimating [cause-specific hazards](../../../../../../../cause-specific-hazard.md); the error is interpreting the separate [net survival](../../../../../../../net-survival.md) complements as [cumulative incidence functions](../../../../../../../cumulative-incidence-function.md). A hypothetical elimination-of-a-cause interpretation of [net survival](../../../../../../../net-survival.md) would require additional causal assumptions.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
