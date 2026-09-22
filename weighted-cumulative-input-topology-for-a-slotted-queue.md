# Weighted cumulative-input topology for a slotted queue

↑ **Parent:** [Sublinear path space for fluid queues](sublinear-path-space-for-fluid-queues.md)

For one-sided past inputs, let $A_n(a)=\sum_{j=0}^{n-1}a_{-j}$ and $A_0=0$. The displayed [metric](metric.md) controls cumulative differences over every past window, including the latest arrival. On the affine class $A_n(a)/n\to\lambda<c$, the [queue workload](workload-of-a-queue.md) $Q(a,c)=\sup_{n\geq0}(A_n(a)-cn)$ is locally [Lipschitz continuous](lipschitz-continuity.md). To prove this, choose $\varepsilon=(c-\lambda)/4$ and $N\geq1$ such that $A_n(a)/n\leq\lambda+\varepsilon$ for $n\geq N$. If $d_\#(a,b)<\varepsilon/2$, then $A_n(b)-cn\leq n(\lambda+2\varepsilon-c)<0$ for all such $n$. Both suprema reduce to $0\leq n<N$, and their difference is at most $(N+1)d_\#(a,b)$. Ignoring the latest coordinate makes this assertion false for a post-slot [workload of a queue](workload-of-a-queue.md).

## ↑ Ancestors (8)

1. [Sublinear path space for fluid queues](sublinear-path-space-for-fluid-queues.md)
2. [Stochastic network](stochastic-network.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Finite-memory continuity of a finite-buffer queue](finite-memory-continuity-of-a-finite-buffer-queue.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-77/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/3/e/solution.md)
- [Slower-server tandem workload identity](slower-server-tandem-workload-identity.md)
