# Convolution of a Cauchy distribution and a uniform distribution

↑ **Parent:** [Convolution of independent random variables](convolution-of-independent-random-variables.md)

Let $X$ have the [Standard Cauchy distribution](standard-cauchy-distribution.md) and let $Y$, independently, have the [uniform distribution](continuous-uniform-distribution.md) on $[-h,h]$, where $h>0$. The [convolution of probability densities](convolution-of-independent-random-variables.md) gives the [probability density](probability-density.md) of $Z=X+Y$ as

$$
p_h(z)=\frac{1}{2h\pi}\int_{-h}^{h}\frac{dy}{1+(z-y)^2}=\frac{\arctan(z+h)-\arctan(z-h)}{2h\pi}.
$$

This is an [even function](even-function.md). Its [derivative](derivative.md) is

$$
p_h'(z)=\frac{-2z}{\pi[1+(z+h)^2][1+(z-h)^2]},
$$

so its unique [mode](mode-statistics.md) is zero. Its tails satisfy $p_h(z)\sim1/(\pi z^2)$ as $|z|\to\infty$: multiplying the integral by $z^2$ makes the integrand converge uniformly to $1$ on the bounded interval $[-h,h]$. Consequently both positive and negative parts of the first moment diverge, so its [expected value](expected-value-split.md) does not exist. The symmetric [Cauchy principal value](cauchy-principal-value.md) of that moment is zero, which is a different assertion. Adding a bounded independent displacement smooths the [probability density](probability-density.md) without removing the divergent first moment of the [Cauchy distribution](cauchy-distribution.md).

## ↑ Ancestors (8)

1. [Convolution of independent random variables](convolution-of-independent-random-variables.md)
2. [Joint probability distribution](joint-probability-distribution.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/14/d/ii/solution.md)
