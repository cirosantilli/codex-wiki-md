<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Series 1 wanders over a changing level rather than fluctuating around a stable local mean. Its sample [autocorrelation function](../../../../../../autocorrelation.md) is strongly positive and decreases very slowly. This is the usual diagnostic evidence for an ordinary [unit root](../../../../../../unit-root.md): an autoregressive polynomial containing $1-z$, with a zero at $z=1$, and a stationary model after first [differencing](../../../../../../differencing.md). The plots support an integrated model, rather than specifying the number of its remaining stationary autoregressive or moving-average terms.

Series 2 has a pronounced oscillation with period about six observations. Its sample [autocorrelation](../../../../../../autocorrelation.md) alternates between large positive and negative values with little damping: approximately positive at multiples of six and negative halfway between. Together with the changing amplitude, this suggests a conjugate pair of unit-circle zeros near

$$
\boxed{z=e^{\pm i\pi/3}.}
$$

The associated real autoregressive factor is $1-2\cos(\pi/3)z+z^2=1-z+z^2$. A targeted filter $1-B+B^2$ removes this pair; the broader [seasonal difference operator](../../../../../../seasonal-difference-operator.md) $1-B^6$ also contains it but introduces additional [differencing](../../../../../../differencing.md) factors. This is the [oscillatory unit-root diagnosis from an undamped sample autocorrelation](../../../../../../oscillatory-unit-root-diagnosis-from-an-undamped-sample-autocorrelation.md).

Thus **Series 1 suggests a zero at 1; Series 2 suggests a conjugate pair on the unit circle at a seasonal frequency**. These are model diagnoses, not deductions of exact roots from a finite sample. A stationary model very close to a [unit root](../../../../../../unit-root.md) can look similar, and an undamped periodic [covariance](../../../../../../covariance.md) can also arise from a stationary random sinusoid. The figure does not identify exact orders or prove nonstationarity by itself.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
