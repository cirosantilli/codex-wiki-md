<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [frailty model](../../../../../frailty-model.md) represents unobserved heterogeneity in susceptibility by a positive latent [frailty random variable](../../../../../frailty-random-variable.md) $U$. In the [proportional frailty model](../../../../../proportional-frailty-model.md), conditional on $U=u$, the individual hazard is $h(t\mid u)=u h_0(t)$, where $h_0$ is a baseline [hazard function](../../../../../hazard-function.md). If $H_0(t)=\int_0^t h_0(s)\,ds$, the conditional [survivor function](../../../../../survival-function.md) is

$$
S(t\mid u)=e^{-uH_0(t)}.
$$

Large frailty gives earlier events on average. Normalizing $\mathbb EU=1$ separates the frailty scale from that of the baseline hazard.

The unheaded final request follows for an arbitrary survival mixture, not only this proportional model. Let a randomly selected individual's type be $U$, with individual survivor function $S(t\mid U)$ and hazard $h(t\mid U)$. The population survivor function is $\overline S(t)=\mathbb E[S(t\mid U)]$. Where differentiation under the expectation is justified, $S'(t\mid U)=-h(t\mid U)S(t\mid U)$ gives

$$
\boxed{\overline h(t)=-\frac{\overline S'(t)}{\overline S(t)}
=\frac{\mathbb E[h(t\mid U)S(t\mid U)]}{\mathbb E[S(t\mid U)]}
=\mathbb E[h(t\mid U)\mid T>t].}
$$

This proves the [population hazard of a survival mixture](../../../../../population-hazard-of-a-survival-mixture.md) formula: the weights are the individual probabilities of still surviving, normalized to sum or integrate to one. For a finite equally weighted population it becomes $\sum_i h_i(t)S_i(t)/\sum_iS_i(t)$. Generally it is not the unweighted average of the original individual hazards. In a [proportional frailty model](../../../../../proportional-frailty-model.md), the [frailty distribution among survivors](../../../../../frailty-distribution-among-survivors.md) is proportional to $e^{-uH_0(t)}$ times the original frailty distribution.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
