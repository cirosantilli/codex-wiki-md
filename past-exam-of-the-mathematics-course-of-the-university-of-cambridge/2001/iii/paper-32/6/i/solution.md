<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [Edgeworth expansion](../../../../../../edgeworth-series.md) refines a central [normal approximation](../../../../../../normal-approximation.md) using higher [cumulants](../../../../../../cumulant.md). Let $Y_i$ be independent and identically distributed, with mean $\mu$, positive [variance](../../../../../../variance-split.md) $\sigma^2$, and [cumulants](../../../../../../cumulant.md) $\kappa_r$. Define

$$
Z_n=\frac{\sqrt n(\bar Y-\mu)}\sigma,\qquad
\gamma_3=\frac{\kappa_3}{\sigma^3},\qquad
\gamma_4=\frac{\kappa_4}{\sigma^4}.
$$

The logarithm of its [characteristic function](../../../../../../characteristic-function.md) has the expansion

$$
\log\mathbb E e^{itZ_n}
=-\frac{t^2}{2}+\frac{\gamma_3(it)^3}{6\sqrt n}
+\frac{\gamma_4(it)^4}{24n}+\cdots.
$$

Expanding the exponential adds the squared cubic term $\gamma_3^2(it)^6/(72n)$. Fourier inversion turns $(it)^r e^{-t^2/2}$ into $\phi(z)H_r(z)$, where the probabilists' [Hermite polynomials](../../../../../../hermite-polynomial.md) satisfy

$$
H_r(z)=(-1)^r\phi(z)^{-1}\frac{d^r}{dz^r}\phi(z).
$$

Thus the density [Edgeworth expansion](../../../../../../edgeworth-series.md) through order $n^{-1}$ is

$$
\boxed{f_{Z_n}(z)=\phi(z)\left[
1+\frac{\gamma_3}{6\sqrt n}H_3(z)
+\frac1n\left\{\frac{\gamma_4}{24}H_4(z)
+\frac{\gamma_3^2}{72}H_6(z)\right\}\right]+o(n^{-1}).}
$$

Here $H_3=z^3-3z$, $H_4=z^4-6z^2+3$, and $H_6=z^6-15z^4+45z^2-15$. Since $(\phi H_{r-1})'=-\phi H_r$, the corresponding [cumulative distribution function](../../../../../../cumulative-distribution-function.md) expansion is

$$
\Pr(Z_n\le z)=\Phi(z)-\phi(z)\left[
\frac{\gamma_3}{6\sqrt n}H_2(z)
+\frac1n\left\{\frac{\gamma_4}{24}H_3(z)
+\frac{\gamma_3^2}{72}H_5(z)\right\}\right]+o(n^{-1}).
$$

These remainder statements require adequate moments and smooth nonlattice conditions allowing transform inversion and error control, not merely a formal cumulant expansion. The density version needs the corresponding local smoothness. A symmetric distribution has $\gamma_3=0$, removing the first correction. Truncation can produce negative densities or nonmonotone distribution functions far from the center; it is not automatically a uniformly reliable relative tail approximation. A lattice distribution needs its lattice correction.

A [Laplace approximation](../../../../../../laplace-approximation.md) instead approximates an integral dominated by a sharp maximum. Suppose $h$ has a unique interior maximizer $\widehat\theta\in\mathbb R^d$, with $A=-h''(\widehat\theta)$ positive definite, and the integral is localized near that point. For smooth amplitude $g$,

$$
I_n=\int g(\theta)e^{nh(\theta)}\,d\theta.
$$

Set $\theta=\widehat\theta+z/\sqrt n$. A [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
n\{h(\theta)-h(\widehat\theta)\}
=-\tfrac12z^{\mathsf T}Az+O(n^{-1/2}\|z\|^3).
$$

Expanding $g$ and integrating the resulting [Gaussian integral](../../../../../../gaussian-integral.md) gives

$$
\boxed{I_n\sim e^{nh(\widehat\theta)}g(\widehat\theta)
\left(\frac{2\pi}{n}\right)^{d/2}|A|^{-1/2}.}
$$

Under sufficient smoothness and localization the relative correction is $O(n^{-1})$: odd terms of order $n^{-1/2}$ integrate to zero over the limiting symmetric Gaussian region. Higher terms use derivatives of $h,g$ and Gaussian moments.

For a [likelihood function](../../../../../../likelihood-function.md) with $\ell_n=nh$ and a smooth positive [prior density](../../../../../../prior-density.md), this gives the integrated likelihood approximation

$$
\int e^{\ell_n(\theta)}\pi(\theta)\,d\theta
\simeq e^{\ell_n(\widehat\theta)}\pi(\widehat\theta)
(2\pi)^{d/2}|j(\widehat\theta)|^{-1/2},
$$

where $j=-\ell_n''$ is the [observed information](../../../../../../observed-fisher-information.md). Ratios of such integrals give [posterior expectation by Laplace approximation](../../../../../../posterior-expectation-by-laplace-approximation.md); the same method is useful when integrating nuisance variables. Boundary maxima, singular [Hessian matrices](../../../../../../hessian-matrix.md), nonlocalized tails and several dominant modes require altered formulas, with contributions summed when appropriate.

Both methods start with a quadratic Gaussian approximation and then retain higher-order terms. The [Edgeworth series](../../../../../../edgeworth-series.md) corrects a sampling distribution through its [cumulants](../../../../../../cumulant.md) and Fourier inversion; [Laplace's method](../../../../../../laplace-s-method.md) corrects an integral through local derivatives at its dominant point. Neither should be confused with simply replacing a likelihood by a normalized posterior density.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
