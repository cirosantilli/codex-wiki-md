# Laplace median robustness example

↑ **Parent:** [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md)

Choose the five numbers $1,2,2,5,10$ as an original illustration. Their [sample median](sample-median.md) is 2 and their [sample mean](sample-mean.md) is 4. The sum of [absolute losses](absolute-error-loss.md) at the [sample median](sample-median.md) is

$$
S(2)=|1-2|+|2-2|+|2-2|+|5-2|+|10-2|=1+0+0+3+8=12.
$$

If these numbers were modeled as an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [Laplace distribution](laplace-distribution.md) sample, the joint [maximum-likelihood estimates](maximum-likelihood-estimator.md) would therefore be $\widehat\mu=2$ and $\widehat b=12/5=2.4$. Using the [sample mean](sample-mean.md) instead gives $S(4)=14$, so it does not maximize this [likelihood function](likelihood-function.md).

Now replace only 10 by 100. The [sample median](sample-median.md) stays at 2, while the [sample mean](sample-mean.md) becomes $(1+2+2+5+100)/5=22$. The minimized sum of [absolute losses](absolute-error-loss.md) rises to $S(2)=102$, and the fitted scale rises to $\widehat b=102/5=20.4$. Stability of the fitted location therefore does not mean stability of every fitted parameter.

<a id="image-chosen-five-value-example-moving-the-largest-value-leaves-the-median-fixed-but-moves-the-mean"></a>
![](laplace-absolute-loss-and-median-robustness.png)

**[Figure 10](#image-chosen-five-value-example-moving-the-largest-value-leaves-the-median-fixed-but-moves-the-mean). Chosen five-value example: moving the largest value leaves the median fixed but moves the mean**.

The left panel subtracts each objective's minimum so the two [absolute loss](absolute-error-loss.md) curves can be compared despite the different totals. The right panel tracks the [sample mean](sample-mean.md) and [sample median](sample-median.md) as the largest chosen value changes. This is an [outlier](outlier.md) sensitivity illustration, not actual observations or a check that a [Laplace distribution](laplace-distribution.md) fits any population. In applications, [regression residuals](regression-residual.md) and the data-generating assumptions need separate examination; a stable [sample median](sample-median.md) alone does not validate a [statistical model](statistical-model-split.md).

## ↑ Ancestors (9)

1. [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md)
2. [Laplace distribution](laplace-distribution.md)
3. [Continuous probability distribution](continuous-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
