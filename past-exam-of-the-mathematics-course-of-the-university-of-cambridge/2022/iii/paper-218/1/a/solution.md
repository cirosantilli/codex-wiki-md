<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\phi=1/\gamma$ and $\theta=-1/\alpha$. The density can be written

$$
f(y;\theta,\phi)
=\exp\left[
\frac{y\theta-b(\theta)}{\phi}+c(y,\phi)
\right],
\qquad
b(\theta)=-\log(-\theta),
$$

where

$$
c(y,\phi)
=-\log\Gamma(1/\phi)-\phi^{-1}\log\phi
+(\phi^{-1}-1)\log y.
$$

Thus this is an [exponential dispersion family](../../../../../../exponential-dispersion-model.md). Its derivative identities give

$$
\mathbb EY=b'(\theta)=-\frac1\theta=\alpha,
\qquad
\operatorname{Var}(Y)=\phi b''(\theta)
=\phi\alpha^2=\frac{\alpha^2}{\gamma}.
$$

The [variance function](../../../../../../variance-function.md) is $V(\mu)=\mu^2$. In the usual Gamma-GLM convention the canonical inverse link is

$$
g(\mu)=\frac1\mu;
$$

it differs by a minus sign from the natural parameter $\theta=-1/\mu$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
