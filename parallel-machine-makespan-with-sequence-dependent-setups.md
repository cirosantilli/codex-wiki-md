# Parallel-machine makespan with sequence-dependent setups

↑ **Parent:** [Scheduling](scheduling.md)

Partition jobs between machines and choose an ordering on each machine. Machine $r$ has load $C_r$ equal to its processing times, initial setup and internal changeovers; the completion time of all jobs is the [maximum](maximum-of-a-subset-of-a-total-order.md) of these loads. Minimize a variable $C_{\max}$ subject to $C_r\leq C_{\max}$ for every machine. [Branch and bound](branch-and-bound.md) can combine machine-assignment decisions with route bounds; heuristic moves relocate jobs between machines, swap jobs, and reorder blocks. Minimizing the sum of route costs alone does not generally minimize the makespan.

## ↑ Ancestors (5)

1. [Scheduling](scheduling.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/5/solution.md)
- [Scheduling](scheduling.md)
