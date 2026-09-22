<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $V=q/r$ under the [posterior density](../../../../../posterior-density.md) $\pi=r/Z$,

$$
\mathbb E_\pi V^2=\frac1Z\int_{\{r>0\}}\frac{q(\theta)^2}{r(\theta)}\,d\theta.
$$

The independent-draw [variance of a sample mean](../../../../../variance-of-a-sample-mean.md) therefore yields

$$
\boxed{\operatorname{Var}(\widehat p_2^{-1})=\frac1T\left[\frac1Z\int\frac{q^2}{r}-\frac1{Z^2}\right]=\frac1{TZ^2}\left[\int\frac{q^2}{\pi}-1\right]}.
$$

Since

$$
\int\frac{q^2}{\pi}-1=\int_{\{\pi>0\}}\frac{(q-\pi)^2}{\pi}\,d\theta\geq0,
$$

we again obtain

$$
\boxed{q_{\rm opt}=\pi,\qquad \min\operatorname{Var}(\widehat p_2^{-1})=0}.
$$

The optimum is again generally unavailable as an evaluable normalized density without knowing $Z$.

**A proposal with too much mass where the posterior density is tiny makes reciprocal weights unstable.** In particular, proposal tails that are too heavy relative to the [posterior distribution](../../../../../bayesian-posterior.md) can make $\int q^2/\pi$ infinite. This contrasts with ordinary [importance sampling](../../../../../importance-sampling.md), whose dangerous denominator is $q$. Choosing a normalized $q$ restricted to a well-covered posterior region is allowed, although a very small region can make most draws contribute zero and increase [variance](../../../../../variance-split.md). Taking $q=p(\theta)$ gives the [Harmonic mean estimator of Bayesian model evidence](../../../../../harmonic-mean-estimator-of-bayesian-model-evidence.md), illustrating why very small [likelihood](../../../../../likelihood-function.md) values can cause severe instability.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
