<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The upper envelope for $\psi$ implies

$$
e^{\psi(\theta x)}
\leq1+\theta x+\frac{\theta^2x^2}{2}.
$$

Writing $\mu_i=\mathbb E[X_i]$, taking expectations, and using $1+u\leq e^u$ gives

$$
\mathbb E e^{\psi(\theta X_i)-\theta\mu_i}
\leq e^{-\theta\mu_i}
\left(1+\theta\mu_i+\frac{\theta^2}{2}\mathbb E[X_i^2]\right)
\leq\exp\left(\frac{\theta^2}{2}\mathbb E[X_i^2]\right).
$$

[Independent random variables](../../../../../../independent-random-variables.md) then yield

$$
\boxed{
\mathbb E\exp\left\{\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mathbb E[X_i])\right\}
\leq
\exp\left\{\frac{\theta^2}{2}\sum_{i=1}^n\mathbb E[X_i^2]\right\}}.
$$

Applying the lower envelope to $-\psi(\theta x)$ similarly gives

$$
\boxed{
\mathbb E\exp\left\{\sum_{i=1}^n
(\theta\mathbb E[X_i]-\psi(\theta X_i))\right\}
\leq
\exp\left\{\frac{\theta^2}{2}\sum_{i=1}^n\mathbb E[X_i^2]\right\}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
