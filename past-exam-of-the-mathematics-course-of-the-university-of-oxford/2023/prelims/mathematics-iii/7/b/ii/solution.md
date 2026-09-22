<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The inverse moments in part [i](../i.md) give

$$
\mathbb E[\hat\theta]=\frac{n\theta}{n-1},\qquad
\mathbb E[\hat\theta^2]=\frac{n^2\theta^2}{(n-1)(n-2)}.
$$

Thus the [bias](../../../../../../../bias-of-an-estimator.md) is positive, and direct expansion of the [mean squared error](../../../../../../../mean-squared-error.md) yields

$$
\boxed{b_\theta(\hat\theta)=\frac\theta{n-1},\qquad
\operatorname{MSE}_\theta(\hat\theta)=\frac{(n+2)\theta^2}{(n-1)(n-2)}.}
$$

For comparison, the [variance](../../../../../../../variance-split.md) is $n^2\theta^2/[(n-1)^2(n-2)]$; adding the squared [bias](../../../../../../../bias-of-an-estimator.md) gives the same answer by the [bias-variance decomposition](../../../../../../../bias-variance-decomposition-of-mean-squared-error.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
