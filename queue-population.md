# Queue population

↑ **Parent:** [Queue (queueing theory)](queue-queueing-theory.md)

The population $N(t)$ of a [queue](queue-queueing-theory.md) counts every admitted customer still inside the selected system at time $t$, including customers receiving service when the server is inside that boundary. Its long-run time average is $L$. The waiting population $N_q(t)$ excludes customers currently receiving service, and its long-run time average is $L_q$. For a single server that serves whenever work is present,

$$
N_q(t)=\max\{N(t)-1,0\},\qquad L=L_q+\rho,
$$

where $\rho$ is the [server utilization](server-utilization.md), assuming at most one customer receives service at a time. In a [stationary process](stationary-process.md) with [ergodicity](ergodicity.md) and finite [expected values](expected-value.md), these time averages equal $\mathbb E N(t)$ and $\mathbb E N_q(t)$. The [workload of a queue](workload-of-a-queue.md) instead counts unfinished work, so two [queues](queue-queueing-theory.md) with the same population can have very different remaining workloads.

## ↑ Ancestors (7)

1. [Queue (queueing theory)](queue-queueing-theory.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Little's law](little-s-law.md)
- [M/M/1 utilization and delay](m-m-1-utilization-and-delay.md)
- [Queueing theory](queueing-theory-split.md)
- [Sample-path area identity for Little's law](sample-path-area-identity-for-little-s-law.md)
