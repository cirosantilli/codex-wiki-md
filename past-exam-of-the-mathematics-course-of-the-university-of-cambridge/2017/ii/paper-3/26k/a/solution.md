<h1 id="26k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [score function](../../../../../../informant-function.md) is

$$
 S_n(\theta)=\frac{d}{d\theta}\log\prod_{i=1}^nf(X_i,\theta)=\sum_{i=1}^n\frac{\partial_\theta f(X_i,\theta)}{f(X_i,\theta)}.
$$

With common parameter-independent support and justified differentiation under the [integral](../../../../../../integral.md), $\mathbb E_\theta[\partial_\theta\log f(X_1,\theta)]=\int\partial_\theta f(x,\theta)dx=\partial_\theta1=0$. Linearity then gives $\boxed{\mathbb E_{\theta_0}S_n(\theta_0)=0}$. These regularity conditions exclude, for example, moving-support uniform models.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
