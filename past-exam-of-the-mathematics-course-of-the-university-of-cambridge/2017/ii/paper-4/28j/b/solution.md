<h1 id="28j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any finite [contingent claim](../../../../../../contingent-claim.md) $C$ measurable at the final date in the natural binomial tree, [backward induction](../../../../../../backward-induction.md) gives

$$
\boxed{V_j=B_j\mathbb E_Q[C/B_N\mid\mathcal F_j].}
$$

At a node with stock $S_j$, let $V_{j+1}^u,V_{j+1}^d$ be its two successor values. Hold, during the next period,

$$
\boxed{\Delta_j=\frac{V_{j+1}^u-V_{j+1}^d}{S_j(u-d)},\qquad
\psi_j=\frac{uV_{j+1}^d-dV_{j+1}^u}{(u-d)B_{j+1}}.}
$$

The stock and bank holdings reproduce both successor values and cost $\Delta_jS_j+\psi_jB_j=R^{-1}[qV_{j+1}^u+(1-q)V_{j+1}^d]=V_j$. Rebalancing at every node is self-financing, and terminal value is $C$. Thus every such claim is replicated and the no-arbitrage price is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
