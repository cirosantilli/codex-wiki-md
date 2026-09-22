<h1 id="b/7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Invest each cash payment $q_vS_v\,dv$ received at time $v$ in the bank account until $T$. Its accumulated terminal amount is $q_vS_ve^{r(T-v)}\,dv$, so the entire future stream is equivalent, path by path, to the terminal payment $\int_t^Tq_vS_ve^{r(T-v)}\,dv$.

The [risk-neutral pricing](../../../../../risk-neutral-pricing.md) formula, including this reinvested payoff, is

$$
\boxed{V(t,s)=e^{-r(T-t)}\mathbb E^{\mathbb Q}\left[
\Psi(\widetilde S_T)+\int_t^Tq_v\widetilde S_ve^{r(T-v)}\,dv
\,\middle|\,\widetilde S_t=s\right],}
$$

where $d\widetilde S_v=r\widetilde S_v\,dv+\sigma\widetilde S_v\,dW_v^{\mathbb Q}$. Equivalently, discount each cash flow directly to time $t$. This is the discounted-gains martingale principle underlying the PDE in part (a).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
