<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the [risk-neutral measure](../../../../risk-neutral-measure.md), write

$$
S_T/s=\exp\left((r-\sigma^2/2)\tau+\sigma\sqrt\tau Z\right),\qquad Z\sim N(0,1).
$$

Complete the square in the [normal density](../../../../normal-density.md) after multiplying by the power of $S_T/s$. The [truncated lognormal moment](../../../../truncated-lognormal-moment.md) gives, for $K>0$,

$$
\boxed{V_p(t,s,K)=M_p(\tau)\Phi(d_p),\quad
M_p(\tau)=e^{[pr+p(p-1)\sigma^2/2]\tau},\quad
d_p=\frac{\log(s/K)+[r+(p-1/2)\sigma^2]\tau}{\sigma\sqrt\tau}.}
$$

All real powers have finite moments in this [lognormal distribution](../../../../log-normal-distribution.md). If $K=0$, the indicator is identically one and $V_p=M_p$. The function $V_p$ is an undiscounted conditional moment; the option prices below additionally include the [discount factor](../../../../discount-factor.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
