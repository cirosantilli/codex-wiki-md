<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the variables are [independent](../../../../../../independent-random-variables.md), the moment-generating function of the sum factors. Whenever $|\lambda|<1/\max_i\alpha_i$,

$$
\mathbb E\exp\left(\lambda\sum_{i=1}^nX_i\right)
=\prod_{i=1}^n\mathbb Ee^{\lambda X_i}
\leq\exp\left(\frac{\lambda^2}{2}\sum_{i=1}^n\nu_i\right).
$$

Therefore $\sum_iX_i$ is sub-exponential with parameters

$$
\boxed{\nu=\sum_{i=1}^n\nu_i,
\qquad
\alpha=\max_{1\leq i\leq n}\alpha_i.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
