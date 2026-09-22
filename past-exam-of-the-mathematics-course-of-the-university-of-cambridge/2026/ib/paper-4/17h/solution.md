<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

The MLE is $\hat\theta=n/S$, $S=\sum X_i$. Since $S\sim\Gamma(n,\theta)$, $\theta S\sim\Gamma(n,1)$ (in general $\gamma Y\sim\Gamma(\beta,\lambda/\gamma)$). If $q_r$ is the $r$-quantile of $\Gamma(n,1)$, a central confidence interval is $[(q_{\alpha/2}/n)\hat\theta,(q_{1-\alpha/2}/n)\hat\theta]$. A $\Gamma(\beta,\lambda)$ prior yields posterior $\Gamma(\beta+n,\lambda+S)$ and mean $\tilde\theta=(\beta+n)/(\lambda+S)$. With $q_r\prime$ the quantiles of $\Gamma(\beta+n,1)$, take $l\prime=q_{\alpha/2}\prime/(\beta+n)$ and $u\prime=q_{1-\alpha/2}\prime/(\beta+n)$.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
