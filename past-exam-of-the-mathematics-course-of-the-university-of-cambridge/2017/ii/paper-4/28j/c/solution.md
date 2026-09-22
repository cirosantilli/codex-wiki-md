<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret $t=m$ and $T=N$ as trading dates in the discrete model; a payoff at nondates would require an interpolation convention absent from the question. Put $n=N-m$. Under $Q$, the independent stock returns after $m$ give

$$
\frac{S_N}{S_m}=u^Jd^{n-J},\qquad J\sim\operatorname{Binomial}(n,q).
$$

The ratio payoff is therefore independent of $\mathcal F_m$ under $Q$, and its time-zero price is

$$
\boxed{V_0=R^{-N}\sum_{j=0}^n\binom njq^j(1-q)^{n-j}(u^jd^{n-j}-K)^+.}
$$

At any date $s\leq m$, its price is the same expectation discounted only for the remaining $N-s$ periods. The formula uses the ratio payoff actually specified; multiplying it by $S_m$ would define a different, conventional monetary forward-start call.

## ↑ Ancestors (11)

1. [C](../c.md)
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
