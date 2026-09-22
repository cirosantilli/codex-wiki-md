<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $r>0$, put $b=S^\star\in(0,K)$ and let $\tau_b=\inf\{u\geq0:S_u\leq b\}$. In the continuation region $S>b$, the time-independent [Black-Scholes equation](../../../../../black-scholes-equation.md) is a [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md). Substituting $V=S^m$ gives

$$
\frac12\sigma^2m(m-1)+rm-r=(m-1)\left(\frac12\sigma^2m+r\right)=0.
$$

Set $\gamma=2r/\sigma^2>0$. The two powers are $S$ and $S^{-\gamma}$. The [boundary condition](../../../../../boundary-condition.md) $V(S)\to0$ as $S\to\infty$ removes the growing solution; value matching at $b$ sets the coefficient. Hence the fixed-trigger value is

$$
\boxed{V_b(S)=(K-b)^n(S/b)^{-\gamma},\qquad S>b}.
$$

For $0\leq S\leq b$ the policy exercises immediately, giving $V_b(S)=(K-S)^n$. The quoted continuation expression alone does not apply below the exercise boundary. Equivalently, the [discounted boundary-hitting representation](../../../../../discounted-boundary-hitting-representation.md) gives $\mathbb E_S[e^{-r\tau_b};\tau_b<\infty]=(S/b)^{-\gamma}$, which multiplies the exercise [financial payoff](../../../../../contingent-claim-payoff.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
