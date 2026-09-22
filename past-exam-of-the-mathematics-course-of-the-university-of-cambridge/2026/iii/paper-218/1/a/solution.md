<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expanding the exponent of the [Inverse Gaussian distribution](../../../../../../inverse-gaussian-distribution.md) gives

$$
-\frac{\lambda(y-\mu)^2}{2\mu^2y}
=\lambda\left(-\frac{y}{2\mu^2}+\frac1\mu-\frac1{2y}\right).
$$

Thus the [exponential dispersion family](../../../../../../exponential-dispersion-model.md) representation

$$
f(y;\theta,\phi)=a(y,\phi)
\exp\left\{\frac{y\theta-K(\theta)}\phi\right\}
$$

has

$$
\theta=-\frac1{2\mu^2},\qquad
K(\theta)=-\sqrt{-2\theta},\qquad
\phi=\frac1\lambda,
$$

and

$$
a(y,\phi)=\frac1{\sqrt{2\pi\phi y^3}}
\exp\left(-\frac1{2\phi y}\right).
$$

The standard cumulant identities yield

$$
\mathbb EY=K'(\theta)=\mu,qquad
\operatorname{Var}(Y)=\phi K''(\theta)=\frac{\mu^3}{\lambda}.
$$

**Hence the [variance function](../../../../../../variance-function.md) is $V(\mu)=\mu^3$, and the [canonical link function](../../../../../../canonical-link-function.md) is $g(\mu)=\theta(\mu)=-1/(2\mu^2)$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
