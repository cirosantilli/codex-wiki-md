<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

This requires an argument using [Lebesgue outer measure](../../../../lebesgue-outer-measure.md), since $E$ need not be a [Lebesgue measurable set](../../../../lebesgue-measurable-set.md). Some bounded portion $F=E\cap[-N,N]$ has $a=m^*(F)>0$: otherwise [countable subadditivity](../../../../countable-subadditivity-of-a-measure.md) would give $m^*(E)=0$. Also $a\leq2N<\infty$.

Suppose, for a contradiction, that every nonempty bounded open [interval](../../../../interval-mathematics.md) $I$ satisfies $m^*(E\cap I)\leq\lambda|I|$. Because $a/\lambda>a$, the definition of [Lebesgue outer measure](../../../../lebesgue-outer-measure.md) gives a countable cover $F\subseteq\bigcup_j I_j$ by nonempty bounded open intervals with

$$
\sum_j|I_j|<\frac a\lambda.
$$

Using [countable subadditivity](../../../../countable-subadditivity-of-a-measure.md) again,

$$
a=m^*(F)\leq\sum_jm^*(F\cap I_j)\leq\sum_jm^*(E\cap I_j)\leq\lambda\sum_j|I_j|<a,
$$

a contradiction. Hence at least one interval in such a cover satisfies

$$
\boxed{m^*(E\cap I)>\lambda|I|.}
$$

This [high-density interval for outer measure](../../../../high-density-interval-for-outer-measure.md) applies even to nonmeasurable sets; the argument does not require the [Lebesgue density theorem](../../../../lebesgue-s-density-theorem.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
