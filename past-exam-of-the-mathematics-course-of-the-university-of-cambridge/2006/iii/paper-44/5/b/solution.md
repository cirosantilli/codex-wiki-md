<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the right-continuous [Breslow estimator](../../../../../../breslow-estimator.md), so the increase from the value at $x_{m-1}$ to the value at $x_m$ means the interval $(x_{m-1},x_m]$. There is no event between these consecutive exit times, and at $x_m$ the [risk set](../../../../../../risk-set.md) contains only subject $m$. Hence

$$
\widehat H_0(x_m)-\widehat H_0(x_{m-1})
=\frac{v_m}{e^{\widehat\beta^Tz_m}},
$$

and the fitted individual [cumulative hazard](../../../../../../cumulative-hazard-function.md) increases by

$$
\boxed{\widehat H_m(x_m)-\widehat H_m(x_{m-1})
=e^{\widehat\beta^Tz_m}\frac{v_m}{e^{\widehat\beta^Tz_m}}=v_m.}
$$

It is the subject's integrated hazard, rather than the reference baseline increment, that equals the event indicator.

For the final unheaded request, a fitted [martingale residual](../../../../../../martingale-residual.md) at a subject's exit is

$$
\widehat M_i=v_i-e^{\widehat\beta^Tz_i}\widehat H_0(x_i).
$$

The revised observation leaves the last subject at risk until a later event time, still after every other subject has exited. Every earlier [risk set](../../../../../../risk-set.md) is exactly the same as before, and the new final event again contributes the constant factor one. Thus part a gives unchanged coefficients, and every earlier [Breslow estimator](../../../../../../breslow-estimator.md) increment is unchanged. No additional events occur during the extended interval because all other subjects have already left observation.

For $i<m$, the event indicator and fitted [cumulative hazard](../../../../../../cumulative-hazard-function.md) at $x_i$ remain unchanged, hence so does $\widehat M_i$. For the terminal subject, let $C$ denote its old fitted integrated hazard at its censored exit. That old residual is $-C$. Part b shows that the new final event adds one to its fitted integrated hazard, giving new residual

$$
\widehat M_m^{\rm new}=1-(C+1)=-C=\widehat M_m^{\rm old}.
$$

Therefore **all fitted [martingale residuals](../../../../../../martingale-residual.md) remain unchanged**. Their invariance does not assert that the fitted [survivor function](../../../../../../survival-function.md) at later times or the terminal event record is unchanged: the new late [baseline hazard](../../../../../../baseline-hazard.md) jump is real. This is the [terminal-observation invariance of Cox martingale residuals](../../../../../../terminal-observation-invariance-of-cox-martingale-residuals.md), which relies on a unique final subject and unchanged covariate history.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
