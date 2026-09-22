# Clearance time after closing an infinite-server queue

↑ **Parent:** [General-service infinite-server queue](general-service-infinite-server-queue.md)

Stop new arrivals at time $t$ in an initially empty [general-service infinite-server queue](general-service-infinite-server-queue.md). The number remaining $v$ time units later is Poisson with mean $\lambda\int_v^{t+v}\mathbb P(S>u)\,du$. Thus the probability that clearance has not occurred is one minus the exponential of the negative of that mean. Letting $t\to\infty$ gives the displayed equilibrium formula, since $\int_v^\infty\mathbb P(S>u)\,du=\mathbb E(S-v)_+$. The clearance time is zero when no customers remain at closing.

## ↑ Ancestors (7)

1. [General-service infinite-server queue](general-service-infinite-server-queue.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/26i/e/solution.md)
