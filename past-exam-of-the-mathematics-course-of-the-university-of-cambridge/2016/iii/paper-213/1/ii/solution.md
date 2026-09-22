<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [effective bandwidth](../../../../../../effective-bandwidth.md) measures how much capacity a random traffic source requires when unusually large demands matter. A mean-rate description loses burstiness; a peak-rate description can waste capacity when peaks are rare. The parameter $s>0$ in an [effective bandwidth](../../../../../../effective-bandwidth.md) controls the emphasis placed on such bursts through the [moment-generating function](../../../../../../moment-generating-function.md):

$$
\alpha(s)=\frac{K(s)}s,\qquad K(s)=\log\mathbb E[e^{sX}].
$$

Here $X$ is the traffic in a chosen time unit. If $X(t)$ instead measures traffic over length $t$, the corresponding rate is $\alpha(s,t)=\log\mathbb E[e^{sX(t)}]/(st)$. With independent stationary increments, this is independent of $t$ whenever the [moment-generating function](../../../../../../moment-generating-function.md) exists. More generally both the time scale and dependence structure matter.

The [Chernoff bound](../../../../../../chernoff-bound.md) follows directly from the [Markov inequality](../../../../../../markov-inequality.md), since $e^{sX}$ is nonnegative and $X\geq b$ implies $e^{sX}\geq e^{sb}$:

$$
\mathbb P(X\geq b)\leq e^{-sb}\mathbb E[e^{sX}]
=e^{s(\alpha(s)-b)}.
$$

**Optimize over the admissible positive values of $s$** to obtain

$$
\boxed{\mathbb P(X\geq b)\leq
\inf_{s>0:\,K(s)<\infty}\exp\{K(s)-sb\}.}
$$

For independent sources $X_1,\ldots,X_N$, [moment-generating functions](../../../../../../moment-generating-function.md) multiply and their [effective bandwidths](../../../../../../effective-bandwidth.md) add. Thus a total capacity $c$ has the one-time overflow bound $\mathbb P(\sum_iX_i\geq c)\leq\exp\{s(\sum_i\alpha_i(s)-c)\}$. In particular, for [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md),

$$
\mathbb P\!\left(\frac1N\sum_{i=1}^NX_i\geq c\right)
\leq\exp\{-N\sup_{s>0}[sc-K(s)]\}.
$$

This is the positive-parameter part of the [Legendre transform of a cumulant-generating function](../../../../../../legendre-transform-of-a-cumulant-generating-function.md). The size of its exponent describes how a service margin reduces the chance of a large aggregate demand. A buffer-overflow event involves traffic over many intervals; a one-time [Chernoff bound](../../../../../../chernoff-bound.md) alone is not automatically a bound on that event. A time-dependent model and, for example, bounds on the union of relevant interval events are then needed.

Assume a finite [moment-generating function](../../../../../../moment-generating-function.md) in a neighborhood of zero. Differentiating the [cumulant-generating function](../../../../../../cumulant-generating-function.md) gives $K(0)=0$, $K'(0)=\mathbb E[X]$ and $K''(0)=\operatorname{Var}(X)$. Therefore the **small-parameter limit is the mean traffic rate**:

$$
\boxed{\lim_{s\downarrow0}\alpha(s)=\mathbb E[X]},
\qquad \alpha(s)=\mathbb E[X]+\frac{s}{2}\operatorname{Var}(X)+O(s^2).
$$

The [variance](../../../../../../variance-split.md) term shows how an [effective bandwidth](../../../../../../effective-bandwidth.md) charges extra capacity for burstiness. Also $K$ is a [convex function](../../../../../../convex-function.md) with $K(0)=0$, so $K(s)/s$ is nondecreasing for $s>0$ in its domain.

For the other limit, let $M=\operatorname{ess\,sup}X$, the [essential supremum](../../../../../../essential-supremum.md). If $M<\infty$, $X\leq M$ almost surely gives $\alpha(s)\leq M$. For every $a<M$, $p_a=\mathbb P(X\geq a)>0$, and

$$
\alpha(s)\geq a+\frac{\log p_a}{s}.
$$

Taking a lower limit and then $a\uparrow M$ proves the **large-parameter limit is peak traffic**:

$$
\boxed{\lim_{s\to\infty}\alpha(s)=\operatorname{ess\,sup}X.}
$$

If $X$ has no finite upper bound and all positive exponential moments exist, the same lower bound for arbitrarily large $a$ makes the limit infinite. If positive exponential moments cease to exist at a finite parameter, the [effective bandwidth](../../../../../../effective-bandwidth.md) is infinite beyond that domain, and the infinite limit is understood in this extended sense. For example, a [normal distribution](../../../../../../normal-distribution.md) with mean $m$ and [variance](../../../../../../variance-split.md) $v$ has $\alpha(s)=m+sv/2$: its unbounded upper tail has no finite peak. Thus [effective bandwidth](../../../../../../effective-bandwidth.md) interpolates between mean and peak demand while permitting independent sources to be aggregated by addition.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 213](../../../paper-213-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
