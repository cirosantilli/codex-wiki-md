<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed [exercise threshold](../../../../exercise-threshold.md) $\bar S>K$, the continuation value solves the same stationary equation but is matched to $\bar S-K$ at that threshold. Boundedness at zero removes the negative power. Thus the [fixed-threshold value of a perpetual call](../../../../fixed-threshold-value-of-a-perpetual-call.md) is

$$
\boxed{\widetilde C(S)=(\bar S-K)(S/\bar S)^p,\qquad 0\leq S\leq\bar S.}
$$

It is also $(\bar S-K)\mathbb E_S^{\mathbb Q}[e^{-r\tau_{\bar S}};\tau_{\bar S}<\infty]$, where $\tau_{\bar S}$ is the first up-crossing [stopping time](../../../../stopping-time.md). Differentiating while keeping the current $S$ fixed gives

$$
\frac{\partial\widetilde C}{\partial\bar S}
=S^p\bar S^{-p-1}\bigl[pK-(p-1)\bar S\bigr].
$$

This is positive for $K<\bar S<\hat S=pK/(p-1)$, so increasing such an early threshold increases its continuation value. The comparison assumes $S<\bar S$; a policy already exercised has no remaining continuation value to vary.

If $\bar S>\hat S$, then

$$
\widetilde C'(\bar S-)=p\left(1-\frac K{\bar S}\right)>1.
$$

Since $\widetilde C(\bar S)=\bar S-K$, the [derivative](../../../../derivative.md) comparison gives $\widetilde C(S)<S-K$ for $S$ just below $\bar S$. Therefore **quoting this policy value as the price of an unrestricted American call permits arbitrage**: buy the option below its immediate exercise value and exercise it at once. A contract that actually commits its holder to the threshold is a different claim; its lower value is a suboptimal policy value, not by itself an arbitrage. The [perpetual American call option](../../../../perpetual-american-call-option.md) optimizes over all exercise policies and remains above its exercise payoff.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
