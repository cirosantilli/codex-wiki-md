<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a terminal price distinct from $K$, differentiating the put's [financial payoff](../../../../../contingent-claim-payoff.md) gives $\partial_K(K-S_T)^+=\mathbf1_{\{S_T<K\}}$. The difference quotients are bounded by one, and the continuous [lognormal distribution](../../../../../log-normal-distribution.md) has zero [probability](../../../../../probability.md) at the strike. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore permits differentiation inside its discounted [expectation](../../../../../expected-value-split.md). The [put-price strike derivative](../../../../../put-price-strike-derivative.md) is exactly the price of the [digital put option](../../../../../digital-put-option.md):

$$
\boxed{P_d(S,t)=\frac{\partial P}{\partial K}=e^{-r\tau}\operatorname N(-d_-).}
$$

Equivalently, [risk-neutral pricing](../../../../../risk-neutral-pricing.md) discounts the [probability](../../../../../probability.md) $\mathbb Q(S_T<K\mid S_t=S)=\Phi(-d_-)$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
