<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Using the representation $X=\mu+\sigma Z$ and [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md),

$$
\frac{\partial f}{\partial\mu}=\mathbb E[U'(X)]>0
$$

because $U$ is strictly increasing. Similarly, part (a) gives

$$
\frac{\partial f}{\partial\sigma}
=\mathbb E[ZU'(X)]
=\sigma\mathbb E[U''(X)]\leq0
$$

because a twice differentiable [concave function](../../../../../../concave-function.md) has $U''\leq0$. Therefore

$$
\boxed{f_\mu>0,\qquad f_\sigma\leq0}.
$$

In [mean-variance optimization](../../../../../../modern-portfolio-theory.md), an expected-utility investor consequently prefers a larger mean at fixed standard deviation and a smaller variance at fixed mean. This is the usual risk-averse ordering of Gaussian payoffs.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
