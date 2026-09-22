<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [reciprocal importance sampling](../../../../../reciprocal-importance-sampling.md), use the same $r$ and $Z$ but draw from the [posterior density](../../../../../posterior-density.md) $\pi=r/Z$. Here the support requirement is reversed: the normalized density $q$ must vanish almost everywhere that $r=0$. Thus $q$ may be confined to a subset of the [posterior distribution](../../../../../bayesian-posterior.md)'s support. For $V=q(\theta)/r(\theta)$,

$$
\mathbb E_\pi V=\int_{\{r>0\}}\frac{q(\theta)}{r(\theta)}\frac{r(\theta)}Z\,d\theta=\frac1Z\int q(\theta)\,d\theta=\frac1Z.
$$

Consequently,

$$
\boxed{\mathbb E\bigl[\widehat p_2(\mathcal D)^{-1}\bigr]=p(\mathcal D)^{-1}}.
$$

It is the estimate of the reciprocal that is an [unbiased estimator](../../../../../unbiased-estimator.md). Taking its reciprocal does not generally produce an [unbiased estimator](../../../../../unbiased-estimator.md) of $Z$: inversion is nonlinear. In fact, when the average is strictly positive and the relevant [expectation](../../../../../expected-value-split.md) exists, [Jensen's inequality](../../../../../jensen-s-inequality.md) gives $\mathbb E\widehat p_2\geq Z$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
