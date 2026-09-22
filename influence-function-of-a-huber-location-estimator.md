# Influence function of a Huber location estimator

↑ **Parent:** [Influence function](influence-function.md)

Fix a scale $s>0$ and cutoff $k>0$. Define the population [Huber location estimator](huber-location-estimator.md) by the root

$$
\mathbb E_F\psi_k\!\left(\frac{X-\theta}{s}\right)=0,\qquad \theta=T(F),\qquad
A=\mathbb E_F\psi_k'\!\left(\frac{X-\theta}{s}\right)>0.
$$

Here $\psi_k$ is the [Huber score](huber-score.md). It has [Lipschitz continuity](lipschitz-continuity.md), so [dominated convergence](dominated-convergence-theorem.md) justifies differentiation when $F$ puts no mass at $\theta\pm ks$. Then $A=\mathbb P_F(|X-\theta|<ks)$, and the nonzero derivative identifies the local population root. The [implicit function theorem](implicit-function-theorem.md) applies away from the contaminating score's kinks; its [Lipschitz continuity](lipschitz-continuity.md) also gives the first-order expansion at those kinks. Differentiating its contaminated equation yields

$$
0=-\frac A s\operatorname{IF}(x;T,F)+\psi_k\!\left(\frac{x-\theta}{s}\right),\qquad
\operatorname{IF}(x;T,F)=\frac{s\psi_k((x-\theta)/s)}{A}.
$$

The normalization matters: the [Huber score](huber-score.md) alone is not the [influence function](influence-function.md). The [gross-error sensitivity](gross-error-sensitivity.md) is $sk/A$, while the [rejection point of an influence function](rejection-point-of-an-influence-function.md) is infinite because the clipped tails stay nonzero. The original clipped estimating criterion and its derivative normalization also appear in the population analysis of [M-estimators](m-estimator.md).[Peter J. Huber, Robust Estimation of a Location Parameter, §3, p. 78: derivative normalization; §4(iii), p. 79: clipped location criterion and central-mass denominator](robust-estimation-of-a-location-parameter-by-peter-j-huber.md)

Scale sets what counts as a large residual. For a [normal distribution](normal-distribution.md) $N(\mu,\sigma^2)$ with fixed $s=\sigma$, [symmetry](symmetry-physics.md) gives $\theta=\mu$ and $A=2\Phi(k)-1$, where $\Phi$ is the [standard normal distribution function](standard-normal-distribution-function.md). If the scale is instead a [statistical functional](statistical-functional.md) $S(F)$, differentiation of the joint equation adds the scale contribution:

$$
\operatorname{IF}(x;T,F)=\frac{s\psi_k(r_x)-B\operatorname{IF}(x;S,F)}{A},\qquad
r_x=\frac{x-\theta}{s},\quad B=\mathbb E_F\left[r_X\psi_k'(r_X)\right].
$$

Under a symmetric baseline and an odd [Huber score](huber-score.md), $B=0$, so scale estimation drops out at first order. This cancellation needs regularity of $S$ and does not protect finite [contamination](contamination-statistics.md) changes: an inflated [standard deviation](standard-deviation.md) enlarges the physical cutoff $ks$. A robust choice, such as a suitable [Scale M-estimator](scale-m-estimator.md), needs its own [influence function](influence-function.md) and [breakdown point](breakdown-point.md) checked. Fixing a numeric cutoff in raw units also sacrifices scale [equivariance](equivariant-map.md) when units change.[Peter J. Huber, Robust Estimation of a Location Parameter, §11, pp. 95-96: estimating location when normal-component scale and contamination fraction are unknown](robust-estimation-of-a-location-parameter-by-peter-j-huber.md)

## ↑ Ancestors (7)

1. [Influence function](influence-function.md)
2. [Robust statistics](robust-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Huber location estimator](huber-location-estimator.md)
- [Normal-location influence curves](normal-location-influence-curves.md)
