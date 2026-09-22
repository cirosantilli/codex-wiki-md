<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Subtract the reflected solution from part [c](../c.md). On the alive side of the [down-and-out barrier option](../../../../down-and-out-claim.md),

$$
\boxed{V_B(S,t)=V(S,t)-(S/B)^{1-2r/\sigma^2}V(B^2/S,t),\qquad S>B.}
$$

Both terms satisfy the [Black-Scholes equation](../../../../black-scholes-equation.md), and at $S=B$ they cancel. At expiry, $S\geq B$ gives $B^2/S\leq B<K$, so the reflected [log-call option](../../../../log-call-option.md) has zero terminal [financial payoff](../../../../contingent-claim-payoff.md); the first term gives the required payoff. With the usual growth condition, uniqueness for the killed pricing problem identifies the expression as the [risk-neutral price](../../../../risk-neutral-price.md). After the barrier has been hit the contract value is zero. The algebraic image expression on $S<B$ is not its financial value.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
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
