<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $A_n$ for work arriving in slot $n$ and $c$ for the [service rate of a queue](../../../../../service-rate-of-a-queue.md). For a work-conserving single-server [queue](../../../../../queue-queueing-theory.md), the [Lindley recursion](../../../../../lindley-recursion.md) is $Q_{n+1}=(Q_n+A_{n+1}-c)^+$. For stable [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with mean $\mu<c$, its [stationary workload supremum](../../../../../stationary-workload-supremum.md) has the form

$$
Q\overset d=\sup_{n\ge0}\left(\sum_{j=1}^nA_j-cn\right).
$$

Different [scaling limits of a queue](../../../../../scaling-limit-of-a-queue.md) concern different quantities growing large; they need not share either a probability speed or a likely path to overflow.

For [large-buffer queue scaling](../../../../../large-buffer-queue-scaling.md), fix the input law and $c>\mu$ and let the [buffer size of a queue](../../../../../buffer-size-of-a-queue.md) $b\to\infty$. Assume finite exponential moments around a positive root $\theta_*$ of $\Lambda_A(\theta)=c\theta$. An overflow accumulated in $n\simeq tb$ slots requires an average input about $c+1/t$, so [Cramér's theorem](../../../../../cramer-s-theorem.md) assigns logarithmic cost $b\,tI_A(c+1/t)$. Optimizing the duration gives the [Cramér-Lundberg workload exponent](../../../../../cramer-lundberg-workload-exponent.md)

$$
\frac1b\log\mathbb P(Q>b)\longrightarrow-\theta_*,
\qquad \theta_* =\inf_{t>0}tI_A(c+1/t).
$$

For an interior root with $\Lambda_A'(\theta_*)>c$, [Fenchel–Young inequality](../../../../../fenchel-young-inequality.md) verifies the minimization: the lower bound is $\theta_*$ because $I_A(x)\ge\theta_*x-\Lambda_A(\theta_*)$, and equality occurs at $t=[\Lambda_A'(\theta_*)-c]^{-1}$. The [exponential workload bound from cumulative arrival moments](../../../../../exponential-workload-bound-from-cumulative-arrival-moments.md) gives the upper exponent for every $\theta<\theta_*$; an [exponentially tilted](../../../../../exponential-tilting.md) positive-drift path or the duration calculation gives the matching lower exponent. In [effective bandwidth](../../../../../effective-bandwidth.md) notation, $\Lambda_A(\theta_*)/\theta_*=c$. This regime measures long accumulation into a large buffer with a fixed positive stability margin.

For [many-source queue scaling](../../../../../many-source-queue-scaling.md), superpose $L$ independent copies of an input process, give the server capacity $Lc$, and give it buffer size $Lb$. For each lookback horizon $n$, the average of the $L$ source cumulative arrivals has a [large deviation principle](../../../../../large-deviation-principle.md) with [rate function](../../../../../rate-function.md) $I_n$. Overflow at that horizon costs $L I_n(b+cn)$. Optimizing the lookback horizon suggests

$$
\frac1L\log\mathbb P(Q_L>Lb)\longrightarrow-V(b),
\qquad V(b)=\inf_{n\ge1}I_n(b+cn).
$$

For [independent](../../../../../independent-random-variables.md) slots, $I_n(x)=nI_A(x/n)$, giving $V(b)=\inf_{n\ge1}nI_A(c+b/n)$. The integer horizon is important in a slotted system. For temporally dependent sources, use the cumulative-input [cumulant-generating function](../../../../../cumulant-generating-function.md), rather than multiplying a one-slot formula by $n$. The heuristic needs uniform control of the tail of the stationary supremum to justify optimizing an unbounded set of horizons; stability and suitable exponential-moment estimates provide this in the usual models. The growing quantity here is the number of independent sources, while per-source capacity and buffer remain fixed.

For [moderate-deviation queue scaling](../../../../../moderate-deviation-queue-scaling.md), consider a [bufferless queue](../../../../../bufferless-queue.md) with aggregate [Poisson](../../../../../poisson-distribution.md) input of mean $L\lambda$ and capacity $L\lambda+C L^{(1+\beta)/2}$, $0<\beta<1$. The spare capacity is much larger than the ordinary [central limit theorem](../../../../../central-limit-theorem.md) scale $\sqrt L$ but much smaller than $L$. The [Poisson sample-mean rate function](../../../../../poisson-sample-mean-rate-function.md) near its minimum has expansion

$$
I_P(\lambda+h)=\frac{h^2}{2\lambda}+O(h^3).
$$

With $h=C L^{(\beta-1)/2}$, the cost $LI_P(\lambda+h)$ is asymptotic to $C^2L^\beta/(2\lambda)$. Hence [Poisson moderate deviations](../../../../../poisson-moderate-deviation-principle.md) give $\log\mathbb P(\mathrm{overflow})\sim-C^2L^\beta/(2\lambda)$. The quadratic cost comes from a shrinking neighborhood of the mean, rather than from a fixed macroscopic overload. The regime is useful for a large aggregate whose service margin lies between its typical fluctuation scale and its mean scale.

For a [heavy-traffic limit of a queue](../../../../../heavy-traffic-limit-of-a-queue.md), instead hold the input law fixed with mean $\mu$ and positive finite [variance](../../../../../variance-split.md) $\sigma^2$, and let $c_\varepsilon=\mu+\varepsilon d$ with $d>0$ and $\varepsilon\downarrow0$. In $t/\varepsilon^2$ slots the net input has mean about $-dt/\varepsilon$ and random fluctuation of size $\sigma\sqrt t/\varepsilon$. Thus the [functional central limit theorem](../../../../../donsker-s-theorem.md), followed by the [Skorokhod reflection map on the half-line](../../../../../skorokhod-reflection-map-on-the-half-line.md), suggests

$$
\varepsilon Q_\varepsilon(\lfloor t/\varepsilon^2\rfloor)
\Rightarrow R(t),
$$

where $R$ is [reflected Brownian motion with negative drift](../../../../../reflected-brownian-motion-with-negative-drift.md) $-d$ and variance parameter $\sigma^2$. The [stationary law of negatively drifted reflected Brownian motion](../../../../../stationary-law-of-negatively-drifted-reflected-brownian-motion.md) has tail $\mathbb P(R_\infty>b)=e^{-2db/\sigma^2}$. When passing the stationary distribution through the limit is justified, this predicts

$$
\mathbb P(Q_\varepsilon>b/\varepsilon)\approx e^{-2db/\sigma^2}.
$$

For dependent input satisfying a suitable invariance principle, replace $\sigma^2$ by its [long-run variance of a stationary process](../../../../../long-run-variance-of-a-stationary-process.md). This regime is appropriate near critical load and on long time scales; a functional transient limit alone does not automatically justify the stationary-limit interchange.

A different large-service regime holds the input law fixed. With [Poisson distribution](../../../../../poisson-distribution.md) of mean $\lambda$ and bufferless capacity $c\to\infty$, let $m=\lfloor c\rfloor+1$. The single-point lower bound $\mathbb P(X=m)$ and the optimized [Chernoff bound](../../../../../chernoff-bound.md) for $X\ge m$, using [Stirling's formula](../../../../../stirling-formula.md), give the [Poisson large-service overflow asymptotic](../../../../../poisson-large-service-overflow-asymptotic.md)

$$
\log\mathbb P(X>c)=-c\log(c/\lambda)+c-\lambda+O(\log c),
\qquad \frac{\log\mathbb P(X>c)}{c\log c}\to-1.
$$

Here the service rate grows while the input mean does not. A quadratic moderate-deviation approximation would describe the wrong part of the [Poisson](../../../../../poisson-distribution.md) tail.

To choose a regime, compare the spare capacity, typical fluctuations, number of sources and buffer size before selecting a formula. Use the large-buffer exponent for a fixed stable input and a long overload episode; use the many-source variational cost when independent flows and resources grow together; use moderate deviations for an intermediate safety margin; use the heavy-traffic diffusion when the stability margin tends to zero; and use the fixed-input Poisson tail when service alone becomes very large. Check temporal dependence and exponential-moment assumptions. For [heavy-tailed subexponential distributions](../../../../../subexponential-distribution-heavy-tailed.md), a single exceptionally large arrival can dominate overflow, so a finite exponential workload root and a Brownian approximation to the far tail need not apply. These comparisons explain why the same nominal [queueing theory](../../../../../queueing-theory-split.md) system can have different useful asymptotic descriptions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
