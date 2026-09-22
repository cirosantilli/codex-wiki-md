# Moore-Hodgson algorithm

↑ **Parent:** [Scheduling](scheduling.md)

For single-machine jobs all available at time zero, order by nondecreasing deadline. Keep a tentative on-time list. Whenever appending a job makes its completion exceed its deadline, delete a job of largest processing time from that list and place it on a rejected list. Append all rejected jobs at the end. This minimizes the number of late jobs: at the first missed deadline at least one job of that prefix must be rejected, and rejecting a longest one frees at least as much processing time as any alternative. The exchange argument applies recursively to the remaining prefixes. The algorithm needs no ordering of the rejected jobs to determine the minimum count.

## ↑ Ancestors (5)

1. [Scheduling](scheduling.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
