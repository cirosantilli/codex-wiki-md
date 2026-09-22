<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate the [dividend](../../../../../dividend.md) PDE with respect to $S$. The diffusion term contributes $\sigma^2S V_{SS}+\tfrac12\sigma^2S^2V_{SSS}$, and the stock-drift term contributes $(r-\delta)(V_S+SV_{SS})$. With $\Delta=V_S$, the coefficient of $\Delta$ is $(r-\delta)-r=-\delta$. Therefore

$$
\boxed{\Delta_t+(r-\delta+\sigma^2)S\Delta_S
+\tfrac12\sigma^2S^2\Delta_{SS}-\delta\Delta=0.}
$$

The terminal condition is $\Delta(T,S)=\Psi'(S)$ wherever the [contingent claim payoff](../../../../../contingent-claim-payoff.md) is differentiable, with an appropriate weak or limiting interpretation at [contingent claim payoff](../../../../../contingent-claim-payoff.md) kinks. In the next part the squared positive-part [contingent claim payoff](../../../../../contingent-claim-payoff.md) is continuously differentiable, so its terminal [option delta](../../../../../option-delta.md) has no jump.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
