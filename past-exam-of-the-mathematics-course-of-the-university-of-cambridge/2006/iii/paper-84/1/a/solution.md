<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A binary [Hopfield network](../../../../../../hopfield-network.md) has $N$ recurrently connected units $s_i\in\{-1,+1\}$, symmetric weights $w_{ij}=w_{ji}$, zero self-weights, and thresholds $\theta_i$. A distributed memory is a desired population pattern $\xi^\mu$. One [Hebbian learning](../../../../../../hebbian-learning.md) prescription is

$$
\boxed{w_{ij}=\frac1N\sum_{\mu=1}^P\xi_i^\mu\xi_j^\mu\quad(i\ne j),\qquad w_{ii}=0}.
$$

Coactive signs strengthen a connection, and opposite signs weaken it. This is [Hebbian memory weights for a Hopfield network](../../../../../../hebbian-memory-weights-for-a-hopfield-network.md), rather than a separate address for each memory.

Initialize the units with the input cue, which can be a corrupted or partially specified pattern. Update one unit at a time by $s_i\leftarrow\operatorname{sign}(\sum_jw_{ij}s_j-\theta_i)$, retaining its old sign when the field is exactly zero. A fair asynchronous schedule revisits every unit. The energy

$$
E=-\tfrac12\sum_{i,j}w_{ij}s_is_j+\sum_i\theta_i s_i
$$

changes on a single update by $\Delta E=-(s_i'-s_i)(\sum_jw_{ij}s_j-\theta_i)\leq0$. An actual flip with the tie convention strictly reduces energy; finitely many states imply eventual arrival at a fixed point. This proves [asynchronous Hopfield energy descent](../../../../../../asynchronous-hopfield-energy-descent.md). Synchronous updating lacks this single-unit argument and can cycle.

For one stored pattern and zero thresholds, the field at $s=\xi$ is $(N-1)\xi_i/N$, so the pattern is a fixed point. With multiple patterns, the desired signal is accompanied by cross-talk from other memories; not every arbitrary set is guaranteed to be stable. **Retrieval is attraction from a cue to a stored-pattern fixed point**, provided the cue lies in its [basin of attraction](../../../../../../basin-of-attraction.md). Spurious minima and limited basins are part of the model, not errors in its update algorithm.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
