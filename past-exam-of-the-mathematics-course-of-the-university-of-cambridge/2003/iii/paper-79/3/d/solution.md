<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the downstream [queue workload](../../../../../../workload-of-a-queue.md) by starting both [queues](../../../../../../queue-queueing-theory.md) empty at time $-N$ and taking the increasing remote-past limit. For each finite $N$, part (c) makes their total [queue workload](../../../../../../workload-of-a-queue.md) exactly the single-server workload with service $d$, while the upstream [queue workload](../../../../../../workload-of-a-queue.md) is the single-server workload with service $c$. Therefore

$$
R_0^{(N)}(a,c,d)=Q_0^{(N)}(a,d)-Q_0^{(N)}(a,c).
$$

The downstream limit is increasing: the coupled upstream and downstream recursions are increasing in their initial state, because $D_t=\min(c,Q_{t-1}+a_t)$ is increasing in $Q_{t-1}$. With finite upstream [queue workload](../../../../../../workload-of-a-queue.md), taking the limit gives

$$
\boxed{R_0(a,c,d)=Q_0(a,d)-Q_0(a,c).}
$$

The result is nonnegative because reducing service cannot reduce [queue workload](../../../../../../workload-of-a-queue.md). It can be $+\infty$ when the slower server is unstable; under $\lambda<d<c$, both quantities are finite. The finite-upstream condition matters: subtracting two infinite [queue workloads](../../../../../../workload-of-a-queue.md) would not define a downstream queue.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
