<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Assume condition (1). Given an adapted cash-flow process $X_1,\ldots,X_T$, construct the holdings backwards. Set $H_{T+1}=0$. Once $H_{t+1}$ is known, the random variable

$$
X_t+H_{t+1}\cdot P_t
$$

is $\mathcal F_t$-measurable. Condition (1) supplies an $\mathcal F_{t-1}$-measurable $H_t$ satisfying

$$
H_t\cdot(P_t+\delta_t)
=X_t+H_{t+1}\cdot P_t.
$$

Hence $\xi_t^H=X_t$ for every $t\leq T$, and setting later holdings to zero proves condition (2).

Conversely, let $X_T$ be any $\mathcal F_T$-measurable random variable and apply condition (2) to the adapted process with cash flow $X_T$ at $T$ and zero cash flow earlier. Since $H_{T+1}=0$,

$$
X_T=\xi_T^H=H_T\cdot(P_T+\delta_T),
$$

where $H_T$ is $\mathcal F_{T-1}$-measurable. This is condition (1). The conditions are therefore equivalent and describe [market completeness](../../../../../../complete-market.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
