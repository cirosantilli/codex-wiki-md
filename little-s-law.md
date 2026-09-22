<h1 id="little-s-law">Little's law</h1>

↑ **Parent:** [Queueing theory](queueing-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Little's_law)

For a stable [queue](queue-queueing-theory.md) with finite long-run averages, a positive finite admitted rate, and negligible initial and terminal contributions after division by observation time, [Little's law](little-s-law.md) states

$$
L=\lambda_{\mathrm{eff}}W.
$$

Here $L$ is the time-average [queue population](queue-population.md), $\lambda_{\mathrm{eff}}$ is the admitted rate through the chosen system, and $W$ is the customer-average [customer sojourn time](customer-sojourn-time.md) inside that same boundary. Without abandonment, admitted rate equals completed-service [queue throughput](queue-throughput.md) in this stable regime. It may differ from the offered arrival rate because of blocking. When customers abandon, count their admissions and exits too, and average their actual time inside; using only service completions would mismatch the population being measured.

For the waiting area alone the matching identity is

$$
L_q=\lambda_{\mathrm{eff}}W_q,
$$

where $W_q$ is mean [queueing delay](queueing-delay.md). For one server with no abandonment, service in arrival order, and finite mean [service time](service-time.md) $\mathbb E S$,

$$
W=W_q+\mathbb E S,\qquad L=L_q+\lambda_{\mathrm{eff}}\mathbb E S=L_q+\rho,
$$

with $\rho$ the [server utilization](server-utilization.md). Mixing total population $L$ with waiting-only duration $W_q$ would count different portions of each customer's visit. Customers who start service immediately contribute zero to $W_q$, and must still be included in that customer average.

The strength of [Little's law](little-s-law.md) is that it does not require a [Poisson process](poisson-process.md), an [exponential distribution](exponential-distribution.md) of [service times](service-time.md), or service in arrival order. The [sample-path area identity for Little's law](sample-path-area-identity-for-little-s-law.md) explains why: counting customer-time across time slices or across customer visits gives the same area. A sufficient probabilistic setting is repeated [independent and identically distributed](independent-and-identically-distributed-random-variables.md) empty-to-empty cycles with finite positive mean cycle duration, finite positive mean customer count, and finite mean population area; the [renewal-reward theorem](renewal-reward-theorem.md) then supplies the long-run averages. Stability alone does not guarantee finite mean [queueing delay](queueing-delay.md): the [Pollaczek-Khinchine mean formula](pollaczek-khinchine-mean-formula.md) shows why a finite [second moment](second-moment.md) of [service time](service-time.md) matters for that mean in an [M/G/1 queue](m-g-1-queue.md).

For example, suppose a service desk receives six requests per hour but admits only four; measured mean [customer sojourn time](customer-sojourn-time.md) of admitted requests is half an hour. Its mean [queue population](queue-population.md) is $4\cdot(1/2)=2$ customers. Multiplying the offered rate by that duration would incorrectly give three. Conversely, counting two customers on average and measuring admitted [queue throughput](queue-throughput.md) of four per hour gives $W=2/4=1/2$ hour. This lets one estimate a hard-to-track duration from occupancy and completed-job counts.

John D. C. Little published a rigorous proof in 1961 under finite-mean, [strict stationarity](strictly-stationary-process.md), and [ergodicity](ergodicity.md) assumptions on the arrival process. Those were assumptions of that proof, rather than a requirement that every useful form of the identity have random arrivals. [Little, A Proof for the Queuing Formula: L = λW, Operations Research 9(3), 383-387](https://pubsonline.informs.org/doi/10.1287/opre.9.3.383). [Original paper, opening statement](https://fisherp.scripts.mit.edu/wordpress/wp-content/uploads/2015/11/ContentServer.pdf).

**Table of contents**

- [Sample-path area identity for Little's law](sample-path-area-identity-for-little-s-law.md)

## ↑ Ancestors (6)

1. [Queueing theory](queueing-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Customer sojourn time](customer-sojourn-time.md)
- [Little's law](little-s-law.md)
- [M/M/1 utilization and delay](m-m-1-utilization-and-delay.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/25i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/1/solution.md)
- [Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md)
- [Queue throughput](queue-throughput.md)
- [Queueing theory](queueing-theory-split.md)
- [Sample-path area identity for Little's law](sample-path-area-identity-for-little-s-law.md)
- [Server utilization](server-utilization.md)
- [Service time](service-time.md)
