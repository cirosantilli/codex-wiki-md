<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed rational $0\leq t_1<t_2<t_3<t_4$, write

$$
\max_{t_3\leq t\leq t_4}B_t-\max_{t_1\leq t\leq t_2}B_t
=\underbrace{B_{t_3}-B_{t_2}}_{Z}+\underbrace{\max_{t_3\leq t\leq t_4}(B_t-B_{t_3})}_{V}+\underbrace{B_{t_2}-\max_{t_1\leq t\leq t_2}B_t}_{W}.
$$

By [independent increments](../../../../../../independent-increments.md), $Z$ is independent of $(V,W)$ and has [normal distribution](../../../../../../normal-distribution.md) $N(0,t_3-t_2)$. Conditional on $(V,W)$, the displayed difference has a continuous [probability density function](../../../../../../probability-density-function.md); in particular it equals zero with probability zero. Taking the countable intersection over all such rational quadruples proves that, on one event of probability one, the maxima over any two separated rational closed intervals are distinct.

Suppose a [local maximum](../../../../../../local-maximum.md) at $t$ were not a [strict local maximum](../../../../../../strict-local-maximum.md). There is a neighbourhood in which every value is at most $B_t$, and, arbitrarily close to $t$, some other time $u$ strictly inside that neighbourhood has $B_u=B_t$. Choose separated rational closed intervals containing $t$ and $u$, both lying inside that neighbourhood. When one time is zero, use a first interval with left endpoint zero. Both interval maxima equal $B_t$, contrary to the preceding event.

Therefore **every [local maximum of Brownian motion](../../../../../../local-maximum-of-brownian-motion.md) is a [strict local maximum](../../../../../../strict-local-maximum.md) [almost surely](../../../../../../almost-sure-convergence.md)**, simultaneously over all times. This countable-interval argument avoids an invalid intersection of probability-one events over uncountably many candidate times.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
