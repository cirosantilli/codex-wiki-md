# Fourier series of periodic hyperbolic sine and cosine

↑ **Parent:** [Fourier series](fourier-series-split.md)

For $\beta>0$, periodically extend $\cosh(\beta x)$ and $\sinh(\beta x)$ from $-1<x\leq1$ with period $2$. Their [Fourier series](fourier-series-split.md) are

$$
\cosh(\beta x)=\frac{\sinh\beta}{\beta}+2\beta\sinh\beta\sum_{n=1}^{\infty}\frac{(-1)^n\cos(n\pi x)}{\beta^2+n^2\pi^2},
$$

and, away from odd integers,

$$
\sinh(\beta x)=2\pi\sinh\beta\sum_{n=1}^{\infty}\frac{(-1)^{n+1}n\sin(n\pi x)}{\beta^2+n^2\pi^2}.
$$

The first identity follows by [integration](integral-split.md) of $\cosh(\beta x)\cos(n\pi x)$ on $[-1,1]$, using the [antiderivative](antiderivative.md)

$$
\frac{\beta\sinh(\beta x)\cos(n\pi x)+n\pi\cosh(\beta x)\sin(n\pi x)}{\beta^2+n^2\pi^2}.
$$

For the second identity, [integration by parts](integration-by-parts.md) and $d\cosh(\beta x)/dx=\beta\sinh(\beta x)$ show that its sine coefficient is $-n\pi/\beta$ times the first series' cosine coefficient. This avoids assuming that a [Fourier series](fourier-series-split.md) can always be differentiated term by term. The periodic [hyperbolic cosine](hyperbolic-cosine.md) is continuous, so its series converges to it everywhere. The periodic [hyperbolic sine](hyperbolic-sine.md) has a [jump discontinuity](jump-discontinuity.md) at each odd integer: the [Dirichlet-Jordan convergence theorem](dirichlet-jordan-convergence-theorem.md) gives the average of its two limiting values, namely zero, there. Both identities hold in the sense of [mean-square convergence](convergence-in-l2.md), which suffices for [Parseval's identity](parseval-identity.md).

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/15/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/18/a/solution.md)
