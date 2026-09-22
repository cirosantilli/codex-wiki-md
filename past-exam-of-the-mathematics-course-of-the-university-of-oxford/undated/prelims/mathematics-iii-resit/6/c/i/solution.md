<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $R$ denote the red die. Conditional on $R=r$, each white roll succeeds independently with [probability](../../../../../../../probability.md) $p_r=(7-r)/6$. Consequently $T\mid R=r$ has the [geometric distribution](../../../../../../../geometric-distribution.md) on $\{1,2,\ldots\}$ and [expected value](../../../../../../../expected-value-split.md) $1/p_r=6/(7-r)$. The [law of total expectation](../../../../../../../law-of-total-expectation.md) gives

$$
\boxed{\mathbb E T=\frac16\sum_{r=1}^6\frac6{7-r}
=\sum_{k=1}^6\frac1k=\frac{49}{20}.}
$$

This is $2.45$ rolls; the averaging must be over conditional [expected values](../../../../../../../expected-value-split.md), not over success [probabilities](../../../../../../../probability.md) before taking a reciprocal.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
