<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $n\ge2$, $k\ge0$, a proper [prior density](../../../../../../prior-density.md) $\pi$ supported on nonnegative mutation rates, and [independence](../../../../../../independent-random-variables.md) of the mutation-rate prior from the neutral genealogy. Put

$$
q(t)=\prod_{j=2}^n\lambda_j e^{-\lambda_jt_j}\mathbf1_{\{t_j>0\}},\qquad
L(t)=\sum_{j=2}^n jt_j,\qquad
w_k(\theta,t)=e^{-\theta L(t)/2}\frac{(\theta L(t)/2)^k}{k!}.
$$

By [Bayes' theorem](../../../../../../bayes-theorem.md), the joint posterior is

$$
\boxed{f(\theta,t\mid S=k)=\frac{\pi(\theta)q(t)w_k(\theta,t)}{Z_k},\quad
Z_k=\int_0^\infty\!\pi(u)\int_{(0,\infty)^{n-1}}q(t)w_k(u,t)\,dt\,du.}
$$

The normalizing constant is the prior predictive [probability](../../../../../../probability.md) $P(S=k)$ and must be positive. For $k=0$, interpret the factor $(\theta L/2)^0$ as 1 even at zero. If $n=1$, there are no [segregating sites](../../../../../../segregating-site.md): $S=0$ surely, so that case supplies no information about $\theta$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
