<h1 id="continuous-mathematics/5/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A convenient choice for this irregular region is [Monte Carlo integration](../../../../../../../monte-carlo-integration.md). The region is contained in $[-1,1]^2$. For independent uniform points $U_j$ in that square, let

$$
\widehat I_N=\frac4N\sum_{j=1}^N\mathbf1_{\{U_j\in R\}}\exp\!\left(e^{(U_j)_1}+e^{(U_j)_2}+e^{(U_j)_1(U_j)_2}\right).
$$

The [indicator random variable](../../../../../../../indicator-random-variable.md) incorporates the curved boundary directly. This estimator is unbiased; the integrand is bounded on the square, so its [variance](../../../../../../../variance-split.md) is finite. The [variance of a sum](../../../../../../../variance-of-a-sum.md) of independent terms gives [root mean square](../../../../../../../root-mean-square.md) error **$O(N^{-1/2})$** in [big O notation](../../../../../../../big-o-notation.md). This is a stochastic error rate. Applying a rectangular [Simpson's rule](../../../../../../../simpson-s-rule.md) to the indicator-weighted integrand would lose the smoothness required for its fourth-order error bound.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Continuous mathematics](../../../../continuous-mathematics.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
