# Finite-memory continuity of a finite-buffer queue

↑ **Parent:** [Finite-buffer workload map](finite-buffer-workload-map.md)

Use the clipped [Lindley recursion](lindley-recursion.md) $q_{t+1}=\min(B,\max(0,q_t+x_t-C))$ and the [weighted cumulative-input topology for a slotted queue](weighted-cumulative-input-topology-for-a-slotted-queue.md). If cumulative past input $S_x(T)\leq\lambda T$ eventually with $\lambda<C$, choose a finite $T$ so $S_x(T)-CT<-B$. Starting with a full buffer at time $-T$, the queue must hit zero before the present, since otherwise its final workload is at most $B+S_x(T)-CT<0$. Monotonicity couples all initial workloads by that zero, establishing a finite memory horizon. The same horizon works for sufficiently close input $y$. Since $|x_{-k}-y_{-k}|\leq(2k-1)\|x-y\|$ and clipping is [Lipschitz continuous](lipschitz-continuity.md) with constant one, the two finite recursions started empty differ by at most $\sum_{k=1}^T(2k-1)\|x-y\|=T^2\|x-y\|$.

## ↑ Ancestors (9)

1. [Finite-buffer workload map](finite-buffer-workload-map.md)
2. [Workload of a queue](workload-of-a-queue.md)
3. [Queue (queueing theory)](queue-queueing-theory.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-77/4/solution.md)
