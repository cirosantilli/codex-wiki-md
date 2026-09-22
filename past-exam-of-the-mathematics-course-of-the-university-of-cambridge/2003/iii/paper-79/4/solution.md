<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Consider a stationary nonnegative work-input process in slotted time, with cumulative work $A_n$ over the last $n$ slots and a work-conserving server of capacity $c$ per slot. Assume its past average tends almost surely to $m<c$. The [Lindley recursion](../../../../../lindley-recursion.md) then defines the finite stationary [queue workload](../../../../../workload-of-a-queue.md)

$$
Q=\sup_{n\geq0}(A_n-cn).
$$

This is work remaining, rather than the number of customers when customer service requirements vary. With unit work per customer the two notions coincide. Stationarity makes the [distribution](../../../../../distribution-mathematical-analysis.md) of a past cumulative window equal to that of a forward window of the same length.

For a parameter $\theta>0$ and a positive window length $n$, the [effective bandwidth](../../../../../effective-bandwidth.md) is

$$
\boxed{\alpha(\theta,n)=\frac{1}{\theta n}\log\mathbb E e^{\theta A_n}.}
$$

It measures a traffic rate through exponential moments, so it retains information about rare bursts that the mean alone discards. If the limiting scaled [cumulant-generating function](../../../../../cumulant-generating-function.md) exists, put

$$
\kappa(\theta)=\lim_{n\to\infty}\frac1n\log\mathbb E e^{\theta A_n},\qquad
\alpha(\theta)=\frac{\kappa(\theta)}{\theta}.
$$

The finite-window [effective bandwidth](../../../../../effective-bandwidth.md) matters when the relevant overflow window is short or when arrivals are correlated; one should not replace it by its long-window limit without justification.

The following proof gives an actual upper bound for the infinite-horizon [queue workload](../../../../../workload-of-a-queue.md). For $B>0$, if $Q>B$, at least one positive integer $n$ has $A_n-cn>B$. The [union bound](../../../../../boole-s-inequality.md) followed by the [Chernoff bound](../../../../../chernoff-bound.md) gives

$$
\mathbb P(Q>B)\leq\sum_{n\geq1}\mathbb P(A_n>B+cn)
\leq e^{-\theta B}\sum_{n\geq1}\exp\{\theta n[\alpha(\theta,n)-c]\}.
$$

Assume each finite-window exponential moment is finite and $\kappa(\theta)<c\theta$. Choose $\eta>0$ such that $\kappa(\theta)+\eta<c\theta$. For all sufficiently large $n$, the summand is at most $e^{-n(c\theta-\kappa(\theta)-\eta)}$. Its tail is a convergent geometric series, and its finite prefix is finite. Denote the resulting sum by $K_\theta$. The [exponential workload bound from cumulative arrival moments](../../../../../exponential-workload-bound-from-cumulative-arrival-moments.md) therefore proves, for $b>0$,

$$
\limsup_{L\to\infty}\frac1L\log\mathbb P(Q>Lb)\leq-\theta b.
$$

Optimizing over admissible parameters gives

$$
\boxed{\limsup_{L\to\infty}\frac1L\log\mathbb P(Q>Lb)\leq-b\theta_*,\qquad
\theta_* =\sup\{\theta>0:\kappa(\theta)<c\theta\}.}
$$

Only parameters with the stated finite-window moments are included. If there are no such positive parameters, the argument yields only the trivial exponent zero. Infinite $\theta_*$ means that the upper rate is $-\infty$. For a non-strict threshold $Q\geq Lb$, first bound it by $Q>L(b-\varepsilon)$ and then let $\varepsilon\downarrow0$. This proof permits dependence between slots. It proves the required upper bound; it does not assert a matching lower bound for every arrival process.

This also gives a closed-set large-deviation upper bound for $Q/L$: set $I_+(q)=\theta_*q$ for $q>0$, $I_+(0)=0$, and $I_+(q)=+\infty$ for $q<0$. If a [closed set](../../../../../closed-set.md) $F$ contains zero, its desired upper bound is the trivial bound zero. If $F$ contains positive points but not zero, its positive part has a smallest point $b>0$, and $\mathbb P(Q/L\in F)\leq\mathbb P(Q\geq Lb)$ gives the bound $-\inf_F I_+$. If it contains no nonnegative points, its probability is zero. This verifies the upper half of a [large deviation principle](../../../../../large-deviation-principle.md); the actual [rate function](../../../../../rate-function.md) can be larger when a matching lower bound is unavailable.

