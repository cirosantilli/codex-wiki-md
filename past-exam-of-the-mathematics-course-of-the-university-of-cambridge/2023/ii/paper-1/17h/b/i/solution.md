<h1 id="17h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $X$ count copies of the [complete graph](../../../../../../../complete-graph.md) $K_4$ in $G$. Its [expected value](../../../../../../../expected-value.md) is

$$
\mu=\mathbb EX=\binom n4p^6
\sim\frac{(\log n)^6}{24}\longrightarrow\infty.
$$

Write $X$ as a sum of [indicator random variable](../../../../../../../indicator-random-variable.md). Indicators for two distinct copies are independent when the copies share at most one vertex, since their edge sets are then disjoint. Pairs sharing two vertices have eleven edges in their union, while pairs sharing three have nine. It follows that

$$
\operatorname{var}(X)
\leq \mu+O(n^6p^{11})+O(n^5p^9)
=O((\log n)^6)+o(1).
$$

**Thus $\operatorname{var}(X)/\mu^2\to0$. By the [second moment method](../../../../../../../second-moment-method.md), $X/\mu\to1$ in probability, so $\mathbb P(X\geq100)\to1$. This is the [sparse clique-count concentration](../../../../../../../sparse-clique-count-concentration.md) estimate.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [17H](../../../17h.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
