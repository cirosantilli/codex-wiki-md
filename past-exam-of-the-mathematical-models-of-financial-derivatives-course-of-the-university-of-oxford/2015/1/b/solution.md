<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [replicating strategy](../../../../replicating-strategy.md) holds $\Delta$ shares and a current cash amount $b$ in the [bank account](../../../../bank-account.md). Matching the two next values gives

$$
\Delta S^u_{t+1}+Rb=V^u_{t+1},\qquad
\Delta S^d_{t+1}+Rb=V^d_{t+1}.
$$

Solving this [linear system](../../../../system-of-linear-equations.md),

$$
\Delta=\frac{V^u_{t+1}-V^d_{t+1}}{S^u_{t+1}-S^d_{t+1}},\qquad
b=\frac{S^u_{t+1}V^d_{t+1}-S^d_{t+1}V^u_{t+1}}{R(S^u_{t+1}-S^d_{t+1})}.
$$

By [no-arbitrage](../../../../no-arbitrage.md), the claim costs $V_t=\Delta S_t+b$. Collecting the coefficients of its two future values yields

$$
\boxed{V_t=R^{-1}\bigl[qV^u_{t+1}+(1-q)V^d_{t+1}\bigr],\qquad
q=\frac{RS_t-S^d_{t+1}}{S^u_{t+1}-S^d_{t+1}}.}
$$

The physical [probability](../../../../probability.md) $p$ does not appear: replication fixes the price of this [contingent claim](../../../../contingent-claim.md) from traded prices.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
