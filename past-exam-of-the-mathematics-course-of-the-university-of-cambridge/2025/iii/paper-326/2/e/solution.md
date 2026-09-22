<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For observed $v\in\mathbb R^N$, the Gaussian likelihood is

$$
\boxed{
\pi(v\mid u)
=(2\pi\sigma^2)^{-N/2}
\exp\left[-\frac1{2\sigma^2}\|v-G(u)\|_{\mathbb R^N}^2\right]}.
$$

Thus the [Bayesian inverse problem](../../../../../../bayesian-inverse-problem.md) is to determine the posterior distribution of $U$ given $V=v$. With

$$
\Phi(u;v)=\frac1{2\sigma^2}\|v-G(u)\|^2,
$$

Bayes' formula gives

$$
\boxed{
\frac{d\mu^v}{d\mu_0}(u)
=\frac1{Z(v)}e^{-\Phi(u;v)},
\qquad
Z(v)=\int_Xe^{-\Phi(u;v)}\,d\mu_0(u)}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
