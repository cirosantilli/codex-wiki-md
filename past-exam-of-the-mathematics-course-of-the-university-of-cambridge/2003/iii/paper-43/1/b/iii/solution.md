<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Every independent proposal/uniform pair succeeds with [probability](../../../../../../../probability.md) $p=1/M$. The number $K$ retained from a fixed budget of 100 attempts therefore has a [binomial distribution](../../../../../../../binomial-distribution.md), rather than a fixed value:

$$
\boxed{K\sim\operatorname{Bin}(100,1/M),\qquad P(K\ge50)=\sum_{r=50}^{100}\binom{100}{r}M^{-r}(1-M^{-1})^{100-r}.}
$$

Conditioned on the accept/reject indicators, each retained value still has the target [probability density function](../../../../../../../probability-density-function.md); the random output count is a separate issue from the correctness of those retained draws.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
