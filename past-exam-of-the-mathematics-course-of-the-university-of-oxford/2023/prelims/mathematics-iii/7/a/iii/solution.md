<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the independent [random sample](../../../../../../../independent-and-identically-distributed-random-variables.md), the [likelihood function](../../../../../../../likelihood-function.md) on its support is $L(\theta)=\theta^ne^{-\theta Y}$, where $Y=\sum X_i$. Its [log-likelihood](../../../../../../../log-likelihood.md) is $\ell(\theta)=n\log\theta-\theta Y$, with

$$
\ell'(\theta)=n/\theta-Y,\qquad\ell''(\theta)=-n/\theta^2<0.
$$

Almost surely $Y>0$, and the unique stationary point is consequently the unique global maximum:

$$
\boxed{\hat\theta=n/Y.}
$$

The exceptional all-zero sample has probability zero; if $Y=0$ were nevertheless supplied, there would be no finite maximizing rate.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
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
