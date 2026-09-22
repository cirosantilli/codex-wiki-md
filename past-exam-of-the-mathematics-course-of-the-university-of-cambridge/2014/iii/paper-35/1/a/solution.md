<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [likelihood function](../../../../../../likelihood-function.md) for the ordered arrival times of a [Poisson process](../../../../../../poisson-process.md), including the absence of further arrivals before $T$, is

$$
\boxed{L(\lambda)=\lambda^n e^{-\lambda T}},\qquad 0<t_1<\cdots<t_n<T.
$$

The arrival-time constraint does not depend on $\lambda$. Equivalently, the [Poisson distribution](../../../../../../poisson-distribution.md) of the total count gives $L(\lambda)=e^{-\lambda T}(\lambda T)^n/n!$, which differs by a parameter-independent factor. Conditional on the count, the [Poisson process conditional arrival times](../../../../../../poisson-process-conditional-arrival-times.md) have density $n!/T^n$, independent of $\lambda$. Thus **the total count contains all the information about the rate when the exposure is known**; it is a [sufficient statistic](../../../../../../sufficient-statistic.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
