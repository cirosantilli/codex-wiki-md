<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The payoff is $(S_0S_T-S_T^2)\mathbf1_{\{S_T<S_0\}}$. Subtract the upper-tail [truncated lognormal moments](../../../../truncated-lognormal-moment.md) from the full moments in part [c](../c.md). With current spot $s=S_t$, the price is

$$
\boxed{e^{-r\tau}\left[S_0s\{M_1(\tau)-V_1(t,s,S_0)\}
-s^2\{M_2(\tau)-V_2(t,s,S_0)\}\right],}
$$

where $M_1=e^{r\tau}$ and $M_2=e^{(2r+\sigma^2)\tau}$. The threshold is the original $S_0$, not the current spot $s$. Since the conditional [lognormal distribution](../../../../log-normal-distribution.md) has no atoms, the strict endpoint convention does not affect the price for $t<T$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
