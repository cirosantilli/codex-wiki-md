<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For the [geometric distribution](../../../../../../geometric-distribution.md) supported on positive integers, set $q=1-p$. The geometric series and its derivative give

$$
E(T)=\sum_{t=1}^{\infty}tpq^{t-1}
=p\frac{d}{dq}\left(\frac1{1-q}\right)
=\frac p{(1-q)^2}
=\boxed{\frac1p}.
$$

Equivalently, the sum of the tail probabilities is $\sum_{k\geq0}P(T>k)=\sum_{k\geq0}q^k=1/p$. For $p=0.02$, the expected wait is **50 years**, so this is the **50-year [return level](../../../../../../return-level.md)**. The exceedance probability determines the return period, but does not by itself determine a numerical flow rate.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
