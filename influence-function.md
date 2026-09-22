# Influence function

↑ **Parent:** [Robust statistics](robust-statistics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Influence_function)

An [influence function](influence-function.md) asks how much a population answer moves when an infinitesimal fraction of its [probability distribution](probability-distribution-split.md) is relocated to a specified point. It distinguishes the unbounded response of the [mean](expected-value-split.md) from the bounded response of the [median](median.md) and the [Huber location estimator](huber-location-estimator.md). The [normal-location influence curves](normal-location-influence-curves.md) and [finite contamination bias of normal location](finite-contamination-bias-of-normal-location.md) below make that difference quantitative.

Let $T$ be a real-valued [statistical functional](statistical-functional.md), $F$ a reference [probability measure](probability-measure.md), and $\delta_x$ the [Dirac measure](dirac-measure.md) concentrated at $x$. Along the [epsilon-contamination neighborhood](epsilon-contamination-neighborhood.md) path $F_{\varepsilon,x}=(1-\varepsilon)F+\varepsilon\delta_x$, define the right [derivative](derivative.md)

$$
\operatorname{IF}(x;T,F)=\lim_{\varepsilon\downarrow0}\frac{T(F_{\varepsilon,x})-T(F)}{\varepsilon},\qquad
T(F_{\varepsilon,x})=T(F)+\varepsilon\operatorname{IF}(x;T,F)+o(\varepsilon).
$$

The name [influence curve](influence-function.md) refers to the same object. The [derivative](derivative.md) is in the signed direction $\delta_x-F$, so the calculation removes baseline mass as well as adding a [Dirac measure](dirac-measure.md). The definition is a [limit](limit-of-a-function.md) for each fixed $x$; it does not automatically give a remainder uniform over arbitrarily distant $x$.[Frank R. Hampel, The Influence Curve and Its Role in Robust Estimation, p. 383, §2: pointwise right-limit definition along mixtures with a point mass](the-influence-curve-and-its-role-in-robust-estimation-by-frank-r-hampel.md)

The [statistical functional](statistical-functional.md) must be defined on these contaminated [probability measures](probability-measure.md), and the right [derivative](derivative.md) must exist and be finite. For a [mean](expected-value-split.md), a finite first absolute [moment](moment.md) suffices. For a [median](median.md), require a unique baseline [median](median.md) and a [probability density function](probability-density-function.md) continuous and strictly positive there. For a smooth [M-estimator](m-estimator.md), require an isolated population root, justified differentiation of its [expected value](expected-value-split.md), and a nonzero derivative with respect to the fitted parameter. These are specific conditions for the formulas below. Existence of the pointwise [influence function](influence-function.md) alone proves neither an [asymptotic linear representation](asymptotic-linear-representation.md) nor [pathwise differentiability of a statistical functional](pathwise-differentiability-of-a-statistical-functional.md); each needs control of its own remainder and admissible [statistical paths](statistical-path.md).

**Table of contents**

- [Influence function of the mean](influence-function-of-the-mean.md)
- [Influence function of a Huber location estimator](influence-function-of-a-huber-location-estimator.md)
- [Normal-location influence curves](normal-location-influence-curves.md)
- [Finite contamination bias of normal location](finite-contamination-bias-of-normal-location.md)
- [Local influence versus replacement breakdown](local-influence-versus-replacement-breakdown.md)
- [Rejection point of an influence function](rejection-point-of-an-influence-function.md)
- [Local-shift sensitivity](local-shift-sensitivity.md)
- [Influence function of a quantile](influence-function-of-a-quantile.md)
- [Empirical influence function](empirical-influence-function.md)
- [Sensitivity curve](sensitivity-curve.md)
- [One-step estimator](one-step-estimator.md)
- [Asymptotic linear representation](asymptotic-linear-representation.md)
- [Gross-error sensitivity](gross-error-sensitivity.md)
- [Influence function of the sample median](influence-function-of-the-sample-median.md)

## ↑ Ancestors (6)

1. [Robust statistics](robust-statistics-split.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (31)

- [B-robust estimator](b-robust-estimator.md)
- [Empirical influence function](empirical-influence-function.md)
- [Finite contamination bias of normal location](finite-contamination-bias-of-normal-location.md)
- [Functional statistic](functional-statistic.md)
- [Huber location response to one outlier](huber-location-response-to-one-outlier.md)
- [Huber score](huber-score.md)
- [Influence function](influence-function.md)
- [Influence function of a Huber location estimator](influence-function-of-a-huber-location-estimator.md)
- [Influence function of a U-statistic](influence-function-of-a-u-statistic.md)
- [Influence function of the mean](influence-function-of-the-mean.md)
- [Influence-function representer](influence-function-representer.md)
- [Local influence versus replacement breakdown](local-influence-versus-replacement-breakdown.md)
- [Local-shift sensitivity](local-shift-sensitivity.md)
- [Normal-location influence curves](normal-location-influence-curves.md)
- [Optimal bounded influence function for normal location](optimal-bounded-influence-function-for-normal-location.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41/6/vii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/6/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-223/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-221/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-221/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-221/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-223/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-223/3/a/solution.md)
- [Rejection point of an influence function](rejection-point-of-an-influence-function.md)
- [Sandwich variance of an M-estimator](sandwich-variance-of-an-m-estimator.md)
- [Sensitivity curve](sensitivity-curve.md)
