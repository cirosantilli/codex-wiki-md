<h1 id="o/o1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $z=\Phi^{-1}(1-\alpha/2)$ for the standard normal cumulative distribution function. Consistency of the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) and [Slutsky's theorem](../../../../../slutsky-theorem.md) give the asymptotic standardization

$$
\sqrt{I_n(\widehat\theta)}(\widehat\theta-\theta)\xrightarrow{d}N(0,1).
$$

Its [probability](../../../../../probability.md) of lying between $-z$ and $z$ tends to $1-\alpha$. Solving those inequalities for the unknown parameter yields the [Wald confidence interval](../../../../../wald-confidence-interval.md)

$$
\boxed{\left[\widehat\theta-\frac{z}{\sqrt{I_n(\widehat\theta)}},\quad
\widehat\theta+\frac{z}{\sqrt{I_n(\widehat\theta)}}\right].}
$$

Thus the estimated [standard error](../../../../../standard-error.md) is $I_n(\widehat\theta)^{-1/2}$. Its coverage is approximate and relies on the large-sample regularity assumptions.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O1](../../o1.md)
3. [O](../../../o.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
