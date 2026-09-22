<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [independent](../../../../../../independent-random-variables.md) draws $X_i$ from a normalized proposal $g$, use the [importance sampling](../../../../../../importance-sampling.md) identity

$$
\mu=\int\theta(x)f(x)\,dx
=\mathbb E_g\!\left[\theta(X)\frac{f(X)}{g(X)}\right].
$$

Thus the [unbiased estimator](../../../../../../unbiased-estimator.md) and its [variance](../../../../../../variance-split.md) are

$$
\boxed{\widehat\mu=\frac1n\sum_{i=1}^n\theta(X_i)\frac{f(X_i)}{g(X_i)},\qquad
\operatorname{Var}(\widehat\mu)=\frac1n\left[\int\frac{\theta(x)^2f(x)^2}{g(x)}\,dx-\mu^2\right].}
$$

The [probability support](../../../../../../support-of-a-probability-distribution.md) condition is $g>0$ wherever $\theta f\ne0$, and the [variance](../../../../../../variance-split.md) formula requires a finite [second moment](../../../../../../second-moment.md). Since both [probability densities](../../../../../../probability-density.md) are normalized, no self-normalization of weights is needed.

In the proposed example, normalize $g$ to $g(x)=3x^2$ on $(0,1)$. It is sampled by $X=U^{1/3}$ for uniform $U$. Taking $\theta(x)=x$ gives

$$
\boxed{\widehat\mu_g=\frac1n\sum_{i=1}^n\frac4{3\pi}\frac{\sqrt{1-X_i^2}}{X_i},
\qquad X_i\sim3x^2\mathbf1_{(0,1)}(x).}
$$

As a check, $\mu_g=\frac4\pi\int_0^1x\sqrt{1-x^2}\,dx=4/(3\pi)$. The [second moment](../../../../../../second-moment.md) of one weighted observation is

$$
\int_0^1\frac{x^2f(x)^2}{3x^2}\,dx
=\frac{16}{3\pi^2}\int_0^1(1-x^2)\,dx
=\frac{32}{9\pi^2},
$$

so $\operatorname{Var}(\widehat\mu_g)=16/(9\pi^2n)$. The weight's singularity at zero does not make this [variance](../../../../../../variance-split.md) infinite.

To prove the optimal proposal rule, apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md):

$$
\left(\int|\theta(x)|f(x)\,dx\right)^2
=\left(\int\frac{|\theta(x)|f(x)}{\sqrt{g(x)}}\sqrt{g(x)}\,dx\right)^2
\leq\int\frac{\theta(x)^2f(x)^2}{g(x)}\,dx.
$$

Equality holds when the two factors are proportional almost everywhere, giving the [minimum-variance importance distribution](../../../../../../minimum-variance-importance-distribution.md)

$$
\boxed{g_0(x)=\frac{|\theta(x)|f(x)}{\int|\theta(u)|f(u)\,du}.}
$$

For the present nonnegative integrand, normalization gives

$$
\boxed{g_0(x)=3x\sqrt{1-x^2}\quad(0<x<1).}
$$

Under this proposal, $xf(x)/g_0(x)=4/(3\pi)$ is constant, so the [variance](../../../../../../variance-split.md) is exactly zero. If sampling is wanted, its distribution function is $1-(1-x^2)^{3/2}$, with inverse $X=\sqrt{1-(1-U)^{2/3}}$. In general the optimal proposal's [normalizing constant](../../../../../../normalizing-constant.md) can itself be the unknown integral, limiting this zero-variance construction's practical use.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
