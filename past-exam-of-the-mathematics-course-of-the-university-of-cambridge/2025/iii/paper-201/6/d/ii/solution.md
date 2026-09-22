<h1 id="6/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Construct the times inductively. Suppose $(B_{T_0},\ldots,B_{T_n})$ has the law of $(S_0,\ldots,S_n)$. Conditional on the past, the martingale increment $S_{n+1}-S_n$ has mean zero and finite second moment. Apply the conditional form of the [Skorokhod embedding theorem](../../../../../../../skorokhod-embedding-theorem.md) to this regular conditional law, using the fresh Brownian motion $B_{T_n+t}-B_{T_n}$ supplied by the [Strong Markov property](../../../../../../../strong-markov-property.md). This gives a stopping time increment $\tau_{n+1}$ and $T_{n+1}=T_n+\tau_{n+1}$ such that the next Brownian increment has the required conditional law. Induction proves

$$
(S_0,\ldots,S_k)\stackrel d=(B_{T_0},\ldots,B_{T_k})
$$

for every $k$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
