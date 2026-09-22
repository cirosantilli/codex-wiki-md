<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The symmetric continuous [prior distribution](../../../../../prior-probability.md) gives $\Pr(\theta<0)=\Pr(\theta\geq0)=1/2$, so the [prior odds](../../../../../prior-odds.md) are one. Therefore the [Bayes factor](../../../../../bayes-factor.md) equals the [posterior odds](../../../../../posterior-odds.md). Standardizing the normal [posterior distribution](../../../../../bayesian-posterior.md), put

$$
z=\frac{\mu_n}{\sqrt{v_n}}
=\frac{n\tau\overline x}{\sigma\sqrt{\sigma^2+n\tau^2}}.
$$

Then $\Pr(H_0\mid x)=\Phi(-z)$ and $\Pr(H_1\mid x)=\Phi(z)$. The endpoint $\theta=0$ has zero posterior probability, so the strict/non-strict split causes no additional term. Hence

$$
\boxed{B=\frac{\Phi(-z)}{\Phi(z)}
=\frac{1-\Phi(z)}{\Phi(z)},\qquad
z=\frac{n\tau\overline x}{\sigma\sqrt{\sigma^2+n\tau^2}}.}
$$

In particular, positive values of the [sample mean](../../../../../sample-mean.md) make this [Bayes factor](../../../../../bayes-factor.md) smaller, favouring the positive-mean hypothesis.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
