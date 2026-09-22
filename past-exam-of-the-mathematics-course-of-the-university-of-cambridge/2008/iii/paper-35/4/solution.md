<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For every $s\ge0$, the pointwise inequality $\mathbf1_{\{Y\ge0\}}\le e^{sY}$ holds: on the event the exponential is at least one, and off it the indicator is zero. Taking [expected values](../../../../../expected-value.md) and then the infimum proves the [Chernoff bound](../../../../../chernoff-bound.md)

$$
\boxed{\mathbb P(Y\ge0)\le\inf_{s\ge0}\mathbb E[e^{sY}].}
$$

An infinite exponential moment merely gives a vacuous bound at that $s$; no existence assumption on moments is needed for this extended-value inequality.

For a positive $s$ at which the relevant [moment-generating functions](../../../../../moment-generating-function.md) are finite, apply the [Chernoff bound](../../../../../chernoff-bound.md) to $Y=Z-C$. Independence of the sources gives

$$
\mathbb P(Z\ge C)\le e^{-sC}\prod_{j=1}^J\prod_{i=1}^{n_j}\mathbb E[e^{sX_{ji}}]=\exp\left\{s\left[\sum_{j=1}^Jn_j\alpha_j(s)-C\right]\right\}.
$$

Thus

$$
\boxed{\sum_{j=1}^Jn_j\alpha_j(s)\le C-\gamma/s\implies\mathbb P(Z\ge C)\le e^{-\gamma}.}
$$

Classes with $n_j=0$ make no contribution, so no moment assumption on those inactive classes is necessary. The [effective bandwidth](../../../../../effective-bandwidth.md) $\alpha_j(s)$ is the exponential-moment capacity demand of one class-$j$ source over this observation interval. Independent sources have additive effective bandwidths; reserving the margin $\gamma/s$ below capacity certifies the desired overflow bound. If $X_{ji}$ describes traffic during one unit of time, this is a bandwidth in traffic per unit time; for a window of length $t$, divide $\log\mathbb E e^{sX(t)}$ by $st$ instead.

To establish [monotonicity and bounds of effective bandwidth](../../../../../monotonicity-and-bounds-of-effective-bandwidth.md), write $K(s)=\log\mathbb E e^{sX}$ for a representative source. The [Holder inequality](../../../../../holder-inequality.md) gives, for $0<t<s$ in its moment domain,

$$
\mathbb E e^{tX}=\mathbb E[(e^{sX})^{t/s}]\le(\mathbb E e^{sX})^{t/s},\qquad \frac{K(t)}t\le\frac{K(s)}s.
$$

Equivalently, the [cumulant-generating function](../../../../../cumulant-generating-function.md) is convex with $K(0)=0$, so its secant slope from zero is nondecreasing. Hence $\alpha(s)$ is nondecreasing, rather than necessarily strictly increasing: if $X$ is deterministic its effective bandwidth is constant.

Assuming the mean is defined and finite, the [Jensen inequality](../../../../../jensen-s-inequality.md) gives $\mathbb E e^{sX}\ge e^{s\mathbb EX}$, hence $\alpha(s)\ge\mathbb EX$. Let

$$
M=\sup\{x:\mathbb P(X>x)>0\}=\operatorname{ess\,sup}X.
$$

For finite $M$, $X\le M$ almost surely, so $\mathbb E e^{sX}\le e^{sM}$ and $\alpha(s)\le M$. Combining these proves

$$
\boxed{\mathbb EX\le\alpha(s)\le\operatorname{ess\,sup}X,\qquad\alpha(t)\le\alpha(s)\quad(0<t<s).}
$$

The upper bound is vacuous if the [essential supremum](../../../../../essential-supremum.md) is infinite. For nonnegative traffic these comparisons also make sense with extended values; for an arbitrary real-valued source with undefined mean, the printed mean comparison itself requires an integrability qualification. The positive parameter domain is essential: $\alpha(0)$ is defined only by a limit when the appropriate moment assumptions hold, and the stated monotonicity comparisons concern $s>0$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
