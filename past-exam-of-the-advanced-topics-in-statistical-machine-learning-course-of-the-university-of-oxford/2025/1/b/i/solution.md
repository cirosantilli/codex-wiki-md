<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $r(\theta)=p(\mathcal D\mid\theta)p(\theta)$ and $Z=\int r(\theta)\,d\theta$. The [support condition for importance sampling](../../../../../support-condition-for-importance-sampling.md) is essential: $q(\theta)>0$ almost everywhere that $r(\theta)>0$. For one draw $\theta\sim q$, the [importance weight](../../../../../importance-weight.md) $W=r(\theta)/q(\theta)$ satisfies

$$
\mathbb E_q W=\int_{\{q>0\}}\frac{r(\theta)}{q(\theta)}q(\theta)\,d\theta=Z.
$$

By [linearity of expectation](../../../../../linearity-of-expectation.md),

$$
\boxed{\mathbb E\widehat p_1(\mathcal D)=\frac1T\sum_{t=1}^T\mathbb E_qW_t=Z=p(\mathcal D)}.
$$

This proves that it is an [unbiased estimator](../../../../../unbiased-estimator.md). If the proposal omits a region of positive target mass, the [expected value](../../../../../expected-value-split.md) instead misses that region's contribution; the unconditional unbiasedness claim needs the stated [support condition for importance sampling](../../../../../support-condition-for-importance-sampling.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
