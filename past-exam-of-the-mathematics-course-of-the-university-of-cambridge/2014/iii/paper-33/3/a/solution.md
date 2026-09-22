<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mu=\alpha/\gamma$ and $\phi=1/\alpha$. With $\theta=-\gamma/\alpha=-1/\mu<0$, the [Gamma exponential dispersion family](../../../../../../gamma-exponential-dispersion-family.md) representation is

$$
\log f(y)=\frac{y\theta-b(\theta)}{\phi}+c(y,\phi),\qquad b(\theta)=-\log(-\theta),
$$

where

$$
c(y,\phi)=\left(\frac1\phi-1\right)\log y-\frac1\phi\log\phi-\log\Gamma(1/\phi).
$$

Substitution gives the original gamma density, so both unknown parameters are included. The [exponential-family derivative identities](../../../../../../exponential-family-derivative-identities.md) yield $\mu=b'(\theta)=-1/\theta$ and $b''(\theta)=1/\theta^2=\mu^2$. Therefore

$$
\boxed{V(\mu)=\mu^2,\quad\phi=\alpha^{-1},\quad\operatorname{Var}(Y)=\phi\mu^2.}
$$

The exact natural-parameter [canonical link function](../../../../../../canonical-link-function.md) is $g_{\rm can}(\mu)=-1/\mu$. **The usual inverse-link convention is $g(\mu)=1/\mu$**, as used by the printed R fits; multiplying the link and coefficients by $-1$ gives the natural-parameter convention. The sign convention changes neither the fitted means nor the weight matrix below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
