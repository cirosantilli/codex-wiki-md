<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First justify that the [moments](../../../../../moment.md) being used exist. For every $r>0$,

$$
\mathbb E e^{r|Y|}\leq\mathbb E e^{rY}+\mathbb E e^{-rY}=M_Y(r)+M_Y(-r)<\infty.
$$

The bound $|y|^k\leq k!r^{-k}e^{r|y|}$ gives $\mathbb E|Y|^k<\infty$ for all $k$.

If $Y$ has a [symmetric distribution](../../../../../symmetric-distribution.md), then $Y$ and $-Y$ have the same [probability distribution](../../../../../probability-distribution-split.md), so for odd $k$,

$$
\mathbb EY^k=\mathbb E(-Y)^k=-\mathbb EY^k,
$$

which forces $\mathbb EY^k=0$.

Conversely, suppose every odd [moment](../../../../../moment.md) vanishes. For fixed $t\in\mathbb R$, the absolute values of the partial [Taylor series](../../../../../taylor-series.md) for $e^{tY}$ are bounded by $e^{|t||Y|}$, whose [expected value](../../../../../expected-value-split.md) is finite by the preceding inequality. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore permits termwise [expectation](../../../../../expected-value-split.md):

$$
M_Y(t)=\sum_{k=0}^\infty\frac{t^k\mathbb EY^k}{k!}
=\sum_{j=0}^\infty\frac{t^{2j}\mathbb EY^{2j}}{(2j)!}=M_Y(-t)=M_{-Y}(t).
$$

The [uniqueness theorem for moment-generating functions](../../../../../uniqueness-theorem-for-moment-generating-functions.md) implies equality of the [probability distributions](../../../../../probability-distribution-split.md) of $Y$ and $-Y$. Hence

$$
\boxed{Y\text{ has a symmetric distribution}\ \Longleftrightarrow\ \mathbb EY^k=0\text{ for every odd }k.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
