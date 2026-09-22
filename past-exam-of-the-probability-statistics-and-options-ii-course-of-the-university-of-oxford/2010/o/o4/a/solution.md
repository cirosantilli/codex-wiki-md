<h1 id="o/o4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [likelihood](../../../../../likelihood-function.md) is $L(\theta;x)=\prod_{i=1}^nf(x_i;\theta)$, and a [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) [likelihood](../../../../../likelihood-function.md) estimator is any maximizer $\hat\theta\in\arg\max_\theta L(\theta;X)$. Write $\ell=\log L$ and score $U=\nabla_\theta\ell$. [Fisher information](../../../../../fisher-information-matrix.md) for the sample is

$$
I_n(\theta)=\mathbb E_\theta[UU^T]=-\mathbb E_\theta[\nabla_\theta^2\ell],
$$

where the equality uses the usual [differentiability](../../../../../differentiability.md) and interchange assumptions. For [independent](../../../../../independent-random-variables.md) identically distributed observations $I_n=nI_1$. Under standard interior, identifiability and regularity assumptions,

$$
\boxed{\sqrt n(\hat\theta-\theta)\Rightarrow N_d(0,I_1(\theta)^{-1}),\quad\hat\theta\approx N_d(\theta,I_n(\theta)^{-1}).}
$$

Without those assumptions the large-sample normal assertion need not hold, for example at a boundary parameter.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
