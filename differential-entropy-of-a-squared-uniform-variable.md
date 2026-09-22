# Differential entropy of a squared uniform variable

↑ **Parent:** [Differential entropy under an increasing transformation](differential-entropy-under-an-increasing-transformation.md)

Take $X$ with [continuous uniform distribution](continuous-uniform-distribution.md) on $(0,1)$ and set $Y=X^2$. This is an increasing invertible transformation on that interval. Its [cumulative distribution function](cumulative-distribution-function.md) is $F_Y(y)=\sqrt y$, giving

$$
f_Y(y)=\frac1{2\sqrt y},\qquad 0<y<1.
$$

Although the [probability density](probability-density.md) diverges near zero, it is [integrable](integrability.md). The logarithmic stretch is integrable too:

$$
h_e(Y)=h_e(X)+\int_0^1\ln(2x)\,dx
=\boxed{\ln2-1\approx-0.306853\text{ nats}.}
$$

The [inverse function](inverse-function.md) $X=\sqrt Y$ recovers every input in the interval. The changed [differential entropy](differential-entropy.md) records a changed coordinate volume, rather than a failure of recovery.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (8)

1. [Differential entropy under an increasing transformation](differential-entropy-under-an-increasing-transformation.md)
2. [Differential entropy](differential-entropy.md)
3. [Information entropy](information-entropy.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
