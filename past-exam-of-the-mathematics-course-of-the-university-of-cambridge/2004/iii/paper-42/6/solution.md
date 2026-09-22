<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a regular model let $\ell_N(\theta)$ be the [log-likelihood](../../../../../log-likelihood.md), $U_N(\theta)=\nabla\ell_N(\theta)$ its score, $I_N(\theta)$ its total [Fisher information](../../../../../fisher-information-matrix.md), and $\widehat\theta$ the unrestricted [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md). For a point null $\theta=\theta_0$ in a p-dimensional parameter space, the standard statistics are

$$
\begin{aligned}
W_N&=(\widehat\theta-\theta_0)^TI_N(\widehat\theta)(\widehat\theta-\theta_0),\\
S_N&=U_N(\theta_0)^TI_N(\theta_0)^{-1}U_N(\theta_0),\\
L_N&=2\{\ell_N(\widehat\theta)-\ell_N(\theta_0)\}.
\end{aligned}
$$

These define the [Wald test](../../../../../wald-test.md), [score test](../../../../../score-test.md) and [likelihood-ratio test](../../../../../likelihood-ratio-test.md). With an interior true parameter, increasing information, suitable differentiability and [asymptotic normality](../../../../../asymptotic-normality.md), all have asymptotic [chi-squared distribution](../../../../../chi-squared-distribution.md) with p degrees of freedom under the null. [Observed information](../../../../../observed-fisher-information.md) can replace expected information when it is asymptotically equivalent.

For q smooth independent restrictions $g(\theta)=0$, replace the [Wald statistic](../../../../../wald-test.md) by $g(\widehat\theta)^T[G I_N(\widehat\theta)^{-1}G^T]^{-1}g(\widehat\theta)$, where G is the derivative of g at the estimate; compare with chi-squared q. The likelihood-ratio statistic uses the difference between unrestricted and null-restricted maxima. The score statistic is computed at the restricted maximum and uses efficient information for the tested coordinates: with nuisance coordinates lambda this is $I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}$. Inverting the acceptance inequalities for point nulls produces approximate coverage-$1-\alpha$ [confidence regions](../../../../../confidence-region.md); for example the Wald region consists of theta satisfying $(\widehat\theta-\theta)^TI_N(\widehat\theta)(\widehat\theta-\theta)\leq\chi^2_{p,1-\alpha}$. Analogous score and likelihood-ratio inequalities give their [confidence regions](../../../../../confidence-region.md).

For the Poisson family, put $Y_{-1}=1$ to include the initial observation, and define

$$
S_n=\sum_{i=0}^nY_i,\qquad T_n=1+\sum_{i=0}^{n-1}Y_i.
$$

Multiplying the initial and conditional Poisson probabilities gives, on the supported observation sequences,

$$
\boxed{\ell_n(\theta)=S_n\log\theta-\theta T_n+c(Y_0,\ldots,Y_n).}
$$

The parameter-free term is $\sum_{i=0}^n[Y_i\log Y_{i-1}-\log(Y_i!)]$, interpreting $0\log0$ as zero. A positive count after a zero preceding count is outside the support.

For $S_n>0$, strict concavity gives unconstrained maximum $\widetilde\theta=S_n/T_n$, and the upper endpoint restriction gives

$$
\boxed{\widehat\theta=\min\left(\frac{S_n}{T_n},1\right)\quad\text{when }S_n>0.}
$$

There is an endpoint qualification in the printed question. With [probability](../../../../../probability.md) $e^{-\theta}$, $Y_0=0$ and all later counts are zero. Then $S_n=0$, $T_n=1$ and the [likelihood](../../../../../likelihood-function.md) is $e^{-\theta}$, which has no maximum on the stated space $0<\theta\leq1$. The formula produces zero only as an extended estimate on the closure $[0,1]$. This is a [likelihood supremum at an excluded boundary](../../../../../likelihood-supremum-at-an-excluded-boundary.md), and zero cannot be called an actual maximum in the original space.

The observed negative second derivative is $S_n/\theta^2$. Conditional expectation gives $\mathbb EY_0=\theta$ and $\mathbb EY_i=\theta\mathbb EY_{i-1}=\theta^{i+1}$. Therefore for $0<\theta<1$,

$$
\boxed{i_n(\theta)=\frac{\mathbb ES_n}{\theta^2}=\frac{1-\theta^{n+1}}{\theta(1-\theta)}\leq\frac1{\theta(1-\theta)}.}
$$

This is the [bounded information in a subcritical Poisson branching process](../../../../../bounded-information-in-a-subcritical-poisson-branching-process.md). Observing more generations of one family does not provide unbounded information. Indeed $\mathbb P(Y_n>0)\leq\mathbb EY_n=\theta^{n+1}\to0$, and zero is absorbing, so extinction occurs at a finite generation almost surely. The total observed progeny $S_\infty$ is finite; eventually $S_n=S_\infty$, $T_n=1+S_\infty$, and the extended estimate equals $S_\infty/(1+S_\infty)$, a discrete nondegenerate random variable rather than a consistent increasingly precise estimate.

Here is a direct proof of the failure of a chi-squared Wald limit which does not rely solely on the information bound. Under any interior null $\theta_0$, the event $Y_0=1$, $Y_1=0$ has [probability](../../../../../probability.md) $\theta_0e^{-2\theta_0}>0$ and forces every later count to be zero. On it the genuine constrained estimate is $1/2$ for every $n\geq1$, so the usual expected-information [Wald statistic](../../../../../wald-test.md) is

$$
W_n=i_n(\widehat\theta)(\widehat\theta-\theta_0)^2=4(1-2^{-(n+1)})(1/2-\theta_0)^2.
$$

Thus it has a persistent atom tending to $4(1/2-\theta_0)^2$. The fact that [atoms obstruct a continuous distributional limit](../../../../../atoms-obstruct-a-continuous-distributional-limit.md) rules out a chi-squared limit, including when $\theta_0$ equals one half and that atom is at zero. Any definition adopted for the separate all-zero sample event leaves this positive-count counterexample intact. Hence **the [Wald statistic](../../../../../wald-test.md) does not have the usual asymptotic chi-squared null law for this increasing observation horizon**.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
