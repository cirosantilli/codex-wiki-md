<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [competing risks model](../../../../../../competing-risks-model.md), the first event has time $T$ and type $J$; observing one type prevents another type from being the first event for that individual. Its [cause-specific hazard](../../../../../../cause-specific-hazard.md) is

$$
h_j(t)=\lim_{\Delta\downarrow0}\frac{\mathbb P(t\leq T<t+\Delta,J=j\mid T\geq t)}{\Delta}.
$$

For absolutely continuous event times the total [hazard function](../../../../../../hazard-function.md) is $\sum_jh_j(t)$, giving the event-free [survivor function](../../../../../../survival-function.md) $S(t)=\exp[-\int_0^t\sum_jh_j(u)\,du]$. Since an event of type $j$ near $t$ has unconditional density $S(t)h_j(t)$, its [cumulative incidence function](../../../../../../cumulative-incidence-function.md) satisfies

$$
\boxed{F_j(t)=\mathbb P(T\leq t,J=j)=\int_0^tS(u)h_j(u)\,du.}
$$

This [cause-specific hazard to cumulative incidence formula](../../../../../../cause-specific-hazard-to-cumulative-incidence-formula.md) does not require [independent](../../../../../../independent-random-variables.md) latent times for the competing causes. In general $F_j(t)$ is not $1-e^{-\int_0^th_j}$, since that expression ignores removal by other causes.

Put $a=\theta_A\geq0$, $b=\theta_B\geq0$ and $q=a+b$, with $\tau\geq0$. Here

$$
S(t)=e^{-at-b\min(t,\tau)}.
$$

Integrating $aS(u)$ separately before and after $\tau$ gives, for $q>0$,

$$
\boxed{F_A(t)=\begin{cases}\dfrac{a}{q}(1-e^{-qt}),&0\leq t\leq\tau,\\[4pt]\dfrac{a}{q}(1-e^{-q\tau})+e^{-q\tau}(1-e^{-a(t-\tau)}),&t>\tau.\end{cases}}
$$

After $\tau$, only type $A$ can occur, so the second term is the fraction event-free at $\tau$ multiplied by their subsequent event [probability](../../../../../../probability.md). The expressions agree at $\tau$. If $a=b=0$, both incidence functions are identically zero; if $a=0<b$, this formula gives $F_A=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
