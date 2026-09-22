<h1 id="o/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The absolute observations are independent [exponential random variables](../../../../../exponential-distribution.md) with mean $\theta$ and [variance](../../../../../variance-split.md) $\theta^2$. Applying the [central limit theorem](../../../../../central-limit-theorem.md) directly to their average proves

$$
\boxed{\frac{\sqrt n(\widehat\theta-\theta)}{\theta}\ \xrightarrow{d}\ N(0,1).}
$$

Thus the large-sample approximation is $\widehat\theta\approx N(\theta,\theta^2/n)$, consistent with inverse [Fisher information](../../../../../fisher-information-matrix.md). Also $\widehat\theta\to\theta$ in [probability](../../../../../probability.md) by the [weak law of large numbers](../../../../../weak-law-of-large-numbers.md), so $\theta$ in the standard error can be replaced by $\widehat\theta$ through [Slutsky's theorem](../../../../../slutsky-theorem.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [O](../../../o.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
