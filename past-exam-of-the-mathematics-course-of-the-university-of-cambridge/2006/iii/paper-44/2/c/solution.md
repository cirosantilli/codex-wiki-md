<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Quarantine](../../../../../../quarantine.md) restricts contacts of exposed people whose infection status is uncertain and monitors them for illness, reducing opportunities for transmission before infection is recognized. Recognized cases are managed by [isolation](../../../../../../isolation-health-care.md) rather than treated as merely uncertain exposures. Duration must be measured from the last possible infection-producing exposure, or otherwise account for uncertainty in exposure time. The mathematical calculations below concern the [incubation period](../../../../../../incubation-period.md) among infected people who develop symptoms, not a complete infectiousness model.

With a credible hard endpoint $M$, the [truncated distribution](../../../../../../truncated-distribution.md) has

$$
F_M(t)=\frac{G(t)}{G(M)}\quad(0<t<M),
\qquad F_M(t)=1\quad(t\geq M).
$$

A duration $q\geq M$ then covers all symptom-onset times under that model, provided the exposure time is correctly specified. If a nonzero late-onset probability $\varepsilon$ is accepted, solve

$$
\boxed{q=G^{-1}\big((1-\varepsilon)G(M)\big),\qquad
\Pr(T>q\mid T<M)=\varepsilon.}
$$

The calculation is appropriate when external biological evidence genuinely supports a hard maximum, or when a deliberately bounded model is justified for the population being considered. Truncation caused by a study's ascertainment window instead requires an observation correction: it does not prove that the disease has a hard biological endpoint. Nor does $\widehat M=t_{(n)}$ guarantee that future cases will develop symptoms by the current sample maximum. Endpoint and nuisance-parameter uncertainty need to enter a conservative duration calculation.

For an untruncated [gamma distribution](../../../../../../gamma-distribution.md), [lognormal distribution](../../../../../../log-normal-distribution.md) or other model with an unbounded upper tail, no finite duration eliminates the modeled late-onset probability. Choose a tail tolerance and solve

$$
\boxed{q=F^{-1}(1-\varepsilon),\qquad \Pr(T>q)=\varepsilon.}
$$

This is appropriate when a hard endpoint is unsupported and rare long incubation times remain possible. One can estimate a high [quantile](../../../../../../quantile-function.md), assess its uncertainty and balance the modeled residual probability against the costs of longer restrictions. Different tail families can give very different high [quantiles](../../../../../../quantile-function.md) even when they fit the central observations similarly, which makes the model dependence seen in part b operationally relevant.

If an individual has already remained symptom-free for $a$ time units after a known exposure, a conditional additional duration $b$ instead uses $S(a+b)/S(a)\leq\varepsilon$, where $S$ is the relevant [survivor function](../../../../../../survival-function.md) and $S(a)>0$. This conditions on being an infected eventual symptomatic case. Incubation data alone do not describe asymptomatic infection, the timing of infectiousness or compliance with restrictions; symptom surveillance, testing where informative and a transmission model may therefore be needed to translate late onset into an actual release-risk calculation. **Use a hard bound only when it is supported; otherwise quantify and allow for the upper-tail uncertainty.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
