<h1 id="6/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

Several finite-sample counterparts of the [influence function](../../../../../../influence-function.md) should be distinguished. The [empirical influence function](../../../../../../empirical-influence-function.md) substitutes the empirical distribution: $\operatorname{EIF}_n(x)=\operatorname{IF}(x;T,F_n)$. For a smooth [M-estimator](../../../../../../m-estimator.md) it is

$$
-\left[n^{-1}\sum_i\partial_\theta\psi(X_i,T(F_n))\right]^{-1}\psi(x,T(F_n)).
$$

It requires a well-defined derivative and nonsingular denominator. An unsmoothed empirical quantile functional, for example, need not admit the population-style density derivative.

The actual one-observation [sensitivity curve](../../../../../../sensitivity-curve.md) is a finite difference:

$$
\boxed{\operatorname{SC}_n(x)=(n+1)\left[T\!\left(\frac{nF_n+\delta_x}{n+1}\right)-T(F_n)\right].}
$$

It records contamination of size $1/(n+1)$ rather than an infinitesimal perturbation. For a smooth functional it approaches the population influence curve as the sample grows. A deletion counterpart uses $F_{n,-i}=(nF_n-\delta_{X_i})/(n-1)$, giving

$$
T(F_{n,-i})-T(F_n)\approx-\frac{\operatorname{EIF}_n(X_i)}{n-1}.
$$

The [Jackknife resampling](../../../../../../jackknife-resampling.md) pseudovalue $J_i=nT(F_n)-(n-1)T(F_{n,-i})$ is therefore approximately $T(F_n)+\operatorname{EIF}_n(X_i)$. The jackknife variance estimate $(n-1)n^{-1}\sum_i[T(F_{n,-i})-\overline T_{(-)}]^2$ corresponds asymptotically to $n^{-2}\sum_i\operatorname{EIF}_n(X_i)^2$ for centered empirical influences.

In linear regression, [Cook's distance](../../../../../../cook-s-distance.md) measures the fitted-value effect of deleting a case. For $p$ coefficients, residual $e_i$, leverage $h_{ii}$ and variance estimate $\widehat\sigma^2$, its usual expression is $D_i=e_i^2h_{ii}/[p\widehat\sigma^2(1-h_{ii})^2]$. It illustrates that a case can be influential through both a large residual and high leverage. Finite perturbations and nonlinear refitting can differ materially from a first-order influence approximation; these diagnostics should not be conflated.

## ↑ Ancestors (11)

1. [Vii](../vii.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
