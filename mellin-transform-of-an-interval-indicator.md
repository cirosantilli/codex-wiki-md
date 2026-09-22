# Mellin transform of an interval indicator

↑ **Parent:** [Mellin transform](mellin-transform.md)

For $0<b<c<\infty$, the [indicator function](indicator-function.md) $f(x)=\mathbf1_{[b,c]}(x)$ has [Mellin transform](mellin-transform.md)

$$
\mathcal Mf(s)=\begin{cases}(c^s-b^s)/s,&s\ne0,\\ \log(c/b),&s=0.\end{cases}
$$

The [interval](interval-mathematics.md) stays away from both zero and infinity, so the [integral](integral.md) is [absolutely convergent](absolute-convergence.md) for every [complex number](complex-number.md) $s$. Its [Mellin fundamental strip](fundamental-strip-of-a-mellin-transform.md) is the whole [complex plane](complex-plane.md). Evaluating the [antiderivative](antiderivative.md) $x^s/s$ proves the formula for $s\ne0$; at $s=0$, integrating $1/x$ gives the real [natural logarithm](natural-logarithm.md) $\log(c/b)$. The apparent division by zero is a [removable singularity](removable-singularity.md), since $c^s-b^s=s(\log c-\log b)+O(s^2)$ by the [Taylor series](taylor-series.md) of the [exponential function](exponential-function.md). The transform is an [entire function](entire-function.md).

For example, $\mathbf1_{[1,4]}$ gives $(4^s-1)/s$ with value $\log4$ at zero. On $s=i\tau$, the [Mellin transform](mellin-transform.md) sums oscillations over the width $\log4$ of the [interval](interval-mathematics.md) in [natural logarithm](natural-logarithm.md) coordinates; this is the same cancellation mechanism as in the [Fourier transform of an interval indicator](fourier-transform-of-an-interval-indicator.md).

## ↑ Ancestors (6)

1. [Mellin transform](mellin-transform.md)
2. [Integral transform](integral-transform.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Mellin transform](mellin-transform.md)
- [Mellin transform in logarithmic coordinates](mellin-transform-in-logarithmic-coordinates.md)
- [Scaling property of the Mellin transform](scaling-property-of-the-mellin-transform.md)
