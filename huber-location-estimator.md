# Huber location estimator

↑ **Parent:** [Robust statistics](robust-statistics-split.md)

The Huber location estimator solves $\sum_i\psi_k(x_i-\theta)=0$, where $\psi_k$ clips its argument to $[-k,k]$.

More generally, fix a known scale $s>0$ and a dimensionless threshold $k>0$ before fitting. For observations $x_1,\ldots,x_n$, a [Huber location estimator](huber-location-estimator.md) is a [minimizer](global-minimizer.md) of the summed [Huber loss](huber-loss.md), equivalently a root of its [estimating equation](estimating-equation.md):

$$
Q_{k,s}(\theta)=\sum_{i=1}^n\rho_k\!\left(\frac{x_i-\theta}{s}\right),\qquad
\widehat\theta_{k,s}\in\operatorname*{argmin}_{\theta\in\mathbb R}Q_{k,s}(\theta),\qquad
\sum_{i=1}^n\psi_k\!\left(\frac{x_i-\widehat\theta_{k,s}}s\right)=0.
$$

Here $\rho_k$ is the [Huber loss](huber-loss.md) and $\psi_k$ the [Huber score](huber-score.md). The physical clipping distance is $ks$, in the observations' units; the initial formula uses $s=1$. A large observation keeps contributing a bounded signed score rather than being discarded. The original clipped location criterion appears in [Peter J. Huber](peter-j-huber.md)'s 1964 paper.[§4(iii), printed p. 79: quadratic-central, linear-tail criterion and clipping around the fitted location](robust-estimation-of-a-location-parameter-by-peter-j-huber.md)

For the original data $(0,1,2,3,4,40)$, take $s=1$ and $k=2$. At $\theta=2.5$, the standardized differences and their [Huber scores](huber-score.md) are

$$
(x_i-2.5)_{i=1}^6=(-2.5,-1.5,-0.5,0.5,1.5,37.5),\qquad
(\psi_2(x_i-2.5))_{i=1}^6=(-2,-1.5,-0.5,0.5,1.5,2).
$$

Their sum is zero, so the [Huber location estimator](huber-location-estimator.md) is $2.5$. Four scores remain in the central linear region, making the root unique. By comparison, the [sample mean](sample-mean.md) is $50/6\simeq8.3333$, and the [sample median](sample-median.md), using the midpoint of the two middle observations, is $(2+3)/2=2.5$. Agreement with the [sample median](sample-median.md) is a feature of these data, rather than an identity between the two [estimators](estimator.md).

The geometry explains both existence and possible nonuniqueness. The [Huber loss](huber-loss.md) is a [convex function](convex-function.md), so $Q_{k,s}$ is a [convex function](convex-function.md) of $\theta$ and its [derivative](derivative.md) is $-s^{-1}\sum_i\psi_k((x_i-\theta)/s)$. For $n\geq1$, $Q_{k,s}(\theta)$ tends to infinity as $|\theta|$ grows, hence attains a [minimum](minimum-of-a-subset-of-a-total-order.md); its zero [derivative](derivative.md) characterizes every [minimizer](global-minimizer.md). Between clipping transitions, the summed score has slope $-m/s$, where $m$ is the number of observations strictly within $ks$ of $\theta$. A root with $m>0$ is unique. If $m=0$, a flat interval is possible: for data $(0,10)$ with $s=1,k=2$, every $\theta\in[2,8]$ is a [minimizer](global-minimizer.md). A complete single-valued [estimator](estimator.md) then needs a selection rule, such as the interval's midpoint.

A bounded [Huber score](huber-score.md) limits one observation's contribution to the [estimating equation](estimating-equation.md). The [influence function of a Huber location estimator](influence-function-of-a-huber-location-estimator.md) additionally divides by the population's central mass, so the size of its bound depends on the reference [probability distribution](probability-distribution-split.md). Clipping does not by itself make the [bias of an estimator](bias-of-an-estimator.md) zero or prove a universal [breakdown point](breakdown-point.md); the separate [local influence versus replacement breakdown](local-influence-versus-replacement-breakdown.md) argument specifies what fixed scale permits. Estimating $s$ from the same data changes the procedure and requires separate analysis.

**Table of contents**

- [Huber location response to one outlier](huber-location-response-to-one-outlier.md)
- [Huber score](huber-score.md)
  - [Optimal bounded influence function for normal location](optimal-bounded-influence-function-for-normal-location.md)
- [Huber loss](huber-loss.md)
  - [Huber gradient regularizer](huber-gradient-regularizer.md)

## ↑ Ancestors (6)

1. [Robust statistics](robust-statistics-split.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Finite contamination bias of normal location](finite-contamination-bias-of-normal-location.md)
- [Huber location estimator](huber-location-estimator.md)
- [Huber location response to one outlier](huber-location-response-to-one-outlier.md)
- [Huber score](huber-score.md)
- [Influence function](influence-function.md)
- [Influence function of a Huber location estimator](influence-function-of-a-huber-location-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-223/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-223/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-223/1/a/solution.md)
