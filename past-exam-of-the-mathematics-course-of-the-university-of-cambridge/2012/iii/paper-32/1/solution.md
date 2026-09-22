<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a stable system in which entering customers eventually leave, [Little's law](../../../../../little-s-law.md) is

$$
\boxed{L=\lambda_{\mathrm{eff}}W.}
$$

Here $L$ is the long-run mean number of customers in the chosen system, $\lambda_{\mathrm{eff}}$ is its actual entry rate, and $W$ is the mean [customer sojourn time](../../../../../customer-sojourn-time.md). The arrival rate counts admitted customers, not rejected attempts. One way to see the identity is to integrate the customer count over time: each customer's time in the system contributes exactly that much area. Dividing by elapsed time gives entry rate times mean [customer sojourn time](../../../../../customer-sojourn-time.md), with negligible endpoint terms under the usual stability and integrability assumptions.

For the server alone in a stationary [M/M/1 queue](../../../../../m-m-1-queue.md), the customer count is the busy indicator. Customers enter this subsystem when their service begins; in a stable, loss-free queue its entry rate equals $\lambda$. Their mean time in this subsystem is the mean [service time](../../../../../service-time.md) $\mu$. Thus **$\boxed{\mathbb P(\text{server busy})=\lambda\mu}$**, with stability requiring $\lambda\mu<1$. In this paper $\mu$ denotes a mean duration, so the exponential service rate is $1/\mu$.

For [finite-buffer server utilization](../../../../../finite-buffer-server-utilization.md), assume the server is work conserving and admitted customers are eventually served, with finite mean [service time](../../../../../service-time.md). [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md), so an offered arrival is rejected with probability $P_n$. Hence the admitted arrival rate, and therefore the service-entry rate, or [queue throughput](../../../../../queue-throughput.md), is $\lambda(1-P_n)$. Apply [Little's law](../../../../../little-s-law.md) to the server alone again. Its mean population, or [server utilization](../../../../../server-utilization.md), is $1-P_0$, and its mean [customer sojourn time](../../../../../customer-sojourn-time.md) is $\mu$, giving **$\boxed{1-P_0=\lambda\mu(1-P_n)}$.** Neither argument requires exponential service times in the finite-buffer system: Poisson arrivals are used for the blocking probability, while the service calculation needs only the mean and the stated independence. Applying the offered rate $\lambda$ directly to this lossy system would miss the admission factor.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
