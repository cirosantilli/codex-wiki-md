<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $S=X+Y$. Given $X$, its conditional [expected value](../../../../../../expected-value-split.md) is $3X/2$ and its conditional [variance](../../../../../../variance-split.md) is $X/4$, since $X$ is then fixed. The [law of total expectation](../../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../../law-of-total-variance.md) give

$$
\boxed{\mathbb E S=\frac{3(1-p)}{2p},\qquad
\operatorname{Var}(S)=\frac14\mathbb E X+\frac94\operatorname{Var}(X)
=\frac{(1-p)(p+9)}{4p^2}.}
$$

The two scores are dependent: the [law of total covariance](../../../../../../law-of-total-covariance.md) gives $\operatorname{Cov}(X,Y)=\operatorname{Cov}(X,X/2)=q/(2p^2)$. Adding their two [variances](../../../../../../variance-split.md) without that [covariance](../../../../../../covariance.md) term would give an incorrect total.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
