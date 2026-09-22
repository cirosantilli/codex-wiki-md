<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A functional statistic has the form $T(F_n)$, where $F_n=n^{-1}\sum_i\delta_{X_i}$ is the [empirical distribution](../../../../../type-information-theory.md) and $T$ is a [statistical functional](../../../../../statistical-functional.md) on a class of distributions. It separates the population quantity $T(F)$ from its sample estimate. [Fisher consistency](../../../../../fisher-consistency.md) for a model $\{F_\theta\}$ means $T(F_\theta)=\theta$ for every model parameter; it does not alone establish consistency of the empirical estimate without continuity and probabilistic conditions.

The [influence function](../../../../../influence-function.md) measures infinitesimal contamination at a point:

$$
\operatorname{IF}(x;T,F)=\lim_{\varepsilon\downarrow0}\frac{T((1-\varepsilon)F+\varepsilon\delta_x)-T(F)}{\varepsilon},
$$

when this derivative exists. A bounded influence function limits first-order sensitivity to an arbitrarily remote observation.

An [M-estimator](../../../../../m-estimator.md) is a minimizer of an empirical loss, or a chosen consistent solution of an [estimating equation](../../../../../estimating-equation.md) $\sum_i\psi(X_i,\widehat\theta)=0$. Its population functional solves $\mathbb E_F\psi(X,T(F))=0$. Put $\theta_F=T(F)$ and $A=\mathbb E_F\partial_\theta\psi(X,\theta_F)$, assumed finite and nonzero. Differentiating the contaminated population equation gives

$$
A\operatorname{IF}(x;T,F)+\psi(x,\theta_F)=0,
$$

since the unperturbed expected score is zero. Hence

$$
\boxed{\operatorname{IF}(x;T,F)=-\frac{\psi(x,\theta_F)}A.}
$$

Under differentiability, consistency and the uniform local laws needed for expansion of the empirical equation,

$$
\sqrt n(\widehat\theta-\theta_F)=-A^{-1}n^{-1/2}\sum_i\psi(X_i,\theta_F)+o_P(1).
$$

The [central limit theorem](../../../../../central-limit-theorem.md) now yields [asymptotic normality](../../../../../asymptotic-normality.md) with [sandwich variance of an M-estimator](../../../../../sandwich-variance-of-an-m-estimator.md)

$$
\boxed{\sqrt n(\widehat\theta-\theta_F)\Rightarrow N\!\left(0,\frac{\mathbb E_F\psi(X,\theta_F)^2}{A^2}\right).}
$$

Thus the leading variance of $\widehat\theta$ itself is the displayed variance divided by $n$. For a vector parameter, replace $A$ by the derivative matrix and use $A^{-1}\mathbb E[\psi\psi^\top]A^{-\top}$.

In a location model with known scale $s$, choose $\psi(x,\theta)=\psi_0((x-\theta)/s)$. For a symmetric reference distribution, an odd score is Fisher consistent. With $Z=(X-\theta_F)/s$ and positive $\mathbb E\psi_0'(Z)$, the formulas become

$$
\operatorname{IF}(x)=\frac{s\psi_0((x-\theta_F)/s)}{\mathbb E\psi_0'(Z)},\qquad n\operatorname{Var}(\widehat\theta)\approx\frac{s^2\mathbb E\psi_0(Z)^2}{(\mathbb E\psi_0'(Z))^2}.
$$

The Gaussian likelihood score $\psi_0(z)=z$ gives the efficient sample mean under normality, but its unbounded influence is vulnerable to large outliers. The [Huber score](../../../../../huber-score.md) $\psi_0(z)=\max(-c,\min(z,c))$ is linear centrally and bounded in the tails, balancing normal-model efficiency against contamination sensitivity. Its denominator is $\mathbb P(|Z|<c)$ for a continuous law. The sign score gives the median and needs a nonsmooth derivation using the density at the median, rather than incorrectly setting its ordinary derivative to zero. Redescending scores can reject very extreme observations, but may have multiple roots and require a consistent root-selection rule.

Thus appropriate choices seek Fisher consistency, a nonzero stable derivative, finite variance, reasonable reference-model efficiency and bounded influence. Robust scale estimation may be needed for the tuning constant; joint location-scale estimation uses the matrix influence calculation rather than treating an estimated scale as known. Bounded influence describes local robustness and is not by itself a global [breakdown point](../../../../../breakdown-point.md) theorem.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
