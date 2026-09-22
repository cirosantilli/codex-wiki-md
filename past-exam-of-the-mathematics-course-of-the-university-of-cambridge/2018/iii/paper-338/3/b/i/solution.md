<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat $Q$ and $B$ as mean detected counts, or as photon counts with unit [quantum efficiency](../../../../../../../quantum-efficiency.md). Let the independent patch measurements be $X\sim\operatorname{Poisson}(Q+B)$ and $Y\sim\operatorname{Poisson}(fB)$. For the specified unweighted [background subtraction](../../../../../../../background-subtraction.md) $\widehat Q=X-Y$,

$$
\mathbb E\widehat Q=Q+(1-f)B,\quad
b=\mathbb E\widehat Q-Q=(1-f)B,\quad
\operatorname{Var}\widehat Q=Q+(1+f)B.
$$

The first error is a fixed [bias of an estimator](../../../../../../../bias-of-an-estimator.md); the last expression is the sum of independent [photon shot noise](../../../../../../../photon-shot-noise.md) variances. Since $Q,B$ are already patch totals, no extra factor of the pixel count $n$ is needed, and [read noise](../../../../../../../read-noise.md) is neglected.

To obtain the systematic-error ceiling requested in the following clause, define the accuracy measure $Z$ using total root-mean-square error relative to the true source count. By the [bias-variance decomposition of mean squared error](../../../../../../../bias-variance-decomposition-of-mean-squared-error.md),

$$
\boxed{Z=\frac{Q}{\sqrt{\mathbb E[(\widehat Q-Q)^2]}}
=\frac{Q}{\sqrt{Q+(1+f)B+(1-f)^2B^2}}.}
$$

For $f\simeq1$, the shot-noise term is approximately $Q+2B$, but the mismatch term must be retained.

There is a terminology qualification: the usual variance-based [signal-to-noise ratio in photon counting](../../../../../../../signal-to-noise-ratio-in-photon-counting.md) is $Q/\sqrt{Q+(1+f)B}$ and does not include a fixed bias as noise. The printed next-part limit requires the root-mean-square accuracy convention above. A deterministic background mismatch contributes $b^2$ to [mean squared error](../../../../../../../mean-squared-error.md), not to the statistical variance.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
