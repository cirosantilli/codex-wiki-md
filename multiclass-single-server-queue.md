# Multiclass single-server queue

↑ **Parent:** [Queueing theory](queueing-theory-split.md)

An ordered state $x=(c_1,\ldots,c_n)$ records the classes and positions of customers at a single server. Class-$r$ arrivals have rate $\alpha_r$ and exponential service parameter $\mu_r$. Under a [symmetric service discipline](symmetric-service-discipline.md), its [stationary distribution](stationary-distribution.md) is $(1-\rho)\prod_i(\alpha_{c_i}/\mu_{c_i})$, where $\rho=\sum_r\alpha_r/\mu_r<1$. If every $\mu_r=\mu$, class-independent insertion and service position rules need not be equal: [time reversal of a continuous-time Markov chain](time-reversal-of-a-continuous-time-markov-chain.md) interchanges them and proves the same law. Aggregating words gives $(1-\rho)n!\prod_r[(\alpha_r/\mu_r)^{n_r}/n_r!]$ by the [multinomial coefficient](multinomial-coefficient.md). With class-dependent service rates, [first come first served](first-come-first-served.md) need not have this product law.

**Table of contents**

- [Priority queue with a shared buffer](priority-queue-with-a-shared-buffer.md)
  - [Effective-bandwidth admission region with a voice delay gate](effective-bandwidth-admission-region-with-a-voice-delay-gate.md)

## ↑ Ancestors (6)

1. [Queueing theory](queueing-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [First come first served](first-come-first-served.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/2/b/solution.md)
- [Product-form stationary distribution of a multiclass queueing network](product-form-stationary-distribution-of-a-multiclass-queueing-network.md)
