<h1 id="s12/2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $S_1(t)$ be the probability that an ATP-waiting state has not yet bound a substrate molecule. A constant bimolecular binding coefficient $k_1$ at fixed [ATP](../../../../../adenosine-triphosphate.md) concentration $c$ gives a pseudo-first-order hazard $\lambda=k_1c$. Thus $\dot S_1=-\lambda S_1$, $S_1(0)=1$, and the [waiting-time distribution](../../../../../waiting-time-distribution.md) is

$$
\boxed{P_1(t)=-\dot S_1(t)=k_1c\,e^{-k_1ct},\quad t\ge0,\qquad \langle t_1\rangle=\frac1{k_1c}.}
$$

The [probability density function](../../../../../probability-density-function.md) starts at $k_1c$ and decreases exponentially. Increasing $c$ shortens the waiting time in inverse proportion. This supports one rate-limiting ATP-binding event before the associated motion, rather than a concentration-independent chemical delay.

For the second delay, consider sequential independent first-order transitions $A\mathrel{\mathop{\longrightarrow}^{k_a}}B\mathrel{\mathop{\longrightarrow}^{k_b}}C$. Their dwell times have [exponential distributions](../../../../../exponential-distribution.md). The total waiting time is their sum, so [convolution](../../../../../convolution.md) gives

$$
P_2(t)=\int_0^t k_ae^{-k_as}k_be^{-k_b(t-s)}\,ds
=\boxed{\frac{k_ak_b}{k_a-k_b}\left(e^{-k_bt}-e^{-k_at}\right),\quad t\ge0.}
$$

It is normalized, symmetric under exchange of $k_a,k_b$, and has

$$
\boxed{\langle t_2\rangle=\frac1{k_a}+\frac1{k_b},\qquad
\operatorname{Var}(t_2)=\frac1{k_a^2}+\frac1{k_b^2}.}
$$

Unlike one exponential delay, it vanishes at $t=0$, rises initially as $k_ak_bt$, reaches a maximum at $t_{\rm mode}=\log(k_a/k_b)/(k_a-k_b)$ and eventually decays at the slower rate. For equal rates the continuous limit is $P_2(t)=k^2t e^{-kt}$, an [Erlang distribution](../../../../../erlang-distribution.md) with mode $1/k$. If one rate is much faster than the other, the observed long-time behavior approaches one exponential. The sketch in the preceding section displays these shapes using arbitrary specified rates.

The simplest [catalytic cycle](../../../../../catalytic-cycle.md) compatible with the fits therefore contains an ATP-dependent binding delay and at least two resolvable ATP-concentration-independent kinetic events. Hydrolysis, product release and conformational changes are possible microscopic assignments, but the two-rate fit alone does not uniquely identify them or the order of $k_a$ and $k_b$. If each complete $120^\circ$ cycle contains these three waits and step durations are negligible, its mean duration is $(k_1c)^{-1}+k_a^{-1}+k_b^{-1}$ and the mean revolution rate is the inverse of three times this duration. Multiple catalytic sites can cooperate during that cycle.

**TODO: the source PDF's stepping plot is absent. Its individual substep angles, numerical timings and the mapping of plotted dwell labels onto the larger or smaller angular movement cannot be read.** The surviving text establishes only the $120^\circ$ total step and the existence of a larger and a smaller substep. No numerical rate, missing angle or plotted label is inferred from a different experiment. The distribution derivations and the concentration-dependence inference above are independent of that illustration.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [2](../../2.md)
3. [S12](../../../s12.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
