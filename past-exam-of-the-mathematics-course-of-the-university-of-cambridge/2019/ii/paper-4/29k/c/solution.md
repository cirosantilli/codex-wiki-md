<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N=T-t$ and use the discounted multipliers $u,d$. Under $Q$, the number $K$ of up moves in the remaining $N$ periods has the [binomial distribution](../../../../../../binomial-distribution.md) $\operatorname{Binomial}(N,q)$. Since

$$
S_T^1=S_t^1u^Kd^{N-K},
$$

the conditional expectation in part (b) becomes

$$
\boxed{
V_t=\sum_{k=0}^{T-t}\binom{T-t}{k}q^k(1-q)^{T-t-k}
h\left(S_t^1u^kd^{T-t-k}\right).}
$$

For an undiscounted stock, replace $u,d$ by $U,D$ and discount the resulting payoff by the appropriate power of $R$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