For [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) slot arrivals $a_t$, let $\kappa(\theta)=\log\mathbb E e^{\theta a_0}$. Now $\log\mathbb E e^{\theta A_n}=n\kappa(\theta)$, so [effective bandwidth](../../../../../effective-bandwidth.md) is independent of window length. For $\kappa(\theta)<c\theta$, the geometric-series prefactor is explicitly

$$
K_\theta=\frac{e^{\kappa(\theta)-c\theta}}{1-e^{\kappa(\theta)-c\theta}}.
$$

Thus the familiar [workload Chernoff bound for independent increments](../../../../../workload-chernoff-bound-for-independent-increments.md) is a special case, and the largest admissible parameter is often the positive root of $\kappa(\theta)=c\theta$.

For these independent increments there is a sharper argument that works at the root itself when its exponential moment is finite. Along the past read in reverse order, put $S_n=A_n-cn$ and $M_n=e^{\theta S_n}$. If $\mathbb E e^{\theta(a_0-c)}\leq1$, then $M_n$ is a nonnegative [supermartingale](../../../../../supermartingale.md) starting at one. For the first crossing time $\tau_B=\inf\{n\geq0:S_n\geq B\}$, bounded [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
1\geq\mathbb E M_{\tau_B\wedge N}\geq e^{\theta B}\mathbb P(\tau_B\leq N).
$$

Let $N\to\infty$. Strict negative drift makes $S_n\to-\infty$ almost surely, so its supremum is attained and the crossing event agrees with $\{Q\geq B\}$. Consequently

$$
\boxed{\mathbb P(Q\geq B)\leq e^{-\theta B}.}
$$

This strengthens the prefactor but uses temporal [independence](../../../../../independent-random-variables.md), which was unnecessary for the previous proof.

Several examples show what the [effective bandwidth](../../../../../effective-bandwidth.md) constraint means. Deterministic traffic of $r$ work units per slot has $\kappa(\theta)=\theta r$ and [effective bandwidth](../../../../../effective-bandwidth.md) $r$ at every parameter; if $c\geq r$ there is no stationary backlog. For independent on-off slots carrying $r$ units with probability $p$ and zero otherwise, the [Bernoulli effective bandwidth](../../../../../bernoulli-effective-bandwidth.md) is

$$
\alpha(\theta)=\frac{\log(1-p+pe^{\theta r})}{\theta}.
$$

For $0<p<1$, it rises from the mean $pr$ to the peak $r$. When $pr<c<r$, strict [convexity](../../../../../convex-function.md) of $\kappa(\theta)-c\theta$, its negative derivative at zero, and its divergence to infinity give a unique positive root. When $c\geq r$, no slot can increase the [queue workload](../../../../../workload-of-a-queue.md). In the specific case $r=2,c=1,p<1/2$, the workload increases by one with probability $p$ and decreases by one, reflected at zero, with probability $1-p$. Its stationary probabilities satisfy

$$
\pi_{k+1}=\frac{p}{1-p}\pi_k,\qquad
\pi_k=(1-q)q^k,\quad q=\frac{p}{1-p}.
$$

The service-root equation has $e^{\theta_*}=(1-p)/p$, and thus $\mathbb P(Q\geq k)=q^k=e^{-\theta_* k}$. This example realizes the upper exponent exactly.

For independent [Poisson](../../../../../poisson-distribution.md) slot counts of mean $\nu$, with unit work per arrival, the [Poisson effective bandwidth](../../../../../poisson-effective-bandwidth.md) is

$$
\alpha(\theta)=\frac{\nu(e^\theta-1)}{\theta}.
$$

Stability requires $c>\nu$. There is a unique positive root of $\nu(e^\theta-1)=c\theta$, again by strict [convexity](../../../../../convex-function.md), negative initial derivative after subtracting $c\theta$, and growth to infinity. For independent exponentially distributed work with rate $\beta$, the corresponding expressions are

$$
\kappa(\theta)=-\log(1-\theta/\beta),\qquad
\alpha(\theta)=\frac{-\log(1-\theta/\beta)}{\theta},\qquad 0<\theta<\beta.
$$

If $c>1/\beta$, the positive service root lies strictly below $\beta$. The finite [moment-generating function](../../../../../moment-generating-function.md) domain cannot be ignored.

To see statistical aggregation explicitly, let the entire arrival processes of $k$ sources be [independent](../../../../../independent-random-variables.md), though each source may itself have dependence over time. Their cumulative totals satisfy

$$
\mathbb E e^{\theta\sum_{j=1}^k A_n^{(j)}}=\prod_{j=1}^k\mathbb E e^{\theta A_n^{(j)}},\qquad
\boxed{\alpha_{\rm total}(\theta,n)=\sum_{j=1}^k\alpha_j(\theta,n).}
$$

Thus the shared [queue](../../../../../queue-queueing-theory.md) has an exponential overflow bound when $\sum_j\alpha_j(\theta)<c$, with the finite-window conditions proved above. One must use a common parameter $\theta$; adding individual service-root exponents is not the rule. For example, an independent [Poisson](../../../../../poisson-distribution.md) source of mean $\nu$ and an independent on-off source of size $r$ and probability $p$ have aggregate [cumulant-generating function](../../../../../cumulant-generating-function.md)

$$
\kappa_{\rm total}(\theta)=\nu(e^\theta-1)+\log(1-p+pe^{\theta r}).
$$

For $\nu>0$ and $c>\nu+pr$, their positive service root exists and determines the optimized upper exponent. Several independent [Poisson](../../../../../poisson-distribution.md) sources similarly have the same formula as one source with intensity $\sum_j\nu_j$.

The connection with [large deviation principles](../../../../../large-deviation-principle.md) also appears in a many-source scaling. For $L$ independent copies of a source, aggregate service $Lc$ and buffer $Lb$, fix a window $n$. Let $X_i(n)$ be each copy's cumulative input in that window. Their total exceeds $L(b+cn)$ only if the empirical mean exceeds $b+cn$. Its [Chernoff bound](../../../../../chernoff-bound.md) has exponent

$$
V_n(b)=\sup_{\theta\geq0}\{\theta(b+cn)-\log\mathbb E e^{\theta X_1(n)}\}
=\sup_{\theta\geq0}\theta\{b+n[c-\alpha(\theta,n)]\}.
$$

If exponential moments exist near zero, [Cramér's theorem](../../../../../cramer-s-theorem.md) gives the corresponding finite-window [large deviation principle](../../../../../large-deviation-principle.md). The threshold exceeds the mean because $m<c$ and $b>0$. A finite union of windows has upper exponential rate at most $-\min_n V_n(b)$ over those windows. Passing to infinitely many windows requires uniform control of long-window probabilities, not simply an interchange of a limit with an infinite union. A good sample-path [large deviation principle](../../../../../large-deviation-principle.md) in a topology where the [queue workload](../../../../../workload-of-a-queue.md) is [continuous](../../../../../continuous-function.md), as in Question 3, instead permits the [contraction principle for large deviations](../../../../../contraction-principle-for-large-deviations.md) to derive a workload [rate function](../../../../../rate-function.md) and its closed-set overflow upper bound.

Finally, the [mean and peak limits of effective bandwidth](../../../../../mean-and-peak-limits-of-effective-bandwidth.md) quantify the safety margin. With exponential moments near zero, independent slot work of mean $m$ and [variance](../../../../../variance-split.md) $v$ has

$$
\alpha(\theta)=m+\frac{v\theta}{2}+O(\theta^2).
$$

For bounded work, its large-parameter limit is the essential peak. Stronger tail requirements select larger $\theta$ and hence more capacity; finite-window [effective bandwidths](../../../../../effective-bandwidth.md) also reflect temporal burst correlations. A stable heavy-tailed input can lack every positive exponential moment, in which case this exponential-bound method supplies no positive decay rate. Stability and exponentially small overflow are distinct requirements.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
