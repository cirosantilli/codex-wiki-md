<h1 id="5/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

In the [martingale residual](../../../../../../../martingale-residual.md)

$$
y_i=v_i-e^{\widehat\beta z_i}\widehat H_0(x_i),
$$

$v_i$ is the observed event count up to the end of the individual's follow-up: 1 for a recorded event and 0 for [right censoring](../../../../../../../right-censoring.md). The second term is the fitted [counting-process compensator](../../../../../../../compensator-of-a-counting-process.md), obtained by integrating that individual's fitted [hazard function](../../../../../../../hazard-function.md) while they remain at risk:

$$
\int_0^{x_i}e^{\widehat\beta z_i}\,d\widehat H_0(u)
=e^{\widehat\beta z_i}\widehat H_0(x_i).
$$

Thus **the residual is observed events minus the fitted cumulative event intensity over follow-up**. The fitted intensity is not an event probability and can exceed 1. Positive values indicate more events than predicted over that observed exposure; negative values indicate fewer. A [right-censored](../../../../../../../right-censoring.md) individual has a nonpositive residual. With true model parameters and [independent censoring](../../../../../../../independent-censoring.md), the underlying observed-minus-compensator process is a [martingale](../../../../../../../martingale-split.md); fitted terminal residuals are not independent identically distributed errors.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
