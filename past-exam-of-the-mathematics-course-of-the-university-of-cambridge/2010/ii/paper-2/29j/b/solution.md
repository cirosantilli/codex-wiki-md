<h1 id="29j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the usual state-space assumption that the prior $X_0$ is independent of future process and observation noises. Suppose inductively $X_t\mid\mathcal Y_t\sim N(\hat X_t,V_t)$. Prediction through the linear dynamics gives $X_{t+1}\mid\mathcal Y_t\sim N(A\hat X_t,M_t)$, where $M_t=AV_tA^T+\Sigma_\varepsilon$. The pair $(X_{t+1},Y_{t+1})$ is conditionally [multivariate normal](../../../../../../multivariate-normal-distribution.md), with means $A\hat X_t,CA\hat X_t$, cross covariance $M_tC^T$, and observation covariance $R_t=\Sigma_\eta+CM_tC^T$. Applying part (a) gives the [Kalman filter](../../../../../../kalman-filter.md)

$$
\boxed{\begin{aligned}
\hat X_{t+1}&=A\hat X_t+M_tC^TR_t^{-1}(Y_{t+1}-CA\hat X_t),\\
V_{t+1}&=M_t-M_tC^TR_t^{-1}CM_t.
\end{aligned}}
$$

This proves the inductive Gaussian assertion. The inverse requires nonsingular innovation covariance, as in the printed formula. Importantly, prediction uses $A\hat X_t$: the TeX conversion drops this $A$ in one place, whereas the original PDF includes it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29J](../../29j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
