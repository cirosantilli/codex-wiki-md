<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the amount of work $A_j(0,t]$ offered by one flow in a time interval of length $t$, its [effective bandwidth](../../../../../../effective-bandwidth.md) at parameter $\theta>0$ and timescale $t>0$ is

$$
\boxed{\alpha_j(\theta,t)=\frac1{\theta t}\log\mathbb E e^{\theta A_j(0,t]}.}
$$

Its units are work per unit time. The parameter $\theta$ measures the price placed on bursts: a stringent rare-overflow target generally requires a larger value of $\theta$ than a loose target. The timescale $t$ describes the duration of the congestion episode. When the limit exists, write

$$
\Lambda_j(\theta)=\lim_{t\to\infty}t^{-1}\log\mathbb E e^{\theta A_j(0,t]},
\qquad a_j(\theta)=\Lambda_j(\theta)/\theta.
$$

This is the long-time [effective bandwidth](../../../../../../effective-bandwidth.md). It includes a burstiness cost, rather than just the [mean](../../../../../../expected-value.md) offered rate. For a finite-time flow with the required moments, $\lim_{\theta\downarrow0}\alpha_j(\theta,t)=\mathbb E A_j(0,t]/t$, and [effective bandwidth](../../../../../../effective-bandwidth.md) is increasing in $\theta$. If $A_j(0,t]/t$ is bounded, its limit as $\theta\to\infty$ is the essential [supremum](../../../../../../supremum.md) of that interval's input rate, the peak-rate limit. The analogous long-time [mean](../../../../../../expected-value.md) limit requires the usual interchange or regularity assumptions.

For [independent](../../../../../../independent-random-variables.md) flows their [cumulant-generating functions](../../../../../../cumulant-generating-function.md) add, so

$$
\alpha_{\rm total}(\theta,t)=\sum_j\alpha_j(\theta,t),\qquad
a_{\rm total}(\theta)=\sum_j a_j(\theta).
$$

The [Chernoff bound](../../../../../../chernoff-bound.md) therefore gives, for any $\theta>0$ in the common domain,

$$
\mathbb P(A_{\rm total}(0,t]>Ct+b)
\leq\exp\{-\theta[b+Ct-t\alpha_{\rm total}(\theta,t)]\}.
$$

Optimizing over $\theta$ produces the relevant [Legendre-Fenchel transform](../../../../../../convex-conjugate.md). The [Cramér theorem](../../../../../../cramer-s-theorem.md) states that sample means of [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md) inputs whose [moment-generating function](../../../../../../moment-generating-function.md) is finite near zero have a [large deviation principle](../../../../../../large-deviation-principle.md), with [rate function](../../../../../../rate-function.md) equal to the [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) of their [cumulant-generating function](../../../../../../cumulant-generating-function.md). More generally, the [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) applies to a convergent scaled log [moment-generating function](../../../../../../moment-generating-function.md) when zero lies inside its domain and the limit is [lower semicontinuous](../../../../../../lower-semicontinuity.md) and [essentially smooth](../../../../../../essential-smoothness-of-a-convex-function.md). It gives the same transform as a [good rate function](../../../../../../good-rate-function.md). A sample-path version, together with the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) for the [queue workload](../../../../../../workload-of-a-queue.md), translates input deviations into overflow deviations. The compact-time and infinite-horizon continuity/tail hypotheses must be checked for the chosen traffic model.

A particularly useful rigorous [queue](../../../../../../queue-queueing-theory.md) bound holds for inputs with [stationary increments](../../../../../../stationary-increments.md) and [independent increments](../../../../../../independent-increments.md), such that $\mathbb E e^{\theta A(t)}=e^{t\Lambda(\theta)}$. If $\Lambda(\theta)\leq C\theta$, then

$$
M_t=e^{\theta(A(t)-Ct)}
$$

is a nonnegative [supermartingale](../../../../../../supermartingale.md), since its conditional increment factor is $e^{(t-s)(\Lambda(\theta)-C\theta)}\leq1$. The [maximal inequality for a nonnegative supermartingale](../../../../../../maximal-inequality-for-a-nonnegative-supermartingale.md) on $[0,T]$, followed by $T\to\infty$, gives the [continuous-time exponential workload bound](../../../../../../continuous-time-exponential-workload-bound.md)

$$
\boxed{\mathbb P(W\geq b)\leq e^{-\theta b},
\qquad W\overset d=\sup_{t\geq0}(A(t)-Ct),\quad
\sum_j a_j(\theta)\leq C.}
$$

Here $W$ is the stationary [queue workload](../../../../../../workload-of-a-queue.md) of the stable infinite-buffer [queue](../../../../../../queue-queueing-theory.md), represented by input from the past. This directly bounds the [supremum](../../../../../../supremum.md) over time; applying a one-time [Chernoff bound](../../../../../../chernoff-bound.md) alone would not establish it.

For a nonzero [Compound Poisson process](../../../../../../compound-poisson-process.md) with bounded positive packet sizes and [mean](../../../../../../expected-value.md) input rate less than $C$, a positive root $\theta_*$ of $\Lambda(\theta)=C\theta$ exists and is unique. Here the root theorem can be made explicit:

$$
e^{-\theta_*(b+s_{\max})}\leq\mathbb P(W\geq b)\leq e^{-\theta_*b}\quad(b>0).
$$

The upper bound was just proved. For the lower bound, use [exponential tilting](../../../../../../exponential-tilting.md) with density $e^{\theta_*(A(t)-Ct)}$ at time $t$. Under the tilted law the net input has positive [mean](../../../../../../expected-value.md) drift $\Lambda'(\theta_*)-C>0$, by strict convexity and the positive-root equation. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) then makes the first crossing time $\tau_b$ finite almost surely under that law. Its overshoot is at most $s_{\max}$. Changing measure at $\tau_b$, first on $\{\tau_b\leq T\}$ and then letting $T\to\infty$, gives

$$
\mathbb P(\tau_b<\infty)=\mathbb E_*\!\left[e^{-\theta_*(A(\tau_b)-C\tau_b)}\right]
\geq e^{-\theta_*(b+s_{\max})}.
$$

Dividing the logarithmic bounds by $b$ proves $\lim_{b\to\infty}b^{-1}\log\mathbb P(W\geq b)=-\theta_*$.

Thus the familiar admission rule compares $\sum_j a_j(\theta)$ with $C$, choosing $\theta$ from the desired buffer-tail exponent. For more general inputs, a logarithmic root theorem requires its own light-tail and renewal or sample-path hypotheses; the displayed supermartingale upper bound needs only the moment and increment assumptions stated above.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
