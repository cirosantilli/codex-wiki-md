<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Integrate the expected [Markov-chain entry count](../../../../../../../entry-count-of-a-continuous-time-markov-chain.md) density and use the [occupation time of a continuous-time Markov chain](../../../../../../../occupation-time-of-a-continuous-time-markov-chain.md) formula:

$$
\boxed{E_{rs}(t)=\int_0^t\sum_{i\ne s}p_{ri}(u)q_{is}\,du
=\sum_{i\ne s}q_{is}T_{ri}(t).}
$$

Each term is a [transition intensity](../../../../../../../transition-intensity.md) multiplied by the expected exposure time to that transition. This counts every entry, including returns, rather than only the first visit. For countably many states the same nonnegative interchange follows from [Tonelli theorem](../../../../../../../tonelli-theorem.md), provided the resulting expected count is finite. The sum excludes $i=s$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
