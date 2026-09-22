<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An exact [Gillespie algorithm](../../../../../../gillespie-algorithm.md) for one particle is:

- Set the current well $k$ and time $t=0$.
- If $k$ is absorbing, stop.
- Set $a=k_++k_-$ and draw $\Delta t=-\log U_1/a$.
- Move to $k+1$ if $U_2<k_+/a$, and otherwise to $k-1$.
- Set $t\leftarrow t+\Delta t$ and repeat, stopping if the jump crosses an absorbing end.

For $N\ll K$, simulate particle identities independently and maintain a priority queue of their next event times. For $N\gg K$, store occupation numbers $n_k$ and use aggregate event rates $n_kk_+$ and $n_kk_-$ for each well; one population-level Gillespie event then decrements one $n_k$ and increments its neighbor. This replaces work proportional to particle number by work proportional to the number of occupied wells.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
