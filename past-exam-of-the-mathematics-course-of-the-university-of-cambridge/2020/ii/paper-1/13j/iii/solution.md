<h1 id="13j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Because `model2` uses a [logarithmic transformation](../../../../../../logarithmic-transformation.md), the logarithm of the payment ratio is the difference of two predicted log payments. The cars have equal `Brand` and `Bonus` values and differ by one `Kilometres` level, so its fitted mean is the displayed mileage [regression coefficient](../../../../../../regression-coefficient.md), $\widehat\beta_K=0.057132$.

For two independent future payments, the [prediction interval](../../../../../../prediction-interval.md) must include both the [standard error](../../../../../../standard-error.md) $0.032654$ of $\widehat\beta_K$ and two independent residual errors. The estimated variance of the predicted log ratio is therefore

$$
0.032654^2+2(0.7817)^2.
$$

Using the residual degrees of freedom shown in the output, a 95% [prediction interval for a ratio of log-normal responses](../../../../../../prediction-interval-for-a-ratio-of-log-normal-responses.md) is

$$
\boxed{
\left[
\exp\!\left\{0.057132-t_{284,0.975}\sqrt{0.032654^2+2(0.7817)^2}\right\},
\exp\!\left\{0.057132+t_{284,0.975}\sqrt{0.032654^2+2(0.7817)^2}\right\}
\right].
}
$$

With $t_{284,0.975}\simeq1.97$, this is approximately $[0.120,9.33]$. The interval is wide because it predicts the ratio of two individual future payments; an interval for the ratio of their fitted mean responses would omit the $2\widehat\sigma^2$ term.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
