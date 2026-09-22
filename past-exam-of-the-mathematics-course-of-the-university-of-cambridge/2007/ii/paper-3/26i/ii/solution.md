<h1 id="26i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $X=\theta+Z$, with $Z\sim N(0,1)$ independent of the prior $\theta\sim N(0,\tau^{-1})$. Then $\lambda X-\theta=(\lambda-1)\theta+\lambda Z$, so

$$
\boxed{r(\Pi_\tau,d_\lambda)=\lambda^2+(1-\lambda)^2/\tau.}
$$

Completing the square in the joint density gives **$\theta\mid X\sim N(X/(1+\tau),1/(1+\tau))$**. Thus the Bayes rule is $d_{1/(1+\tau)}$, with [Bayes risk](../../../../../../bayes-risk.md) $1/(1+\tau)$. The rule $d_1=X$ has integrated risk one for every $\tau>0$, so its excess [Bayes risk](../../../../../../bayes-risk.md) is $\tau/(1+\tau)\to0$ as $\tau\downarrow0$. The priors remain proper at every positive $\tau$. Therefore **$d_1$ is extended Bayes**, without treating the limiting improper flat prior as a proper Bayes prior.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [26I](../../26i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
