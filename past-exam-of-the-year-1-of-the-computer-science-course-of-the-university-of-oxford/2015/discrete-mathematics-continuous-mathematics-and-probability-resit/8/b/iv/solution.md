<h1 id="8/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Given $M=m$, there are exactly $m$ independent opportunities to stay awake, each with [probability](../../../../../../probability.md) $p$. Hence

$$
\boxed{W\mid M=m\sim\operatorname{Binomial}(m,p).}
$$

The standard [binomial distribution](../../../../../../binomial-distribution.md) formulas are $\mathbb E[W\mid M]=pM$ and $\operatorname{var}(W\mid M)=Mp(1-p)$. The [Poisson distribution](../../../../../../poisson-distribution.md) formulas are $\mathbb E[M]=\lambda$, $\operatorname{var}(M)=\lambda$, and therefore $\mathbb E[M^2]=\lambda^2+\lambda$. By the [law of total expectation](../../../../../../law-of-total-expectation.md),

$$
\mathbb E[WM]=\mathbb E\bigl[M\mathbb E[W\mid M]\bigr]
=p\mathbb E[M^2]=p(\lambda^2+\lambda),
\qquad \mathbb E[W]=p\lambda.
$$

Using the definition of [covariance](../../../../../../covariance.md),

$$
\boxed{\operatorname{cov}(W,M)=\mathbb E[WM]-\mathbb E[W]\mathbb E[M]=p\lambda.}
$$

Thus $W$ and $M$ are not independent, even though the separate awake and asleep counts produced by [Poisson thinning](../../../../../../poisson-thinning.md) are independent.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
