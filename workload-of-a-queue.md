# Workload of a queue

↑ **Parent:** [Queue (queueing theory)](queue-queueing-theory.md)

The [queue workload](workload-of-a-queue.md) of a [queue](queue-queueing-theory.md) is the total remaining service work of all present customers, including residual work in service. With a work-conserving server of rate $C$ and stationary input $A$, the stationary [queue workload](workload-of-a-queue.md) is represented by

$$
W(0)=\sup_{t\geq0}\{A(-t,0]-Ct\}.
$$

This is the amount by which past offered work exceeds available service, maximized over possible starts of a busy period. It is the reflection of net input at zero. Under [first come first served](first-come-first-served.md), an arriving infinitesimal customer waits $W/C$; a priority customer instead waits for the remaining work ahead of it under its [service discipline](service-discipline.md).

**Table of contents**

- [Stationary workload supremum](stationary-workload-supremum.md)
- [Linear workload rate for a local convex action](linear-workload-rate-for-a-local-convex-action.md)
- [Constant-rate burst path](constant-rate-burst-path.md)
- [Finite-buffer workload map](finite-buffer-workload-map.md)
  - [Finite-memory continuity of a finite-buffer queue](finite-memory-continuity-of-a-finite-buffer-queue.md)
  - [Finite-buffer workload rate truncation](finite-buffer-workload-rate-truncation.md)
- [Lindley recursion](lindley-recursion.md)
  - [Slower-server tandem workload identity](slower-server-tandem-workload-identity.md)

## ↑ Ancestors (7)

1. [Queue (queueing theory)](queue-queueing-theory.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/3/b/solution.md)
- [Weighted cumulative-input topology for a slotted queue](weighted-cumulative-input-topology-for-a-slotted-queue.md)
