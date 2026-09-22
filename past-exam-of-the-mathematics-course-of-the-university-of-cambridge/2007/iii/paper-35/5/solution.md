<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For any $s\geq0$, $Y\geq0$ implies $e^{sY}\geq1$. Hence $\mathbf1_{\{Y\geq0\}}\leq e^{sY}$, and taking [expected values](../../../../../expected-value.md) gives the [Chernoff bound](../../../../../chernoff-bound.md)

$$
\boxed{\mathbb P(Y\geq0)\leq\inf_{s\geq0}\mathbb E[e^{sY}].}
$$

At $s=0$ this is the trivial bound one; an infinite exponential moment merely gives a noninformative bound. For positive $s$ at which all required [moment-generating functions](../../../../../moment-generating-function.md) are finite, define $\alpha_j(s)=s^{-1}\log\mathbb E[e^{sX_{ji}}]$. Independence of the source [random variables](../../../../../random-variable-split.md) implies

$$
\log\mathbb E[e^{sX}]=\sum_{j=1}^{J}n_j\log\mathbb E[e^{sX_{ji}}]=s\sum_{j=1}^{J}n_j\alpha_j(s).
$$

Applying the [Chernoff bound](../../../../../chernoff-bound.md) to $Y=X-C$ gives

$$
\mathbb P(X\geq C)\leq\exp\!\left(s\sum_jn_j\alpha_j(s)-sC\right).
$$

Consequently

$$
\boxed{\sum_jn_j\alpha_j(s)\leq C-\gamma/s\quad\Longrightarrow\quad\mathbb P(X\geq C)\leq e^{-\gamma}.}
$$

Here $s>0$ and, for a nontrivial target, $\gamma>0$.

The [effective bandwidth](../../../../../effective-bandwidth.md) $\alpha_j(s)$ is the capacity charge of one source for this exponential-moment tail criterion. Independent sources contribute additively. It incorporates variability as well as mean demand: the [Jensen inequality](../../../../../jensen-s-inequality.md) gives $\alpha_j(s)\geq\mathbb E X_{ji}$, and, under exponential integrability near zero, $\alpha_j(s)\to\mathbb E X_{ji}$ as $s\downarrow0$. For bounded traffic its large-$s$ limit is the essential peak, as described by the [mean and peak limits of effective bandwidth](../../../../../mean-and-peak-limits-of-effective-bandwidth.md). Thus larger $s$ gives more weight to rare high demands. This is a one-window demand bound; a queue's overflow probability over many windows requires additional temporal modeling, not just this single-window calculation.

For the [normal distribution](../../../../../normal-distribution.md) $X_{ji}\sim N(\lambda_j,\sigma_j^2)$, completing the square in its density gives the [moment-generating function](../../../../../moment-generating-function.md)

$$
\mathbb E[e^{sX_{ji}}]=\exp\!\left(s\lambda_j+\frac{s^2\sigma_j^2}{2}\right),\qquad\alpha_j(s)=\lambda_j+\frac{s\sigma_j^2}{2}.
$$

Write $m=\sum_jn_j\lambda_j$ and $v=\sum_jn_j\sigma_j^2$ for the aggregate mean and [variance](../../../../../variance-split.md). The exponential-moment capacity condition becomes

$$
m+\frac{sv}{2}+\frac{\gamma}{s}\leq C.
$$

For $v>0$, the last two terms are minimized at $s=\sqrt{2\gamma/v}$, where their sum is $\sqrt{2\gamma v}$. Therefore [Gaussian effective bandwidth](../../../../../gaussian-effective-bandwidth.md) yields the sufficient condition

$$
\boxed{m+\sqrt{2\gamma v}\leq C\quad\Longrightarrow\quad\mathbb P(X\geq C)\leq e^{-\gamma}.}
$$

Equivalently, optimizing the exponential bound directly when $C>m$ gives $\exp[-(C-m)^2/(2v)]$; when $C\leq m$ the best nonnegative-$s$ bound is one. The square-root condition is sufficient rather than necessary because an exponential bound does not equal the exact normal tail.

For the exact condition, independence and multiplication of the normal [moment-generating functions](../../../../../moment-generating-function.md) show that $X\sim N(m,v)$. For $v>0$, let $\Phi$ be the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). The normal law is continuous, so

$$
\mathbb P(X\geq C)=1-\Phi\!\left(\frac{C-m}{\sqrt v}\right).
$$

Since $\Phi$ is continuous and strictly increasing from zero to one, the [exact Gaussian overflow constraint](../../../../../exact-gaussian-overflow-constraint.md) is

$$
\boxed{\mathbb P(X\geq C)\leq e^{-\gamma}\quad\Longleftrightarrow\quad\sum_jn_j\lambda_j+\phi\left(\sum_jn_j\sigma_j^2\right)^{1/2}\leq C,\qquad\phi=\Phi^{-1}(1-e^{-\gamma}).}
$$

The constant depends only on the desired tail exponent $\gamma$, not on the source counts. It is positive when $\gamma>\log2$, zero when $\gamma=\log2$, and negative when $0<\gamma<\log2$. For example, at $\gamma=\log100$ the exact normal quantile is about $2.32635$, whereas the [Chernoff bound](../../../../../chernoff-bound.md) uses $\sqrt{2\log100}\approx3.03485$; the latter reserves more capacity.

Finally, the positive-variance hypothesis must not be hidden. If $v=0$, then $X=m$ almost surely, and the [zero-variance boundary of an overflow constraint](../../../../../zero-variance-boundary-of-an-overflow-constraint.md) gives $\mathbb P(X\geq C)=\mathbf1_{\{m\geq C\}}$. For $\gamma>0$, the exact condition is then $m<C$. In particular $m=C$ does not meet the target even though substituting $v=0$ into the printed non-strict square-root inequalities would allow it. The displayed normal-quantile equivalence applies to nondegenerate Gaussian traffic; the deterministic case requires this strict boundary convention.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
