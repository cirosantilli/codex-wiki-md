<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

For the fixed observation interval, $N_3$ has [Poisson distribution](../../../../../poisson-distribution.md) with mean and [variance](../../../../../variance-split.md) $3\lambda$. Hence $N_3/3$ is unbiased and has [variance](../../../../../variance-split.md) $\lambda/3$. Its [score function](../../../../../informant-function.md) is $N_3/\lambda-3$, and its [Fisher information](../../../../../fisher-information-matrix.md) is $3/\lambda$. The [Cramér-Rao bound](../../../../../cramer-rao-bound.md) for unbiased estimation of $\lambda$ therefore gives [variance](../../../../../variance-split.md) at least $\lambda/3$, attained by $N_3/3$.

For the stopping-time observation, $T_{10}$ has [Gamma distribution](../../../../../gamma-distribution.md) with shape $10$ and rate $\lambda$. Direct integration of its density gives

$$
\mathbb E_\lambda(T_{10}^{-1})=\frac\lambda9,\qquad
\mathbb E_\lambda(T_{10}^{-2})=\frac{\lambda^2}{9\cdot8}.
$$

Thus $k=9$, and

$$
\boxed{\widetilde\Lambda_2=9/T_{10},\qquad \operatorname{Var}(\widetilde\Lambda_2)=\lambda^2/8.}
$$

The [score function](../../../../../informant-function.md) is $10/\lambda-T_{10}$, so the [Fisher information](../../../../../fisher-information-matrix.md) is $10/\lambda^2$. Its [Cramér-Rao lower bound](../../../../../cramer-rao-bound.md) is $\lambda^2/10$, strictly below this estimator's [variance](../../../../../variance-split.md).

Nevertheless, $9/T_{10}$ is [uniformly minimum-variance unbiased](../../../../../uniformly-minimum-variance-unbiased-estimator.md). The observed $T_{10}$ is a [sufficient statistic](../../../../../sufficient-statistic.md), and its family is complete: if $\mathbb E_\lambda h(T_{10})=0$ for all $\lambda>0$, then $\int_0^\infty h(t)t^9e^{-\lambda t}\,dt=0$ for all $\lambda>0$. Uniqueness of the [Laplace transform](../../../../../laplace-transform.md), applied after an exponential tilt to make an [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md), implies $h=0$ almost everywhere. The [Lehmann–Scheffé theorem](../../../../../lehmann-scheffe-theorem.md) now proves the minimum-variance assertion. Failure to attain the Cramér–Rao bound does not disprove minimum [variance](../../../../../variance-split.md) within the class of [unbiased estimators](../../../../../unbiased-estimator.md).

For the actual observations, the two [likelihood functions](../../../../../likelihood-function.md) are

$$
L_1(\lambda)=\frac{(3\lambda)^{10}}{10!}e^{-3\lambda},\qquad
L_2(\lambda)=\frac{\lambda^{10}3^9}{9!}e^{-3\lambda}.
$$

They differ by a factor independent of $\lambda$. The [likelihood principle](../../../../../likelihood-principle.md) consequently requires the same inferential conclusions, since the observed data carry proportional likelihoods. But the two minimum-variance unbiased estimates are $\boxed{10/3\text{ and }3}$ respectively. Minimum-variance unbiased estimation therefore violates the [likelihood principle](../../../../../likelihood-principle.md): its unbiasedness and [variance](../../../../../variance-split.md) refer to the sampling plan, including the stopping rule, rather than solely to the observed [Likelihood function](../../../../../likelihood-function.md).

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
