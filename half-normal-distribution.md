# Half-normal distribution

↑ **Parent:** [Normal distribution](normal-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Half-normal_distribution)

The [half-normal distribution](half-normal-distribution.md) describes the [absolute value](absolute-value.md) of a centered [Gaussian random variable](gaussian-random-variable.md). Its unit-scale version is $H=|Z|$ for a [standard normal random variable](standard-normal-random-variable.md) $Z$. It folds the negative half of the [standard normal distribution](standard-normal-distribution.md) onto the positive half, retaining the size of a deviation while discarding its sign. If a centered [Gaussian random variable](gaussian-random-variable.md) models [measurement error](measurement-error.md), its magnitude therefore has a [half-normal distribution](half-normal-distribution.md).

$$
f_H(x)=\begin{cases}2\phi(x)=\sqrt{\dfrac2\pi}e^{-x^2/2},&x\geq0,\\0,&x<0,\end{cases}
\qquad
F_H(x)=\begin{cases}2\Phi(x)-1,&x\geq0,\\0,&x<0.\end{cases}
$$

Here $\phi$ is the [standard normal density](standard-normal-density.md) and $\Phi$ is the [standard normal distribution function](standard-normal-distribution-function.md). For $x\geq0$, the [event](event.md) $H\leq x$ is $-x\leq Z\leq x$, so the [symmetric probability distribution](symmetric-probability-distribution.md) of $Z$ gives $F_H(x)=\Phi(x)-\Phi(-x)=2\Phi(x)-1$. The upper-tail [probability](probability.md) is therefore $\mathbb P(H>x)=2(1-\Phi(x))$. For example, $\mathbb P(H\leq1)\approx0.6826894921$. The doubled [probability density function](probability-density-function.md) integrates to one on $[0,\infty)$, and $\mathbb P(H=0)=0$.

The [mean](expected-value.md) and [variance](variance-split.md) of the unit-scale [half-normal distribution](half-normal-distribution.md) are

$$
\mathbb E[H]=\sqrt{\frac2\pi},\qquad\operatorname{Var}(H)=1-\frac2\pi.
$$

For a short derivation, $\mathbb E[H]=2\int_0^\infty x\phi(x)\,dx=2\phi(0)$ because $\phi'(x)=-x\phi(x)$, while $H^2=Z^2$ gives $\mathbb E[H^2]=1$. More generally, $\sigma|Z|$ for $\sigma>0$ has a [half-normal distribution](half-normal-distribution.md) with [probability density function](probability-density-function.md) $2\phi(x/\sigma)/\sigma$ for $x\geq0$. Its [mean](expected-value.md) is $\sigma\sqrt{2/\pi}$ and its [variance](variance-split.md) is $\sigma^2(1-2/\pi)$; here $\sigma$ is the scale of the underlying [Gaussian random variable](gaussian-random-variable.md), not the [standard deviation](standard-deviation.md) of its [absolute value](absolute-value.md).

**Table of contents**

- [Radial-ratio independence of two half-normal variables](radial-ratio-independence-of-two-half-normal-variables.md)

## ↑ Ancestors (7)

1. [Normal distribution](normal-distribution.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Half-Cauchy distribution](half-cauchy-distribution.md)
- [Half-normal distribution](half-normal-distribution.md)
- [Maximally prograde stellar distribution](maximally-prograde-stellar-distribution.md)
- [Normal rejection sampling with an exponential envelope](normal-rejection-sampling-with-an-exponential-envelope.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-58/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-223/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/28k/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/28k/e/solution.md)
