<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let U be the total payload arriving in one slot. Conditional on its Poisson packet count, use the exponential moment of each independent payload to get, for $\theta<1$,

$$
\mathbb E e^{\theta U}=\exp\left\{\lambda\delta\left(\frac1{1-\theta}-1\right)\right\}.
$$

For net work $Z=U-C\delta$, its [cumulant-generating function](../../../../../../cumulant-generating-function.md) is

$$
\log\mathbb E e^{\theta Z}=\delta\left(\frac{\lambda\theta}{1-\theta}-C\theta\right).
$$

The [mean](../../../../../../expected-value.md) net work is $\delta(\lambda-C)<0$. Under the arrivals-before-service slot convention the [Lindley recursion](../../../../../../lindley-recursion.md) gives stationary [queue workload](../../../../../../workload-of-a-queue.md) $R_\delta\overset d=\sup_{m\geq0}\sum_{j=1}^mZ_j$. The positive root of the exponential-moment equation is $\theta_*=1-\rho$. Thus $\exp(\theta_*\sum_{j=1}^mZ_j)$ is a nonnegative [martingale](../../../../../../martingale-split.md). Stop it at the first crossing of r or a finite horizon; its value on the crossing event is at least $e^{\theta_*r}$. Increasing the horizon proves

$$
\mathbb P(R_\delta\geq r)\leq e^{-(1-\rho)r},\qquad r>0.
$$

This is an infinite-horizon bound, not a one-slot Chernoff estimate.

A useful refinement identifies both the exponential rate and the small-slot prefactor. Couple the [random walk](../../../../../../random-walk.md) to the continuous compound Poisson input U(t), and write $W=\sup_{t\geq0}(U(t)-Ct)$ and $W_\delta=\sup_{k\geq0}(U(k\delta)-Ck\delta)$. Their laws are the continuous and slot-boundary stationary [queue workloads](../../../../../../workload-of-a-queue.md). Monotonicity of U implies the [grid-sampled compound Poisson workload bound](../../../../../../grid-sampled-compound-poisson-workload-bound.md): $W_\delta\leq W\leq W_\delta+C\delta$, by rounding each t up to the next grid point.

The continuous [queue workload](../../../../../../workload-of-a-queue.md) law can be obtained directly from the stationary packet count. Conditional on Q=k, the k remaining payloads are independent unit-mean exponentials: unserved payloads have not affected earlier service completions, and the in-service residual uses the [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md). Hence

$$
\mathbb E e^{-sW}=\sum_{k\geq0}(1-\rho)\rho^k(1+s)^{-k}=\frac{(1-\rho)(1+s)}{1+s-\rho}=(1-\rho)+\rho\frac{1-\rho}{1-\rho+s}.
$$

Thus W has mass $1-\rho$ at zero, and its positive part is exponential with rate $1-\rho$. Combining this [stationary workload of an exponential-payload queue](../../../../../../stationary-workload-of-an-exponential-payload-queue.md) with the grid bound gives the explicit estimate

$$
\boxed{\rho e^{-(1-\rho)(r+C\delta)}\leq\mathbb P(R_\delta\geq r)\leq\rho e^{-(1-\rho)r},\qquad r>0.}
$$

In particular $\lim_{r\to\infty}r^{-1}\log\mathbb P(R_\delta\geq r)=-(1-\rho)$, and for small delta the estimate is $\rho e^{-(1-\rho)r}$. The exact continuous-time tail is that latter expression. Another slot convention may shift [queue workload](../../../../../../workload-of-a-queue.md) by the within-slot input/service timing; its convention must be specified before asserting a prefactor, while this exponential tail rate is unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
