# Poisson arrivals see time averages

↑ **Parent:** [Queueing theory](queueing-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_arrivals_see_time_averages)

[Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md) says that an exogenous, homogeneous [Poisson process](poisson-process.md) samples prearrival states with the same long-run frequencies as observation over time, provided the observed system cannot anticipate future arrivals and the relevant time averages exist. The system may depend on all past arrivals: an ordinary [queue](queue-queueing-theory.md) does. The required [independence](independent-random-variables.md) is between future increments of the [Poisson process](poisson-process.md) and the history available to the system, including its service information. Assume measurable state observations with ordinary [piecewise continuous functions](piecewise-continuous-function.md) as [sample paths](sample-path.md); write $X(t-)$ for the state immediately before time $t$.

For a state set $B$, let $A(T)$ count offered arrivals by time $T$ and let $t_k$ be their times. With a positive finite constant arrival rate, the [PASTA](poisson-arrivals-see-time-averages.md) equality is

$$
\lim_{T\to\infty}\frac{1}{A(T)}\sum_{k:t_k\leq T}\mathbf 1_{\{X(t_k-)\in B\}}
=\lim_{T\to\infty}\frac1T\int_0^T\mathbf 1_{\{X(t)\in B\}}\,dt,
$$

almost surely when the time limit exists. The [indicator functions](indicator-function.md) count visits on the left and time spent on the right. For a [stationary process](stationary-process.md) with [ergodicity](ergodicity.md), the right side is the stationary [probability](probability.md) of $B$. It matters that the arriving customer has not yet changed the observed state.

In the [M/M/1 utilization and delay](m-m-1-utilization-and-delay.md) example, [server utilization](server-utilization.md) is $0.8$. Thus [PASTA](poisson-arrivals-see-time-averages.md) says that 80 percent of offered arrivals find the server busy and 20 percent find the whole [queue](queue-queueing-theory.md) empty. If an offered arrival seeing population $n$ is admitted with [conditional probability](conditional-probability.md) $p(n)$, using fresh randomness independent of that state, the accepted fraction is $\sum_n\pi_np(n)$, where $\pi$ is the [stationary distribution](stationary-distribution.md). Multiplying this fraction by the offered rate gives the admitted [queue throughput](queue-throughput.md) when every admitted customer eventually completes service. Accepted arrivals are selected by state and need not themselves form a [Poisson process](poisson-process.md) or see the unconditioned time frequencies.

Arbitrary arrivals need not see time averages. Suppose a customer arrives every two minutes and its [service time](service-time.md) is exactly one minute, with one server and no other customers. The server is busy half the time, but every arrival finds it idle. A uniformly random initial phase can even make the occupancy a [stationary process](stationary-process.md), without repairing the disagreement. Nevertheless [Little's law](little-s-law.md) still gives $L=(1/2)\cdot1=1/2$, with rate measured in customers per minute. This separates [Little's law](little-s-law.md) from [PASTA](poisson-arrivals-see-time-averages.md).

Ronald W. Wolff's 1982 paper gave a general [PASTA](poisson-arrivals-see-time-averages.md) theorem under nonanticipation, rather than requiring the observed system to be independent of its driving [Poisson process](poisson-process.md). Its Theorem 1 compares the two long-run fractions; stationarity is a way to establish convergence, not the central sampling condition. [Wolff, Poisson Arrivals See Time Averages, Operations Research 30(2), 223-231](https://pubsonline.informs.org/doi/10.1287/opre.30.2.223). [Original paper, section 1 and Theorem 1](https://www.math.purdue.edu/~peterson/Teaching/532/PASTA.pdf).

## ↑ Ancestors (6)

1. [Queueing theory](queueing-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Blocking partition ratio for a loss network](blocking-partition-ratio-for-a-loss-network.md)
- [Blocking probability in a finite-line sequential-service network](blocking-probability-in-a-finite-line-sequential-service-network.md)
- [Effective-bandwidth admission region with a voice delay gate](effective-bandwidth-admission-region-with-a-voice-delay-gate.md)
- [Finite-buffer server utilization](finite-buffer-server-utilization.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/27j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/27j/b/ii/solution.md)
- [Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md)
- [Queueing theory](queueing-theory-split.md)
- [Rearrangeable triangular loss network](rearrangeable-triangular-loss-network.md)
- [Stationary flow conservation in a finite-line switchboard](stationary-flow-conservation-in-a-finite-line-switchboard.md)
