<h1 id="29l/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the simple null, the restricted maximum-likelihood estimator is $\widetilde\theta=\theta_0$, and hence

$$
T_n=(n^{-1/2}S_n(\theta_0))^T
I_1(\theta_0)^{-1}
(n^{-1/2}S_n(\theta_0)).
$$

The individual scores are independent, have mean zero by part (ii), and have covariance $I_1(\theta_0)$. The multivariate central limit theorem gives

$$
n^{-1/2}S_n(\theta_0)
\xrightarrow{d}N_p(0,I_1(\theta_0)).
$$

After multiplying by $I_1(\theta_0)^{-1/2}$, the limit is standard normal in $\mathbb R^p$. The continuous mapping theorem therefore yields

$$
\boxed{T_n\xrightarrow{d}\chi_p^2.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [29L](../../../29l.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
