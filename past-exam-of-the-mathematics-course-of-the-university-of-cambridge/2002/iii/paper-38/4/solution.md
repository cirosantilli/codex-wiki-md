<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [statistical functional](../../../../../statistical-functional.md) is a map $T$ defined on a class of [probability distributions](../../../../../probability-distribution.md). Its associated [functional statistic](../../../../../functional-statistic.md) is $T(F_n)$, where $F_n=n^{-1}\sum_i\delta_{X_i}$ is the [empirical distribution](../../../../../type-information-theory.md) and each $\delta_{X_i}$ is a [Dirac measure](../../../../../dirac-measure.md). For example, $T(F)=\int x\,dF(x)$ yields the [sample mean](../../../../../sample-mean.md). The [influence function](../../../../../influence-function.md) records the [derivative](../../../../../derivative.md) in the direction of point contamination:

$$
\operatorname{IF}(z;T,F)=\left.\frac{d}{d\varepsilon}T\big((1-\varepsilon)F+\varepsilon\delta_z\big)\right|_{\varepsilon=0+}.
$$

It is a local, infinitesimal robustness diagnostic, not a description of arbitrary large contamination.

Suppose $T$ is differentiable in a sense strong enough to linearize it at the [empirical distribution](../../../../../type-information-theory.md), and that its [derivative](../../../../../derivative.md) in a signed direction $G-F$ is $\int\operatorname{IF}(x;T,F)\,d(G-F)(x)$. Averaging the directions $\delta_z-F$ over $z\sim F$ gives the zero direction, so linearity implies $\int\operatorname{IF}\,dF=0$. The resulting [asymptotic linear representation](../../../../../asymptotic-linear-representation.md) is

$$
T(F_n)-T(F)=\frac1n\sum_i\operatorname{IF}(X_i;T,F)+o_p(n^{-1/2}).
$$

If $\int\operatorname{IF}^2\,dF<\infty$, the [central limit theorem](../../../../../central-limit-theorem.md) and the negligible remainder give

$$
\boxed{\sqrt n\{T(F_n)-T(F)\}\ \xrightarrow{d}\ N\left(0,\int\operatorname{IF}(x;T,F)^2\,dF(x)\right).}
$$

Thus the [asymptotic variance](../../../../../asymptotic-variance.md) is $n^{-1}\int\operatorname{IF}^2\,dF$. For a vector functional the integral is $n^{-1}\int\operatorname{IF}\operatorname{IF}^{\mathsf T}\,dF$. Convergence of the actual finite-sample [variance](../../../../../variance-split.md) to this leading expression additionally requires control of second moments of the remainder, or an appropriate [uniform integrability](../../../../../uniform-integrability.md) condition; [convergence in distribution](../../../../../convergence-in-distribution.md) alone does not provide that. Existence of a contamination [derivative](../../../../../derivative.md) by itself also does not guarantee the required empirical linearization.

Several complementary robustness measures follow. [Gross-error sensitivity](../../../../../gross-error-sensitivity.md) is $\gamma^*=\sup_z|\operatorname{IF}(z)|$. Under contamination $(1-\varepsilon)F+\varepsilon H$, the first-order bias is $\varepsilon\int\operatorname{IF}\,dH$, whose worst absolute coefficient is $\gamma^*$; bounded influence therefore bounds infinitesimal gross-error bias. The [local-shift sensitivity](../../../../../local-shift-sensitivity.md) is $\lambda^*=\sup_{x\ne y}|\operatorname{IF}(x)-\operatorname{IF}(y)|/|x-y|$, equal to $\sup|\operatorname{IF}'|$ when the [influence function](../../../../../influence-function.md) is smoothly differentiable. It measures the effect of moving a contaminant a small distance. The [rejection point of an influence function](../../../../../rejection-point-of-an-influence-function.md) is $\rho^*=\inf\{r:\operatorname{IF}(x)=0\text{ for }|x|>r\}$, using centered, standardized coordinates; it is infinite if there is no such cutoff. A finite cutoff completely rejects sufficiently extreme observations to first order. These measures address different aspects of robustness. The integral of squared influence controls asymptotic precision and efficiency, while [breakdown point](../../../../../breakdown-point.md) concerns finite amounts of contamination and is not determined by bounded influence alone.

For the [quantile](../../../../../quantile-function.md), assume $0<p<1$, a unique solution $q=q_p(F)$, and a [density](../../../../../density.md) continuous and positive at $q$. Define [quantiles](../../../../../quantile-function.md) of the contaminated distribution by generalized inversion, since a distribution with a point mass need not attain $p$ as an equality. If $z\ne q$, its indicator is constant near $q$ for sufficiently small contamination, and differentiating

$$
(1-\varepsilon)F(q_\varepsilon)+\varepsilon\mathbf1_{z\le q_\varepsilon}=p
$$

at zero gives $-p+f(q)q'_0+\mathbf1_{z\le q}=0$. Hence

$$
\boxed{\operatorname{IF}(z;q_p,F)=\frac{p-\mathbf1_{z\le q}}{f(q)}\quad(F\text{-almost every }z).}
$$

At the exceptional point $z=q$, the generalized-inverse [quantile](../../../../../quantile-function.md) remains exactly $q$: below $q$ the contaminated [cumulative distribution function](../../../../../cumulative-distribution-function.md) is below $p$, and its value at $q$ exceeds $p$. Its actual [derivative](../../../../../derivative.md) there is zero. The usual step-function expression is an almost-everywhere version, which is all that the [asymptotic variance](../../../../../asymptotic-variance.md) needs. Its mean is zero, and its second moment is

$$
\frac{p(p-1)^2+(1-p)p^2}{f(q)^2}=\frac{p(1-p)}{f(q)^2}.
$$

Therefore the [influence function of a quantile](../../../../../influence-function-of-a-quantile.md) gives [asymptotic variance](../../../../../asymptotic-variance.md) $p(1-p)/(nf(q)^2)$ and [gross-error sensitivity](../../../../../gross-error-sensitivity.md) $\max(p,1-p)/f(q)$. Its jump makes [local-shift sensitivity](../../../../../local-shift-sensitivity.md) infinite, and its nonzero constant tails make its rejection point infinite. If $f(q)=0$ or the [quantile](../../../../../quantile-function.md) is not unique, this regular derivation does not apply.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
