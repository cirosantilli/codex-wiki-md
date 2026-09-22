<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is the [waiting time to observe both Bernoulli outcomes](../../../../../../waiting-time-to-observe-both-bernoulli-outcomes.md). Write $q=1-p$, and let $S$ record the sex of the first captured animal. That first capture is always needed. If $S$ is male, every subsequent trial independently produces the required female with [probability](../../../../../../probability.md) $q$, so $N-1$ has a [geometric distribution](../../../../../../geometric-distribution.md) with parameter $q$. If $S$ is female, $N-1$ has a [geometric distribution](../../../../../../geometric-distribution.md) with parameter $p$. By the [law of total expectation](../../../../../../law-of-total-expectation.md),

$$
EN=1+p\frac1q+q\frac1p.
$$

Since $p+q=1$, this simplifies to **$\boxed{EN=1/(pq)-1}$**, or

$$
\boxed{EN=\frac1{p(1-p)}-1.}
$$

The [expectation](../../../../../../expected-value.md) includes both the first capture and the final capture completing the pair.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
