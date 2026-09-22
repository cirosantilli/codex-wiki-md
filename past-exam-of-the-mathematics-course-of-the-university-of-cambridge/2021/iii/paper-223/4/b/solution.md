<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Markov inequality](../../../../../../markov-inequality.md) applied to the first exponential-moment bound gives

$$
\mathbb P\left\{
\frac1\theta\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mu)\geq t
\right\}
\leq
\exp\left(-\theta t+\frac{\theta^2\sigma^2n}{2}\right).
$$

The second bound controls the lower tail. The [union bound](../../../../../../boole-s-inequality.md) therefore gives

$$
\mathbb P\left\{
\left|\frac1\theta\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mu)\right|\geq t
\right\}
\leq
2\exp\left(-\theta t+\frac{\theta^2\sigma^2n}{2}\right).
$$

Since

$$
\widehat\mu_\theta-\mu
=\frac1{n\theta}\sum_{i=1}^n
(\psi(\theta X_i)-\theta\mu),
$$

putting $L=\log(2/\delta)$,

$$
\theta=\sqrt{\frac{2L}{\sigma^2n}},
\qquad
t=\sqrt{2\sigma^2nL}
$$

makes the exponent equal to $-L$. It follows that the [Catoni mean estimator](../../../../../../catoni-mean-estimator.md) satisfies

$$
\boxed{
\mathbb P\left(
|\widehat\mu_\theta-\mu|
\geq\sigma\sqrt{\frac{2\log(2/\delta)}n}
\right)\leq\delta}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
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
