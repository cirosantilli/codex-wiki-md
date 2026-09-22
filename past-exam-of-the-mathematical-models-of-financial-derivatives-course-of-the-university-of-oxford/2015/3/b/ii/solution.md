<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

While the [up-and-out digital put](../../../../../up-and-out-digital-put.md) is alive, its pricing domain is $0<S<B$, $t<T$. Its [Black-Scholes equation](../../../../../black-scholes-equation.md), terminal [financial payoff](../../../../../contingent-claim-payoff.md), and absorbing [boundary condition](../../../../../boundary-condition.md) are

$$
\boxed{\begin{aligned}
H_t+\tfrac12\sigma^2S^2H_{SS}+rSH_S-rH&=0,&0<S<B,\ t<T,\\
H(S,T)&=\mathbf1_{\{S<K\}},&0<S<B,\\
H(B,t)&=0,&t\leq T.
\end{aligned}}
$$

For completeness, the natural limiting condition is $\lim_{S\downarrow0}H(S,t)=e^{-r(T-t)}$, with $0\leq H(S,t)\leq e^{-r(T-t)}$. A positive [geometric Brownian motion](../../../../../geometric-brownian-motion.md) cannot hit zero in finite time, and from a very small starting value the survival and below-strike terminal events have probability tending to one. If the barrier has already been hit, its value is zero regardless of the current stock price.

For $K>B$, the terminal payoff tends to one from inside at $S=B$, while an already hit barrier pays zero. Thus there is a terminal-boundary corner discontinuity; the terminal condition is imposed only for $S<B$, not as a requirement of continuous extension at $(B,T)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
