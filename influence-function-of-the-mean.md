# Influence function of the mean

↑ **Parent:** [Influence function](influence-function.md)

For the [statistical functional](statistical-functional.md) $T(F)=\mu=\mathbb E_F X$, assuming $\mathbb E_F|X|<\infty$, the contaminated [mean](expected-value.md) is exactly

$$
T(F_{\varepsilon,x})=(1-\varepsilon)\mu+\varepsilon x.
$$

Thus the [influence function of the mean](influence-function-of-the-mean.md) is $x-\mu$, and its [gross-error sensitivity](gross-error-sensitivity.md) is infinite on an unbounded sample space. The [linear approximation](linear-approximation.md) is exact here: any fixed positive contamination fraction allows an arbitrarily large change by moving $x$ far enough. No finite second [moment](moment.md) is needed for this [derivative](derivative.md), although a finite [variance](variance-split.md) is needed for the usual [central limit theorem](central-limit-theorem.md) for the [sample mean](sample-mean.md).

For comparison, the [influence function of the sample median](influence-function-of-the-sample-median.md) is

$$
\operatorname{IF}(x;\operatorname{Med},F)=\frac{\operatorname{sgn}(x-m)}{2f(m)},\qquad x\ne m,
$$

when the [median](median.md) $m$ is unique and the [probability density function](probability-density-function.md) $f$ is positive and continuous at $m$. The [sign function](sign-function.md) records which side of $m$ receives the contaminating mass. The [influence function of a quantile](influence-function-of-a-quantile.md) supplies the short derivation. With the generalized-inverse [quantile](quantile-function.md) convention, contamination exactly at $x=m$ leaves the [median](median.md) at $m$, giving derivative zero there. If $f(m)$ is very small, this bounded [influence function](influence-function.md) can still be large; if $f(m)=0$, the displayed formula is unavailable.

## ↑ Ancestors (7)

1. [Influence function](influence-function.md)
2. [Robust statistics](robust-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Influence function of the mean](influence-function-of-the-mean.md)
- [Normal-location influence curves](normal-location-influence-curves.md)
