<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [frailty model](../../../../../frailty-model.md) represents unobserved individual heterogeneity by a [random effect](../../../../../random-effect.md) in the [hazard function](../../../../../hazard-function.md). In a [proportional frailty model](../../../../../proportional-frailty-model.md), an individual with [frailty random variable](../../../../../frailty-random-variable.md) $U=u$ has hazard $u h_0(t)$. The normalization $\mathbb E U=1$ identifies the scale of the [baseline hazard](../../../../../baseline-hazard.md): without it, multiplying all frailties by a constant and dividing $h_0$ by that constant would leave all individual hazards unchanged.

Let $H_0(t)=\int_0^t h_0(v)\,dv$. Conditional survival follows by integrating the [hazard function](../../../../../hazard-function.md):

$$
S(t\mid U=u)=\exp\left(-\int_0^tu h_0(v)\,dv\right)=e^{-uH_0(t)}.
$$

Taking the [expectation](../../../../../expected-value.md) over the frailty law yields

$$
\boxed{S(t)=\int_0^\infty e^{-uH_0(t)}g(u)\,du
=\widetilde g\big(H_0(t)\big),\qquad
\widetilde g(s)=\int_0^\infty e^{-su}g(u)\,du.}
$$

This is the [Laplace transform](../../../../../laplace-transform.md) of the frailty density evaluated at the [cumulative hazard](../../../../../cumulative-hazard-function.md). More generally, the same calculation integrates against a [probability measure](../../../../../probability-measure.md), allowing atoms. It averages conditional survival rather than substituting $\mathbb E U$ into its exponent. Indeed, the [frailty distribution among survivors](../../../../../frailty-distribution-among-survivors.md) is proportional to $e^{-uH_0(t)}g(u)$, giving population hazard

$$
h_{\rm pop}(t)=h_0(t)\frac{\mathbb E[Ue^{-UH_0(t)}]}{\mathbb E[e^{-UH_0(t)}]}.
$$

Survival progressively selects smaller frailties, so the population hazard need not be the baseline or even retain the individual's proportional structure.

For the [cure model](../../../../../cure-model.md), first take $0\leq\pi<1$. The necessary mean-one frailty law and [baseline hazard](../../../../../baseline-hazard.md) are

$$
\boxed{\Pr(U=0)=\pi,\qquad
\Pr\left(U=\frac1{1-\pi}\right)=1-\pi,
\qquad h_0(t)=(1-\pi)h_*(t).}
$$

Then $\mathbb E U=\pi\cdot0+(1-\pi)/(1-\pi)=1$. A cured person's conditional hazard is zero, while a susceptible person's conditional hazard is $h_0/(1-\pi)=h_*$. Taking $U$ to be zero or one while leaving $h_0=h_*$ would instead have mean frailty $1-\pi$ and violate the required normalization.

The frailty law is the measure

$$
g(du)=\pi\delta_0(du)+(1-\pi)\delta_{1/(1-\pi)}(du),
$$

where the $\delta$ terms are [Dirac measures](../../../../../dirac-measure.md). This is not an ordinary Lebesgue density; the cure construction requires permitting a discrete frailty law. Its [Laplace transform](../../../../../laplace-transform.md) is

$$
\widetilde g(s)=\pi+(1-\pi)e^{-s/(1-\pi)}.
$$

Writing $H_*(t)=\int_0^t h_*(v)\,dv$, we have $H_0=(1-\pi)H_*$, and therefore

$$
\boxed{S(t)=\widetilde g(H_0(t))=\pi+(1-\pi)e^{-H_*(t)}.}
$$

If $H_*(t)\to\infty$, the susceptible class eventually experiences the event and $S(t)\to\pi$. If $H_*(\infty)<\infty$, the limiting survival is larger than $\pi$ because some susceptible subjects also never experience the event. At $\pi=1$, everyone is cured: set $h_0\equiv0$ and, for example, $U\equiv1$ to retain mean one, giving $S\equiv1$ without using the singular formula $1/(1-\pi)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
