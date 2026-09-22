<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the terminal [financial payoff](../../../../contingent-claim-payoff.md) $f(S)=S$. The function $V(S,t)=S$ satisfies the [Black-Scholes equation](../../../../black-scholes-equation.md): its time derivative and second stock derivative vanish, while $rSV_S-rV=rS-rS=0$. It also has the correct terminal value. Part [a](../a.md) therefore gives

$$
S_t=e^{-r(T-t)}\mathbb E[S_T\mid\mathcal F_t],
\qquad
\boxed{\mathbb E[e^{-rT}S_T\mid\mathcal F_t]=e^{-rt}S_t.}
$$

Thus the discounted [stock](../../../../stock.md) is a [martingale](../../../../martingale-split.md). The explicit [lognormal distribution](../../../../log-normal-distribution.md) in part [b](../b.md) supplies the necessary finite [expectation](../../../../expected-value-split.md), so here this is a true martingale identity.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
