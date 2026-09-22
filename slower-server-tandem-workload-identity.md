# Slower-server tandem workload identity

↑ **Parent:** [Lindley recursion](lindley-recursion.md)

Consider two work-conserving slotted [queues](queue-queueing-theory.md) in tandem, with upstream service $c$ and downstream service $d<c$, where upstream departures can be served downstream in the same slot. Put $D_t=\min\{c,Q_{t-1}+a_t\}$. Then $Q_t=Q_{t-1}+a_t-D_t$ and $R_t=(R_{t-1}+D_t-d)^+$. If $R_{t-1}+D_t\geq d$, addition gives $(Q_{t-1}+R_{t-1}+a_t-d)^+$. Otherwise $D_t<d<c$, so the upstream queue empties and both sides of that identity are zero. Thus total workload obeys the [Lindley recursion](lindley-recursion.md) with service $d$. Starting empty in the remote past yields the displayed identity whenever the upstream workload is finite. Both workloads, and hence their difference, are [continuous](continuous-function.md) in the [weighted cumulative-input topology for a slotted queue](weighted-cumulative-input-topology-for-a-slotted-queue.md) under strictly subcritical mean input $\lambda<d<c$.

## ↑ Ancestors (9)

1. [Lindley recursion](lindley-recursion.md)
2. [Workload of a queue](workload-of-a-queue.md)
3. [Queue (queueing theory)](queue-queueing-theory.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/3/c/solution.md)
