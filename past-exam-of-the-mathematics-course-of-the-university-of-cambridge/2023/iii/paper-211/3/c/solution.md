<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First, no arbitrage implies the lower bound

$$
C_t^{T+1,K}\geq S_t-KP_t^{T+1}:
$$

otherwise buy the call and $K$ maturity-$(T+1)$ bonds and short one non-dividend-paying stock; the initial receipt is positive and the terminal payoff is nonnegative. At time $T$, the assumption $P_T^{T+1}\leq1$ therefore gives $C_T^{T+1,K}\geq(S_T-K)^+$.

If $C_t^{T,K}>C_t^{T+1,K}$, sell the shorter call and buy the longer one. At time $T$, the longer call's no-arbitrage value covers the shorter call's payoff, with a strictly positive initial receipt. This is impossible, so $T\mapsto C_t^{T,K}$ is nondecreasing.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
