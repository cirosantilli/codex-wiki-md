<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret the printed expression as $d^*(x)=x/(\sigma^2\lambda)$. If $X\sim N(\theta,\sigma^2)$, the Gaussian exponential-moment formula gives

$$
R(\theta,d^*)=\mathbb E_\theta e^{-\theta X/\sigma^2}=\exp\left(-\frac{\theta^2}{\sigma^2}+\frac{\theta^2}{2\sigma^2}\right)=e^{-\theta^2/(2\sigma^2)}.
$$

Its supremum is one, attained at zero. For every rule $d$, $L(0,d(X))=1$, so $R(0,d)=1$ and $\sup_\theta R(\theta,d)\geq1$. Hence

$$
\boxed{d^*(x)=\frac{x}{\sigma^2\lambda}\text{ is minimax, with minimax risk }1.}
$$

In the language of part (b), the point-mass prior $\delta_0$ makes every rule Bayes with [Bayes risk](../../../../../../bayes-risk.md) one, and $d^*$ has exactly that worst-case risk.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
