<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md) gives

$$
\boxed{f_*\mid\mathbf y,\theta\sim\mathcal N(m_n(x_*),v_n(x_*))},
$$

where

$$
\boxed{m_n(x_*)=k_*^TC^{-1}\mathbf y,\qquad v_n(x_*)=k_{**}-k_*^TC^{-1}k_*}.
$$

For a direct justification, form $R=f_*-k_*^TC^{-1}\mathbf y$. It is jointly [Gaussian](../../../../../normal-distribution.md) with $\mathbf y$, has zero [mean](../../../../../expected-value-split.md), and satisfies

$$
\operatorname{Cov}(R,\mathbf y)=k_*^T-k_*^TC^{-1}C=0,\qquad\operatorname{Var}(R)=k_{**}-k_*^TC^{-1}k_*.
$$

The [independence of uncorrelated jointly normal variables](../../../../../independence-of-uncorrelated-jointly-normal-variables.md) therefore makes $R$ independent of $\mathbf y$. Conditional on $\mathbf y$, only the displayed affine shift remains, proving the result. This is the latent-function [posterior variance](../../../../../posterior-variance.md); a new observation $y_*=f_*+\sigma\epsilon_*$ with fresh independent noise has [predictive variance](../../../../../predictive-variance.md) $v_n(x_*)+\sigma^2$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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
