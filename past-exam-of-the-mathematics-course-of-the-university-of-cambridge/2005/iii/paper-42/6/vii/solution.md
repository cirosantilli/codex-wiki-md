<h1 id="6/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

For a fully specified continuous null distribution $F_0$, compare the [empirical distribution function](../../../../../../empirical-distribution-function.md) $F_n$ with $F_0$. The [probability integral transform](../../../../../../probability-integral-transform.md) makes $F_0(Y_i)$ iid uniform under the null, giving distribution-free calibration. Three common discrepancies are

$$
D_n=\sup_x|F_n(x)-F_0(x)|,\qquad
C_n=n\int(F_n-F_0)^2dF_0,\qquad
A_n=n\int\frac{(F_n-F_0)^2}{F_0(1-F_0)}dF_0.
$$

These define the [Kolmogorov-Smirnov test](../../../../../../kolmogorov-smirnov-test.md), [Cramér–von Mises criterion](../../../../../../cramer-von-mises-criterion.md) and [Anderson–Darling test](../../../../../../anderson-darling-test.md), respectively. Reject for large values. The supremum detects the largest discrepancy, the unweighted integral combines discrepancies throughout the distribution, and the reciprocal weight emphasizes the tails.

The [Donsker theorem for empirical distribution functions](../../../../../../donsker-theorem-for-empirical-distribution-functions.md) gives $\sqrt n(F_n-F_0)\Rightarrow B^0\circ F_0$ for a [Brownian bridge](../../../../../../brownian-bridge.md) $B^0$, with [covariance](../../../../../../covariance.md) $\min(u,v)-uv$. Consequently the standard continuous-null limits are $\sup_{0\leq u\leq1}|B^0(u)|$, $\int_0^1B^0(u)^2du$, and $\int_0^1B^0(u)^2/[u(1-u)]du$ for $\sqrt nD_n,C_n,A_n$, respectively; the weighted last limit also requires control near the endpoints. Exact finite-sample or asymptotic null [quantiles](../../../../../../quantile-function.md) provide critical values.

If parameters in $F_\theta$ are estimated from the same observations, these fully specified-null critical values generally fail. A first-order expansion is

$$
\sqrt n(F_n-F_{\widehat\theta})(x)
=\sqrt n(F_n-F_{\theta_0})(x)-\dot F_{\theta_0}(x)^T\sqrt n(\widehat\theta-\theta_0)+o_p(1),
$$

so the estimated parameter changes the limiting process. One must use the fitted-model null law, adjusted asymptotic theory, or a [parametric bootstrap](../../../../../../parametric-bootstrap.md) that re-estimates the parameters in each replicate.

## ↑ Ancestors (11)

1. [Vii](../vii.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
