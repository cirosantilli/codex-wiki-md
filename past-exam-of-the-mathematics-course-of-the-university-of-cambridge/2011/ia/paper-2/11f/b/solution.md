<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $m_k$ be the expected remaining [hitting time](../../../../../../first-passage-time.md) of either endpoint, measured in minutes. The first step consumes one minute, after which [first-step analysis](../../../../../../first-step-analysis.md) gives

$$
\boxed{m_k=1+\frac12m_{k-1}+\frac12m_{k+1},\quad1\le k\le19;\qquad m_0=m_{20}=0.}
$$

The [expectation](../../../../../../expected-value.md) is finite: from any interior state, a block of twenty leftward steps guarantees absorption and has probability $2^{-20}$. Thus the survival probability over successive twenty-step blocks has a geometric upper bound. This justifies using finite [expectations](../../../../../../expected-value.md) in the recurrence.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
