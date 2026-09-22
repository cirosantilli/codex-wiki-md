<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret stationarity in the usual second-order time-series sense and assume nondegenerate noise, $\sigma_z^2>0$. For a two-sided autoregressive equation, the missing existence condition is

$$
\boxed{|\phi|\ne1.}
$$

It is important to separate this from causality. If $|\phi|<1$, the unique stationary solution is $X_t=\sum_{j\geq0}\phi^jZ_{t-j}$. If $|\phi|>1$, there is still a stationary solution, but it is [anticausal](../../../../../../anticausal-time-series.md):

$$
\boxed{X_t=-\sum_{j=1}^\infty\phi^{-j}Z_{t+j}.}
$$

Both expansions converge in L2 because their coefficients are square summable. Substitution verifies the equation. Their means are zero and their [covariance](../../../../../../covariance.md) functions depend only on lag. Uniqueness follows by iterating the equation backward in the first case and forward in the second: the remainders $\phi^nX_{t-n}$ or $\phi^{-n}X_{t+n}$ tend to zero in L2 for any stationary finite-[variance](../../../../../../variance-split.md) solution. This is the [stationary versus causal solution of a two-sided AR(1) equation](../../../../../../stationary-versus-causal-solution-of-a-two-sided-ar-1-equation.md).

For $\phi=\pm1$, iteration gives

$$
X_t-\phi^nX_{t-n}=\sum_{j=0}^{n-1}\phi^jZ_{t-j}.
$$

The [variance](../../../../../../variance-split.md) of the right side is $n\sigma_z^2$. The [variance](../../../../../../variance-split.md) of the left side is at most $4\operatorname{Var}(X_t)$ by stationarity and [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). These are incompatible as $n\to\infty$. Thus no weakly stationary finite-[variance](../../../../../../variance-split.md) solution exists at those [unit roots](../../../../../../unit-root.md).

If the intended claim includes a causal innovation representation, its condition is instead **$|\phi|<1$**, as in the next part. The stated [white noise](../../../../../../white-noise.md) equation alone does not say that $Z_t$ is orthogonal to the past of $X$. If zero innovation [variance](../../../../../../variance-split.md) is allowed, the unit-root exclusion has degenerate exceptions, such as random constant solutions when $\phi=1$; the nondegenerate convention is necessary for the asserted nonexistence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
