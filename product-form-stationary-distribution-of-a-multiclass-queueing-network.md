# Product-form stationary distribution of a multiclass queueing network

↑ **Parent:** [Stochastic network](stochastic-network.md)

Connect [multiclass single-server queues](multiclass-single-server-queue.md) by Markovian routing. Each node must either have common exponential service parameters across its classes or use a [symmetric service discipline](symmetric-service-discipline.md). If the [traffic equations for a multiclass queueing network](traffic-equations-for-a-multiclass-queueing-network.md) give loads $\rho_j=\sum_r\lambda_{jr}/\mu_{jr}<1$, its equilibrium word law is the product of the individual queue laws. Queue populations are independent at a fixed equilibrium time. A proof reverses routing with $p_{ba}^*=\lambda_a p_{ab}/\lambda_b$, external arrivals with $\nu_a^*=\lambda_a p_{a0}$, and exits with $p_{a0}^*=\nu_a/\lambda_a$, and interchanges the insertion and service position rules. Weight ratios verify each reversed transition, and the traffic equations match total rates. This is a [quasireversibility](quasireversibility.md) construction. A standard ordered-queue formulation is described in [Walton's paper on multiclass queueing networks, Section 2](https://arxiv.org/pdf/0809.2697).

## ↑ Ancestors (7)

1. [Stochastic network](stochastic-network.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/2/b/solution.md)
